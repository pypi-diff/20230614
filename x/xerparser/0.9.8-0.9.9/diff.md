# Comparing `tmp/xerparser-0.9.8.tar.gz` & `tmp/xerparser-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xerparser-0.9.8.tar", max compression
+gzip compressed data, was "xerparser-0.9.9.tar", max compression
```

## Comparing `xerparser-0.9.8.tar` & `xerparser-0.9.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35149 2022-12-03 05:25:25.921903 xerparser-0.9.8/LICENSE
--rw-r--r--   0        0        0     5337 2023-04-19 13:53:53.195483 xerparser-0.9.8/README.md
--rw-r--r--   0        0        0      743 2023-05-24 14:27:09.133625 xerparser-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      962 2023-05-24 14:29:38.233531 xerparser-0.9.8/xerparser/__init__.py
--rw-r--r--   0        0        0      465 2023-03-01 00:04:03.499449 xerparser-0.9.8/xerparser/schemas/__init__.py
--rw-r--r--   0        0        0     2643 2023-03-01 00:04:28.289431 xerparser-0.9.8/xerparser/schemas/account.py
--rw-r--r--   0        0        0     3247 2023-02-06 03:09:28.587242 xerparser-0.9.8/xerparser/schemas/actvcode.py
--rw-r--r--   0        0        0     1547 2023-01-25 01:32:05.201004 xerparser-0.9.8/xerparser/schemas/actvtype.py
--rw-r--r--   0        0        0    11154 2023-03-01 03:39:04.104780 xerparser-0.9.8/xerparser/schemas/calendars.py
--rw-r--r--   0        0        0      957 2023-03-01 00:04:28.289431 xerparser-0.9.8/xerparser/schemas/ermhdr.py
--rw-r--r--   0        0        0     1367 2023-01-25 01:32:05.211004 xerparser-0.9.8/xerparser/schemas/findates.py
--rw-r--r--   0        0        0      749 2023-01-16 21:15:50.835852 xerparser-0.9.8/xerparser/schemas/memotype.py
--rw-r--r--   0        0        0     1094 2023-02-26 04:48:17.672946 xerparser-0.9.8/xerparser/schemas/pcattype.py
--rw-r--r--   0        0        0     3227 2023-02-26 04:48:17.672946 xerparser-0.9.8/xerparser/schemas/pcatval.py
--rw-r--r--   0        0        0     9136 2023-05-14 15:40:28.944059 xerparser-0.9.8/xerparser/schemas/project.py
--rw-r--r--   0        0        0     2897 2023-03-01 00:04:03.499449 xerparser-0.9.8/xerparser/schemas/projwbs.py
--rw-r--r--   0        0        0     1103 2023-03-01 00:04:03.499449 xerparser-0.9.8/xerparser/schemas/rsrc.py
--rw-r--r--   0        0        0     2970 2023-03-01 00:04:28.289431 xerparser-0.9.8/xerparser/schemas/schedoptions.py
--rw-r--r--   0        0        0    16706 2023-05-24 13:28:30.701948 xerparser-0.9.8/xerparser/schemas/task.py
--rw-r--r--   0        0        0     1462 2023-03-06 00:43:40.451659 xerparser-0.9.8/xerparser/schemas/taskfin.py
--rw-r--r--   0        0        0      805 2022-12-26 20:40:30.667590 xerparser-0.9.8/xerparser/schemas/taskmemo.py
--rw-r--r--   0        0        0     2039 2023-05-24 14:27:09.133625 xerparser-0.9.8/xerparser/schemas/taskpred.py
--rw-r--r--   0        0        0     5063 2023-03-17 20:28:16.137376 xerparser-0.9.8/xerparser/schemas/taskrsrc.py
--rw-r--r--   0        0        0     1927 2023-01-25 01:32:05.211004 xerparser-0.9.8/xerparser/schemas/trsrcfin.py
--rw-r--r--   0        0        0     1524 2023-03-01 00:04:03.499449 xerparser-0.9.8/xerparser/schemas/udftype.py
--rw-r--r--   0        0        0        0 2022-12-21 14:16:15.278744 xerparser-0.9.8/xerparser/scripts/__init__.py
--rw-r--r--   0        0        0     1548 2022-12-30 22:42:20.878909 xerparser-0.9.8/xerparser/scripts/dates.py
--rw-r--r--   0        0        0      402 2023-01-25 01:32:05.211004 xerparser-0.9.8/xerparser/scripts/decorators.py
--rw-r--r--   0        0        0        0 2022-12-21 14:16:15.278744 xerparser-0.9.8/xerparser/src/__init__.py
--rw-r--r--   0        0        0     2851 2023-04-08 15:29:35.029582 xerparser-0.9.8/xerparser/src/errors.py
--rw-r--r--   0        0        0     2377 2023-04-08 15:29:35.029582 xerparser-0.9.8/xerparser/src/parser.py
--rw-r--r--   0        0        0      883 2023-05-24 14:27:09.133625 xerparser-0.9.8/xerparser/src/validators.py
--rw-r--r--   0        0        0    10822 2023-05-14 15:40:28.944059 xerparser-0.9.8/xerparser/src/xer.py
--rw-r--r--   0        0        0     6062 1970-01-01 00:00:00.000000 xerparser-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-03 05:25:25.921903 xerparser-0.9.9/LICENSE
+-rw-r--r--   0        0        0     5337 2023-04-19 13:53:53.195483 xerparser-0.9.9/README.md
+-rw-r--r--   0        0        0      743 2023-06-14 20:49:09.061050 xerparser-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0      962 2023-06-14 20:49:09.061050 xerparser-0.9.9/xerparser/__init__.py
+-rw-r--r--   0        0        0      465 2023-03-01 00:04:03.499449 xerparser-0.9.9/xerparser/schemas/__init__.py
+-rw-r--r--   0        0        0     2643 2023-03-01 00:04:28.289431 xerparser-0.9.9/xerparser/schemas/account.py
+-rw-r--r--   0        0        0     3247 2023-02-06 03:09:28.587242 xerparser-0.9.9/xerparser/schemas/actvcode.py
+-rw-r--r--   0        0        0     1547 2023-01-25 01:32:05.201004 xerparser-0.9.9/xerparser/schemas/actvtype.py
+-rw-r--r--   0        0        0    11154 2023-03-01 03:39:04.104780 xerparser-0.9.9/xerparser/schemas/calendars.py
+-rw-r--r--   0        0        0      957 2023-03-01 00:04:28.289431 xerparser-0.9.9/xerparser/schemas/ermhdr.py
+-rw-r--r--   0        0        0     1367 2023-01-25 01:32:05.211004 xerparser-0.9.9/xerparser/schemas/findates.py
+-rw-r--r--   0        0        0      749 2023-01-16 21:15:50.835852 xerparser-0.9.9/xerparser/schemas/memotype.py
+-rw-r--r--   0        0        0     1094 2023-02-26 04:48:17.672946 xerparser-0.9.9/xerparser/schemas/pcattype.py
+-rw-r--r--   0        0        0     3269 2023-06-14 20:49:09.061050 xerparser-0.9.9/xerparser/schemas/pcatval.py
+-rw-r--r--   0        0        0     8970 2023-06-14 20:49:09.061050 xerparser-0.9.9/xerparser/schemas/project.py
+-rw-r--r--   0        0        0     2897 2023-03-01 00:04:03.499449 xerparser-0.9.9/xerparser/schemas/projwbs.py
+-rw-r--r--   0        0        0     1103 2023-03-01 00:04:03.499449 xerparser-0.9.9/xerparser/schemas/rsrc.py
+-rw-r--r--   0        0        0     2970 2023-03-01 00:04:28.289431 xerparser-0.9.9/xerparser/schemas/schedoptions.py
+-rw-r--r--   0        0        0    16866 2023-06-14 20:49:09.071050 xerparser-0.9.9/xerparser/schemas/task.py
+-rw-r--r--   0        0        0     1462 2023-03-06 00:43:40.451659 xerparser-0.9.9/xerparser/schemas/taskfin.py
+-rw-r--r--   0        0        0      805 2022-12-26 20:40:30.667590 xerparser-0.9.9/xerparser/schemas/taskmemo.py
+-rw-r--r--   0        0        0     2039 2023-05-24 14:27:09.133625 xerparser-0.9.9/xerparser/schemas/taskpred.py
+-rw-r--r--   0        0        0     5063 2023-03-17 20:28:16.137376 xerparser-0.9.9/xerparser/schemas/taskrsrc.py
+-rw-r--r--   0        0        0     1927 2023-01-25 01:32:05.211004 xerparser-0.9.9/xerparser/schemas/trsrcfin.py
+-rw-r--r--   0        0        0     1524 2023-03-01 00:04:03.499449 xerparser-0.9.9/xerparser/schemas/udftype.py
+-rw-r--r--   0        0        0        0 2022-12-21 14:16:15.278744 xerparser-0.9.9/xerparser/scripts/__init__.py
+-rw-r--r--   0        0        0     1548 2022-12-30 22:42:20.878909 xerparser-0.9.9/xerparser/scripts/dates.py
+-rw-r--r--   0        0        0      402 2023-01-25 01:32:05.211004 xerparser-0.9.9/xerparser/scripts/decorators.py
+-rw-r--r--   0        0        0        0 2022-12-21 14:16:15.278744 xerparser-0.9.9/xerparser/src/__init__.py
+-rw-r--r--   0        0        0     2851 2023-04-08 15:29:35.029582 xerparser-0.9.9/xerparser/src/errors.py
+-rw-r--r--   0        0        0     2377 2023-04-08 15:29:35.029582 xerparser-0.9.9/xerparser/src/parser.py
+-rw-r--r--   0        0        0      883 2023-05-24 14:27:09.133625 xerparser-0.9.9/xerparser/src/validators.py
+-rw-r--r--   0        0        0    10822 2023-05-14 15:40:28.944059 xerparser-0.9.9/xerparser/src/xer.py
+-rw-r--r--   0        0        0     6062 1970-01-01 00:00:00.000000 xerparser-0.9.9/PKG-INFO
```

### Comparing `xerparser-0.9.8/LICENSE` & `xerparser-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/README.md` & `xerparser-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/pyproject.toml` & `xerparser-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xerparser"
-version = "0.9.8"
+version = "0.9.9"
 description = "Parse a P6 .xer file to a Python object."
 authors = ["Jesse <code@seqmanagement.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 keywords = ["primavera", "p6", "xer", "schedule", "scheduling", "planning", "project management", "project controls"]
 repository = "https://github.com/jjCode01/xerparser"
```

### Comparing `xerparser-0.9.8/xerparser/__init__.py` & `xerparser-0.9.9/xerparser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 from xerparser.src.errors import find_xer_errors, CorruptXerFile
 from xerparser.src.parser import parser, file_reader
 from xerparser.src.xer import Xer
 from xerparser.schemas.actvcode import ACTVCODE
 from xerparser.schemas.actvtype import ACTVTYPE
 from xerparser.schemas.calendars import CALENDAR
```

### Comparing `xerparser-0.9.8/xerparser/schemas/account.py` & `xerparser-0.9.9/xerparser/schemas/account.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/schemas/actvcode.py` & `xerparser-0.9.9/xerparser/schemas/actvcode.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/schemas/actvtype.py` & `xerparser-0.9.9/xerparser/schemas/actvtype.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/schemas/calendars.py` & `xerparser-0.9.9/xerparser/schemas/calendars.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/schemas/ermhdr.py` & `xerparser-0.9.9/xerparser/schemas/ermhdr.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/schemas/findates.py` & `xerparser-0.9.9/xerparser/schemas/findates.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/schemas/memotype.py` & `xerparser-0.9.9/xerparser/schemas/memotype.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/schemas/pcattype.py` & `xerparser-0.9.9/xerparser/schemas/pcattype.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/schemas/pcatval.py` & `xerparser-0.9.9/xerparser/schemas/pcatval.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,27 +77,27 @@
     @parent.setter
     def parent(self, value: Optional["PCATVAL"]) -> None:
         if value is None:
             self._parent = None
         else:
             if not isinstance(value, PCATVAL):
                 raise ValueError(
-                    f"ValueError: expected <class PCATVAL> for parent, got {type(value)}."
+                    f"ValueError: expected <class PCATVAL> for parent, got {type(value)}."  # noqa: E501
                 )
             if value.uid != self.parent_proj_catg_id:
                 raise ValueError(
-                    f"ValueError: Parent ID {value.uid} does not match parent_actv_code_id {self.parent_proj_catg_id}"
+                    f"ValueError: Parent ID {value.uid} does not match parent_actv_code_id {self.parent_proj_catg_id}"  # noqa: E501
                 )
 
             self._parent = value
 
     def _valid_pcattype(self, value: PCATTYPE) -> PCATTYPE:
         """Validate Activity Code Type"""
         if not isinstance(value, PCATTYPE):
             raise ValueError(
                 f"ValueError: expected <class PCATTYPE>; got {type(value)}"
             )
         if value.uid != self.proj_catg_type_id:
             raise ValueError(
-                f"ValueError: Unique ID {value.uid} does not match proj_catg_type_id {self.proj_catg_type_id}"
+                f"ValueError: Unique ID {value.uid} does not match proj_catg_type_id {self.proj_catg_type_id}"  # noqa: E501
             )
         return value
```

### Comparing `xerparser-0.9.8/xerparser/schemas/project.py` & `xerparser-0.9.9/xerparser/schemas/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,14 @@
             return self.wbs_by_path.get(obj.full_code)
 
     @cached_property
     @rounded()
     def actual_cost(self) -> float:
         """Sum of task resource actual costs"""
         return sum(res.act_total_cost for res in self.resources)
-        # return sum(task.actual_cost for task in self.tasks)
 
     @property
     def actual_duration(self) -> int:
         """Project actual duration in calendar days from start date to data date"""
         return max((0, (self.data_date - self.actual_start).days))
 
     @cached_property
@@ -141,15 +140,14 @@
         return min((task.start for task in self.tasks))
 
     @cached_property
     @rounded()
     def budgeted_cost(self) -> float:
         """Sum of task resource budgeted costs"""
         return sum(res.target_cost for res in self.resources)
-        # return sum(task.budgeted_cost for task in self.tasks)
 
     @property
     @rounded(ndigits=4)
     def duration_percent(self) -> float:
         """Project duration percent complete"""
         if self.original_duration == 0:
             return 0.0
@@ -194,30 +192,33 @@
         return {hash(rel): rel for rel in self.relationships}
 
     @cached_property
     @rounded()
     def remaining_cost(self) -> float:
         """Sum of task resource remaining costs"""
         return sum(res.remain_cost for res in self.resources)
-        # return sum(task.remaining_cost for task in self.tasks)
 
     @property
     def remaining_duration(self) -> int:
         """Project remaining duration in calendar days from data date to finish date"""
         return max((0, (self.finish_date - self.data_date).days))
 
     @cached_property
     @rounded(ndigits=4)
     def task_percent(self) -> float:
         """Calculated Project percent complete based on task updates"""
         if not self.tasks:
             return 0.0
 
-        orig_dur_sum = sum(task.original_duration for task in self.tasks)
-        rem_dur_sum = sum(task.remaining_duration for task in self.tasks)
+        orig_dur_sum = sum(
+            task.original_duration for task in self.tasks if not task.type.is_loe
+        )
+        rem_dur_sum = sum(
+            task.remaining_duration for task in self.tasks if not task.type.is_loe
+        )
         task_dur_percent = 1 - rem_dur_sum / orig_dur_sum if orig_dur_sum else 0.0
 
         status_cnt = Counter([t.status for t in self.tasks])
         status_percent = (
             status_cnt[TASK.TaskStatus.TK_Active] / 2
             + status_cnt[TASK.TaskStatus.TK_Complete]
         ) / len(self.tasks)
@@ -229,15 +230,14 @@
         return {task.task_code: task for task in self.tasks}
 
     @cached_property
     @rounded()
     def this_period_cost(self) -> float:
         """Sum of task resource this period costs"""
         return sum(res.act_this_per_cost for res in self.resources)
-        # return sum(task.this_period_cost for task in self.tasks)
 
     @cached_property
     def wbs_by_path(self) -> dict[str, PROJWBS]:
         return {node.full_code: node for node in self.wbs_nodes}
 
     def planned_progress(self, before_date: datetime) -> dict[str, list[TASK]]:
         """All planned progress through a given date.
```

### Comparing `xerparser-0.9.8/xerparser/schemas/projwbs.py` & `xerparser-0.9.9/xerparser/schemas/projwbs.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/schemas/rsrc.py` & `xerparser-0.9.9/xerparser/schemas/rsrc.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/schemas/schedoptions.py` & `xerparser-0.9.9/xerparser/schemas/schedoptions.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/schemas/task.py` & `xerparser-0.9.9/xerparser/schemas/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,15 +232,16 @@
                 "date": self.cstr_date2,
             },
         }
 
     @property
     def duration(self) -> int:
         """
-        Returns remaining duration if task is not started; otherwise, returns original duration.
+        Returns remaining duration if task is not started;
+        otherwise, returns original duration.
         """
         # This is usefull when the remaining duration is unlinked from the
         # original duration in the project settings
         # In these cases, the remaining duration can be different from the
         # original duration in tasks that have not started.
 
         if self.status.is_not_started:
@@ -314,17 +315,21 @@
         if self.remain_drtn_hr_cnt is None:
             return 0
         return int(self.remain_drtn_hr_cnt / 8)
 
     def rem_hours_per_day(self, late_dates=False) -> dict[datetime, float]:
         """
         Calculate the remaining workhours per day for a task.
-        Will only return valid workdays in a list of tuples containing the date and workhour values.
+        Will only return valid workdays in a list of tuples containing
+        the date and workhour values.
         This is usefull for calculating projections like cash flow.
 
+        P6 calculates remaining duration based on hours rather than days,
+        So the start and/or finish date for an activity may be a partial day.
+
         Returns:
             dict[datetime, float]: date and workhour pairs
         """
         if self.remain_drtn_hr_cnt == 0:
             return {}
 
         if self.status.is_completed or not self.restart_date:
@@ -346,17 +351,17 @@
                 start_date, start_date.time(), end_date.time()
             )
             return {clean_date(start_date): round(work_hrs, 3)}
 
         # Get a list of all workdays between the start and end dates
         date_range = list(self.calendar.iter_workdays(start_date, end_date))
 
-        # edge cases that only 1 valid workday between start date and end date
-        # these may never actually occur since the dates are pulled directly from the schedule
-        # did not find any case where these occur in testing, but leaving it just in case
+        # edge cases that only 1 valid workday between start date and end date these
+        # may never actually occur since the dates are pulled directly from the schedule
+        # did not find any case where these occur in testing, but leaving anyway
         if len(date_range) == 1 and end_date.date() > start_date.date():
             if start_date.date() == date_range[0].date():
                 work_day = self.calendar._get_workday(start_date)
                 work_hrs = self.calendar._calc_work_hours(
                     start_date, start_date.time(), work_day.finish
                 )
                 return {clean_date(start_date): round(work_hrs, 3)}
```

### Comparing `xerparser-0.9.8/xerparser/schemas/taskfin.py` & `xerparser-0.9.9/xerparser/schemas/taskfin.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/schemas/taskmemo.py` & `xerparser-0.9.9/xerparser/schemas/taskmemo.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/schemas/taskpred.py` & `xerparser-0.9.9/xerparser/schemas/taskpred.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/schemas/taskrsrc.py` & `xerparser-0.9.9/xerparser/schemas/taskrsrc.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/schemas/trsrcfin.py` & `xerparser-0.9.9/xerparser/schemas/trsrcfin.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/schemas/udftype.py` & `xerparser-0.9.9/xerparser/schemas/udftype.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/scripts/dates.py` & `xerparser-0.9.9/xerparser/scripts/dates.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/src/errors.py` & `xerparser-0.9.9/xerparser/src/errors.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/src/parser.py` & `xerparser-0.9.9/xerparser/src/parser.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/src/validators.py` & `xerparser-0.9.9/xerparser/src/validators.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/xerparser/src/xer.py` & `xerparser-0.9.9/xerparser/src/xer.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.8/PKG-INFO` & `xerparser-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xerparser
-Version: 0.9.8
+Version: 0.9.9
 Summary: Parse a P6 .xer file to a Python object.
 Home-page: https://github.com/jjCode01/xerparser
 License: GPL-3.0-only
 Keywords: primavera,p6,xer,schedule,scheduling,planning,project management,project controls
 Author: Jesse
 Author-email: code@seqmanagement.com
 Requires-Python: >=3.10,<4.0
```

