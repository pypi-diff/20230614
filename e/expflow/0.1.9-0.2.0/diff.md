# Comparing `tmp/expflow-0.1.9.tar.gz` & `tmp/expflow-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expflow-0.1.9.tar", max compression
+gzip compressed data, was "expflow-0.2.0.tar", max compression
```

## Comparing `expflow-0.1.9.tar` & `expflow-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-02-20 15:10:38.501837 expflow-0.1.9/LICENSE
--rw-r--r--   0        0        0    18897 2023-03-06 20:25:40.767341 expflow-0.1.9/README.md
--rw-r--r--   0        0        0      348 2023-03-07 18:02:04.676641 expflow-0.1.9/expflow/__init__.py
--rw-r--r--   0        0        0    42300 2023-03-07 17:58:27.764614 expflow-0.1.9/expflow/expflow.py
--rw-r--r--   0        0        0     1195 2023-03-07 18:02:17.540153 expflow-0.1.9/pyproject.toml
--rw-r--r--   0        0        0    20163 1970-01-01 00:00:00.000000 expflow-0.1.9/setup.py
--rw-r--r--   0        0        0    20434 1970-01-01 00:00:00.000000 expflow-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-02-20 15:10:38.501837 expflow-0.2.0/LICENSE
+-rw-r--r--   0        0        0    18897 2023-03-06 20:25:40.767341 expflow-0.2.0/README.md
+-rw-r--r--   0        0        0      427 2023-06-01 15:37:12.661919 expflow-0.2.0/expflow/__init__.py
+-rw-r--r--   0        0        0    46043 2023-06-14 15:47:32.615035 expflow-0.2.0/expflow/expflow.py
+-rw-r--r--   0        0        0     1195 2023-06-14 15:47:57.854469 expflow-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    20163 1970-01-01 00:00:00.000000 expflow-0.2.0/setup.py
+-rw-r--r--   0        0        0    20434 1970-01-01 00:00:00.000000 expflow-0.2.0/PKG-INFO
```

### Comparing `expflow-0.1.9/LICENSE` & `expflow-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `expflow-0.1.9/README.md` & `expflow-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `expflow-0.1.9/expflow/expflow.py` & `expflow-0.2.0/expflow/expflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,38 @@
-import datetime
 import gzip
 import re
 
 from dataclasses import dataclass, field
-from datetime import datetime as dt
+from datetime import date, datetime as dt
+from typing import Optional
+
+"""Note about datetime.
+
+I find this module super confusing. The module called datetime defines classes called
+date and datetime, and the class datetime defines a method called date. Therefore, if
+you do `import datetime` and then type `datetime.date`, you get the class date, which
+is the correct one for typing dates. If you do `from datetime import datetime` and then
+type `datetime.date`, you get the method, which isn't the correct one for typing dates.
+My solution is to import the classes date and datetime from the module. Also note that
+dataclasses-json doesn't support encoding or decoding of datetime.date into JSON, so
+functions need to be defined explicitly for that purpose.
+
+"""
+
 from getpass import getuser
 from logging import getLogger, Logger
 from os import getcwd
 from pathlib import Path
 from socket import gethostname
 from tempfile import TemporaryDirectory
 from uuid import UUID, uuid4
 from warnings import warn
 
-from dataclasses_json import DataClassJsonMixin, config
-from localnow import now
+from dataclasses_json import DataClassJsonMixin, config, cfg
+from localnow import now, tz
 from logmixin import get_logger, LogMixin
 
 module_logger: Logger = getLogger(__name__)
 module_logger.debug(f"Importing {__name__} from {__file__}")
 module_logger.debug(f"Creating a temporary directory for expflow data")
 tmpdir: TemporaryDirectory = TemporaryDirectory()
 module_logger.debug(f"Temporary directory created: {tmpdir.name}")
@@ -56,14 +70,26 @@
         "transitions": set(),
     },
 }
 module_logger.debug(f"Defined statuses dictionary: {statuses}")
 kw = {"repr": False, "compare": False, "hash": False, "init": True}
 USER_DIR: Path = Path.home() / "Expflow"
 
+_enc = cfg.global_config.encoders
+_enc[date] = date.isoformat
+_enc[Optional[date]] = lambda x: None if x is None else date.isoformat(x)
+_enc[Path] = str
+_enc[Optional[Path]] = lambda x: None if x is None else str(x)
+
+_dec = cfg.global_config.decoders
+_dec[date] = date.fromisoformat
+_dec[Optional[date]] = lambda x: None if x is None else date.fromisoformat(x)
+_dec[Path] = Path
+_dec[Optional[Path]] = lambda x: None if x is None else Path(x)
+
 
 def _get_subdir(subdir: str) -> Path:
     """Returns the path to a subdirectory of the expflow data directory.
 
     This function is used internally by expflow to get the path to a subdirectory of
     the expflow data directory. It is not intended to be used by users. The subdirectory
     is created if it does not already exist.
@@ -201,32 +227,32 @@
 
     """
     get_logger().debug(
         f"Checking if {id_} is a valid ID (must be at least 4 characters "
         f"long and contain only letters, numbers, underscores, and "
         f"dashes)"
     )
