# Comparing `tmp/ssi_fctrading-1.0.0.tar.gz` & `tmp/ssi_fctrading-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssi_fctrading-1.0.0.tar", last modified: Wed Jun 14 02:46:12 2023, max compression
+gzip compressed data, was "ssi_fctrading-1.1.0.tar", last modified: Wed Jun 14 03:59:13 2023, max compression
```

## Comparing `ssi_fctrading-1.0.0.tar` & `ssi_fctrading-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:46:12.816758 ssi_fctrading-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      983 2023-06-14 02:46:12.816758 ssi_fctrading-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      356 2023-06-14 02:46:04.000000 ssi_fctrading-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)      149 2023-06-14 02:46:12.816758 ssi_fctrading-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1641 2023-06-14 02:46:04.000000 ssi_fctrading-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:46:12.812758 ssi_fctrading-1.0.0/ssi_fctrading/
--rw-r--r--   0 root         (0) root         (0)      260 2023-06-14 02:46:10.000000 ssi_fctrading-1.0.0/ssi_fctrading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:46:12.816758 ssi_fctrading-1.0.0/ssi_fctrading/constant/
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-14 02:46:04.000000 ssi_fctrading-1.0.0/ssi_fctrading/constant/__init__.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-06-14 02:46:04.000000 ssi_fctrading-1.0.0/ssi_fctrading/constant/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:46:12.816758 ssi_fctrading-1.0.0/ssi_fctrading/core/
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-14 02:46:04.000000 ssi_fctrading-1.0.0/ssi_fctrading/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-06-14 02:46:04.000000 ssi_fctrading-1.0.0/ssi_fctrading/core/core_crypto.py
--rw-r--r--   0 root         (0) root         (0)      427 2023-06-14 02:46:04.000000 ssi_fctrading-1.0.0/ssi_fctrading/core/core_helper.py
--rw-r--r--   0 root         (0) root         (0)     6154 2023-06-14 02:46:04.000000 ssi_fctrading-1.0.0/ssi_fctrading/fc_client.py
--rw-r--r--   0 root         (0) root         (0)     1329 2023-06-14 02:46:04.000000 ssi_fctrading-1.0.0/ssi_fctrading/fc_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:46:12.816758 ssi_fctrading-1.0.0/ssi_fctrading/models/
--rw-r--r--   0 root         (0) root         (0)      571 2023-06-14 02:46:04.000000 ssi_fctrading-1.0.0/ssi_fctrading/models/AccessTokenModel.py
--rw-r--r--   0 root         (0) root         (0)     1734 2023-06-14 02:46:04.000000 ssi_fctrading-1.0.0/ssi_fctrading/models/Requests.py
--rw-r--r--   0 root         (0) root         (0)      191 2023-06-14 02:46:04.000000 ssi_fctrading-1.0.0/ssi_fctrading/models/Responses.py
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-14 02:46:04.000000 ssi_fctrading-1.0.0/ssi_fctrading/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:46:12.812758 ssi_fctrading-1.0.0/ssi_fctrading.egg-info/
--rw-r--r--   0 root         (0) root         (0)      983 2023-06-14 02:46:12.000000 ssi_fctrading-1.0.0/ssi_fctrading.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      597 2023-06-14 02:46:12.000000 ssi_fctrading-1.0.0/ssi_fctrading.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 02:46:12.000000 ssi_fctrading-1.0.0/ssi_fctrading.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-14 02:46:12.000000 ssi_fctrading-1.0.0/ssi_fctrading.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-14 02:46:12.000000 ssi_fctrading-1.0.0/ssi_fctrading.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 03:59:13.478983 ssi_fctrading-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      983 2023-06-14 03:59:13.478983 ssi_fctrading-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      356 2023-06-14 03:58:43.000000 ssi_fctrading-1.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-14 03:59:13.478983 ssi_fctrading-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1641 2023-06-14 03:58:43.000000 ssi_fctrading-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 03:59:13.474983 ssi_fctrading-1.1.0/ssi_fctrading/
+-rw-r--r--   0 root         (0) root         (0)      260 2023-06-14 03:59:11.000000 ssi_fctrading-1.1.0/ssi_fctrading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 03:59:13.474983 ssi_fctrading-1.1.0/ssi_fctrading/constant/
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-14 03:58:43.000000 ssi_fctrading-1.1.0/ssi_fctrading/constant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      992 2023-06-14 03:58:43.000000 ssi_fctrading-1.1.0/ssi_fctrading/constant/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 03:59:13.474983 ssi_fctrading-1.1.0/ssi_fctrading/core/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-14 03:58:43.000000 ssi_fctrading-1.1.0/ssi_fctrading/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-06-14 03:58:43.000000 ssi_fctrading-1.1.0/ssi_fctrading/core/core_crypto.py
+-rw-r--r--   0 root         (0) root         (0)      427 2023-06-14 03:58:43.000000 ssi_fctrading-1.1.0/ssi_fctrading/core/core_helper.py
+-rw-r--r--   0 root         (0) root         (0)     6154 2023-06-14 03:58:43.000000 ssi_fctrading-1.1.0/ssi_fctrading/fc_client.py
+-rw-r--r--   0 root         (0) root         (0)     1329 2023-06-14 03:58:43.000000 ssi_fctrading-1.1.0/ssi_fctrading/fc_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 03:59:13.478983 ssi_fctrading-1.1.0/ssi_fctrading/models/
+-rw-r--r--   0 root         (0) root         (0)      571 2023-06-14 03:58:43.000000 ssi_fctrading-1.1.0/ssi_fctrading/models/AccessTokenModel.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-06-14 03:58:43.000000 ssi_fctrading-1.1.0/ssi_fctrading/models/Requests.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-06-14 03:58:43.000000 ssi_fctrading-1.1.0/ssi_fctrading/models/Responses.py
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-14 03:58:43.000000 ssi_fctrading-1.1.0/ssi_fctrading/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 03:59:13.474983 ssi_fctrading-1.1.0/ssi_fctrading.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      983 2023-06-14 03:59:13.000000 ssi_fctrading-1.1.0/ssi_fctrading.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-14 03:59:13.000000 ssi_fctrading-1.1.0/ssi_fctrading.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 03:59:13.000000 ssi_fctrading-1.1.0/ssi_fctrading.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-14 03:59:13.000000 ssi_fctrading-1.1.0/ssi_fctrading.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-14 03:59:13.000000 ssi_fctrading-1.1.0/ssi_fctrading.egg-info/top_level.txt
```

### Comparing `ssi_fctrading-1.0.0/PKG-INFO` & `ssi_fctrading-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssi_fctrading
-Version: 1.0.0
+Version: 1.1.0
 Summary: FastConnect TradingAPI client by Python
 Home-page: https://github.com/SSI-Securities-Corporation/python-fctrading
 Author: ducdv
 Author-email: ducdv@ssi.com.vn
 License: MIT
 Platform: POSIX
 Platform: Windows
