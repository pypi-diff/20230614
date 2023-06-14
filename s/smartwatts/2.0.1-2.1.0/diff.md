# Comparing `tmp/smartwatts-2.0.1.tar.gz` & `tmp/smartwatts-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartwatts-2.0.1.tar", last modified: Fri Mar 24 10:30:09 2023, max compression
+gzip compressed data, was "smartwatts-2.1.0.tar", last modified: Fri May  5 13:35:15 2023, max compression
```

## Comparing `smartwatts-2.0.1.tar` & `smartwatts-2.1.0.tar`

### file list

```diff
@@ -1,37 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:30:09.769929 smartwatts-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-24 10:29:58.000000 smartwatts-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-24 10:30:09.769929 smartwatts-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-24 10:29:58.000000 smartwatts-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-03-24 10:30:09.769929 smartwatts-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-03-24 10:29:58.000000 smartwatts-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:30:09.765929 smartwatts-2.0.1/smartwatts/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-03-24 10:29:58.000000 smartwatts-2.0.1/smartwatts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-03-24 10:29:58.000000 smartwatts-2.0.1/smartwatts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-24 10:29:58.000000 smartwatts-2.0.1/smartwatts/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:30:09.769929 smartwatts-2.0.1/smartwatts/report/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-03-24 10:29:58.000000 smartwatts-2.0.1/smartwatts/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-03-24 10:29:58.000000 smartwatts-2.0.1/smartwatts/report/formula_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-03-24 10:29:58.000000 smartwatts-2.0.1/smartwatts/smartwatts_dispatcher_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-03-24 10:29:58.000000 smartwatts-2.0.1/smartwatts/smartwatts_formula_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18919 2023-03-24 10:29:58.000000 smartwatts-2.0.1/smartwatts/smartwatts_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-03-24 10:29:58.000000 smartwatts-2.0.1/smartwatts/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:30:09.765929 smartwatts-2.0.1/smartwatts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-24 10:30:09.000000 smartwatts-2.0.1/smartwatts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-24 10:30:09.000000 smartwatts-2.0.1/smartwatts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 10:30:09.000000 smartwatts-2.0.1/smartwatts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 10:30:09.000000 smartwatts-2.0.1/smartwatts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:30:09.000000 smartwatts-2.0.1/smartwatts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-24 10:30:09.000000 smartwatts-2.0.1/smartwatts.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:30:09.769929 smartwatts-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-24 10:29:58.000000 smartwatts-2.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:30:09.769929 smartwatts-2.0.1/tests/acceptation/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-24 10:29:58.000000 smartwatts-2.0.1/tests/acceptation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-03-24 10:29:58.000000 smartwatts-2.0.1/tests/acceptation/test_hwpc_report_with_mperf_to_zero_must_not_crash_the_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-03-24 10:29:58.000000 smartwatts-2.0.1/tests/acceptation/test_normal_behaviour.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:30:09.769929 smartwatts-2.0.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-24 10:29:58.000000 smartwatts-2.0.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-03-24 10:29:58.000000 smartwatts-2.0.1/tests/utils/acceptation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:30:09.769929 smartwatts-2.0.1/tests/utils/db/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-24 10:29:58.000000 smartwatts-2.0.1/tests/utils/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-03-24 10:29:58.000000 smartwatts-2.0.1/tests/utils/db/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)   140797 2023-03-24 10:29:58.000000 smartwatts-2.0.1/tests/utils/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:35:15.385504 smartwatts-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-05 13:35:00.000000 smartwatts-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-05-05 13:35:15.385504 smartwatts-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-05 13:35:00.000000 smartwatts-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-05 13:35:00.000000 smartwatts-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:35:15.385504 smartwatts-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:35:15.381504 smartwatts-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:35:15.381504 smartwatts-2.1.0/src/smartwatts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-05 13:35:00.000000 smartwatts-2.1.0/src/smartwatts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-05-05 13:35:00.000000 smartwatts-2.1.0/src/smartwatts/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:35:15.385504 smartwatts-2.1.0/src/smartwatts/actor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-05 13:35:00.000000 smartwatts-2.1.0/src/smartwatts/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-05 13:35:00.000000 smartwatts-2.1.0/src/smartwatts/actor/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-05 13:35:00.000000 smartwatts-2.1.0/src/smartwatts/actor/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:35:15.385504 smartwatts-2.1.0/src/smartwatts/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-05 13:35:00.000000 smartwatts-2.1.0/src/smartwatts/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-05 13:35:00.000000 smartwatts-2.1.0/src/smartwatts/cli/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-05 13:35:00.000000 smartwatts-2.1.0/src/smartwatts/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:35:15.385504 smartwatts-2.1.0/src/smartwatts/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-05 13:35:00.000000 smartwatts-2.1.0/src/smartwatts/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-05-05 13:35:00.000000 smartwatts-2.1.0/src/smartwatts/handler/hwpc_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:35:15.385504 smartwatts-2.1.0/src/smartwatts/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-05 13:35:00.000000 smartwatts-2.1.0/src/smartwatts/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-05 13:35:00.000000 smartwatts-2.1.0/src/smartwatts/model/cpu_topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-05 13:35:00.000000 smartwatts-2.1.0/src/smartwatts/model/power_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-05 13:35:00.000000 smartwatts-2.1.0/src/smartwatts/model/report_history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:35:15.385504 smartwatts-2.1.0/src/smartwatts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-05-05 13:35:15.000000 smartwatts-2.1.0/src/smartwatts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-05 13:35:15.000000 smartwatts-2.1.0/src/smartwatts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:35:15.000000 smartwatts-2.1.0/src/smartwatts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-05 13:35:15.000000 smartwatts-2.1.0/src/smartwatts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 13:35:15.000000 smartwatts-2.1.0/src/smartwatts.egg-info/top_level.txt
```

### Comparing `smartwatts-2.0.1/LICENSE` & `smartwatts-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartwatts-2.0.1/setup.py` & `smartwatts-2.1.0/src/smartwatts/handler/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,9 +23,12 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from setuptools import setup
-setup()
+from .hwpc_report import HwPCReportHandler
+
+__all__ = [
+    'HwPCReportHandler'
+]
```

### Comparing `smartwatts-2.0.1/smartwatts/__init__.py` & `smartwatts-2.1.0/src/smartwatts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.0.1"
+__version__ = "2.1.0"
```

### Comparing `smartwatts-2.0.1/smartwatts/exception.py` & `smartwatts-2.1.0/src/smartwatts/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+class InvalidConfigurationParameterException(Exception):
+    """
+    This exception happens when a user try to set an invalid configuration parameter.
+    """
+
+
 class PowerModelNotInitializedException(Exception):
     """
     This exception happens when a user try to compute a power estimation without having learned a power model.
     """
 
 
 class NotEnoughReportsInHistoryException(Exception):
