# Comparing `tmp/philipstv_gui-1.1.0.tar.gz` & `tmp/philipstv_gui-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philipstv_gui-1.1.0.tar", max compression
+gzip compressed data, was "philipstv_gui-1.1.1.tar", max compression
```

## Comparing `philipstv_gui-1.1.0.tar` & `philipstv_gui-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1079 2022-04-13 18:06:23.352265 philipstv_gui-1.1.0/LICENSE
--rw-r--r--   0        0        0     1316 2023-01-15 10:54:26.163383 philipstv_gui-1.1.0/README.md
--rw-r--r--   0        0        0     1751 2023-01-16 18:41:16.003198 philipstv_gui-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       84 2023-01-15 10:54:26.173383 philipstv_gui-1.1.0/src/philipstv_gui/__init__.py
--rw-r--r--   0        0        0      118 2022-03-15 18:59:28.946042 philipstv_gui-1.1.0/src/philipstv_gui/__main__.py
--rw-r--r--   0        0        0     4930 2022-04-12 17:53:10.968676 philipstv_gui-1.1.0/src/philipstv_gui/ambilight.py
--rw-r--r--   0        0        0      662 2022-03-23 18:50:58.528468 philipstv_gui-1.1.0/src/philipstv_gui/app.py
--rw-r--r--   0        0        0     1559 2022-03-24 19:37:57.213576 philipstv_gui-1.1.0/src/philipstv_gui/applications.py
--rw-r--r--   0        0        0     1694 2022-03-24 19:37:57.213576 philipstv_gui-1.1.0/src/philipstv_gui/channels.py
--rw-r--r--   0        0        0     1382 2022-03-24 19:37:57.210243 philipstv_gui-1.1.0/src/philipstv_gui/connector.py
--rw-r--r--   0        0        0     1089 2022-03-24 19:37:57.213576 philipstv_gui-1.1.0/src/philipstv_gui/errors.py
--rw-r--r--   0        0        0     3820 2022-04-12 17:53:10.968676 philipstv_gui-1.1.0/src/philipstv_gui/frame.py
--rw-r--r--   0        0        0     7672 2022-04-12 17:53:10.968676 philipstv_gui-1.1.0/src/philipstv_gui/remote.py
--rw-r--r--   0        0        0     1021 2022-03-23 18:47:30.489900 philipstv_gui-1.1.0/src/philipstv_gui/storage.py
--rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 philipstv_gui-1.1.0/setup.py
--rw-r--r--   0        0        0     2356 1970-01-01 00:00:00.000000 philipstv_gui-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-14 17:21:26.746320 philipstv_gui-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1316 2023-06-14 17:21:26.746320 philipstv_gui-1.1.1/README.md
+-rw-r--r--   0        0        0     1758 2023-06-14 18:04:54.882700 philipstv_gui-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-06-14 17:21:26.746320 philipstv_gui-1.1.1/src/philipstv_gui/__init__.py
+-rw-r--r--   0        0        0      118 2023-06-14 17:21:26.746320 philipstv_gui-1.1.1/src/philipstv_gui/__main__.py
+-rw-r--r--   0        0        0     4930 2023-06-14 17:21:26.746320 philipstv_gui-1.1.1/src/philipstv_gui/ambilight.py
+-rw-r--r--   0        0        0      662 2023-06-14 17:21:26.746320 philipstv_gui-1.1.1/src/philipstv_gui/app.py
+-rw-r--r--   0        0        0     1559 2023-06-14 17:21:26.746320 philipstv_gui-1.1.1/src/philipstv_gui/applications.py
+-rw-r--r--   0        0        0     1694 2023-06-14 17:21:26.746320 philipstv_gui-1.1.1/src/philipstv_gui/channels.py
+-rw-r--r--   0        0        0     1382 2023-06-14 17:21:26.746320 philipstv_gui-1.1.1/src/philipstv_gui/connector.py
+-rw-r--r--   0        0        0     1089 2023-06-14 17:21:26.746320 philipstv_gui-1.1.1/src/philipstv_gui/errors.py
+-rw-r--r--   0        0        0     3820 2023-06-14 17:21:26.746320 philipstv_gui-1.1.1/src/philipstv_gui/frame.py
+-rw-r--r--   0        0        0     7672 2023-06-14 17:21:26.746320 philipstv_gui-1.1.1/src/philipstv_gui/remote.py
+-rw-r--r--   0        0        0     1021 2023-06-14 17:21:26.746320 philipstv_gui-1.1.1/src/philipstv_gui/storage.py
+-rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 philipstv_gui-1.1.1/PKG-INFO
```

### Comparing `philipstv_gui-1.1.0/LICENSE` & `philipstv_gui-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `philipstv_gui-1.1.0/README.md` & `philipstv_gui-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `philipstv_gui-1.1.0/pyproject.toml` & `philipstv_gui-1.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philipstv-gui"
-version = "1.1.0"  # this will be set during build by poetry-dynamic-versioning
+version = "1.1.1"  # this will be set during build by poetry-dynamic-versioning
 description = "GUI remote for Philips Android-powered TVs."
 license = "MIT"
 authors = ["Bazyli Cyran <bazyli.cyran@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/bcyran/philipstv-gui"
 keywords = ["philips", "tv", "remote", "ambilight", "gui"]
 classifiers = [
@@ -28,24 +28,24 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 philipstv = ">=0.4,<2"
 appdirs = "^1.4.4"
 ttkbootstrap = "^1.7.3"
 
 [tool.poetry.dev-dependencies]
-black = "^22.12.0"
-isort = "^5.11.4"
+black = "^23.3.0"
+isort = "^5.12.0"
 flake8 = "^6.0.0"
-mypy = "^0.991"
-tox = "^4.2.8"
-types-appdirs = "^1.4.2"
+mypy = "^1.3"
+tox = "^4.5.2"
+types-appdirs = "^1.4.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 pattern = """(?x)
 ^(?P<base>\\d+(\\.\\d+)*)
```

### Comparing `philipstv_gui-1.1.0/src/philipstv_gui/ambilight.py` & `philipstv_gui-1.1.1/src/philipstv_gui/ambilight.py`

 * *Files identical despite different names*

### Comparing `philipstv_gui-1.1.0/src/philipstv_gui/app.py` & `philipstv_gui-1.1.1/src/philipstv_gui/app.py`

 * *Files identical despite different names*

### Comparing `philipstv_gui-1.1.0/src/philipstv_gui/applications.py` & `philipstv_gui-1.1.1/src/philipstv_gui/applications.py`

 * *Files identical despite different names*

### Comparing `philipstv_gui-1.1.0/src/philipstv_gui/channels.py` & `philipstv_gui-1.1.1/src/philipstv_gui/channels.py`

 * *Files identical despite different names*

### Comparing `philipstv_gui-1.1.0/src/philipstv_gui/connector.py` & `philipstv_gui-1.1.1/src/philipstv_gui/connector.py`

 * *Files identical despite different names*

### Comparing `philipstv_gui-1.1.0/src/philipstv_gui/errors.py` & `philipstv_gui-1.1.1/src/philipstv_gui/errors.py`

 * *Files identical despite different names*

### Comparing `philipstv_gui-1.1.0/src/philipstv_gui/frame.py` & `philipstv_gui-1.1.1/src/philipstv_gui/frame.py`

 * *Files identical despite different names*

### Comparing `philipstv_gui-1.1.0/src/philipstv_gui/remote.py` & `philipstv_gui-1.1.1/src/philipstv_gui/remote.py`

 * *Files identical despite different names*

### Comparing `philipstv_gui-1.1.0/src/philipstv_gui/storage.py` & `philipstv_gui-1.1.1/src/philipstv_gui/storage.py`

 * *Files identical despite different names*

### Comparing `philipstv_gui-1.1.0/PKG-INFO` & `philipstv_gui-1.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: philipstv-gui
-Version: 1.1.0
+Version: 1.1.1
 Summary: GUI remote for Philips Android-powered TVs.
 Home-page: https://github.com/bcyran/philipstv-gui
 License: MIT
 Keywords: philips,tv,remote,ambilight,gui
 Author: Bazyli Cyran
 Author-email: bazyli.cyran@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: philipstv (>=0.4,<2)
 Requires-Dist: ttkbootstrap (>=1.7.3,<2.0.0)
 Project-URL: Repository, https://github.com/bcyran/philipstv-gui
 Description-Content-Type: text/markdown
 
 # PhilipstvTV GUI
```