-    return len(id_) > 3 and bool(re.match(r"^[a-zA-Z0-9_\-]+$", id_))
+    return len(id_) >= 3 and bool(re.match(r"^[a-zA-Z0-9_\-]+$", id_))
 
 
-def _pe(p: Path | None) -> str | None:
+def _pe(p: Optional[Path]) -> Optional[str]:
     """Private function for encoding strings as Path objects.
 
     Args:
         p: Path to encode
 
     Returns:
         String representation of the path or None.
 
     """
     if isinstance(p, Path):
         return str(p)
 
 
-def _pd(s: str | None) -> Path | None:
+def _pd(s: Optional[str]) -> Optional[Path]:
     """Private function for decoding strings as Path objects.
 
     Args:
         s: String to decode.
 
     Returns:
         Path object or None if `s` does not contain ".json".
@@ -262,16 +288,16 @@
 
     """
 
     hostname: str = field(default_factory=gethostname, **kw)
     username: str = field(default_factory=getuser, **kw)
     datetime_created: dt = field(default_factory=now, **kw)
     uuid: UUID = field(default_factory=uuid4, **kw)
-    class_name: str | None = field(default=None, **kw)
-    base_name: str | None = field(default=None, **kw)
+    class_name: Optional[str] = field(default=None, **kw)
+    base_name: Optional[str] = field(default=None, **kw)
 
     def __post_init__(self) -> None:
         """Sets the class and base names immediately after initialisation if not already
         set."""
         if self.class_name is None:
             self.class_name = self._get_class_name()
         if self.base_name is None:
@@ -340,32 +366,30 @@
 
     Instance methods:
         save: Saves the object to a JSON file.
         to_json: Returns the JSON representation of the object.
 
     """
 
-    path: Path | None = field(
-        metadata=config(encoder=_pe, decoder=_pd),
-        default=None,
-        **kw,
-    )
-    datetime_last_saved: dt | None = field(default=None, **kw)
-    compression: bool = field(default=using_compression, **kw)
+    path: Optional[Path] = field(default=None, **kw)
+    datetime_last_saved: Optional[dt] = field(default=None, **kw)
+    compression: bool = field(default_factory=lambda: using_compression, **kw)
 
     def __post_init__(self) -> None:
         """Performs numerous validation checks to ensure the object was created or loaded
         properly."""
         super().__post_init__()
-        self.path = self._get_default_path()
+        self.no_save_on_gc: bool = True
+        self.path: Path = self._get_default_path()
         if self.datetime_last_saved is None:
             self._ensure_default_path_doesnt_exist()
             self.save()
+        self.no_save_on_gc = False
 
-    def _get_default_path(self) -> Path | None:
+    def _get_default_path(self) -> Optional[Path]:
         """Returns the default path of the object."""
         logger: Logger = self.get_logger()
         logger.debug("Getting default path")
         if not hasattr(self, "participant_id") or self.participant_id is None:
             logger.warning("Participant ID not found, cannot return default path")
             return
         suffix = ".json" + (".gz" if self.compression else "")
@@ -392,15 +416,15 @@
             if base.__name__ in ("Participant", "Experiment", "Trial"):
                 return base.__name__
 
     @classmethod
     def get_default_path(
         cls,
         participant_id: str,
-        experiment_id: str | None = None,
+        experiment_id: Optional[str] = None,
         compression: bool = using_compression,
     ) -> Path:
         """Returns the default path of the object."""
         logger: Logger = cls.get_logger()
         logger.debug("Getting default path")
         suffix = ".json" + (".gz" if compression else "")
         if cls.get_base_name() == "Participant":
@@ -453,15 +477,15 @@
         if str(expflow_dir) == tmpdir.name:
             msg: str = "Using temporary directory; data will be lost when program ends"
             logger.warning(msg)
             warn(msg)
         self.to_json(self.path)
         logger.info(f"Saved {self} to {self.path}")
 
-    def to_json(self, path: Path | str | None = None, **kwargs) -> None | str:
+    def to_json(self, path: Optional[Path | str] = None, **kwargs) -> None | str:
         """Write to JSON format.
 
         The preferred way to save data is to use the `save` method, which updates the
         `datetime_last_saved` field and saves to the default path. However, this method
         can be used to save to a custom path or to return the JSON string without saving
         to a file, which can be useful for debugging or data analysis.
 
