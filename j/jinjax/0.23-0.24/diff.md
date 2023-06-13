# Comparing `tmp/jinjax-0.23.tar.gz` & `tmp/jinjax-0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinjax-0.23.tar", max compression
+gzip compressed data, was "jinjax-0.24.tar", max compression
```

## Comparing `jinjax-0.23.tar` & `jinjax-0.24.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      493 2023-04-02 03:49:15.124261 jinjax-0.23/README.md
--rw-r--r--   0        0        0     2672 2023-04-02 03:49:15.124261 jinjax-0.23/pyproject.toml
--rw-r--r--   0        0        0      189 2023-04-02 03:49:15.124261 jinjax-0.23/src/jinjax/__init__.py
--rw-r--r--   0        0        0     8485 2023-04-02 03:49:15.124261 jinjax-0.23/src/jinjax/catalog.py
--rw-r--r--   0        0        0     4141 2023-04-02 03:49:15.124261 jinjax-0.23/src/jinjax/component.py
--rw-r--r--   0        0        0      409 2023-04-02 03:49:15.124261 jinjax-0.23/src/jinjax/exceptions.py
--rw-r--r--   0        0        0     4835 2023-04-02 03:49:15.124261 jinjax-0.23/src/jinjax/html_attrs.py
--rw-r--r--   0        0        0     4427 2023-04-02 03:49:15.124261 jinjax-0.23/src/jinjax/jinjax.py
--rw-r--r--   0        0        0      863 2023-04-02 03:49:15.124261 jinjax-0.23/src/jinjax/middleware.py
--rw-r--r--   0        0        0        0 2023-04-02 03:49:15.124261 jinjax-0.23/src/jinjax/py.typed
--rw-r--r--   0        0        0      139 2023-04-02 03:49:15.124261 jinjax-0.23/src/jinjax/utils.py
--rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 jinjax-0.23/PKG-INFO
+-rw-r--r--   0        0        0      493 2023-06-13 23:49:25.734055 jinjax-0.24/README.md
+-rw-r--r--   0        0        0     2672 2023-06-13 23:49:25.734055 jinjax-0.24/pyproject.toml
+-rw-r--r--   0        0        0      189 2023-06-13 23:49:25.734055 jinjax-0.24/src/jinjax/__init__.py
+-rw-r--r--   0        0        0     8485 2023-06-13 23:49:25.734055 jinjax-0.24/src/jinjax/catalog.py
+-rw-r--r--   0        0        0     4141 2023-06-13 23:49:25.734055 jinjax-0.24/src/jinjax/component.py
+-rw-r--r--   0        0        0      409 2023-06-13 23:49:25.734055 jinjax-0.24/src/jinjax/exceptions.py
+-rw-r--r--   0        0        0     5248 2023-06-13 23:49:25.734055 jinjax-0.24/src/jinjax/html_attrs.py
+-rw-r--r--   0        0        0     4427 2023-06-13 23:49:25.734055 jinjax-0.24/src/jinjax/jinjax.py
+-rw-r--r--   0        0        0      863 2023-06-13 23:49:25.734055 jinjax-0.24/src/jinjax/middleware.py
+-rw-r--r--   0        0        0        0 2023-06-13 23:49:25.734055 jinjax-0.24/src/jinjax/py.typed
+-rw-r--r--   0        0        0      139 2023-06-13 23:49:25.734055 jinjax-0.24/src/jinjax/utils.py
+-rw-r--r--   0        0        0     1844 1970-01-01 00:00:00.000000 jinjax-0.24/PKG-INFO
```

### Comparing `jinjax-0.23/pyproject.toml` & `jinjax-0.24/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "jinjax"
-version = "0.23"
+version = "0.24"
 description = "Replace your HTML templates with Python server-Side components"
 authors = ["Juan-Pablo Scaletti <juanpablo@jpscaletti.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://jinjax.scaletti.dev/"
 repository = "https://github.com/jpsca/jinjax"
 documentation = "https://jinjax.scaletti.dev/guides/"
```

### Comparing `jinjax-0.23/src/jinjax/catalog.py` & `jinjax-0.24/src/jinjax/catalog.py`

 * *Files identical despite different names*

### Comparing `jinjax-0.23/src/jinjax/component.py` & `jinjax-0.24/src/jinjax/component.py`

 * *Files identical despite different names*

### Comparing `jinjax-0.23/src/jinjax/html_attrs.py` & `jinjax-0.24/src/jinjax/html_attrs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import re
+from collections import UserString
+from functools import cached_property
 from typing import Any
 
 
 CLASS_KEY = "class"
 CLASS_ALT_KEY = "classes"
 CLASS_KEYS = (CLASS_KEY, CLASS_ALT_KEY)
 
@@ -18,31 +20,45 @@
             return f'"{text}"'
         else:
             return f"'{text}'"
 
     return f'"{text}"'
 
 
+class LazyString(UserString):
+    """Behave like regular strings, but the actual casting of the initial value
+    is deferred until the value is actually required."""
+
+    __slots__ = ("_seq",)
+
+    def __init__(self, seq):
+        self._seq = seq
+
+    @cached_property
+    def data(self):
+        return str(self._seq)
+
+
 class HTMLAttrs:
     def __init__(self, attrs) -> None:
-        attributes: "dict[str, str]" = {}
+        attributes: "dict[str, str|LazyString]" = {}
         properties: "set[str]" = set()
 
         class_names = split(" ".join([
             attrs.pop(CLASS_KEY, ""),
             attrs.get(CLASS_ALT_KEY, ""),
         ]))
         self.__classes = {name for name in class_names if name}
 
         for name, value in attrs.items():
             name = name.replace("_", "-")
             if value is True:
                 properties.add(name)
             elif value not in (False, None):
-                attributes[name] = str(value)
+                attributes[name] = LazyString(value)
 
         self.__attributes = attributes
         self.__properties = properties
 
     @property
     def classes(self) -> str:
         return " ".join(sorted(list(self.__classes)))
```

### Comparing `jinjax-0.23/src/jinjax/jinjax.py` & `jinjax-0.24/src/jinjax/jinjax.py`

 * *Files identical despite different names*

### Comparing `jinjax-0.23/src/jinjax/middleware.py` & `jinjax-0.24/src/jinjax/middleware.py`

 * *Files identical despite different names*

### Comparing `jinjax-0.23/PKG-INFO` & `jinjax-0.24/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjax
-Version: 0.23
+Version: 0.24
 Summary: Replace your HTML templates with Python server-Side components
 Home-page: https://jinjax.scaletti.dev/
 License: MIT
 Author: Juan-Pablo Scaletti
 Author-email: juanpablo@jpscaletti.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -12,18 +12,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Typing :: Typed
 Requires-Dist: jinja2 (>=3.0)
```