```

### Comparing `smartwatts-2.0.1/smartwatts/report/__init__.py` & `smartwatts-2.1.0/src/smartwatts/cli/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,8 +23,12 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from smartwatts.report.formula_report import FormulaReport
+from .config_validator import SmartWattsConfigValidator
+
+__all__ = [
+    'SmartWattsConfigValidator'
+]
```

### Comparing `smartwatts-2.0.1/smartwatts/report/formula_report.py` & `smartwatts-2.1.0/src/smartwatts/model/report_history.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright (c) 2022, INRIA
-# Copyright (c) 2022, University of Lille
+# Copyright (c) 2023, INRIA
+# Copyright (c) 2023, University of Lille
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -23,57 +23,40 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from __future__ import annotations
+from collections import deque
+from typing import List
 
-from datetime import datetime
-from typing import Dict, Any
 
-from powerapi.report import Report
-
-
-class FormulaReport(Report):
+class ReportHistory:
     """
-    FormulaReport stores information about a formula.
-    This is useful to gather information about a running formula in order to debug or compute statistics.
+    This class stores the reports history to use when learning a new power model.
     """
 
-    def __init__(self, timestamp: datetime, sensor: str, target: str, metadata: Dict[str, Any]):
-        """
-        Initialize a Power report using the given parameters.
-        :param timestamp: Report timestamp
-        :param sensor: Sensor name
-        :param target: Target name
-        :param metadata: Metadata values, can be anything that add useful information
-        """
-        Report.__init__(self, timestamp, sensor, target)
-        self.metadata = metadata
-
-    def __repr__(self) -> str:
-        return 'FormulaReport(%s, %s, %s, %s)' % (self.timestamp, self.sensor, self.target, self.metadata)
-
-    @staticmethod
-    def from_json(data: Dict) -> FormulaReport:
+    def __init__(self, max_length: int):
         """
-        Generate a report using the given data.
-        :param data: Dictionary containing the report attributes
-        :return: The Formula report initialized with the given data
+        Initialize a new reports history container.
+        :param max_length: Maximum amount of samples to keep before overriding the oldest sample at insertion
         """