@@ -494,15 +518,15 @@
             logger.info(f"Returning {self} JSON string")
             return j
 
     @classmethod
     def load(
         cls,
         participant_id: str,
-        experiment_id: str | None = None,
+        experiment_id: Optional[str] = None,
     ) -> "_SerialisationMixin":
         """Load an instance of this dataclass from a JSON file at the default path.
 
         Args:
             path = str | Path: The path to the JSON file. If no path is given,
                 the default path is used.
 
@@ -526,21 +550,42 @@
                     return cls.from_json(fp.read())
             else:
                 with open(path, "r") as fp:
                     return cls.from_json(fp.read())
         else:
             cls.get_logger().warning("Cannot save if without a default path")
 
+    def delete(self) -> None:
+        """Delete the file at the default path."""
+        logger: Logger = self.get_logger()
+        if self.path is None:
+            logger.warning("Cannot delete if without a default path")
+            return
+        if self.path.exists():
+            self.path.unlink()
+            logger.info(f"Deleted {self.path}")
+        else:
+            logger.warning(f"{self.path} does not exist")
+        logger.debug("Since we deleted the file, we should turn off saving during g.c.")
+        if self.no_save_on_gc is False:
+            self.no_save_on_gc = True
+
     def __del__(self):
-        self.get_logger().info(f"Deleting {self}")
+        logger: Logger = self.get_logger()
+        logger.info(f"Garbage collecting {self}")
         try:
-            if self.path is not None:
-                if self.path.exists():  # prevents saving on g.c. if we removed the file
+            if self.path is not None and self.path.exists():
+                logger.debug(f"Path is {self.path} and exists")
+                if not self.no_save_on_gc:
+                    logger.debug(f"Saving {self} before garbage collection")
                     self.save()
+                else:
+                    logger.debug(f"Not saving {self} before g.c.")
         except ImportError:
+            logger.error("Got an ImportError, probably because we're in a test")
             pass
 
 
 @dataclass
 class _ParReqFieldsMixin:
     """Participant required fields mixin dataclass.
 
@@ -604,20 +649,21 @@
     `SomeSubclassParticipant(participant_id="test")`. This is a good thing!
 
     Participant objects have `save()`, `load()`, `to_json()` and `from_json()`methods for
     serialisation.
 
     """
 
-    dob: datetime.date | None = field(default=None, **kw)
-    age: float | int | None = field(default=None, **kw)
-    gender: str | None = field(default=None, **kw)
-    language: str | None = field(default=None, **kw)
-    comments: str | None = field(default=None, **kw)
-    group: str | None = field(default=None, **kw)
+    dob: Optional[date] = field(default=None, **kw)  # not `datetime.date` ... see note!
+    age: Optional[float | int] = field(default=None, **kw)
+    gender: Optional[str] = field(default=None, **kw)
+    language: Optional[str] = field(default=None, **kw)
+    comments: Optional[str] = field(default=None, **kw)
+    group: Optional[str] = field(default=None, **kw)
+    temporary_participant: bool = field(default=False, **kw)
 
     def __post_init__(self):
         super().__post_init__()
         if not is_valid_id(self.participant_id):
             msg: str = f"Invalid participant ID: {self.participant_id}"
             self.get_logger().error(msg)
             raise ValueError(msg)
@@ -691,19 +737,19 @@
         get_duration: Get the duration of the experiment or trial.
 
     """
 
     current_status: str = field(default="pending", **kw)
     status_history: list[dict[str, str | dt]] = field(default_factory=list, **kw)
     event_history: list[dict[str, str | dt]] = field(default_factory=list, **kw)
-    datetime_started: dt | None = field(default=None, **kw)
-    datetime_finished: dt | None = field(default=None, **kw)
+    datetime_started: Optional[dt] = field(default=None, **kw)
+    datetime_finished: Optional[dt] = field(default=None, **kw)
     datetimes_paused: list[tuple[dt, dt]] = field(default_factory=list, **kw)
-    datetime_last_paused: dt | None = field(default=None, **kw)
-    duration: float | None = field(default=None, **kw)
+    datetime_last_paused: Optional[dt] = field(default=None, **kw)
+    duration: Optional[float] = field(default=None, **kw)
 
     @property
     def is_pending(self) -> bool:
         return self.current_status == "pending"
 
     @property
     def is_running(self) -> bool:
@@ -788,54 +834,61 @@
         self.current_status = new_status
         logger.debug(f"Changed status of {self} from {old_status} to {new_status}")
 
         logger.debug("Updating datetime fields as necessary")
         if new_status == "running":
             if old_status == "paused":
                 logger.debug("Updating datetimes_paused")
+                assert isinstance(self.datetime_last_paused, dt)
+                assert isinstance(then, dt)
                 pause = (self.datetime_last_paused, then)
                 self.datetimes_paused.append(pause)
             elif old_status == "pending":
                 logger.debug("Updating datetime_started")
                 self.datetime_started = then
         elif new_status == "finished" or new_status == "timed_out":
             logger.debug("Updating datetime_finished")
             self.datetime_finished = then
             self.duration = self.get_duration()
         elif new_status == "paused":
-            logger.debug("Updating datetime_last_pause")
+            logger.debug("Updating datetime_last_paused")
             self.datetime_last_paused = then
 
-    def get_duration(self) -> float | None:
+    def get_duration(self) -> Optional[float]:
         """Return the duration in seconds.
 
         If not finished, returns None. If finished, returns datetime_finished minus
         datetime_started, minus the sum of the durations of all pauses.
 
         """
         self.get_logger().debug("Calculating duration")
         if self.datetime_finished is None:
             self.get_logger().warning("Cannot calculate duration if not finished")
             return None
         dur = (self.datetime_finished - self.datetime_started).total_seconds()
         for start, end in self.datetimes_paused:
