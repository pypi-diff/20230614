# Comparing `tmp/robocorp_log-1.0.0.tar.gz` & `tmp/robocorp_log-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_log-1.0.0.tar", max compression
+gzip compressed data, was "robocorp_log-1.0.1.tar", max compression
```

## Comparing `robocorp_log-1.0.0.tar` & `robocorp_log-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10142 2023-06-13 14:27:00.011423 robocorp_log-1.0.0/LICENSE
--rw-r--r--   0        0        0     5607 2023-06-13 14:27:00.011423 robocorp_log-1.0.0/README.md
--rw-r--r--   0        0        0     1225 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    29168 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/__init__.py
--rw-r--r--   0        0        0    17962 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_ast_utils.py
--rw-r--r--   0        0        0    12969 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_auto_logging_setup.py
--rw-r--r--   0        0        0     5362 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_config.py
--rw-r--r--   0        0        0      572 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_convert_units.py
--rw-r--r--   0        0        0     6719 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_decoder.py
--rw-r--r--   0        0        0     6724 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_decoder_spec.py
--rw-r--r--   0        0        0   449572 2023-06-13 14:27:51.804093 robocorp_log-1.0.0/src/robocorp/log/_index_v3.py
--rw-r--r--   0        0        0     6586 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_lifecycle_hooks.py
--rw-r--r--   0        0        0     1128 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_logger_instances.py
--rw-r--r--   0        0        0     1208 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_null.py
--rw-r--r--   0        0        0      385 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_obj_info_repr.py
--rw-r--r--   0        0        0    27732 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_rewrite_ast_add_callbacks.py
--rw-r--r--   0        0        0     9217 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/_rewrite_filtering.py
--rw-r--r--   0        0        0    12517 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/_rewrite_importhook.py
--rw-r--r--   0        0        0    10310 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/_robo_logger.py
--rw-r--r--   0        0        0    62363 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/_robo_output_impl.py
--rw-r--r--   0        0        0     1436 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/_sensitive_variable_names.py
--rw-r--r--   0        0        0     1915 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/_suppress_helper.py
--rw-r--r--   0        0        0     7802 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/console.py
--rw-r--r--   0        0        0     1082 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/protocols.py
--rw-r--r--   0        0        0        0 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/py.typed
--rw-r--r--   0        0        0     8025 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/redirect.py
--rw-r--r--   0        0        0     6287 1970-01-01 00:00:00.000000 robocorp_log-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-06-14 19:40:40.345299 robocorp_log-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5607 2023-06-14 19:40:40.345299 robocorp_log-1.0.1/README.md
+-rw-r--r--   0        0        0     1225 2023-06-14 19:40:40.353299 robocorp_log-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    29168 2023-06-14 19:40:40.353299 robocorp_log-1.0.1/src/robocorp/log/__init__.py
+-rw-r--r--   0        0        0    17962 2023-06-14 19:40:40.353299 robocorp_log-1.0.1/src/robocorp/log/_ast_utils.py
+-rw-r--r--   0        0        0    12969 2023-06-14 19:40:40.353299 robocorp_log-1.0.1/src/robocorp/log/_auto_logging_setup.py
+-rw-r--r--   0        0        0     5362 2023-06-14 19:40:40.353299 robocorp_log-1.0.1/src/robocorp/log/_config.py
+-rw-r--r--   0        0        0      572 2023-06-14 19:40:40.353299 robocorp_log-1.0.1/src/robocorp/log/_convert_units.py
+-rw-r--r--   0        0        0     6719 2023-06-14 19:40:40.353299 robocorp_log-1.0.1/src/robocorp/log/_decoder.py
+-rw-r--r--   0        0        0     6724 2023-06-14 19:40:40.353299 robocorp_log-1.0.1/src/robocorp/log/_decoder_spec.py
+-rw-r--r--   0        0        0   784387 2023-06-14 19:41:51.497888 robocorp_log-1.0.1/src/robocorp/log/_index_v3.py
+-rw-r--r--   0        0        0     6586 2023-06-14 19:40:40.353299 robocorp_log-1.0.1/src/robocorp/log/_lifecycle_hooks.py
+-rw-r--r--   0        0        0     1128 2023-06-14 19:40:40.353299 robocorp_log-1.0.1/src/robocorp/log/_logger_instances.py
+-rw-r--r--   0        0        0     1208 2023-06-14 19:40:40.353299 robocorp_log-1.0.1/src/robocorp/log/_null.py
+-rw-r--r--   0        0        0      385 2023-06-14 19:40:40.353299 robocorp_log-1.0.1/src/robocorp/log/_obj_info_repr.py
+-rw-r--r--   0        0        0    27732 2023-06-14 19:40:40.353299 robocorp_log-1.0.1/src/robocorp/log/_rewrite_ast_add_callbacks.py
+-rw-r--r--   0        0        0     9217 2023-06-14 19:40:40.353299 robocorp_log-1.0.1/src/robocorp/log/_rewrite_filtering.py
+-rw-r--r--   0        0        0    12517 2023-06-14 19:40:40.353299 robocorp_log-1.0.1/src/robocorp/log/_rewrite_importhook.py
+-rw-r--r--   0        0        0    10310 2023-06-14 19:40:40.353299 robocorp_log-1.0.1/src/robocorp/log/_robo_logger.py
+-rw-r--r--   0        0        0    62363 2023-06-14 19:40:40.357299 robocorp_log-1.0.1/src/robocorp/log/_robo_output_impl.py
+-rw-r--r--   0        0        0     1436 2023-06-14 19:40:40.357299 robocorp_log-1.0.1/src/robocorp/log/_sensitive_variable_names.py
+-rw-r--r--   0        0        0     1915 2023-06-14 19:40:40.357299 robocorp_log-1.0.1/src/robocorp/log/_suppress_helper.py
+-rw-r--r--   0        0        0     7802 2023-06-14 19:40:40.357299 robocorp_log-1.0.1/src/robocorp/log/console.py
+-rw-r--r--   0        0        0     1082 2023-06-14 19:40:40.357299 robocorp_log-1.0.1/src/robocorp/log/protocols.py
+-rw-r--r--   0        0        0        0 2023-06-14 19:40:40.357299 robocorp_log-1.0.1/src/robocorp/log/py.typed
+-rw-r--r--   0        0        0     8025 2023-06-14 19:40:40.357299 robocorp_log-1.0.1/src/robocorp/log/redirect.py
+-rw-r--r--   0        0        0     6287 1970-01-01 00:00:00.000000 robocorp_log-1.0.1/PKG-INFO
```

### Comparing `robocorp_log-1.0.0/LICENSE` & `robocorp_log-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/README.md` & `robocorp_log-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/pyproject.toml` & `robocorp_log-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-log"
-version = "1.0.0"
+version = "1.0.1"
 description = "Automatic trace logging for Python"
 authors = [
     "Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp/log", from = "src"}]
 include = ["**/_index.py", "**/_index_v2.py", "**/_index_v3.py"]