```

### Comparing `ssi_fctrading-1.0.0/setup.py` & `ssi_fctrading-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `ssi_fctrading-1.0.0/ssi_fctrading/constant/api.py` & `ssi_fctrading-1.1.0/ssi_fctrading/constant/api.py`

 * *Files identical despite different names*

### Comparing `ssi_fctrading-1.0.0/ssi_fctrading/core/core_crypto.py` & `ssi_fctrading-1.1.0/ssi_fctrading/core/core_crypto.py`

 * *Files identical despite different names*

### Comparing `ssi_fctrading-1.0.0/ssi_fctrading/fc_client.py` & `ssi_fctrading-1.1.0/ssi_fctrading/fc_client.py`

 * *Files identical despite different names*

### Comparing `ssi_fctrading-1.0.0/ssi_fctrading/fc_stream.py` & `ssi_fctrading-1.1.0/ssi_fctrading/fc_stream.py`

 * *Files identical despite different names*

### Comparing `ssi_fctrading-1.0.0/ssi_fctrading/models/AccessTokenModel.py` & `ssi_fctrading-1.1.0/ssi_fctrading/models/AccessTokenModel.py`

 * *Files identical despite different names*

### Comparing `ssi_fctrading-1.0.0/ssi_fctrading/models/Requests.py` & `ssi_fctrading-1.1.0/ssi_fctrading/models/Requests.py`

 * *Files identical despite different names*

### Comparing `ssi_fctrading-1.0.0/ssi_fctrading.egg-info/PKG-INFO` & `ssi_fctrading-1.1.0/ssi_fctrading.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssi-fctrading
-Version: 1.0.0
+Version: 1.1.0
 Summary: FastConnect TradingAPI client by Python
 Home-page: https://github.com/SSI-Securities-Corporation/python-fctrading
 Author: ducdv
 Author-email: ducdv@ssi.com.vn
 License: MIT
 Platform: POSIX
 Platform: Windows
```

### Comparing `ssi_fctrading-1.0.0/ssi_fctrading.egg-info/SOURCES.txt` & `ssi_fctrading-1.1.0/ssi_fctrading.egg-info/SOURCES.txt`

 * *Files identical despite different names*