+            if isinstance(start, float):
+                start = dt.fromtimestamp(start, tz=tz)
+            if isinstance(end, float):
+                end = dt.fromtimestamp(end, tz=tz)
             dur -= (end - start).total_seconds()
         return dur
 
 
 @dataclass
 class Trial(_IdentificationMixin, _StatusMixin, LogMixin, DataClassJsonMixin):
     """Trial dataclass.
 
     This is the base dataclass for trials. Users should create an instance of this class
     (or one of its subclasses) for each trial in an experiment.
 
     Trial dataclasses have several optional user-specifiable fields:
         stimulus: Information presented to the participant.
         response: The participant's subsequent behavior.
+        reaction_time: The time taken to respond.
         trial_number: The trial number within the experiment.
         block_number: The block number within the experiment.
         condition: The condition of the trial.
         practice: Whether the trial is a practice trial.
 
     These can be set during or after instantiation. It makes sense to set `stimulus`
     before the trial is run and `response` afterwards, but you can do whatever you want.
@@ -852,19 +905,20 @@
     marked as finished.
 
     The `event_history` field is meant to be set by the user to record any events that
     occur during the trial but aren't captured elsewhere.
 
     """
 
-    stimulus: str | list | float | int | dict | set | None = None
-    response: str | list | float | int | dict | set | None = None
-    trial_number: int | None = None
-    block_number: int | None = None
-    condition: str | None = None
+    stimulus: Optional[str | list | float | int | dict | set] = None
+    response: Optional[str | list | float | int | dict | set] = None
+    reaction_time: Optional[float] = None
+    trial_number: Optional[int] = None
+    block_number: Optional[int] = None
+    condition: Optional[str] = None
     practice: bool = False
 
 
 @dataclass
 class _ExpReqFieldsMixin:
     participant_id: str
     experiment_id: str