```

### Comparing `robocorp_log-1.0.0/src/robocorp/log/__init__.py` & `robocorp_log-1.0.1/src/robocorp/log/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from ._logger_instances import _get_logger_instances
 from ._suppress_helper import SuppressHelper as _SuppressHelper
 from .protocols import IReadLines, LogHTMLStyle, OptExcInfo, Status
 
 if typing.TYPE_CHECKING:
     from ._robo_logger import _RoboLogger
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 version_info = [int(x) for x in __version__.split(".")]
 
 from . import _config
 
 # --- Make these a part of the public API.
 
 Filter = _config.Filter
```

### Comparing `robocorp_log-1.0.0/src/robocorp/log/_ast_utils.py` & `robocorp_log-1.0.1/src/robocorp/log/_ast_utils.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/_auto_logging_setup.py` & `robocorp_log-1.0.1/src/robocorp/log/_auto_logging_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/_config.py` & `robocorp_log-1.0.1/src/robocorp/log/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/_convert_units.py` & `robocorp_log-1.0.1/src/robocorp/log/_convert_units.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/_decoder.py` & `robocorp_log-1.0.1/src/robocorp/log/_decoder.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/_decoder_spec.py` & `robocorp_log-1.0.1/src/robocorp/log/_decoder_spec.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/_lifecycle_hooks.py` & `robocorp_log-1.0.1/src/robocorp/log/_lifecycle_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/_logger_instances.py` & `robocorp_log-1.0.1/src/robocorp/log/_logger_instances.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/_null.py` & `robocorp_log-1.0.1/src/robocorp/log/_null.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/_rewrite_ast_add_callbacks.py` & `robocorp_log-1.0.1/src/robocorp/log/_rewrite_ast_add_callbacks.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/_rewrite_filtering.py` & `robocorp_log-1.0.1/src/robocorp/log/_rewrite_filtering.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/_rewrite_importhook.py` & `robocorp_log-1.0.1/src/robocorp/log/_rewrite_importhook.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/_robo_logger.py` & `robocorp_log-1.0.1/src/robocorp/log/_robo_logger.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/_robo_output_impl.py` & `robocorp_log-1.0.1/src/robocorp/log/_robo_output_impl.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/_sensitive_variable_names.py` & `robocorp_log-1.0.1/src/robocorp/log/_sensitive_variable_names.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/_suppress_helper.py` & `robocorp_log-1.0.1/src/robocorp/log/_suppress_helper.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/console.py` & `robocorp_log-1.0.1/src/robocorp/log/console.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/protocols.py` & `robocorp_log-1.0.1/src/robocorp/log/protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/src/robocorp/log/redirect.py` & `robocorp_log-1.0.1/src/robocorp/log/redirect.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-1.0.0/PKG-INFO` & `robocorp_log-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-log
-Version: 1.0.0
+Version: 1.0.1
 Summary: Automatic trace logging for Python
 Author: Fabio Zadrozny
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

