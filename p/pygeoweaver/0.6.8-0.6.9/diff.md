# Comparing `tmp/pygeoweaver-0.6.8.tar.gz` & `tmp/pygeoweaver-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoweaver-0.6.8.tar", last modified: Sun Jun  4 15:31:47 2023, max compression
+gzip compressed data, was "pygeoweaver-0.6.9.tar", last modified: Sun Jun  4 16:14:15 2023, max compression
```

## Comparing `pygeoweaver-0.6.8.tar` & `pygeoweaver-0.6.9.tar`

### file list

```diff
@@ -1,30 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:31:47.036620 pygeoweaver-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-04 15:31:47.036620 pygeoweaver-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:31:47.036620 pygeoweaver-0.6.8/pygeoweaver/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_help.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_resetpassword.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:31:47.036620 pygeoweaver-0.6.8/pygeoweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-04 15:31:47.000000 pygeoweaver-0.6.8/pygeoweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-04 15:31:47.000000 pygeoweaver-0.6.8/pygeoweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 15:31:47.000000 pygeoweaver-0.6.8/pygeoweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-04 15:31:47.000000 pygeoweaver-0.6.8/pygeoweaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-04 15:31:47.036620 pygeoweaver-0.6.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:31:47.036620 pygeoweaver-0.6.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/test/test_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/test/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:14:15.488549 pygeoweaver-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-04 16:14:15.488549 pygeoweaver-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:14:15.484549 pygeoweaver-0.6.9/pygeoweaver/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/download_gw.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/download_gw.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_resetpassword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/start.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      518 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/start.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/stop.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      269 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/stop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:14:15.488549 pygeoweaver-0.6.9/pygeoweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-04 16:14:15.000000 pygeoweaver-0.6.9/pygeoweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-04 16:14:15.000000 pygeoweaver-0.6.9/pygeoweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:14:15.000000 pygeoweaver-0.6.9/pygeoweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-04 16:14:15.000000 pygeoweaver-0.6.9/pygeoweaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-04 16:14:15.488549 pygeoweaver-0.6.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:14:15.488549 pygeoweaver-0.6.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/test/test_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/test/test_server.py
```

### Comparing `pygeoweaver-0.6.8/LICENSE` & `pygeoweaver-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.8/PKG-INFO` & `pygeoweaver-0.6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.6.8
+Version: 0.6.9
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygeoweaver-0.6.8/README.md` & `pygeoweaver-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.8/pygeoweaver/__main__.py` & `pygeoweaver-0.6.9/pygeoweaver/__main__.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.8/pygeoweaver/sc_detail.py` & `pygeoweaver-0.6.9/pygeoweaver/sc_detail.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.8/pygeoweaver/sc_export.py` & `pygeoweaver-0.6.9/pygeoweaver/sc_export.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.8/pygeoweaver/sc_help.py` & `pygeoweaver-0.6.9/pygeoweaver/sc_help.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.8/pygeoweaver/sc_import.py` & `pygeoweaver-0.6.9/pygeoweaver/sc_import.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.8/pygeoweaver/sc_list.py` & `pygeoweaver-0.6.9/pygeoweaver/sc_list.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.8/pygeoweaver/sc_run.py` & `pygeoweaver-0.6.9/pygeoweaver/sc_run.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.8/pygeoweaver/server.py` & `pygeoweaver-0.6.9/pygeoweaver/server.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.8/pygeoweaver/utils.py` & `pygeoweaver-0.6.9/pygeoweaver/utils.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.8/pygeoweaver.egg-info/PKG-INFO` & `pygeoweaver-0.6.9/pygeoweaver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.6.8
+Version: 0.6.9
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygeoweaver-0.6.8/pygeoweaver.egg-info/SOURCES.txt` & `pygeoweaver-0.6.9/pygeoweaver.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 pygeoweaver/__init__.py
 pygeoweaver/__main__.py
 pygeoweaver/constants.py
+pygeoweaver/download_gw.bat
+pygeoweaver/download_gw.sh
 pygeoweaver/sc_detail.py
 pygeoweaver/sc_export.py
 pygeoweaver/sc_help.py
 pygeoweaver/sc_history.py
 pygeoweaver/sc_import.py
 pygeoweaver/sc_interface.py
 pygeoweaver/sc_list.py
 pygeoweaver/sc_resetpassword.py
 pygeoweaver/sc_run.py
 pygeoweaver/server.py
+pygeoweaver/start.bat
+pygeoweaver/start.sh
+pygeoweaver/stop.bat
+pygeoweaver/stop.sh
 pygeoweaver/utils.py
 pygeoweaver.egg-info/PKG-INFO
 pygeoweaver.egg-info/SOURCES.txt
 pygeoweaver.egg-info/dependency_links.txt
 pygeoweaver.egg-info/top_level.txt
 test/__init__.py
 test/test_detail.py
```

### Comparing `pygeoweaver-0.6.8/pyproject.toml` & `pygeoweaver-0.6.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "pytest-cov"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygeoweaver"
-version = "0.6.8"
+version = "0.6.9"
 authors = [
   { name="Geoweaver team", email="geoweaver.app@gmail.com" },
 ]
 description = "This is a wrapper package of the Geoweaver app."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -18,15 +18,15 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry]
 name = "pygeoweaver"
-version = "0.6.8"
+version = "0.6.9"
 description = "This is a wrapper package of the Geoweaver app."
 authors = ["Geoweaver team <geoweaver.app@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
```

### Comparing `pygeoweaver-0.6.8/test/test_detail.py` & `pygeoweaver-0.6.9/test/test_detail.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.8/test/test_server.py` & `pygeoweaver-0.6.9/test/test_server.py`

 * *Files identical despite different names*

