# Comparing `tmp/tira-0.0.8.tar.gz` & `tmp/tira-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tira-0.0.8.tar", last modified: Tue Feb  7 16:48:40 2023, max compression
+gzip compressed data, was "tira-0.0.9.tar", last modified: Tue Feb  7 17:49:38 2023, max compression
```

## Comparing `tira-0.0.8.tar` & `tira-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-02-07 16:48:40.319409 tira-0.0.8/
--rw-r--r--   0 maik      (1000) maik      (1000)      810 2023-02-07 16:48:40.319409 tira-0.0.8/PKG-INFO
--rw-r--r--   0 maik      (1000) maik      (1000)      999 2023-02-07 16:48:40.329409 tira-0.0.8/setup.cfg
--rw-r--r--   0 maik      (1000) maik      (1000)       39 2023-01-26 17:02:55.000000 tira-0.0.8/setup.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-02-07 16:48:40.319409 tira-0.0.8/tira/
--rw-r--r--   0 maik      (1000) maik      (1000)       23 2023-02-07 16:48:35.000000 tira-0.0.8/tira/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)     1012 2023-02-04 08:06:23.000000 tira-0.0.8/tira/io_utils.py
--rw-r--r--   0 maik      (1000) maik      (1000)     3609 2023-02-04 08:01:37.000000 tira-0.0.8/tira/rest_api_client.py
--rw-r--r--   0 maik      (1000) maik      (1000)     4220 2023-02-07 16:47:56.000000 tira-0.0.8/tira/third_party_integrations.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-02-07 16:48:40.319409 tira-0.0.8/tira.egg-info/
--rw-r--r--   0 maik      (1000) maik      (1000)      810 2023-02-07 16:48:40.000000 tira-0.0.8/tira.egg-info/PKG-INFO
--rw-r--r--   0 maik      (1000) maik      (1000)      248 2023-02-07 16:48:40.000000 tira-0.0.8/tira.egg-info/SOURCES.txt
--rw-r--r--   0 maik      (1000) maik      (1000)        1 2023-02-07 16:48:40.000000 tira-0.0.8/tira.egg-info/dependency_links.txt
--rw-r--r--   0 maik      (1000) maik      (1000)       69 2023-02-07 16:48:40.000000 tira-0.0.8/tira.egg-info/requires.txt
--rw-r--r--   0 maik      (1000) maik      (1000)        5 2023-02-07 16:48:40.000000 tira-0.0.8/tira.egg-info/top_level.txt
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-02-07 17:49:38.238439 tira-0.0.9/
+-rw-r--r--   0 maik      (1000) maik      (1000)      810 2023-02-07 17:49:38.238439 tira-0.0.9/PKG-INFO
+-rw-r--r--   0 maik      (1000) maik      (1000)      999 2023-02-07 17:49:38.238439 tira-0.0.9/setup.cfg
+-rw-r--r--   0 maik      (1000) maik      (1000)       39 2023-01-26 17:02:55.000000 tira-0.0.9/setup.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-02-07 17:49:38.238439 tira-0.0.9/tira/
+-rw-r--r--   0 maik      (1000) maik      (1000)       23 2023-02-07 17:47:57.000000 tira-0.0.9/tira/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1012 2023-02-04 08:06:23.000000 tira-0.0.9/tira/io_utils.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     3609 2023-02-04 08:01:37.000000 tira-0.0.9/tira/rest_api_client.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     4213 2023-02-07 16:58:55.000000 tira-0.0.9/tira/third_party_integrations.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-02-07 17:49:38.238439 tira-0.0.9/tira.egg-info/
+-rw-r--r--   0 maik      (1000) maik      (1000)      810 2023-02-07 17:49:38.000000 tira-0.0.9/tira.egg-info/PKG-INFO
+-rw-r--r--   0 maik      (1000) maik      (1000)      248 2023-02-07 17:49:38.000000 tira-0.0.9/tira.egg-info/SOURCES.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)        1 2023-02-07 17:49:38.000000 tira-0.0.9/tira.egg-info/dependency_links.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)       69 2023-02-07 17:49:38.000000 tira-0.0.9/tira.egg-info/requires.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)        5 2023-02-07 17:49:38.000000 tira-0.0.9/tira.egg-info/top_level.txt
```

### Comparing `tira-0.0.8/PKG-INFO` & `tira-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tira
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple access to the TIRA API.
 Home-page: https://github.com/tira-io/tira
 Author: Maik Fröbe
 Author-email: maik.froebe@uni-weimar.de
 Maintainer: Maik Fröbe
 Project-URL: Bug Tracker, https://github.com/tira-io/tira/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tira-0.0.8/setup.cfg` & `tira-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `tira-0.0.8/tira/io_utils.py` & `tira-0.0.9/tira/io_utils.py`

 * *Files identical despite different names*

### Comparing `tira-0.0.8/tira/rest_api_client.py` & `tira-0.0.9/tira/rest_api_client.py`

 * *Files identical despite different names*

### Comparing `tira-0.0.8/tira/third_party_integrations.py` & `tira-0.0.9/tira/third_party_integrations.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
     run['system'] = system_name
     run = run.copy().sort_values(["qid", "score", "docno"], ascending=[True, False, False]).reset_index()
 
     if 'Q0' not in run.columns:
         run['Q0'] = 0
 
-    run = run.groupby("qid")[["qid", "Q0", "docno", "rank", "score", "system"]].head(1000)
+    run = run.groupby("qid")[["qid", "Q0", "docno", "score", "system"]].head(depth)
 
     # Make sure that rank position starts by 1
     run["rank"] = 1
     run["rank"] = run.groupby("qid")["rank"].cumsum()
     
     return run[['qid', 'Q0', 'docno', 'rank', 'score', 'system']]
```

### Comparing `tira-0.0.8/tira.egg-info/PKG-INFO` & `tira-0.0.9/tira.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tira
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple access to the TIRA API.
 Home-page: https://github.com/tira-io/tira
 Author: Maik Fröbe
 Author-email: maik.froebe@uni-weimar.de
 Maintainer: Maik Fröbe
 Project-URL: Bug Tracker, https://github.com/tira-io/tira/issues
 Classifier: Programming Language :: Python :: 3
```

