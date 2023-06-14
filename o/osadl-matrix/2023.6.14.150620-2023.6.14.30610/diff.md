# Comparing `tmp/osadl-matrix-2023.6.14.150620.tar.gz` & `tmp/osadl-matrix-2023.6.14.30610.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osadl-matrix-2023.6.14.150620.tar", last modified: Wed Jun 14 15:00:23 2023, max compression
+gzip compressed data, was "osadl-matrix-2023.6.14.30610.tar", last modified: Wed Jun 14 03:19:16 2023, max compression
```

## Comparing `osadl-matrix-2023.6.14.150620.tar` & `osadl-matrix-2023.6.14.30610.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:00:23.808478 osadl-matrix-2023.6.14.150620/
--rw-r--r--   0 runner    (1001) docker     (123)    18956 2023-06-14 14:59:56.000000 osadl-matrix-2023.6.14.150620/DATALOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-14 14:59:56.000000 osadl-matrix-2023.6.14.150620/LICENSE.Unlicensed
--rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-06-14 14:59:56.000000 osadl-matrix-2023.6.14.150620/LICENSE.ccby40
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-14 14:59:56.000000 osadl-matrix-2023.6.14.150620/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-14 15:00:23.808478 osadl-matrix-2023.6.14.150620/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-14 14:59:56.000000 osadl-matrix-2023.6.14.150620/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 15:00:20.000000 osadl-matrix-2023.6.14.150620/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:00:23.808478 osadl-matrix-2023.6.14.150620/osadl_matrix/
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-06-14 14:59:56.000000 osadl-matrix-2023.6.14.150620/osadl_matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38552 2023-06-14 14:59:56.000000 osadl-matrix-2023.6.14.150620/osadl_matrix/osadl-matrix.csv
--rw-r--r--   0 runner    (1001) docker     (123)   213361 2023-06-14 14:59:56.000000 osadl-matrix-2023.6.14.150620/osadl_matrix/osadl-matrix.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:00:23.808478 osadl-matrix-2023.6.14.150620/osadl_matrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-14 15:00:23.000000 osadl-matrix-2023.6.14.150620/osadl_matrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-14 15:00:23.000000 osadl-matrix-2023.6.14.150620/osadl_matrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:00:23.000000 osadl-matrix-2023.6.14.150620/osadl_matrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-14 15:00:23.000000 osadl-matrix-2023.6.14.150620/osadl_matrix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 15:00:23.000000 osadl-matrix-2023.6.14.150620/osadl_matrix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-14 14:59:56.000000 osadl-matrix-2023.6.14.150620/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:59:56.000000 osadl-matrix-2023.6.14.150620/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-14 15:00:23.808478 osadl-matrix-2023.6.14.150620/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-14 14:59:56.000000 osadl-matrix-2023.6.14.150620/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:19:16.815147 osadl-matrix-2023.6.14.30610/
+-rw-r--r--   0 runner    (1001) docker     (123)    18956 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/DATALOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/LICENSE.Unlicensed
+-rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/LICENSE.ccby40
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-14 03:19:16.815147 osadl-matrix-2023.6.14.30610/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 03:19:10.000000 osadl-matrix-2023.6.14.30610/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:19:16.811147 osadl-matrix-2023.6.14.30610/osadl_matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/osadl_matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38552 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/osadl_matrix/osadl-matrix.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   213361 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/osadl_matrix/osadl-matrix.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:19:16.815147 osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-14 03:19:16.000000 osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-14 03:19:16.000000 osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:19:16.000000 osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-14 03:19:16.000000 osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 03:19:16.000000 osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-14 03:19:16.815147 osadl-matrix-2023.6.14.30610/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/setup.py
```

### Comparing `osadl-matrix-2023.6.14.150620/DATALOG.md` & `osadl-matrix-2023.6.14.30610/DATALOG.md`

 * *Files identical despite different names*

### Comparing `osadl-matrix-2023.6.14.150620/LICENSE.Unlicensed` & `osadl-matrix-2023.6.14.30610/LICENSE.Unlicensed`

 * *Files identical despite different names*

### Comparing `osadl-matrix-2023.6.14.150620/LICENSE.ccby40` & `osadl-matrix-2023.6.14.30610/LICENSE.ccby40`

 * *Files identical despite different names*

### Comparing `osadl-matrix-2023.6.14.150620/PKG-INFO` & `osadl-matrix-2023.6.14.30610/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osadl-matrix
-Version: 2023.6.14.150620
+Version: 2023.6.14.30610
 Summary: OSADL license compatibility matrix
 Home-page: UNKNOWN
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `osadl-matrix-2023.6.14.150620/README.md` & `osadl-matrix-2023.6.14.30610/README.md`

 * *Files identical despite different names*

