# Comparing `tmp/napari-plugin-manager-0.1.0a1.tar.gz` & `tmp/napari-plugin-manager-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-plugin-manager-0.1.0a1.tar", last modified: Mon Jun 12 09:06:56 2023, max compression
+gzip compressed data, was "napari-plugin-manager-0.1.0a2.tar", last modified: Tue Jun 13 23:45:41 2023, max compression
```

## Comparing `napari-plugin-manager-0.1.0a1.tar` & `napari-plugin-manager-0.1.0a2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:06:56.535792 napari-plugin-manager-0.1.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:06:56.531792 napari-plugin-manager-0.1.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:06:56.531792 napari-plugin-manager-0.1.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-12 09:06:56.535792 napari-plugin-manager-0.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:06:56.531792 napari-plugin-manager-0.1.0a1/napari_plugin_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:06:56.535792 napari-plugin-manager-0.1.0a1/napari_plugin_manager/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager/_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager/_tests/test_installer_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager/_tests/test_qt_plugin_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 09:06:56.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18125 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager/qt_package_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)    39782 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager/qt_plugin_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:06:56.531792 napari-plugin-manager-0.1.0a1/napari_plugin_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-12 09:06:56.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-12 09:06:56.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:06:56.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-12 09:06:56.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 09:06:56.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 09:06:56.535792 napari-plugin-manager-0.1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:41.074596 napari-plugin-manager-0.1.0a2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:41.070595 napari-plugin-manager-0.1.0a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:41.074596 napari-plugin-manager-0.1.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-13 23:45:26.000000 napari-plugin-manager-0.1.0a2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-13 23:45:26.000000 napari-plugin-manager-0.1.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-13 23:45:26.000000 napari-plugin-manager-0.1.0a2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-13 23:45:26.000000 napari-plugin-manager-0.1.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-13 23:45:41.074596 napari-plugin-manager-0.1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-13 23:45:26.000000 napari-plugin-manager-0.1.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:41.074596 napari-plugin-manager-0.1.0a2/napari_plugin_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:26.000000 napari-plugin-manager-0.1.0a2/napari_plugin_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:41.074596 napari-plugin-manager-0.1.0a2/napari_plugin_manager/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:26.000000 napari-plugin-manager-0.1.0a2/napari_plugin_manager/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-13 23:45:26.000000 napari-plugin-manager-0.1.0a2/napari_plugin_manager/_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-13 23:45:26.000000 napari-plugin-manager-0.1.0a2/napari_plugin_manager/_tests/test_installer_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-06-13 23:45:26.000000 napari-plugin-manager-0.1.0a2/napari_plugin_manager/_tests/test_qt_plugin_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-13 23:45:40.000000 napari-plugin-manager-0.1.0a2/napari_plugin_manager/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18125 2023-06-13 23:45:26.000000 napari-plugin-manager-0.1.0a2/napari_plugin_manager/qt_package_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39782 2023-06-13 23:45:26.000000 napari-plugin-manager-0.1.0a2/napari_plugin_manager/qt_plugin_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:41.074596 napari-plugin-manager-0.1.0a2/napari_plugin_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-13 23:45:41.000000 napari-plugin-manager-0.1.0a2/napari_plugin_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-13 23:45:41.000000 napari-plugin-manager-0.1.0a2/napari_plugin_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:45:41.000000 napari-plugin-manager-0.1.0a2/napari_plugin_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-13 23:45:41.000000 napari-plugin-manager-0.1.0a2/napari_plugin_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 23:45:41.000000 napari-plugin-manager-0.1.0a2/napari_plugin_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-13 23:45:26.000000 napari-plugin-manager-0.1.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:45:41.074596 napari-plugin-manager-0.1.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-13 23:45:26.000000 napari-plugin-manager-0.1.0a2/tox.ini
```

### Comparing `napari-plugin-manager-0.1.0a1/.github/workflows/test_and_deploy.yml` & `napari-plugin-manager-0.1.0a2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a1/.gitignore` & `napari-plugin-manager-0.1.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a1/.pre-commit-config.yaml` & `napari-plugin-manager-0.1.0a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a1/LICENSE` & `napari-plugin-manager-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a1/PKG-INFO` & `napari-plugin-manager-0.1.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-plugin-manager
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Install plugins for napari, in napari.
 Author-email: napari team <napari-steering-council@googlegroups.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2018, Napari
         All rights reserved.
```

### Comparing `napari-plugin-manager-0.1.0a1/README.md` & `napari-plugin-manager-0.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a1/napari_plugin_manager/_tests/conftest.py` & `napari-plugin-manager-0.1.0a2/napari_plugin_manager/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a1/napari_plugin_manager/_tests/test_installer_process.py` & `napari-plugin-manager-0.1.0a2/napari_plugin_manager/_tests/test_installer_process.py`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a1/napari_plugin_manager/_tests/test_qt_plugin_dialog.py` & `napari-plugin-manager-0.1.0a2/napari_plugin_manager/_tests/test_qt_plugin_dialog.py`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a1/napari_plugin_manager/qt_package_installer.py` & `napari-plugin-manager-0.1.0a2/napari_plugin_manager/qt_package_installer.py`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a1/napari_plugin_manager/qt_plugin_dialog.py` & `napari-plugin-manager-0.1.0a2/napari_plugin_manager/qt_plugin_dialog.py`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a1/napari_plugin_manager.egg-info/PKG-INFO` & `napari-plugin-manager-0.1.0a2/napari_plugin_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-plugin-manager
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Install plugins for napari, in napari.
 Author-email: napari team <napari-steering-council@googlegroups.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2018, Napari
         All rights reserved.
```

### Comparing `napari-plugin-manager-0.1.0a1/napari_plugin_manager.egg-info/SOURCES.txt` & `napari-plugin-manager-0.1.0a2/napari_plugin_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a1/pyproject.toml` & `napari-plugin-manager-0.1.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
     "Operating System :: Unix",
     "Operating System :: MacOS"
 ]
 requires-python = ">=3.8"
 dependencies = [
-  "napari",
   "npe2",
   "qtpy",
   "superqt",
   "pip"
 ]
 dynamic = [
   "version"
```

### Comparing `napari-plugin-manager-0.1.0a1/tox.ini` & `napari-plugin-manager-0.1.0a2/tox.ini`

 * *Files identical despite different names*