-        return FormulaReport(data['timestamp'], data['sensor'], data['target'], data['metadata'])
+        self.max_length = max_length
+        self.X = deque(maxlen=max_length)
+        self.y = deque(maxlen=max_length)
 
-    @staticmethod
-    def from_mongodb(data: Dict) -> FormulaReport:
+    def __len__(self) -> int:
         """
-        Cast from mongoDB
+        Compute the length of the history.
+        :return: Length of the history
         """
-        return FormulaReport.from_json(data)
+        return len(self.X)
 
-    @staticmethod
-    def to_mongodb(report: FormulaReport) -> Dict:
+    def store_report(self, power_reference: float, events_value: List[float]) -> None:
         """
-        Cast to mongoDB
+        Append a report to the report's history.
+        :param events_value: List of raw events value
+        :param power_reference: Power reference corresponding to the events value
         """
-        return report.__dict__
+        self.X.append(events_value)
+        self.y.append(power_reference)
```

### Comparing `smartwatts-2.0.1/smartwatts/smartwatts_handlers.py` & `smartwatts-2.1.0/src/smartwatts/handler/hwpc_report.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,172 +22,51 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-from collections import deque, OrderedDict, defaultdict
-from hashlib import sha1
+
+import itertools
+import logging
+from collections import OrderedDict, defaultdict
 from math import ldexp, fabs
-from pickle import dumps
 
-from powerapi.formula import FormulaPoisonPillMessageHandler
-from powerapi.formula.abstract_cpu_dram_formula import AbstractCpuDramFormulaState
 from powerapi.handler import Handler
-from powerapi.report import PowerReport, HWPCReport
+from powerapi.report import PowerReport, HWPCReport, FormulaReport
 from sklearn.exceptions import NotFittedError
-from sklearn.linear_model import ElasticNet as Regression
-
-from smartwatts.report import FormulaReport
-
-
-class History:
-    """
-    This class stores the reports history to use when learning a new power model.
-    """
-
-    def __init__(self, max_length):
-        """
-        Initialize a new reports history container.
-        :param max_length: Maximum amount of samples to keep before overriding the oldest sample at insertion
-        """
-        self.max_length = max_length
-        self.X = deque(maxlen=max_length)
-        self.y = deque(maxlen=max_length)
 
-    def __len__(self):
-        """
-        Compute the length of the history.
-        :return: Length of the history
-        """
-        return len(self.X)
-
-    def store_report(self, power_reference, events_value):
-        """
-        Append a report to the reports history.
-        :param events_value: List of raw events value
-        :param power_reference: Power reference corresponding to the events value
-        """
-        self.X.append(events_value)
-        self.y.append(power_reference)
+from smartwatts.model.power_model import PowerModel
 
 
-class PowerModel:
+class HwPCReportHandler(Handler):
     """
-    This Power model compute the power estimations and handle the learning of a new model when needed.
+    HwPC reports handler.
     """
 
