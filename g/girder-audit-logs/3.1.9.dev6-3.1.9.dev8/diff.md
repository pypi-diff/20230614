# Comparing `tmp/girder-audit-logs-3.1.9.dev6.tar.gz` & `tmp/girder-audit-logs-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-audit-logs-3.1.9.dev6.tar", last modified: Wed Feb 23 16:09:28 2022, max compression
+gzip compressed data, was "dist/girder-audit-logs-3.1.9.dev8.tar", last modified: Wed Feb 23 17:41:29 2022, max compression
```

## Comparing `girder-audit-logs-3.1.9.dev6.tar` & `girder-audit-logs-3.1.9.dev8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:28.000000 girder-audit-logs-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:28.000000 girder-audit-logs-3.1.9.dev6/girder_audit_logs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1963 2022-02-23 16:09:15.000000 girder-audit-logs-3.1.9.dev6/girder_audit_logs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      838 2022-02-23 16:09:15.000000 girder-audit-logs-3.1.9.dev6/girder_audit_logs/cleanup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2559 2022-02-23 16:09:15.000000 girder-audit-logs-3.1.9.dev6/girder_audit_logs/report.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:28.000000 girder-audit-logs-3.1.9.dev6/girder_audit_logs.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      712 2022-02-23 16:09:28.000000 girder-audit-logs-3.1.9.dev6/girder_audit_logs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      383 2022-02-23 16:09:28.000000 girder-audit-logs-3.1.9.dev6/girder_audit_logs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:28.000000 girder-audit-logs-3.1.9.dev6/girder_audit_logs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      193 2022-02-23 16:09:28.000000 girder-audit-logs-3.1.9.dev6/girder_audit_logs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:28.000000 girder-audit-logs-3.1.9.dev6/girder_audit_logs.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 16:09:28.000000 girder-audit-logs-3.1.9.dev6/girder_audit_logs.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       18 2022-02-23 16:09:28.000000 girder-audit-logs-3.1.9.dev6/girder_audit_logs.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1837 2022-02-23 16:09:15.000000 girder-audit-logs-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      712 2022-02-23 16:09:28.000000 girder-audit-logs-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:09:28.000000 girder-audit-logs-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:29.000000 girder-audit-logs-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:29.000000 girder-audit-logs-3.1.9.dev8/girder_audit_logs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1963 2022-02-23 17:41:16.000000 girder-audit-logs-3.1.9.dev8/girder_audit_logs/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      838 2022-02-23 17:41:16.000000 girder-audit-logs-3.1.9.dev8/girder_audit_logs/cleanup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2559 2022-02-23 17:41:16.000000 girder-audit-logs-3.1.9.dev8/girder_audit_logs/report.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:29.000000 girder-audit-logs-3.1.9.dev8/girder_audit_logs.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      712 2022-02-23 17:41:29.000000 girder-audit-logs-3.1.9.dev8/girder_audit_logs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      383 2022-02-23 17:41:29.000000 girder-audit-logs-3.1.9.dev8/girder_audit_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:29.000000 girder-audit-logs-3.1.9.dev8/girder_audit_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      193 2022-02-23 17:41:29.000000 girder-audit-logs-3.1.9.dev8/girder_audit_logs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:29.000000 girder-audit-logs-3.1.9.dev8/girder_audit_logs.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 17:41:29.000000 girder-audit-logs-3.1.9.dev8/girder_audit_logs.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       18 2022-02-23 17:41:29.000000 girder-audit-logs-3.1.9.dev8/girder_audit_logs.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1837 2022-02-23 17:41:16.000000 girder-audit-logs-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      712 2022-02-23 17:41:29.000000 girder-audit-logs-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:41:29.000000 girder-audit-logs-3.1.9.dev8/setup.cfg
```

### Comparing `girder-audit-logs-3.1.9.dev6/girder_audit_logs/__init__.py` & `girder-audit-logs-3.1.9.dev8/girder_audit_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-audit-logs-3.1.9.dev6/girder_audit_logs/cleanup.py` & `girder-audit-logs-3.1.9.dev8/girder_audit_logs/cleanup.py`

 * *Files identical despite different names*

### Comparing `girder-audit-logs-3.1.9.dev6/girder_audit_logs/report.py` & `girder-audit-logs-3.1.9.dev8/girder_audit_logs/report.py`

 * *Files identical despite different names*

### Comparing `girder-audit-logs-3.1.9.dev6/girder_audit_logs.egg-info/PKG-INFO` & `girder-audit-logs-3.1.9.dev8/girder_audit_logs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-audit-logs
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Keeps detailed logs of every REST request and low-level file download event.
 Home-page: UNKNOWN
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `girder-audit-logs-3.1.9.dev6/setup.py` & `girder-audit-logs-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-audit-logs-3.1.9.dev6/PKG-INFO` & `girder-audit-logs-3.1.9.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-audit-logs
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Keeps detailed logs of every REST request and low-level file download event.
 Home-page: UNKNOWN
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

