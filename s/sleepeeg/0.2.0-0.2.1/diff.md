# Comparing `tmp/sleepeeg-0.2.0.tar.gz` & `tmp/sleepeeg-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepeeg-0.2.0.tar", last modified: Tue Jun  6 06:18:47 2023, max compression
+gzip compressed data, was "sleepeeg-0.2.1.tar", last modified: Wed Jun  7 16:31:03 2023, max compression
```

## Comparing `sleepeeg-0.2.0.tar` & `sleepeeg-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 06:18:47.666786 sleepeeg-0.2.0/
--rw-rw-rw-   0        0        0     1088 2023-03-20 20:54:05.000000 sleepeeg-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1422 2023-06-06 06:18:47.665789 sleepeeg-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1000 2023-06-06 06:12:40.000000 sleepeeg-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 06:18:47.635870 sleepeeg-0.2.0/docs/
--rw-rw-rw-   0        0        0     2495 2023-06-06 06:12:53.000000 sleepeeg-0.2.0/docs/conf.py
--rw-rw-rw-   0        0        0      861 2023-06-06 06:07:20.000000 sleepeeg-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 06:18:47.666786 sleepeeg-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 06:18:47.645843 sleepeeg-0.2.0/sleepeeg/
--rw-rw-rw-   0        0        0    47580 2023-06-05 11:10:20.000000 sleepeeg-0.2.0/sleepeeg/base.py
--rw-rw-rw-   0        0        0     9796 2023-06-06 05:52:35.000000 sleepeeg-0.2.0/sleepeeg/dashboard.py
--rw-rw-rw-   0        0        0    24536 2023-06-05 13:36:04.000000 sleepeeg-0.2.0/sleepeeg/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:18:47.663795 sleepeeg-0.2.0/sleepeeg.egg-info/
--rw-rw-rw-   0        0        0     1422 2023-06-06 06:18:47.000000 sleepeeg-0.2.0/sleepeeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-06-06 06:18:47.000000 sleepeeg-0.2.0/sleepeeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:18:47.000000 sleepeeg-0.2.0/sleepeeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2023-06-06 06:18:47.000000 sleepeeg-0.2.0/sleepeeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-06 06:18:47.000000 sleepeeg-0.2.0/sleepeeg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 16:31:03.354054 sleepeeg-0.2.1/
+-rw-rw-rw-   0        0        0     1088 2023-03-20 20:54:05.000000 sleepeeg-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1422 2023-06-07 16:31:03.353057 sleepeeg-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1000 2023-06-06 06:12:40.000000 sleepeeg-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 16:31:03.297207 sleepeeg-0.2.1/docs/
+-rw-rw-rw-   0        0        0     2495 2023-06-06 06:12:53.000000 sleepeeg-0.2.1/docs/conf.py
+-rw-rw-rw-   0        0        0      861 2023-06-07 16:29:05.000000 sleepeeg-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-07 16:31:03.355052 sleepeeg-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-07 16:31:03.329121 sleepeeg-0.2.1/sleepeeg/
+-rw-rw-rw-   0        0        0    47624 2023-06-07 16:27:20.000000 sleepeeg-0.2.1/sleepeeg/base.py
+-rw-rw-rw-   0        0        0     9796 2023-06-06 05:52:35.000000 sleepeeg-0.2.1/sleepeeg/dashboard.py
+-rw-rw-rw-   0        0        0    27717 2023-06-07 14:44:52.000000 sleepeeg-0.2.1/sleepeeg/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:31:03.350065 sleepeeg-0.2.1/sleepeeg.egg-info/
+-rw-rw-rw-   0        0        0     1422 2023-06-07 16:31:03.000000 sleepeeg-0.2.1/sleepeeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-06-07 16:31:03.000000 sleepeeg-0.2.1/sleepeeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 16:31:03.000000 sleepeeg-0.2.1/sleepeeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2023-06-07 16:31:03.000000 sleepeeg-0.2.1/sleepeeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-07 16:31:03.000000 sleepeeg-0.2.1/sleepeeg.egg-info/top_level.txt
```

### Comparing `sleepeeg-0.2.0/LICENSE` & `sleepeeg-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.2.0/PKG-INFO` & `sleepeeg-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepeeg
-Version: 0.2.0
+Version: 0.2.1
 Summary: Sleep EEG preprocessing and analysis
 Author-email: Gennadiy Belonosov <gennadiyb@mail.tau.ac.il>
 License: MIT
 Project-URL: Homepage, https://github.com/NirLab-TAU/sleepeeg
 Project-URL: Documentation, https://nirlab-tau.github.io/sleepeeg/
 Keywords: sleep,eeg
 Requires-Python: >=3.10
```

### Comparing `sleepeeg-0.2.0/README.md` & `sleepeeg-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.2.0/docs/conf.py` & `sleepeeg-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.2.0/pyproject.toml` & `sleepeeg-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 exclude = ["notebooks"]  # empty by default
 
 [project]
 name = "sleepeeg"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     {name = "Gennadiy Belonosov", email = "gennadiyb@mail.tau.ac.il"},
 ]
 description = "Sleep EEG preprocessing and analysis"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