-    def __init__(self, frequency, history_window_size):
-        """
-        Initialize a new power model.
-        :param frequency: Frequency of the power model
-        :param history_window_size: Size of the history window used to keep samples to learn from
-        """
-        self.frequency = frequency
-        self.model = Regression()
-        self.hash = 'uninitialized'
-        self.history = History(history_window_size)
-        self.id = 0
-
-    def learn_power_model(self, min_samples, min_intercept, max_intercept):
-        """
-        Learn a new power model using the stored reports and update the formula id/hash.
-        :param min_samples: Minimum amount of samples required to learn the power model
-        :param min_intercept: Minimum value allowed for the intercept of the model
-        :param max_intercept: Maximum value allowed for the intercept of the model
-        """
-        if len(self.history) < min_samples:
-            return
-
-        fit_intercept = len(self.history) == self.history.max_length
-        model = Regression(fit_intercept=fit_intercept, positive=True).fit(self.history.X, self.history.y)
-
-        # Discard the new model when the intercept is not in specified range
-        if not min_intercept <= model.intercept_ < max_intercept:
-            return
-
-        self.model = model
-        self.hash = sha1(dumps(self.model)).hexdigest()
-        self.id += 1
-
-    @staticmethod
-    def _extract_events_value(events):
-        """
-        Creates and return a list of events value from the events group.
-        :param events: Events group
-        :return: List containing the events value sorted by event name
-        """
-        return [value for _, value in sorted(events.items())]
-
-    def store_report_in_history(self, power_reference, events):
-        """
-        Store the events group into the System reports list and learn a new power model.
-        :param power_reference: Power reference (in Watt)
-        :param events: Events value
-        """
-        self.history.store_report(power_reference, self._extract_events_value(events))
-
-    def compute_power_estimation(self, events):
-        """
-        Compute a power estimation from the events value using the power model.
-        :param events: Events value
-        :raise: NotFittedError when the model haven't been fitted
-        :return: Power estimation for the given events value
-        """
-        return self.model.predict([self._extract_events_value(events)])[0]
-
-    def cap_power_estimation(self, raw_target_power, raw_global_power):
-        """
-        Cap target's power estimation to the global power estimation.
-        :param raw_target_power: Target power estimation from the power model (in Watt)
-        :param raw_global_power: Global power estimation from the power model (in Watt)
-        :return: Capped power estimation (in Watt) with its ratio over global power consumption
-        """
-        target_power = raw_target_power - self.model.intercept_
-        global_power = raw_global_power - self.model.intercept_
-
-        ratio = target_power / global_power if global_power > 0.0 and target_power > 0.0 else 0.0
-        power = target_power if target_power > 0.0 else 0.0
-        return power, ratio
-
-    def apply_intercept_share(self, target_power, target_ratio):
-        """
-        Apply the target's share of intercept from its ratio from the global power consumption.
-        :param target_power: Target power estimation (in Watt)
-        :param target_ratio: Target ratio over the global power consumption
-        :return: Target power estimation including intercept (in Watt) and ratio over global power consumption
-        """
-        intercept = target_ratio * self.model.intercept_
-        return target_power + intercept
-
-
-class ReportHandler(Handler):
-    """
-    Handler behaviour for HWPC Reports
-    """
-
-    def __init__(self, state: AbstractCpuDramFormulaState):
-        Handler.__init__(self, state=state)
+    def __init__(self, state):
+        Handler.__init__(self, state)
         self.models = self._gen_models_dict()
+        self.ticks = OrderedDict()
 
     def _gen_models_dict(self):
         """
         Generate and returns a layered container to store per-frequency power models
         :return: Initialized Ordered dict containing a power model for each frequency layer
         """
         return OrderedDict(
             (freq, PowerModel(freq, self.state.config.history_window_size)) for freq
             in self.state.config.cpu_topology.get_supported_frequencies())
 
     def _get_frequency_layer(self, frequency):
         """
         Find and returns the nearest frequency layer for the given frequency.
         :param frequency: CPU frequency
-        :return: Nearest frequency layer for the given frequency
+        :return: The nearest frequency layer for the given frequency
         """
         last_layer_freq = 0
         for current_layer_freq in self.models.keys():
             if frequency < current_layer_freq:
                 return last_layer_freq
             last_layer_freq = current_layer_freq
 
@@ -205,66 +84,51 @@
         """
         Fetch the suitable power model for the current frequency.
         :param system_core: Core events group of System target
         :return: Power model to use for the current frequency
         """
         return self.models[self._get_frequency_layer(self.compute_pkg_frequency(system_core))]
 
-    def handle(self, message: HWPCReport):
+    def handle(self, msg: HWPCReport):
 
         """
          Process a HWPC report and send the result(s) to a pusher actor.
-         :param message: Received message
+         :param msg: Received message
         """
-        self.state.actor.logger.debug('received message ' + str(message))
-        self.state.ticks.setdefault(message.timestamp, {}).update({message.target: message})
+        logging.debug('received message: %s', msg)
+        self.ticks.setdefault(msg.timestamp, {}).update({msg.target: msg})
 
-        # start to process the oldest tick only after receiving at least 5 ticks.
-        # we wait before processing the ticks in order to mitigate the possible delay of the sensor/database.
-        if self.state.config.real_time_mode:
-            if len(self.state.ticks) > 2:
-                power_reports, formula_reports = self._process_oldest_tick()
-                for report in power_reports:
-                    for name, pusher in self.state.pushers.items():
-                        pusher.send_data(report)
-                        self.state.actor.logger.debug('send ' + str(report) + ' to ' + name)
-                for report in formula_reports:
-                    for name, pusher in self.state.formula_pushers.items():
-                        pusher.send_data(report)
-                        self.state.actor.logger.debug('send ' + str(report) + ' to ' + name)
-
-        else:
-            if len(self.state.ticks) > 5:
-                power_reports, formula_reports = self._process_oldest_tick()
-                for report in power_reports:
-                    for name, pusher in self.state.pushers.items():
-                        pusher.send_data(report)
-                        self.state.actor.logger.debug('send ' + str(report) + ' to ' + name)
-                for report in formula_reports:
-                    for name, pusher in self.state.formula_pushers.items():
+        # Start to process the oldest tick only after receiving at least 5 ticks.
+        # We wait before processing the ticks in order to mitigate the possible delay between the sensor/database.
+        if len(self.ticks) > 5:
+            power_reports, formula_reports = self._process_oldest_tick()
+            for report in itertools.chain(power_reports, formula_reports):
+                for name, pusher in self.state.pushers.items():
+                    if isinstance(report, pusher.state.report_model):
                         pusher.send_data(report)
