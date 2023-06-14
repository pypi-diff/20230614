# Comparing `tmp/rv_ltl-0.1.0a1.tar.gz` & `tmp/rv_ltl-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rv_ltl-0.1.0a1.tar", max compression
+gzip compressed data, was "rv_ltl-0.1.0a2.tar", max compression
```

## Comparing `rv_ltl-0.1.0a1.tar` & `rv_ltl-0.1.0a2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      405 2022-02-27 00:25:51.740006 rv_ltl-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      250 2022-02-27 00:19:39.605178 rv_ltl-0.1.0a1/rv_ltl/__init__.py
--rw-r--r--   0        0        0     1387 2022-01-29 11:16:47.461987 rv_ltl-0.1.0a1/rv_ltl/b4.py
--rw-r--r--   0        0        0      774 2022-02-27 00:18:00.638281 rv_ltl-0.1.0a1/rv_ltl/exceptions.py
--rw-r--r--   0        0        0     6352 2022-02-27 00:18:00.638581 rv_ltl-0.1.0a1/rv_ltl/monitor.py
--rw-r--r--   0        0        0     3059 2022-02-27 00:18:00.638866 rv_ltl-0.1.0a1/rv_ltl/proposition.py
--rw-r--r--   0        0        0      488 2022-02-27 00:27:47.567169 rv_ltl-0.1.0a1/setup.py
--rw-r--r--   0        0        0      388 2022-02-27 00:27:47.567309 rv_ltl-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0      424 2023-04-24 18:52:23.936715 rv_ltl-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     2709 2023-04-24 18:52:23.940716 rv_ltl-0.1.0a2/rv_ltl/README.md
+-rw-r--r--   0        0        0      383 2023-04-24 18:52:23.940716 rv_ltl-0.1.0a2/rv_ltl/__init__.py
+-rw-r--r--   0        0        0     1425 2023-04-24 18:52:23.940716 rv_ltl-0.1.0a2/rv_ltl/b4.py
+-rw-r--r--   0        0        0      821 2023-04-24 18:52:23.940716 rv_ltl-0.1.0a2/rv_ltl/exception.py
+-rw-r--r--   0        0        0     6616 2023-04-24 18:52:23.940716 rv_ltl-0.1.0a2/rv_ltl/monitor.py
+-rw-r--r--   0        0        0     3275 2023-04-24 18:52:23.940716 rv_ltl-0.1.0a2/rv_ltl/proposition.py
+-rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 rv_ltl-0.1.0a2/PKG-INFO
```

### Comparing `rv_ltl-0.1.0a1/rv_ltl/b4.py` & `rv_ltl-0.1.0a2/rv_ltl/b4.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"Provides four-valued boolean value"
+
 from enum import unique, Enum
 
 
 @unique
 class B4(Enum):
     """
     B4 represents a four-value boolean used in RV-LTL
```

### Comparing `rv_ltl-0.1.0a1/rv_ltl/exceptions.py` & `rv_ltl-0.1.0a2/rv_ltl/exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"Exceptions that are used across the package"
+
 from typing import Set
 
 
 class MissingAtomicsException(Exception):
     """
     raised when `update` is called with state that does not contain all atomic
     propositions on tree
```

### Comparing `rv_ltl-0.1.0a1/rv_ltl/monitor.py` & `rv_ltl-0.1.0a2/rv_ltl/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,31 @@
+"Provides Monitor to evaluate traces"
+
 from functools import reduce
 from operator import concat
 from typing import Any, Dict, List, Set, Union
 from rv_ltl.b4 import B4
-from .exceptions import MissingAtomicsException
+from .exception import MissingAtomicsException
 
 Step = Dict[Union[Any, str], bool]
 
 
 class Monitor:
     def __init__(self) -> None:
         self._last_index = -1
 
     def update(self, step: Step):
+        """takes a step of the trace
+
+        Args:
+            step (Step): A dictionary that represents a step
+
+        Raises:
+            MissingAtomicsException: When not all atomic propositions are specified
+        """
         # get all atomic nodes on the tree
         nodes: Set["Monitor"] = set(self._flatten())
         atomic_monitors: Set[AtomicMonitor] = set(
             filter(lambda node: isinstance(node, AtomicMonitor), nodes)
         )
         atomic_propositions = {m.proposition for m in atomic_monitors}
         id_to_atomics = {ap.identifier: ap for ap in atomic_propositions}
```

### Comparing `rv_ltl-0.1.0a1/rv_ltl/proposition.py` & `rv_ltl-0.1.0a2/rv_ltl/proposition.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"Provide classes to compose RV-LTL formulae"
+
 from typing import Union
 from uuid import uuid4
 from .monitor import (
     AlwaysMonitor,
     AndMonitor,
     EventuallyMonitor,
     ImpliesMonitor,
@@ -12,14 +14,19 @@
     OrMonitor,
     UntilMonitor,
 )
 
 
 class Proposition:
     def create_monitor(self) -> Monitor:
+        """Using the proposition, create a monitor that can be used to evaluate a trace
+
+        Returns:
+            Monitor: A monitor for this proposition
+        """
         raise NotImplementedError()
 
 
 class Atomic(Proposition):
     def __init__(self, *, identifier: Union[str, None] = None, name="") -> None:
         """
         Construct an atomic proposition.
```