@@ -931,16 +985,17 @@
     experiment is marked as finished.
 
     The `event_history` field is meant to be set by the user to record any events that
     occur during the trial but aren't captured elsewhere.
 
     """
 
-    trial_index: int | None = field(default=None, **kw)
+    trial_index: Optional[int] = field(default=None, **kw)
     trials: list[Trial] = field(default_factory=list, **kw)
+    summary: Optional[dict[str, int | float | dt | str]] = field(default=None, **kw)
 
     def __post_init__(self):
         super().__post_init__()
         self._check_participant_exists()
         self._check_experiment_wasnt_interrupted()
         if not is_valid_id(self.participant_id):
             msg: str = f"Invalid participant ID: {self.participant_id}"
@@ -972,28 +1027,40 @@
                 "experiment will be incorrect."
             )
             logger.warning(msg)
             warn(msg)
             self.pause()
 
     @property
-    def current_trial(self) -> Trial | None:
+    def current_trial(self) -> Optional[Trial]:
         return self.trials[self.trial_index]
 
     @property
     def previous_trial(self) -> Trial:
         return self.trials[self.trial_index - 1]
 
     @property
+    def previous_trials(self) -> list[Trial]:
+        return self.trials[: self.trial_index]
+
+    @property
     def next_trial(self) -> Trial:
         return self.trials[self.trial_index + 1]
 
     @property
     def remaining_trials(self) -> list[Trial]:
-        return self.trials[self.trial_index + 1 :]
+        return self.trials[self.trial_index + 1:]
+
+    @property
+    def is_first_trial(self) -> bool:
+        return self.trial_index == 0
+
+    @property
+    def finished_trials(self) -> list[Trial]:
+        return [t for t in self.trials if t.is_finished]
 
     def __del__(self):
         self.get_logger().debug("Deleting experiment object")
         if self.is_running:
             self.get_logger().debug("Experiment was running, so it is now paused")
             self.pause()
             self.current_trial.pause()
@@ -1021,35 +1088,42 @@
             self.trial_index += 1
 
         if self.trial_index > 0:
             logger.debug("Updating statuses of previous trial if necessary")
             if self.previous_trial.is_running:
                 logger.debug("Previous trial was running, so it is now finished")
                 self.previous_trial.finish()
+            else:
+                x = self.previous_trial.status
+                logger.debug(f"Previous trial was {x}, so nothing to update")
 
         logger.debug(f"Updating statuses of current trial if necessary")
         try:
             if self.current_trial.is_pending:
                 logger.debug("Current trial was pending, so it is now running")
                 self.current_trial.run()
             elif self.current_trial.is_paused:
                 logger.debug("Current trial was paused, so it is now running")
                 self.current_trial.unpause()
             elif self.current_trial.is_skipped:
                 logger.debug("Current trial was skipped, iterating again")
                 next(self)
+            else:
+                x = self.current_trial.status
+                logger.debug(f"Current trial was {x}, so nothing to update")
         except IndexError:
             logger.debug("There is no current trial, so nothing to update")
 
         self.save()
 
         if self.trial_index >= len(self.trials):
             logger.debug("Experiment finished")
             self.finish()
             self.trial_index = None
+            self.save()
             raise StopIteration
 
         return self.current_trial
 
     def _ok_to_add_trial(self) -> None:
         """Check if it is OK to add a trial to the experiment."""
         if self.is_finished or self.is_skipped or self.is_timed_out:
@@ -1116,15 +1190,28 @@
     pass
 
 
 class ParticipantDoesNotExistError(FileNotFoundError):
     pass
 
 
-def get_participant_ids() -> set[str]:
+def get_participant_ids() -> list[str]:
     """Get a list of participant IDs."""
-    return {str(p).split(".")[0] for p in _get_pdir().glob("*.json*")}
+
+    return [f.stem.replace(".json", "") for f in _get_pdir().glob("*.json*")]
 
 
-def get_experiment_ids() -> set[str]:
+def get_experiment_ids() -> list[str]:
     """Get a list of experiment IDs."""
-    return {str(e).split(".")[1] for e in _get_edir().glob("*.json*")}
+    return list(
+        {f.stem.replace(".json", "").split(".")[1] for f in _get_edir().glob("*.json*")}
+    )
+
+
+def get_participated_in(participant_id: str) -> list[str]:
+    """Get a list of experiment IDs that a participant has participated in."""
+    return list(
+        {
+            f.stem.replace(".json", "").split(".")[1]
+            for f in _get_edir().glob(f"{participant_id}.*.json*")
+        }
+    )
```

### Comparing `expflow-0.1.9/pyproject.toml` & `expflow-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "expflow"
-version = "0.1.9"
+version = "0.2.0"
 description = "A Python library for controlling the flow of psychological experiments."
 authors = ["Sam Mathias"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/sammosummo/expflow"
 repository = "https://github.com/sammosummo/expflow"
 documentation = "https://github.com/sammosummo/expflow"
```

### Comparing `expflow-0.1.9/setup.py` & `expflow-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['dataclasses_json>=0.5.7,<0.6.0',
  'localnow>=0.1.0,<0.2.0',
  'logmixin>=0.1.4,<0.2.0']
 
 setup_kwargs = {
     'name': 'expflow',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'description': 'A Python library for controlling the flow of psychological experiments.',
     'long_description': '# Expflow\n  \n## Description  \n  \nExpflow is a Python library that controls the flow and handles the data of psychological experiments. While it isn\'t a \nfull-fledged experiment builder like [PsychoPy](https://www.psychopy.org), it may be used with other tools to create \nrobust experiments with minimal coding.\n  \n## Installation  \n  \nExpflow is available on PyPI and can be installed in the typical way with `pip`:  \n  \n```bash  \npip install expflow\n```  \n  \n## Tutorial  \n  \n### Overview  \n\nExpflow has strong opinions about how psychological experiments should be structered and coded, and performs extensive \nautomatic bookkeeping and numerous validation checks under the hood to ensure that the user\'s code is consistent with \nthese opinions.\n\nExpflow defines an experiment as a sequence of trials presented to a participant. Typically, trials are identical except\nfor a small number of critical details, such as the stimulus. The participant makes a response on each trial, after \nwhich the trial ends. The next trial begins after the previous one. After the last trial, the experiment is finished.\n\n### Logging  \n  \nExpflow makes extensive use of the [logging](https://docs.python.org/3/library/logging.html) module. The first few times\nyou use expflow, I recommend setting up basic logging at the most verbose level at beginning of your experiment script, \nwhich will allow you to see exactly what expflow does. If blazing fast performance is not a major concern — which \ntypically it isn\'t, because psychological experiment are often simple things and modern computers are powerful — you \ncould leave verbose logging switched on all the time (that\'s what I do). \n  \n```python  \nimport logging  \n  \nlogging.basicConfig(level=logging.DEBUG)  \nlogging.debug("Hello, world!")  \n```  \n\nThe rest of this tutorial will now print many log message to the console.\n\n### Importing expflow\n\nImport expflow as follows.\n  \n```python  \nimport expflow  \n```  \n  \n### Directories\n\n#### Temporary directory\n  \nSee the bit about creating a temporary directory in the log output?\n\nExpflow needs somewhere to store data right away, and the default behaviour is to use a temporary directory. This is \nsuitable for testing, but a bad idea for real work, because the data you generate will be lost when the program ends. \nExpflow will bug you with warnings if you don\'t set a permanent data directory. For example, try this:\n\n```python\nexpflow.get_expflow_dir()  # produces a warning\n```\n\n#### Permanent directory\n\nTo set a permanent directory, use the `set_expflow_dir` function. You can pass any valid writable path to a directory. A\ngood choice is a dedicated subdirectory of your home directory. For convenience, expflow provides this as a constant \ncalled `expflow.USER_DIR`. \n  \n```python  \nexpflow.set_expflow_dir(expflow.USER_DIR)  # set a dir\nexpflow.get_expflow_dir()  # prints something like `/Users/username/Expflow`\n```  \n\n#### Subdirectories\n\nThe function `set_expflow_dir` creates several subdirectories if they don\'t already exist. These are used to store \ndifferent types of data. Currently, participant data are stored in the `participants` subdirectory and experiment data \nare stored in the `experiment` subdirectory. The others will be used by future versions of expflow.\n\n### Cleaning up\n  \nBefore we go on, let\'s take a moment delete some files that may exist in your user directory if you ran this tutorial\npreviously. \n  \n```python  \nfor i in range(1, 10):  \n    (expflow.USER_DIR / "Participants" / f"example_p{i}.json").unlink(True)  \n    (expflow.USER_DIR / "Experiments" / f"example_p{i}.example_e1.json").unlink(True) \n```  \n  \n### Participants \n\n#### Creating participants\n  \nA participant is a person who takes part in an experiment. In expflow, a participant is represented by a `Participant` \nobject. You should create an instance of this class for each participant in an experiment.\n\n```python  \np = expflow.Participant("example_p1")  # creates a new participant\n```\n\nParticipant objects are [dataclasses](https://docs.python.org/3/library/dataclasses.html). The single required argument\nbecomes a field called `participant_id`, which must be a unique string for each participant. Other optional fields you \ncan set are:\n\n- `dob`: Date of birth. Should be a `date` object.\n- `age`: Age. Should be an `int` or `float`. Doesn\'t make sense to use this if `dob` is specified.\n- `gender`: Participant gender.\n- `language`: Participant language.\n-  `comments`: Any comments about the participant.\n-  `group`: Participant group.\n\nThere are other fields as well. You can see them all like so:\n  \n```python  \nimport dataclasses  \n  \nfor field in dataclasses.fields(p):  \n    logging.info(f"{field.name}: {getattr(p, field.name)}")  \n```  \n\nHowever, **don\'t go changing the values of the other fields willy-nilly!** Expflow manages them  \nautomatically and uses them for bookkeeping. Generally, I recommend setting participant fields at object instantiation \nand, except perhaps for the `comments` field, never changing them.\n\n#### Saving and loading\n  \nWhen we created our participant object, it automatically saved a [JSON](https://www.json.org/json-en.html) \nrepresentation of itself to a file in the `participants` subdirectory, whose path is given by the `path` field. This \nwill always happen every time we create a participant object and there is no way to stop it, by design. A participant \nobject will also save itself before garbage collection.\n  \n```python  \ndel p  # delete the participant \n```\n\nThis "autosaving" feature allows expflow to enforce ***Golden Rule #1: A given participant can\'t be created twice***. An\nexception will be raised if you try to create a new participant with the same `participant_id` as an existing \nparticipant, even if the older participant was not created during the current Python session.\n\n```python\ntry:\n    p = expflow.Participant("example_p1")  # even though we deleted `p`!\n    raise RuntimeError("You won\'t see this message")\n\nexcept expflow.ParticipantExistsError as er:\n    logging.error(er)\n```\n\nSometimes you may need to load a participant, for example to add something to their `comments` field. You can do so \nusing the `load` class method, which requires the `participant_id`.\n\n```python\np = expflow.Participant.load("example_p1")\np.comments += "- Here\'s a comment\\n"\np.comments += "- Here\'s another\\n"\ndel p  # autosave on deletion\n```\n\nYou can overtly save the participant with the `save` method, but you shouldn\'t need to. If you want to quickly get at \nthe participant data for testing or debugging purposes, you can use the `to_dict` and `to_json` methods. But otherwise,\nparticipant objects will save on garbage collection.\n\n#### Compression\n\nBy default, JSON representations of participants are uncompressed, but you can use [gzip](https://www.gzip.org) \ncompression instead by setting the optional field `compression` to `True` when creating a new participant or setting the\nglobal variable `expflow.using_compression` to `True` to turn on compresson by default. Compressed files usually much \nsmaller, but not human readable, and have the extension `.json.gz` instead of `.json`.\n\n### Experiments and trials\n\n#### Creating experiments\n\nExperiments are represented by the `Experiment` dataclass. You must create an instance of this class each time a new \nparticipant is about to run an experiment. Experiment objects have two required fields: `participant_id` and  \n`experiment_id`. \n\n```python\ne = expflow.Experiment("example_p1", "example_e1")\n```\n\nThe *combination* of these identifiers must be unique. In other words, a single participant can perform multiple \ndifferent experiments, and multiple different participants can perform the same experiment, but  ***Golden Rule #2: A \ngiven participant can\'t perform a given experiment twice.***. You can load an experiment object with an existing \ncombination of identifiers.\n\n```python\ndel e  \ntry:  \n    e = expflow.Experiment("example_p1", "example_e1")  \n    raise RuntimeError("You won\'t see this message")  \nexcept expflow.ExperimentExistsError as er:  \n    logging.error(er)  \ne = expflow.Experiment.load("example_p1", "example_e1")\n```\n\nUnder the hood, this is enforced by saving on creation and garbage collection.\n\nYou also can\'t create an experiment if the participant doesn\'t exist.\n\n```python  \ntry:  \n    _ = expflow.Experiment("example_p2", "example_e1")  \n    raise RuntimeError("You won\'t see this message")  \nexcept expflow.ParticipantDoesNotExistError as er:  \n    logging.error(er)\n```\n\nFinally, experiments have an optional user-specified field called `trials`, which is discussed in the next section. You \ncan set this on instantiation or later via special methods.\n\n#### Creating trials\n\nExperiments contain trials. Trials are represented by instance of the `Trial` dataclass, but unlike participant and \nexperiment dataclasses, they can\'t be saved or loaded individually (maybe in a future version). Expflow doesn\'t insist \non trials having unique identifiers or on required fields, either.\n\nThere are a number of optional fields:\n\n- `stimulus`\n- `response` \n- `trial_number`\n- `block_number`\n- `condition` \n- `practice`\n\nIt should be obvious what each of these is supposed to represent.\n\nLet\'s create a list of trials.\n\n```python  \ntrials = [expflow.Trial(trial_number=i) for i in range(3)]  \n```  \n\n#### Appending trials to an experiment\n  \nInside an experiment object, trials are stored in field called `trials`, which is a list of `Trial` objects. The \nexperiment we created currently has an empty `trials` field.  \n  \n```python  \nassert len(e.trials) == 0  \n```  \n  \nThis is a good time to bring up ***Golden Rule #3: Run experiments by iterating experiment objects***. Accordingly, `e` \nis iterable and its `__len__` method returns the number of trials it contains.  \n  \n```python  \nassert len(e) == 0  \n```  \n  \nWe can append the trials we created to the experiment using the `append_trials` method.  \n  \n```python  \ne.append_trials(trials)  \n```  \n\nYou can append to or otherwise directly modify `e.trials` **but please don\'t**, because the `append_trials` method does \nextra things like checks you are actually appending `Trial` instances and saves the experiment object.\n\nAfter appending, the experiment has three trials.  \n  \n```python  \nassert len(e) == 3  \n```  \n  \nExperiments save themselves after a trial is appended, so if we delete the experiment and reload it, we will see that \nthe appended trials are there.  \n  \n```python  \ndel e  \ne = expflow.Experiment.load("example_p1", "example_e1")\nassert len(e) == 3  \n```  \n  \n#### Other manipulations to the trial list\n\nCurrently, there are only `append_trials`, `append_trial`, and `insert_trial` methods, but more may be added in future \nversions of expflow.\n\n###  Experiment flow\n\nThis section will describe the core features that allows expflow to control experiment flow. First, it is important to \nknow about two variables inside experiment objects: the trial index and the status.\n\n#### Trial index\n\nExperiments have a field called `trial_index`, which is automatically managed. Its value is `None` on instantiation, and\nbecomes an integer when the experiment runs. Predictably, this is used to index the experiment\'s current position in \nthe trial list. User\'s shouldn\'t set this field themselves.\n\n#### Statuses\n  \nExperiments (and trials) have a special `status` property (mirrored by the `current_status` field). Users shouldn\'t set\nthis property or its field themselves, but they can read it or test its value with `is_*` boolean properties. \n\nThere are only six possible statuses and only certain status transitions are possible. The possible statuses, their \nmeanings, and acceptable transitions are given in the table below.\n\n| Status        | Description                          | Acceptable transitions      |\n|---------------| ------------------------------------ |-----------------------------|\n| `"pending"`   | Trial is scheduled to run later      | running, skipped            |\n| `"running"`   | Trial is running right now           | finished, timed_out, paused |\n| `"paused"`    | Trial is temporarily paused          | running                     |\n| `"timed_out"` | Trial went on too long and has ended | -                           |\n| `"finished"`  | Trial ended as expected              | -                           |\n| `"skipped"`   | Trial will not run                   | -                           |\n\nThis is designed to conisistent with the common usage of the words. On instantiation, the status of an experiment is \nalways `"pending"`. This is natural, because experiments are created before they are run. Pending experiments can be \nchanged to `"running"` or `"skipped"`. Running experiments can be changed to `"finished"` if they were completed normally, `"paused"` if they were paused, or `"timed_out"` if they were timed out. Paused experiments must be unpaused (i.e., set back to `"running"`) before they can be `"finished"`. `"finished"`, `"timed_out"`, and `"skipped"` are terminal statuses. Hopefully this all makes intuitive sense.\n\nIndividual trials have a status property that behaves in exactly the same way.\n\nAs we shall see, experiment and trial statuses are managed automatically as we run an experiment. In fact, this is the\nmajor trick expflow employs to ensure proper flow.\n  \n#### Running experiments  \n  \nAs per Golden Rule #3, to run an experiment, you iterate over the experiment object, such as in a  `for` loop.\n  \n```python  \ndef show_stimulus(stimulus):\n\t"""Replace this with something that presents stimuli."""\n    pass  \n  \ndef get_response(): \n\t"""Replace this with something that collects responses."""\n    return "response"  \n  \nfor trial in e:\n\n\t# do experimental stuff here, for example ...\n\tshow_stimulus(trial.stimulus)  \n    trial.response = get_response()\n    # ... end of experimental stuff\n    \n    if not e.is_running:\n\t    break  \n```  \n  \nThis is *almost* a completely normal Python `for` loop. I say almost because it contains an `if` statement that will \nprematurely break the loop if the experiment status is no longer set to `"running"`. This is necessary to catch pauses,\nskips, and time outs (discussed later).\n\nIf your experiment is embedded within a larger program and it is not convenient or possible to use the `for` syntax, \nyou could use `next(e)` instead, but just remember to catch the `StopIteration` exception.\n\n#### Saving data\n\nNotice that in our toy experiment above, the `response` field of the current trial was set to the participant\'s response\non that trial. How do we make sure those responses are recorded?\n\nEach `trial` in the loop was a reference to the experiment\'s current trial (also available via `self.current_trial`). \nTherefore, because we set `trial.response` to `"response"`, participant responses are available after iteration (i.e., \nafter the experiment has finished).\n\n```python\nfor trial in e.trials:  # remember Golden Rule #3  \n    assert trial.response == "response"\n```\n\nFurthermore, experiments save themselves after each iteration and status change, so we have also *serialised* the data \nas well. Let\'s delete the experiment object and reload it. \n  \n```python  \ndel e  \ne = expflow.Experiment.load("example_p1", "example_e1")  \nfor trial in e.trials: # Golden Rule #3 \n    assert trial.response == "response"\n```  \n\nThe responses were recorded! This is important — it means that expflow automatically stores data across Python sessions\nwith no extra effort on the part of the user.\n\n#### Pausing\n\nSuppose an experiment is too long to be completed all in one session: we need to pause it and resume it later. The \nfollowing code simulates a pause halfway through an experiment.\n\n```python\np2 = expflow.Participant("example_p2")\ntrials = [expflow.Trial(trial_number=i) for i in range(10)]\ne3 = expflow.Experiment("example_p2", "example_e1", trials=trials)\n\nfor trial in e:\n\n\tif e.trial_index > 5:\n\t\n\t\tshow_stimulus(trial.stimulus)  \n\t    trial.response = get_response()\n\n\telse:\n\t\te.pause()\n    \n    if not e.is_running:\n\t    break  \n\nassert e.is_paused\nassert e.current_trial.is_paused\n```\n\nYou can resume a paused experiment by iterating over it again.\n\n```python\nfor trial in e:\n\n\tassert e.trial_index > 5\n\t\n\tshow_stimulus(trial.stimulus)  \n\ttrial.response = get_response()\n    \n    if not e.is_running:\n\t    break\n```\n\n#### Timing out\n\nIndividual trials or entire experiments may have time limits. If so, you can use the `trial.time_out` and \n`experiment.time_out` methods to time out a trial or experiment, respectively. Timed out trials and experiments cannot \nbe resumed (unlike paused trials).\n\n#### Skipping\n\nSometimes an experiment may skip upcoming trials, or an experiment may be skipped enitrely (if it is part of a batch of\nexperiments, for example). You can use the `trial.skip` and `experiment.skip` methods to achieve this. You can\'t skip a\ntrial or experiment that was already started, nor can you ever\nstart a skipped trial or experiment.\n\nExperiments don\'t always present every trial to every participant. Sometimes an experiment may have a stopping rule, \nwhere some or all remaining trials are skipped due to poor performance, or trial-specific or whole-experiment time \nlimits. The statuses `"skipped"` and `"timed_out"` — and their respecitve methods, `skip` and `timeout` (or `time_out`) — exist to deal with these circumstances. You can skip or time out individual trials or entire experiments. Skipped or timed out experiments/trials cannot be rerun afterwards under any circumstances.\n\n#### Duration\n\nExperiments and trials have a  `duration` field that is calculated when the experiment/trial is finished or timed out. \nIt represents the total time taken to complete the experiment/trial, minus any time spent in a paused state, in seconds.\n\n#### Crash recovery\n\nExpflow has a rudimentary crash-recovery feature. It doesn\'t work all the time, but it could save your bacon once in a\nwhile.\n\nConsider this example:\n\n```python\np3 = expflow.Participant("example_p3")\ntrials = [expflow.Trial(trial_number=i) for i in range(3)]\ne2 = expflow.Experiment("example_p3", "example_e1", trials=trials)  \n\nfor trial in e3:  \n    \n    show_stimulus(trial.stimulus)  \n    trial.response = get_response()  \n    \n    break  # <- crash!  \n\ndel e3  # <- crash!  \n\ne3 = expflow.Experiment.load("example_p3", "example_e1")  \nassert e3.is_paused  \nassert e3.current_trial.is_paused\n```\n\nHere, we have simulated a computer crash by breaking the trial loop and deleting our experiment object, which is \napproximately what would happen if you encountered an unexpected exception during your experiment. On garbage \ncollection, an experiment object will change its status from running to \npaused if necessary, and save itself. Therefore, when this experiment is loaded again, it behaves as if it were paused \nat the point of garbage collection.',
     'author': 'Sam Mathias',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/sammosummo/expflow',
```

### Comparing `expflow-0.1.9/PKG-INFO` & `expflow-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expflow
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python library for controlling the flow of psychological experiments.
 Home-page: https://github.com/sammosummo/expflow
 License: MIT
 Keywords: psychology,neuroscience
 Author: Sam Mathias
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 3 - Alpha
```