-                        self.state.actor.logger.debug('send ' + str(report) + ' to ' + name)
+                        logging.debug('sent report: %s to %s', report, name)
 
     def _process_oldest_tick(self):
         """
         Process the oldest tick stored in the stack and generate power reports for the running target(s).
         :return: Power reports of the running target(s)
         """
-        timestamp, hwpc_reports = self.state.ticks.popitem(last=False)
+        timestamp, hwpc_reports = self.ticks.popitem(last=False)
 
         # reports of the current tick
         power_reports = []
         formula_reports = []
 
         # prepare required events group of Global target
         try:
             global_report = hwpc_reports.pop('all')
         except KeyError:
             # cannot process this tick without the reference measurements
             return power_reports, formula_reports
+
         rapl = self._gen_rapl_events_group(global_report)
         avg_msr = self._gen_msr_events_group(global_report)
         global_core = self._gen_agg_core_report_from_running_targets(hwpc_reports)
 
         # compute RAPL power report
         rapl_power = rapl[self.state.config.rapl_event]
         power_reports.append(
@@ -288,18 +152,16 @@
         except NotFittedError:
             model.store_report_in_history(rapl_power, global_core)
             model.learn_power_model(self.state.config.min_samples_required, 0.0, self.state.config.cpu_topology.tdp)
             return power_reports, formula_reports
 
         # compute per-target power report
         for target_name, target_report in hwpc_reports.items():
-            target_core = self._gen_core_events_group(target_report)
-            raw_target_power = model.compute_power_estimation(target_core)
+            raw_target_power = model.compute_power_estimation(self._gen_core_events_group(target_report))
             target_power, target_ratio = model.cap_power_estimation(raw_target_power, raw_global_power)
-            target_power = model.apply_intercept_share(target_power, target_ratio)
             power_reports.append(
                 self._gen_power_report(
                     timestamp,
                     target_name,
                     model.hash,
                     raw_target_power,
                     target_power,
@@ -407,18 +269,7 @@
         """
         agg_core_events_group = defaultdict(int)
         for _, target_report in targets_report.items():
             for event_name, event_value in self._gen_core_events_group(target_report).items():
                 agg_core_events_group[event_name] += event_value
 
         return agg_core_events_group
-
-
-class SmartWattsFormulaPoisonPillMessageHandler(FormulaPoisonPillMessageHandler):
-    """
-    Smartwatts Handler for dealing with PoisonPillMessage
-    """
-
-    def teardown(self, soft=False):
-        FormulaPoisonPillMessageHandler.teardown(self, soft=soft)
-        for pusher in self.state.formula_pushers:
-            pusher.socket_interface.close()
```

### Comparing `smartwatts-2.0.1/smartwatts/topology.py` & `smartwatts-2.1.0/src/smartwatts/model/cpu_topology.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,54 +23,57 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from typing import List
+
+
 class CPUTopology:
     """
     This class stores the necessary information about the CPU topology.
     """
 
-    def __init__(self, tdp, freq_bclk, ratio_min, ratio_base, ratio_max):
+    def __init__(self, tdp: int, freq_bclk: float, ratio_min: int, ratio_base: int, ratio_max: int):
         """
         Create a new CPU topology object.
         :param tdp: TDP of the CPU in Watt
         :param freq_bclk: Base clock in MHz
         :param ratio_min: Maximum efficiency ratio
         :param ratio_base: Base frequency ratio
         :param ratio_max: Maximum frequency ratio (with Turbo-Boost)
         """
         self.tdp = tdp
         self.freq_bclk = freq_bclk
         self.ratio_min = ratio_min
         self.ratio_base = ratio_base
         self.ratio_max = ratio_max
 
-    def get_min_frequency(self):
+    def get_min_frequency(self) -> float:
         """
         Compute and return the CPU max efficiency frequency.
         :return: The CPU max efficiency frequency in MHz
         """
         return self.freq_bclk * self.ratio_min
 
-    def get_base_frequency(self):
+    def get_base_frequency(self) -> float:
         """
         Compute and return the CPU base frequency.
         :return: The CPU base frequency in MHz
         """
         return self.freq_bclk * self.ratio_base
 
-    def get_max_frequency(self):
+    def get_max_frequency(self) -> float:
         """
         Compute and return the CPU maximum frequency. (Turbo-Boost included)
         :return: The CPU maximum frequency in MHz
         """
         return self.freq_bclk * self.ratio_max
 
-    def get_supported_frequencies(self):
+    def get_supported_frequencies(self) -> List[float]:
         """
         Compute the supported frequencies for this CPU.
         :return: A list of supported frequencies in MHz
         """
-        return list(range(self.get_min_frequency(), self.get_max_frequency() + 1, self.freq_bclk))
+        return [ratio * self.freq_bclk for ratio in range(self.ratio_min, self.ratio_max + 1)]
```

### Comparing `smartwatts-2.0.1/tests/__init__.py` & `smartwatts-2.1.0/src/smartwatts/model/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,7 +22,17 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+from .cpu_topology import CPUTopology
+from .report_history import ReportHistory
+from .power_model import PowerModel
+
+__all__ = [
+    'CPUTopology',
+    'ReportHistory',
+    'PowerModel'
+]
```

### Comparing `smartwatts-2.0.1/tests/acceptation/__init__.py` & `smartwatts-2.1.0/src/smartwatts/actor/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,7 +22,17 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+from .actor import SmartWattsFormulaActor, SmartWattsFormulaState
+from .config import SmartWattsFormulaConfig, SmartWattsFormulaScope
+
+__all__ = [
+    'SmartWattsFormulaActor',
+    'SmartWattsFormulaState',
+    'SmartWattsFormulaConfig',
+    'SmartWattsFormulaScope'
+]
```

### Comparing `smartwatts-2.0.1/tests/acceptation/test_hwpc_report_with_mperf_to_zero_must_not_crash_the_system.py` & `smartwatts-2.1.0/src/smartwatts/actor/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,38 +23,43 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-# pylint: disable=redefined-outer-name,unused-import
-"""
-Run smartwatts on a mongodb database that contain 10 hwpc report per target
-
-- all
-- mongodb
-- influxdb
-- sensor
-The first hwpc report contains mperf value equals to 0
-Test if the system don't crash after receiving the first report and deal with the other report
-"""
-import pytest
+from enum import Enum
 
-from tests.utils.acceptation import AbstractAcceptationTest
-from tests.utils.reports import smartwatts_timeline_with_mperf_0, smartwatts_timeline
 
-
-@pytest.fixture
-def mongodb_content(smartwatts_timeline_with_mperf_0):
+class SmartWattsFormulaScope(Enum):
     """
-    Define the content of the input database
-    :param smartwatts_timeline_with_mperf_0: The content of the database. One of the reports has mperf=0
-    :return: The content of the database
+    Enum used to set the scope of the SmartWatts formula.
     """
-    return smartwatts_timeline_with_mperf_0
+    CPU = "cpu"
+    DRAM = "dram"
 
 
-class TestSmartwattsFormulaWithMperf0(AbstractAcceptationTest):
+class SmartWattsFormulaConfig:
     """
-    Execute acceptation test for SmartwattsFormula by using MPERF = 0
+    Global config of the SmartWatts formula.
     """
+
+    def __init__(self, scope, reports_frequency, rapl_event, error_threshold, cpu_topology, min_samples_required,
+                 history_window_size, real_time_mode):
+        """
+        Initialize a new formula config object.
+        :param scope: Scope of the formula
+        :param reports_frequency: Frequency at which the reports (in milliseconds)
+        :param rapl_event: RAPL event to use as reference
+        :param error_threshold: Error threshold (in Watt)
+        :param cpu_topology: Topology of the CPU
+        :param min_samples_required: Minimum amount of samples required before trying to learn a power model
+        :param history_window_size: Size of the history window used to keep samples to learn from
+        """
+        self.scope = scope
+        self.reports_frequency = reports_frequency
+        self.rapl_event = rapl_event
+        self.error_threshold = error_threshold
+        self.cpu_topology = cpu_topology
+        self.min_samples_required = min_samples_required
+        self.history_window_size = history_window_size
+        self.real_time_mode = real_time_mode
```

