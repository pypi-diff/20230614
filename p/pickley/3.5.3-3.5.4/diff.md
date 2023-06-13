# Comparing `tmp/pickley-3.5.3.tar.gz` & `tmp/pickley-3.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pickley-3.5.3.tar", last modified: Tue Jun 13 22:23:46 2023, max compression
+gzip compressed data, was "pickley-3.5.4.tar", last modified: Tue Jun 13 23:10:53 2023, max compression
```

## Comparing `pickley-3.5.3.tar` & `pickley-3.5.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:23:46.943123 pickley-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 22:22:09.000000 pickley-3.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 22:22:09.000000 pickley-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-13 22:23:46.943123 pickley-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-13 22:22:09.000000 pickley-3.5.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-13 22:22:09.000000 pickley-3.5.3/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 22:22:09.000000 pickley-3.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 22:23:46.943123 pickley-3.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 22:22:09.000000 pickley-3.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:23:46.939123 pickley-3.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:23:46.939123 pickley-3.5.3/src/pickley/
--rw-r--r--   0 runner    (1001) docker     (123)    36044 2023-06-13 22:22:09.000000 pickley-3.5.3/src/pickley/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-13 22:22:09.000000 pickley-3.5.3/src/pickley/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-06-13 22:22:09.000000 pickley-3.5.3/src/pickley/bstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    31338 2023-06-13 22:22:09.000000 pickley-3.5.3/src/pickley/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-13 22:22:09.000000 pickley-3.5.3/src/pickley/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-06-13 22:22:09.000000 pickley-3.5.3/src/pickley/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:23:46.943123 pickley-3.5.3/src/pickley.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-13 22:23:46.000000 pickley-3.5.3/src/pickley.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-13 22:23:46.000000 pickley-3.5.3/src/pickley.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 22:23:46.000000 pickley-3.5.3/src/pickley.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 22:23:46.000000 pickley-3.5.3/src/pickley.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 22:23:46.000000 pickley-3.5.3/src/pickley.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 22:23:46.000000 pickley-3.5.3/src/pickley.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:23:46.943123 pickley-3.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-13 22:22:09.000000 pickley-3.5.3/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-13 22:22:09.000000 pickley-3.5.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-13 22:22:09.000000 pickley-3.5.3/tests/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)    17772 2023-06-13 22:22:09.000000 pickley-3.5.3/tests/test_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-13 22:22:09.000000 pickley-3.5.3/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-13 22:22:09.000000 pickley-3.5.3/tests/test_venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:10:53.435780 pickley-3.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 23:09:07.000000 pickley-3.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 23:09:07.000000 pickley-3.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-13 23:10:53.435780 pickley-3.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-13 23:09:07.000000 pickley-3.5.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-13 23:09:07.000000 pickley-3.5.4/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 23:09:07.000000 pickley-3.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:10:53.435780 pickley-3.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 23:09:07.000000 pickley-3.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:10:53.431780 pickley-3.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:10:53.431780 pickley-3.5.4/src/pickley/
+-rw-r--r--   0 runner    (1001) docker     (123)    36044 2023-06-13 23:09:07.000000 pickley-3.5.4/src/pickley/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-13 23:09:07.000000 pickley-3.5.4/src/pickley/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-06-13 23:09:07.000000 pickley-3.5.4/src/pickley/bstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31357 2023-06-13 23:09:07.000000 pickley-3.5.4/src/pickley/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-13 23:09:07.000000 pickley-3.5.4/src/pickley/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-06-13 23:09:07.000000 pickley-3.5.4/src/pickley/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:10:53.431780 pickley-3.5.4/src/pickley.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-13 23:10:53.000000 pickley-3.5.4/src/pickley.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-13 23:10:53.000000 pickley-3.5.4/src/pickley.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:10:53.000000 pickley-3.5.4/src/pickley.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 23:10:53.000000 pickley-3.5.4/src/pickley.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 23:10:53.000000 pickley-3.5.4/src/pickley.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 23:10:53.000000 pickley-3.5.4/src/pickley.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:10:53.435780 pickley-3.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-13 23:09:07.000000 pickley-3.5.4/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-13 23:09:07.000000 pickley-3.5.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-13 23:09:07.000000 pickley-3.5.4/tests/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17772 2023-06-13 23:09:07.000000 pickley-3.5.4/tests/test_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-13 23:09:07.000000 pickley-3.5.4/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-13 23:09:07.000000 pickley-3.5.4/tests/test_venv.py
```

### Comparing `pickley-3.5.3/LICENSE` & `pickley-3.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pickley-3.5.3/PKG-INFO` & `pickley-3.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickley
-Version: 3.5.3
+Version: 3.5.4
 Summary: Automate installation of standalone python CLIs
 Home-page: https://github.com/codrsquad/pickley
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/pickley/wiki
 Project-URL: Release notes, https://github.com/codrsquad/pickley/wiki/Release-notes
