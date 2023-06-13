# Comparing `tmp/pickley-3.5.1.tar.gz` & `tmp/pickley-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pickley-3.5.1.tar", last modified: Tue Jun 13 22:03:07 2023, max compression
+gzip compressed data, was "pickley-3.5.2.tar", last modified: Tue Jun 13 22:15:53 2023, max compression
```

## Comparing `pickley-3.5.1.tar` & `pickley-3.5.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:03:07.618745 pickley-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 22:01:36.000000 pickley-3.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 22:01:36.000000 pickley-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-13 22:03:07.618745 pickley-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-13 22:01:36.000000 pickley-3.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-13 22:01:36.000000 pickley-3.5.1/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 22:01:36.000000 pickley-3.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 22:03:07.618745 pickley-3.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 22:01:36.000000 pickley-3.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:03:07.618745 pickley-3.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:03:07.618745 pickley-3.5.1/src/pickley/
--rw-r--r--   0 runner    (1001) docker     (123)    36044 2023-06-13 22:01:36.000000 pickley-3.5.1/src/pickley/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-13 22:01:36.000000 pickley-3.5.1/src/pickley/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-06-13 22:01:36.000000 pickley-3.5.1/src/pickley/bstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    31262 2023-06-13 22:01:36.000000 pickley-3.5.1/src/pickley/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-13 22:01:36.000000 pickley-3.5.1/src/pickley/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-06-13 22:01:36.000000 pickley-3.5.1/src/pickley/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:03:07.618745 pickley-3.5.1/src/pickley.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-13 22:03:07.000000 pickley-3.5.1/src/pickley.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-13 22:03:07.000000 pickley-3.5.1/src/pickley.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 22:03:07.000000 pickley-3.5.1/src/pickley.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 22:03:07.000000 pickley-3.5.1/src/pickley.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 22:03:07.000000 pickley-3.5.1/src/pickley.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 22:03:07.000000 pickley-3.5.1/src/pickley.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:03:07.618745 pickley-3.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-13 22:01:36.000000 pickley-3.5.1/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-13 22:01:36.000000 pickley-3.5.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-13 22:01:36.000000 pickley-3.5.1/tests/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)    17772 2023-06-13 22:01:36.000000 pickley-3.5.1/tests/test_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-13 22:01:36.000000 pickley-3.5.1/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-13 22:01:36.000000 pickley-3.5.1/tests/test_venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:15:53.392997 pickley-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 22:14:21.000000 pickley-3.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 22:14:21.000000 pickley-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-13 22:15:53.392997 pickley-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-13 22:14:21.000000 pickley-3.5.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-13 22:14:21.000000 pickley-3.5.2/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 22:14:21.000000 pickley-3.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 22:15:53.392997 pickley-3.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 22:14:21.000000 pickley-3.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:15:53.388997 pickley-3.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:15:53.392997 pickley-3.5.2/src/pickley/
+-rw-r--r--   0 runner    (1001) docker     (123)    36044 2023-06-13 22:14:21.000000 pickley-3.5.2/src/pickley/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-13 22:14:21.000000 pickley-3.5.2/src/pickley/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-06-13 22:14:21.000000 pickley-3.5.2/src/pickley/bstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31276 2023-06-13 22:14:21.000000 pickley-3.5.2/src/pickley/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-13 22:14:21.000000 pickley-3.5.2/src/pickley/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-06-13 22:14:21.000000 pickley-3.5.2/src/pickley/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:15:53.392997 pickley-3.5.2/src/pickley.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-13 22:15:53.000000 pickley-3.5.2/src/pickley.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-13 22:15:53.000000 pickley-3.5.2/src/pickley.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 22:15:53.000000 pickley-3.5.2/src/pickley.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 22:15:53.000000 pickley-3.5.2/src/pickley.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 22:15:53.000000 pickley-3.5.2/src/pickley.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 22:15:53.000000 pickley-3.5.2/src/pickley.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:15:53.392997 pickley-3.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-13 22:14:21.000000 pickley-3.5.2/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-13 22:14:21.000000 pickley-3.5.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-13 22:14:21.000000 pickley-3.5.2/tests/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17772 2023-06-13 22:14:21.000000 pickley-3.5.2/tests/test_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-13 22:14:21.000000 pickley-3.5.2/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-13 22:14:21.000000 pickley-3.5.2/tests/test_venv.py
```

### Comparing `pickley-3.5.1/LICENSE` & `pickley-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pickley-3.5.1/PKG-INFO` & `pickley-3.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickley
-Version: 3.5.1
+Version: 3.5.2
 Summary: Automate installation of standalone python CLIs
 Home-page: https://github.com/codrsquad/pickley
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/pickley/wiki
 Project-URL: Release notes, https://github.com/codrsquad/pickley/wiki/Release-notes
```

### Comparing `pickley-3.5.1/README.rst` & `pickley-3.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `pickley-3.5.1/setup.py` & `pickley-3.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.1/src/pickley/__init__.py` & `pickley-3.5.2/src/pickley/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 from datetime import datetime
 
 import runez
 from runez.pyenv import PypiStd, PythonDepot, PythonInstallationScanner, Version
 
 
-__version__ = "3.5.1"
+__version__ = "3.5.2"
 LOG = logging.getLogger(__name__)
 PICKLEY = "pickley"
 DOT_META = ".pk"
 K_CLI = {"delivery", "index", "python"}
 K_DIRECTIVES = {"include"}
 K_GROUPS = {"bundle", "pinned"}
 K_LEAVES = {
```

### Comparing `pickley-3.5.1/src/pickley/bstrap.py` & `pickley-3.5.2/src/pickley/bstrap.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.1/src/pickley/cli.py` & `pickley-3.5.2/src/pickley/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 def _find_base_from_program_path(path):
     if not path or len(path) <= 1:
         return None
 
     dirpath, basename = os.path.split(path)
     if basename:
         basename = basename.lower()
-        if basename == DOT_META:
+        if basename in (DOT_META, ".pickley"):
             return dirpath  # We're running from an installed pickley
 
         if basename == ".venv":
             return os.path.join(path, "root")  # Convenience for development
 
     return _find_base_from_program_path(dirpath)
```

### Comparing `pickley-3.5.1/src/pickley/delivery.py` & `pickley-3.5.2/src/pickley/delivery.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.1/src/pickley/package.py` & `pickley-3.5.2/src/pickley/package.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.1/src/pickley.egg-info/PKG-INFO` & `pickley-3.5.2/src/pickley.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickley
-Version: 3.5.1
+Version: 3.5.2
 Summary: Automate installation of standalone python CLIs
 Home-page: https://github.com/codrsquad/pickley
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/pickley/wiki
 Project-URL: Release notes, https://github.com/codrsquad/pickley/wiki/Release-notes
```

### Comparing `pickley-3.5.1/src/pickley.egg-info/SOURCES.txt` & `pickley-3.5.2/src/pickley.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pickley-3.5.1/tests/test_bootstrap.py` & `pickley-3.5.2/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.1/tests/test_config.py` & `pickley-3.5.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.1/tests/test_delivery.py` & `pickley-3.5.2/tests/test_delivery.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.1/tests/test_ops.py` & `pickley-3.5.2/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.1/tests/test_run.py` & `pickley-3.5.2/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.1/tests/test_venv.py` & `pickley-3.5.2/tests/test_venv.py`

 * *Files identical despite different names*

