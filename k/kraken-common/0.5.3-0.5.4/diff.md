# Comparing `tmp/kraken_common-0.5.3.tar.gz` & `tmp/kraken_common-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_common-0.5.3.tar", max compression
+gzip compressed data, was "kraken_common-0.5.4.tar", max compression
```

## Comparing `kraken_common-0.5.3.tar` & `kraken_common-0.5.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      998 2023-02-15 06:37:08.238295 kraken_common-0.5.3/LICENSE
--rw-r--r--   0        0        0     1570 2023-02-15 06:56:43.083608 kraken_common-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     2068 2023-02-15 06:37:08.239200 kraken_common-0.5.3/readme.md
--rw-r--r--   0        0        0     2179 2023-02-15 06:56:43.083979 kraken_common-0.5.3/src/kraken/common/__init__.py
--rw-r--r--   0        0        0      471 2023-02-15 06:37:08.240791 kraken_common-0.5.3/src/kraken/common/_argparse.py
--rw-r--r--   0        0        0     1917 2023-02-15 06:37:08.241490 kraken_common-0.5.3/src/kraken/common/_asciitable.py
--rw-r--r--   0        0        0     4007 2023-02-15 06:37:08.241698 kraken_common-0.5.3/src/kraken/common/_buildscript.py
--rw-r--r--   0        0        0      611 2023-02-15 06:37:08.241884 kraken_common-0.5.3/src/kraken/common/_buildscript_test.py
--rw-r--r--   0        0        0      609 2023-02-15 06:37:08.242064 kraken_common-0.5.3/src/kraken/common/_date.py
--rw-r--r--   0        0        0      690 2023-02-15 06:37:08.242242 kraken_common-0.5.3/src/kraken/common/_date_test.py
--rw-r--r--   0        0        0     1803 2023-02-15 06:37:08.242420 kraken_common-0.5.3/src/kraken/common/_environment.py
--rw-r--r--   0        0        0     3075 2023-02-15 06:37:08.242776 kraken_common-0.5.3/src/kraken/common/_fs.py
--rw-r--r--   0        0        0      556 2023-02-15 06:37:08.242954 kraken_common-0.5.3/src/kraken/common/_generic.py
--rw-r--r--   0        0        0     1056 2023-02-15 06:37:08.243238 kraken_common-0.5.3/src/kraken/common/_importlib.py
--rw-r--r--   0        0        0     1825 2023-02-15 06:37:08.243425 kraken_common-0.5.3/src/kraken/common/_option_sets.py
--rw-r--r--   0        0        0    10081 2023-02-15 06:55:59.403461 kraken_common-0.5.3/src/kraken/common/_requirements.py
--rw-r--r--   0        0        0     1594 2023-02-15 06:37:08.244004 kraken_common-0.5.3/src/kraken/common/_requirements_test.py
--rw-r--r--   0        0        0     9143 2023-02-15 06:55:59.317679 kraken_common-0.5.3/src/kraken/common/_runner.py
--rw-r--r--   0        0        0     3451 2023-02-15 06:37:08.244410 kraken_common-0.5.3/src/kraken/common/_runner_test.py
--rw-r--r--   0        0        0      494 2023-02-15 06:37:08.244583 kraken_common-0.5.3/src/kraken/common/_terminal.py
--rw-r--r--   0        0        0     1258 2023-02-15 06:37:08.244764 kraken_common-0.5.3/src/kraken/common/_text.py
--rw-r--r--   0        0        0      197 2023-02-15 06:37:08.244943 kraken_common-0.5.3/src/kraken/common/_text_test.py
--rw-r--r--   0        0        0     1174 2023-02-15 06:37:08.245126 kraken_common-0.5.3/src/kraken/common/_tomlconfig.py
--rw-r--r--   0        0        0      802 2023-02-15 06:37:08.245299 kraken_common-0.5.3/src/kraken/common/_tomlconfig_test.py
--rw-r--r--   0        0        0      824 2023-02-15 06:37:08.245476 kraken_common-0.5.3/src/kraken/common/path.py
--rw-r--r--   0        0        0        0 2023-02-15 06:37:08.245623 kraken_common-0.5.3/src/kraken/common/py.typed
--rw-r--r--   0        0        0      326 2023-02-15 06:37:08.245971 kraken_common-0.5.3/src/kraken/common/pyenv/__init__.py
--rw-r--r--   0        0        0     5188 2023-02-15 06:37:08.246167 kraken_common-0.5.3/src/kraken/common/pyenv/_distributions.py
--rw-r--r--   0        0        0     2000 2023-02-15 06:37:08.246338 kraken_common-0.5.3/src/kraken/common/pyenv/_virtualenv.py
--rw-r--r--   0        0        0     2941 1970-01-01 00:00:00.000000 kraken_common-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      998 2023-02-15 06:37:08.238295 kraken_common-0.5.4/LICENSE
+-rw-r--r--   0        0        0     1570 2023-02-15 07:00:12.839332 kraken_common-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2068 2023-02-15 06:37:08.239200 kraken_common-0.5.4/readme.md
+-rw-r--r--   0        0        0     2179 2023-02-15 07:00:12.839521 kraken_common-0.5.4/src/kraken/common/__init__.py
+-rw-r--r--   0        0        0      471 2023-02-15 06:37:08.240791 kraken_common-0.5.4/src/kraken/common/_argparse.py
+-rw-r--r--   0        0        0     1917 2023-02-15 06:37:08.241490 kraken_common-0.5.4/src/kraken/common/_asciitable.py
+-rw-r--r--   0        0        0     4007 2023-02-15 06:37:08.241698 kraken_common-0.5.4/src/kraken/common/_buildscript.py
+-rw-r--r--   0        0        0      611 2023-02-15 06:37:08.241884 kraken_common-0.5.4/src/kraken/common/_buildscript_test.py
+-rw-r--r--   0        0        0      609 2023-02-15 06:37:08.242064 kraken_common-0.5.4/src/kraken/common/_date.py
+-rw-r--r--   0        0        0      690 2023-02-15 06:37:08.242242 kraken_common-0.5.4/src/kraken/common/_date_test.py
+-rw-r--r--   0        0        0     1803 2023-02-15 06:37:08.242420 kraken_common-0.5.4/src/kraken/common/_environment.py
+-rw-r--r--   0        0        0     3075 2023-02-15 06:37:08.242776 kraken_common-0.5.4/src/kraken/common/_fs.py
+-rw-r--r--   0        0        0      684 2023-02-15 07:00:03.285659 kraken_common-0.5.4/src/kraken/common/_generic.py
+-rw-r--r--   0        0        0     1056 2023-02-15 06:37:08.243238 kraken_common-0.5.4/src/kraken/common/_importlib.py
+-rw-r--r--   0        0        0     1825 2023-02-15 06:37:08.243425 kraken_common-0.5.4/src/kraken/common/_option_sets.py
+-rw-r--r--   0        0        0    10081 2023-02-15 06:55:59.403461 kraken_common-0.5.4/src/kraken/common/_requirements.py
+-rw-r--r--   0        0        0     1594 2023-02-15 06:37:08.244004 kraken_common-0.5.4/src/kraken/common/_requirements_test.py
+-rw-r--r--   0        0        0     9143 2023-02-15 06:55:59.317679 kraken_common-0.5.4/src/kraken/common/_runner.py
+-rw-r--r--   0        0        0     3451 2023-02-15 06:37:08.244410 kraken_common-0.5.4/src/kraken/common/_runner_test.py
+-rw-r--r--   0        0        0      494 2023-02-15 06:37:08.244583 kraken_common-0.5.4/src/kraken/common/_terminal.py
+-rw-r--r--   0        0        0     1258 2023-02-15 06:37:08.244764 kraken_common-0.5.4/src/kraken/common/_text.py
+-rw-r--r--   0        0        0      197 2023-02-15 06:37:08.244943 kraken_common-0.5.4/src/kraken/common/_text_test.py
+-rw-r--r--   0        0        0     1174 2023-02-15 06:37:08.245126 kraken_common-0.5.4/src/kraken/common/_tomlconfig.py
+-rw-r--r--   0        0        0      802 2023-02-15 06:37:08.245299 kraken_common-0.5.4/src/kraken/common/_tomlconfig_test.py
+-rw-r--r--   0        0        0      824 2023-02-15 06:37:08.245476 kraken_common-0.5.4/src/kraken/common/path.py
+-rw-r--r--   0        0        0        0 2023-02-15 06:37:08.245623 kraken_common-0.5.4/src/kraken/common/py.typed
+-rw-r--r--   0        0        0      326 2023-02-15 06:37:08.245971 kraken_common-0.5.4/src/kraken/common/pyenv/__init__.py
+-rw-r--r--   0        0        0     5188 2023-02-15 06:37:08.246167 kraken_common-0.5.4/src/kraken/common/pyenv/_distributions.py
+-rw-r--r--   0        0        0     2000 2023-02-15 06:37:08.246338 kraken_common-0.5.4/src/kraken/common/pyenv/_virtualenv.py
+-rw-r--r--   0        0        0     2941 1970-01-01 00:00:00.000000 kraken_common-0.5.4/PKG-INFO
```

### Comparing `kraken_common-0.5.3/LICENSE` & `kraken_common-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/pyproject.toml` & `kraken_common-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kraken-common"
-version = "0.5.3"
+version = "0.5.4"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{ include = "kraken/common", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `kraken_common-0.5.3/readme.md` & `kraken_common-0.5.4/readme.md`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/__init__.py` & `kraken_common-0.5.4/src/kraken/common/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,8 +79,8 @@
     "inline_text",
     "lazy_str",
     # _tomlconfig
     "TomlConfigFile",
     # global
     "path",
 ]