```

### Comparing `pickley-3.5.3/README.rst` & `pickley-3.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `pickley-3.5.3/setup.py` & `pickley-3.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.3/src/pickley/__init__.py` & `pickley-3.5.4/src/pickley/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 from datetime import datetime
 
 import runez
 from runez.pyenv import PypiStd, PythonDepot, PythonInstallationScanner, Version
 
 
-__version__ = "3.5.3"
+__version__ = "3.5.4"
 LOG = logging.getLogger(__name__)
 PICKLEY = "pickley"
 DOT_META = ".pk"
 K_CLI = {"delivery", "index", "python"}
 K_DIRECTIVES = {"include"}
 K_GROUPS = {"bundle", "pinned"}
 K_LEAVES = {
```

### Comparing `pickley-3.5.3/src/pickley/bstrap.py` & `pickley-3.5.4/src/pickley/bstrap.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.3/src/pickley/cli.py` & `pickley-3.5.4/src/pickley/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -483,23 +483,22 @@
     if not packages:
         print("No packages installed")
         sys.exit(0)
 
     report = TabularReport("Package,Version,Python", additional="Delivery,Index", border=border, verbose=verbose)
     for pspec in packages:
         manifest = pspec.manifest
-        if manifest:
-            python = CFG.available_pythons.find_python(manifest.python)
-            report.add_row(
-                Package=pspec.dashed,
-                Version=manifest.version,
-                Python=python,
-                Delivery=manifest.delivery,
-                Index=manifest.index
-            )
+        python = manifest and manifest.python and CFG.available_pythons.find_python(manifest.python)
+        report.add_row(
+            Package=pspec.dashed,
+            Version=manifest and manifest.version,
+            Python=python,
+            Delivery=manifest and manifest.delivery,
+            Index=manifest and manifest.index
+        )
 
     print(report.represented(format))
 
 
 class RunSetup:
     """Convenience defaults to use for 'run' commands"""
```

### Comparing `pickley-3.5.3/src/pickley/delivery.py` & `pickley-3.5.4/src/pickley/delivery.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.3/src/pickley/package.py` & `pickley-3.5.4/src/pickley/package.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.3/src/pickley.egg-info/PKG-INFO` & `pickley-3.5.4/src/pickley.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickley
-Version: 3.5.3
+Version: 3.5.4
 Summary: Automate installation of standalone python CLIs
 Home-page: https://github.com/codrsquad/pickley
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/pickley/wiki
 Project-URL: Release notes, https://github.com/codrsquad/pickley/wiki/Release-notes
```

### Comparing `pickley-3.5.3/src/pickley.egg-info/SOURCES.txt` & `pickley-3.5.4/src/pickley.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pickley-3.5.3/tests/test_bootstrap.py` & `pickley-3.5.4/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.3/tests/test_config.py` & `pickley-3.5.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.3/tests/test_delivery.py` & `pickley-3.5.4/tests/test_delivery.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.3/tests/test_ops.py` & `pickley-3.5.4/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.3/tests/test_run.py` & `pickley-3.5.4/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.3/tests/test_venv.py` & `pickley-3.5.4/tests/test_venv.py`

 * *Files identical despite different names*

