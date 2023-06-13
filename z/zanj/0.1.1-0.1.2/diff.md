# Comparing `tmp/zanj-0.1.1.tar.gz` & `tmp/zanj-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zanj-0.1.1.tar", max compression
+gzip compressed data, was "zanj-0.1.2.tar", max compression
```

## Comparing `zanj-0.1.1.tar` & `zanj-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 zanj-0.1.1/LICENSE
--rw-r--r--   0        0        0      937 2023-05-28 07:22:02.319290 zanj-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4213 2023-05-28 05:11:39.608638 zanj-0.1.1/README.md
--rw-r--r--   0        0        0      146 2023-05-28 07:19:30.975404 zanj-0.1.1/zanj/__init__.py
--rw-r--r--   0        0        0     1468 2023-05-28 05:22:18.527493 zanj-0.1.1/zanj/externals.py
--rw-r--r--   0        0        0    15618 2023-05-28 05:22:18.537492 zanj-0.1.1/zanj/loading.py
--rw-r--r--   0        0        0     4143 2023-05-28 05:13:20.057826 zanj-0.1.1/zanj/readme.md
--rw-r--r--   0        0        0     8121 2023-05-28 05:22:18.541492 zanj-0.1.1/zanj/serializing.py
--rw-r--r--   0        0        0     9696 2023-05-28 05:22:18.549492 zanj-0.1.1/zanj/torchutil.py
--rw-r--r--   0        0        0     8468 2023-05-28 05:22:18.555490 zanj-0.1.1/zanj/zanj.py
--rw-r--r--   0        0        0     5089 1970-01-01 00:00:00.000000 zanj-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 zanj-0.1.2/LICENSE
+-rw-r--r--   0        0        0      937 2023-06-13 22:17:51.834629 zanj-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4291 2023-05-28 07:47:30.325865 zanj-0.1.2/README.md
+-rw-r--r--   0        0        0      146 2023-06-13 22:17:56.392498 zanj-0.1.2/zanj/__init__.py
+-rw-r--r--   0        0        0     1468 2023-05-28 05:22:18.527493 zanj-0.1.2/zanj/externals.py
+-rw-r--r--   0        0        0    15618 2023-05-28 05:22:18.537492 zanj-0.1.2/zanj/loading.py
+-rw-r--r--   0        0        0        0 2023-06-13 22:16:55.290434 zanj-0.1.2/zanj/py.typed
+-rw-r--r--   0        0        0     4143 2023-05-28 05:13:20.057826 zanj-0.1.2/zanj/readme.md
+-rw-r--r--   0        0        0     8121 2023-05-28 05:22:18.541492 zanj-0.1.2/zanj/serializing.py
+-rw-r--r--   0        0        0     9696 2023-05-28 05:22:18.549492 zanj-0.1.2/zanj/torchutil.py
+-rw-r--r--   0        0        0     8468 2023-05-28 05:22:18.555490 zanj-0.1.2/zanj/zanj.py
+-rw-r--r--   0        0        0     5167 1970-01-01 00:00:00.000000 zanj-0.1.2/PKG-INFO
```

### Comparing `zanj-0.1.1/LICENSE` & `zanj-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zanj-0.1.1/pyproject.toml` & `zanj-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zanj"
-version = "0.1.1"
+version = "0.1.2"
 description = "save and load complex objects to disk without pickling"
 license = "GPL-3.0-only"
 authors = ["mivanit <mivanits@umich.edu>"]
 readme = "README.md"
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `zanj-0.1.1/README.md` & `zanj-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # ZANJ
 
+# installation
+PyPi: https://pypi.org/project/zanj/
+
+```
+pip install zanj
+```
 
 # Overview
 
 The `ZANJ` format is meant to be a way of saving arbitrary objects to disk, in a way that is flexible, allows to keep configuration and data together, and is human readable. It is loosely inspired by HDF5 and the derived `exdir` format, and the implementation is similar to `npz` files. The on-disk format is as follows:
 
 a file `<filename>.zanj` is a zip file containing:
```

### Comparing `zanj-0.1.1/zanj/externals.py` & `zanj-0.1.2/zanj/externals.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.1/zanj/loading.py` & `zanj-0.1.2/zanj/loading.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.1/zanj/readme.md` & `zanj-0.1.2/zanj/readme.md`

 * *Files identical despite different names*

### Comparing `zanj-0.1.1/zanj/serializing.py` & `zanj-0.1.2/zanj/serializing.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.1/zanj/torchutil.py` & `zanj-0.1.2/zanj/torchutil.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.1/zanj/zanj.py` & `zanj-0.1.2/zanj/zanj.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.1/PKG-INFO` & `zanj-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zanj
-Version: 0.1.1
+Version: 0.1.2
 Summary: save and load complex objects to disk without pickling
 Home-page: https://github.com/mivanit/ZANJ
 License: GPL-3.0-only
 Author: mivanit
 Author-email: mivanits@umich.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -19,14 +19,20 @@
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: torch (>=1.13.1,<2.0.0)
 Project-URL: Repository, https://github.com/mivanit/ZANJ
 Description-Content-Type: text/markdown
 
 # ZANJ
 
+# installation
+PyPi: https://pypi.org/project/zanj/
+
+```
+pip install zanj
+```
 
 # Overview
 
 The `ZANJ` format is meant to be a way of saving arbitrary objects to disk, in a way that is flexible, allows to keep configuration and data together, and is human readable. It is loosely inspired by HDF5 and the derived `exdir` format, and the implementation is similar to `npz` files. The on-disk format is as follows:
 
 a file `<filename>.zanj` is a zip file containing:
```