### Comparing `osadl-matrix-2023.6.14.150620/osadl_matrix/__init__.py` & `osadl-matrix-2023.6.14.30610/osadl_matrix/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-FileCopyrightText: 2021 Konrad Weihmann
 # SPDX-FileCopyrightText: 2023 Henrik Sandklef
 # SPDX-License-Identifier: Unlicensed
 
-import csv
 import json
 import os
 from enum import Enum, unique
 
 OSADL_MATRIX = os.path.join(os.path.dirname(__file__), 'osadl-matrix.csv')
 OSADL_MATRIX_JSON = os.path.join(os.path.dirname(__file__), 'osadl-matrix.json')
 __osadl_db = {}
@@ -40,32 +39,16 @@
 
 
 def __read_db(customdb=None):
     """reads (first call only) matrix file
     """
     global __osadl_db
     if not __osadl_db:
-        try:
-            with open(customdb or OSADL_MATRIX_JSON) as i:
-                __osadl_db = json.load(i)
-        except json.JSONDecodeError:
-            if customdb:  # pragma: no cover
-                with open(customdb) as i:
-                    _reader = csv.DictReader(i, delimiter=',', quotechar='"')
-                    for row in _reader:
-                        import logging
-                        logging.warning(row)
-                        key = row['Compatibility*']
-                        for k, v in row.items():
-                            if k == 'Compatibility*':
-                                continue
-                            if key not in __osadl_db:
-                                __osadl_db[key] = {}
-                            __osadl_db[key][k] = v
-
+        with open(customdb or OSADL_MATRIX_JSON) as i:
+            __osadl_db = json.load(i)
 
 def is_compatible(outbound, inbound, customdb=None):
     """checks if the 'outbound' license is compatible with the 'inbound'
    license. If the licenses can be found in the matrix and the
    licenses are compatible, True is returned. In all other cases False
    is returned.
```

### Comparing `osadl-matrix-2023.6.14.150620/osadl_matrix/osadl-matrix.csv` & `osadl-matrix-2023.6.14.30610/osadl_matrix/osadl-matrix.csv`

 * *Files identical despite different names*

### Comparing `osadl-matrix-2023.6.14.150620/osadl_matrix/osadl-matrix.json` & `osadl-matrix-2023.6.14.30610/osadl_matrix/osadl-matrix.json`

 * *Files identical despite different names*

### Comparing `osadl-matrix-2023.6.14.150620/osadl_matrix.egg-info/PKG-INFO` & `osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osadl-matrix
-Version: 2023.6.14.150620
+Version: 2023.6.14.30610
 Summary: OSADL license compatibility matrix
 Home-page: UNKNOWN
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `osadl-matrix-2023.6.14.150620/osadl_matrix.egg-info/requires.txt` & `osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `osadl-matrix-2023.6.14.150620/requirements-dev.txt` & `osadl-matrix-2023.6.14.30610/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `osadl-matrix-2023.6.14.150620/setup.py` & `osadl-matrix-2023.6.14.30610/setup.py`

 * *Files identical despite different names*