-__version__ = "0.5.3"
+__version__ = "0.5.4"
```

### Comparing `kraken_common-0.5.3/src/kraken/common/_asciitable.py` & `kraken_common-0.5.4/src/kraken/common/_asciitable.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/_buildscript.py` & `kraken_common-0.5.4/src/kraken/common/_buildscript.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/_buildscript_test.py` & `kraken_common-0.5.4/src/kraken/common/_buildscript_test.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/_date.py` & `kraken_common-0.5.4/src/kraken/common/_date.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/_date_test.py` & `kraken_common-0.5.4/src/kraken/common/_date_test.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/_environment.py` & `kraken_common-0.5.4/src/kraken/common/_environment.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/_fs.py` & `kraken_common-0.5.4/src/kraken/common/_fs.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/_generic.py` & `kraken_common-0.5.4/src/kraken/common/_generic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
 import enum
-from typing import Iterable, TypeVar
+from typing import Callable, Iterable, TypeVar
 
 __all__ = [
     "flatten",
     "not_none",
 ]
 
 T = TypeVar("T")
@@ -14,19 +16,21 @@
     Flatten a nested iterable into a single iterable.
     """
 
     for item in it:
         yield from item
 
 
-def not_none(v: "T | None", message: str = "expected not-None") -> T:
+def not_none(v: "T | None", message: str | Callable[[], str] = "expected not-None") -> T:
     """
     Raise a :class:`RuntimeError` if *v* is `None`, otherwise return *v*.
     """
 
     if v is None:
+        if callable(message):
+            message = message()
         raise RuntimeError(message)
     return v
 
 
 class NotSet(enum.Enum):
     Value = 1
```

### Comparing `kraken_common-0.5.3/src/kraken/common/_importlib.py` & `kraken_common-0.5.4/src/kraken/common/_importlib.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/_option_sets.py` & `kraken_common-0.5.4/src/kraken/common/_option_sets.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/_requirements.py` & `kraken_common-0.5.4/src/kraken/common/_requirements.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/_requirements_test.py` & `kraken_common-0.5.4/src/kraken/common/_requirements_test.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/_runner.py` & `kraken_common-0.5.4/src/kraken/common/_runner.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/_runner_test.py` & `kraken_common-0.5.4/src/kraken/common/_runner_test.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/_text.py` & `kraken_common-0.5.4/src/kraken/common/_text.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/_tomlconfig.py` & `kraken_common-0.5.4/src/kraken/common/_tomlconfig.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/_tomlconfig_test.py` & `kraken_common-0.5.4/src/kraken/common/_tomlconfig_test.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/path.py` & `kraken_common-0.5.4/src/kraken/common/path.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/pyenv/_distributions.py` & `kraken_common-0.5.4/src/kraken/common/pyenv/_distributions.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/src/kraken/common/pyenv/_virtualenv.py` & `kraken_common-0.5.4/src/kraken/common/pyenv/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `kraken_common-0.5.3/PKG-INFO` & `kraken_common-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kraken-common
-Version: 0.5.3
+Version: 0.5.4
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