```

### Comparing `sleepeeg-0.2.0/sleepeeg/base.py` & `sleepeeg-0.2.1/sleepeeg/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,16 @@
             overwrite: Whether to overwrite annotations and bad_channels files if exist.
                 Defaults to False.
             **kwargs: Arguments passed to :py:meth:`mne:mne.io.Raw.plot`.
         """
         kwargs.setdefault("theme", "dark")
         kwargs.setdefault("bad_color", "r")
         kwargs.setdefault("scalings", "auto")
+        kwargs.setdefault("block", True)
+
         self.mne_raw.plot(**kwargs)
 
         if save_annotations:
             self.mne_raw.annotations.save(
                 self.output_dir / self.__class__.__name__ / "annotations.txt",
                 overwrite=overwrite,
             )
```

### Comparing `sleepeeg-0.2.0/sleepeeg/dashboard.py` & `sleepeeg-0.2.1/sleepeeg/dashboard.py`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.2.0/sleepeeg/pipeline.py` & `sleepeeg-0.2.1/sleepeeg/pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -650,9 +650,82 @@
 
     mne_raw: mne.io.Raw = field(init=False)
 
     @mne_raw.default
     def _get_mne_raw_from_pipe(self):
         return self.pipes[0].mne_raw
 
-    def compute_psds_per_stage(self):
-        ...
+    def compute_psds_per_stage(
+        self,
+        sleep_stages: dict = {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4},
+        reference: Iterable[str] | str | None = None,
+        method: str = "welch",
+        fmin: float = 0,
+        fmax: float = 60,
+        picks: str | Iterable[str] = "eeg",
+        reject_by_annotation: bool = True,
+        save: bool = False,
+        overwrite: bool = False,
+        n_jobs: bool = -1,
+        verbose: bool = False,
+        **psd_kwargs,
+    ):
+        """For each sleep stage creates a :class:`.SleepSpectrum` object.
+
+        Args:
+            sleep_stages: Sleep stages mapping in hypnogram.
+                Defaults to {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4}.
+            reference: Which eeg reference to compute PSD with.
+                If None, the reference isn't changed. Defaults to None.
+            method: Spectral estimation method.. Defaults to "welch".
+            fmin: Lower frequency bound. Defaults to 0.
+            fmax: Upper frequency bound. Defaults to 60.
+            picks: Channels to compute spectra for. Refer to :py:meth:`mne:mne.io.Raw.pick`.
+                Defaults to "eeg".
+            reject_by_annotation: Whether to not use the annotations for the spectra computation.
+                Defaults to True.
+            save: Whether to save the spectra in .h5 files. Defaults to False.
+            overwrite: Whether to overwrite the file. Defaults to False.
+            n_jobs: _description_. Defaults to -1.
+            verbose: _description_. Defaults to False.
+            **psd_kwargs: Additional arguments passed to :py:func:`mne:mne.time_frequency.psd_array_welch`
+                or :py:func:`mne:mne.time_frequency.psd_array_multitaper`.
+        """
+        from collections import defaultdict
+
+        psds = defaultdict([])
+        for pipe in self.pipes:
+            inst = pipe.mne_raw.copy().load_data()
+            if reference is not None:
+                inst.set_eeg_reference(ref_channels=reference)
+            for stage, stage_idx in sleep_stages.items():
+                psds[stage].append(
+                    SleepSpectrum(
+                        inst,
+                        hypno=pipe.hypno_up,
+                        stage_idx=stage_idx,
+                        method=method,
+                        fmin=fmin,
+                        fmax=fmax,
+                        tmin=None,
+                        tmax=None,
+                        picks=picks,
+                        proj=False,
+                        reject_by_annotation=reject_by_annotation,
+                        n_jobs=n_jobs,
+                        verbose=verbose,
+                        **psd_kwargs,
+                    )
+                )
+
+        for stage, psd in psds.items():
+            self.psds[stage] = np.mean(psd, axis=0)
+
+        if save:
+            import re
+
+            for stage, spectrum in self.psds.items():
+                stage = re.sub(r"[^\w\s-]", "_", stage)
+                spectrum.save(
+                    self.output_dir / self.__class__.__name__ / f"{stage}-psd.h5",
+                    overwrite=overwrite,
+                )
```

### Comparing `sleepeeg-0.2.0/sleepeeg.egg-info/PKG-INFO` & `sleepeeg-0.2.1/sleepeeg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepeeg
-Version: 0.2.0
+Version: 0.2.1
 Summary: Sleep EEG preprocessing and analysis
 Author-email: Gennadiy Belonosov <gennadiyb@mail.tau.ac.il>
 License: MIT
 Project-URL: Homepage, https://github.com/NirLab-TAU/sleepeeg
 Project-URL: Documentation, https://nirlab-tau.github.io/sleepeeg/
 Keywords: sleep,eeg
 Requires-Python: >=3.10
```

