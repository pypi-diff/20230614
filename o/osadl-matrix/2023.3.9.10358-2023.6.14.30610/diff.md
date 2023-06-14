# Comparing `tmp/osadl-matrix-2023.3.9.10358.tar.gz` & `tmp/osadl-matrix-2023.6.14.30610.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osadl-matrix-2023.3.9.10358.tar", last modified: Thu Mar  9 01:29:02 2023, max compression
+gzip compressed data, was "osadl-matrix-2023.6.14.30610.tar", last modified: Wed Jun 14 03:19:16 2023, max compression
```

## Comparing `osadl-matrix-2023.3.9.10358.tar` & `osadl-matrix-2023.6.14.30610.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 01:29:02.190106 osadl-matrix-2023.3.9.10358/
--rw-r--r--   0 runner    (1001) docker     (123)    14191 2023-03-09 01:28:32.000000 osadl-matrix-2023.3.9.10358/DATALOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-09 01:28:32.000000 osadl-matrix-2023.3.9.10358/LICENSE.Unlicensed
--rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-03-09 01:28:32.000000 osadl-matrix-2023.3.9.10358/LICENSE.ccby40
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-09 01:28:32.000000 osadl-matrix-2023.3.9.10358/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-03-09 01:29:02.190106 osadl-matrix-2023.3.9.10358/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-03-09 01:28:32.000000 osadl-matrix-2023.3.9.10358/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-09 01:28:58.000000 osadl-matrix-2023.3.9.10358/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 01:29:02.190106 osadl-matrix-2023.3.9.10358/osadl_matrix/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-03-09 01:28:32.000000 osadl-matrix-2023.3.9.10358/osadl_matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37701 2023-03-09 01:28:32.000000 osadl-matrix-2023.3.9.10358/osadl_matrix/osadl-matrix.csv
--rw-r--r--   0 runner    (1001) docker     (123)   208790 2023-03-09 01:28:32.000000 osadl-matrix-2023.3.9.10358/osadl_matrix/osadl-matrix.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 01:29:02.190106 osadl-matrix-2023.3.9.10358/osadl_matrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-03-09 01:29:02.000000 osadl-matrix-2023.3.9.10358/osadl_matrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-09 01:29:02.000000 osadl-matrix-2023.3.9.10358/osadl_matrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 01:29:02.000000 osadl-matrix-2023.3.9.10358/osadl_matrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-09 01:29:02.000000 osadl-matrix-2023.3.9.10358/osadl_matrix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-09 01:29:02.000000 osadl-matrix-2023.3.9.10358/osadl_matrix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-09 01:28:32.000000 osadl-matrix-2023.3.9.10358/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 01:28:32.000000 osadl-matrix-2023.3.9.10358/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-03-09 01:29:02.190106 osadl-matrix-2023.3.9.10358/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-09 01:28:32.000000 osadl-matrix-2023.3.9.10358/setup.py
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

### Comparing `osadl-matrix-2023.3.9.10358/DATALOG.md` & `osadl-matrix-2023.6.14.30610/DATALOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,110 @@
+# Changes in 2023-03-15T03:08:00+00:00
+
+
+# Changes in 2023-03-13T03:11:00+00:00
+
+
+# Changes in 2023-03-10T03:09:00+00:00
+
+- Libpng -> CC-BY-3.0: newly added with "Yes"
+- ECL-2.0 -> CC-BY-3.0: newly added with "Yes"
+- EPL-1.0 -> CC-BY-3.0: newly added with "Unknown"
+- CDDL-1.0 -> CC-BY-3.0: newly added with "Unknown"
+- Apache-1.1 -> CC-BY-3.0: newly added with "Yes"
+- Unicode-DFS-2016 -> CC-BY-3.0: newly added with "Yes"
+- BSD-2-Clause-Patent -> CC-BY-3.0: newly added with "Yes"
+- LGPL-2.1-or-later -> CC-BY-3.0: newly added with "Unknown"
+- GPL-2.0-or-later -> CC-BY-3.0: newly added with "Unknown"
+- Artistic-1.0-Perl -> CC-BY-3.0: newly added with "Yes"
+- 0BSD -> CC-BY-3.0: newly added with "Yes"
+- Info-ZIP -> CC-BY-3.0: newly added with "Yes"
+- MIT -> CC-BY-3.0: newly added with "Yes"
+- EUPL-1.1 -> CC-BY-3.0: newly added with "Unknown"
+- FSFAP -> CC-BY-3.0: newly added with "Yes"
+- Artistic-1.0 -> CC-BY-3.0: newly added with "Yes"
+- BSD-1-Clause -> CC-BY-3.0: newly added with "Yes"
+- RSA-MD -> CC-BY-3.0: newly added with "Yes"
+- W3C-20150513 -> CC-BY-3.0: newly added with "Yes"
+- Unlicense -> CC-BY-3.0: newly added with "Yes"
+- bzip2-1.0.6 -> CC-BY-3.0: newly added with "Yes"
+- EPL-2.0 -> CC-BY-3.0: newly added with "Unknown"
+- zlib-acknowledgement -> CC-BY-3.0: newly added with "Yes"
+- IJG -> CC-BY-3.0: newly added with "Yes"
+- LGPL-2.1-only -> CC-BY-3.0: newly added with "Unknown"
+- GPL-2.0-only -> WITH: newly added with "Unknown"
+- Apache-1.0 -> CC-BY-3.0: newly added with "Yes"
+- BSD-4-Clause -> CC-BY-3.0: newly added with "Yes"
+- Qhull -> CC-BY-3.0: newly added with "Yes"
+- ICU -> CC-BY-3.0: newly added with "Yes"
+- GPL-2.0-only -> CC-BY-3.0: newly added with "Unknown"
+- BSD-4-Clause-UC -> CC-BY-3.0: newly added with "Yes"
+- XFree86-1.1 -> CC-BY-3.0: newly added with "Yes"
+- Python-2.0 -> CC-BY-3.0: newly added with "Yes"
+- WTFPL -> CC-BY-3.0: newly added with "Yes"
+- PHP-3.01 -> CC-BY-3.0: newly added with "Yes"
+- PostgreSQL -> CC-BY-3.0: newly added with "Yes"
+- AGPL-3.0-only -> CC-BY-3.0: newly added with "Unknown"
+- MPL-2.0-no-copyleft-exception -> CC-BY-3.0: newly added with "Unknown"
+- blessing -> CC-BY-3.0: newly added with "Yes"
+- HPND -> CC-BY-3.0: newly added with "Yes"
+- CC0-1.0 -> CC-BY-3.0: newly added with "Yes"
+- Zlib -> CC-BY-3.0: newly added with "Yes"
+- AFL-2.0 -> CC-BY-3.0: newly added with "Yes"
+- BSL-1.0 -> CC-BY-3.0: newly added with "Yes"
+- ZPL-2.0 -> CC-BY-3.0: newly added with "Yes"
+- MS-RL -> CC-BY-3.0: newly added with "Unknown"
+- OLDAP-2.8 -> CC-BY-3.0: newly added with "Yes"
+- GPL-3.0-only -> CC-BY-3.0: newly added with "Unknown"
+- Artistic-2.0 -> CC-BY-3.0: newly added with "Yes"
+- AFL-3.0 -> CC-BY-3.0: newly added with "Yes"
+- Apache-2.0 -> CC-BY-3.0: newly added with "Yes"
+- GPL-1.0-only -> CC-BY-3.0: newly added with "Unknown"
+- EUPL-1.2 -> CC-BY-3.0: newly added with "Unknown"
+- W3C -> CC-BY-3.0: newly added with "Yes"
+- ImageMagick -> CC-BY-3.0: newly added with "Yes"
+- AGPL-3.0-or-later -> CC-BY-3.0: newly added with "Unknown"
+- AFL-2.1 -> CC-BY-3.0: newly added with "Yes"
+- IPL-1.0 -> CC-BY-3.0: newly added with "Unknown"
+- LGPL-3.0-or-later -> CC-BY-3.0: newly added with "Unknown"
+- MPL-2.0 -> CC-BY-3.0: newly added with "Unknown"
+- BSD-2-Clause -> CC-BY-3.0: newly added with "Yes"
+- MIT-CMU -> CC-BY-3.0: newly added with "Yes"
+- OSL-3.0 -> CC-BY-3.0: newly added with "Unknown"
+- ISC -> CC-BY-3.0: newly added with "Yes"
+- EFL-2.0 -> CC-BY-3.0: newly added with "Yes"
+- LGPL-3.0-only -> CC-BY-3.0: newly added with "Unknown"
+- Sleepycat -> CC-BY-3.0: newly added with "Unknown"
+- NTP -> CC-BY-3.0: newly added with "Yes"
+- Unicode-DFS-2015 -> CC-BY-3.0: newly added with "Yes"
+- BSD-3-Clause -> CC-BY-3.0: newly added with "Yes"
+- W3C-19980720 -> CC-BY-3.0: newly added with "Yes"
+- SunPro -> CC-BY-3.0: newly added with "Yes"
+- curl -> CC-BY-3.0: newly added with "Yes"
+- NBPL-1.0 -> CC-BY-3.0: newly added with "Yes"
+- FSFULLR -> CC-BY-3.0: newly added with "Yes"
+- GPL-1.0-or-later -> CC-BY-3.0: newly added with "Unknown"
+- OpenSSL -> CC-BY-3.0: newly added with "Unknown"
+- UPL-1.0 -> CC-BY-3.0: newly added with "Yes"
+- CPL-1.0 -> CC-BY-3.0: newly added with "Unknown"
+- GPL-3.0-or-later -> CC-BY-3.0: newly added with "Unknown"
+- FTL -> CC-BY-3.0: newly added with "Yes"
+- MPL-1.1 -> CC-BY-3.0: newly added with "Unknown"
+- bzip2-1.0.5 -> CC-BY-3.0: newly added with "Yes"
+- libtiff -> CC-BY-3.0: newly added with "Yes"
+- X11 -> CC-BY-3.0: newly added with "Yes"
+- IBM-pibs -> CC-BY-3.0: newly added with "Yes"
+- BSD-Source-Code -> CC-BY-3.0: newly added with "Yes"
+- MirOS -> CC-BY-3.0: newly added with "Yes"
+- CDDL-1.1 -> CC-BY-3.0: newly added with "Unknown"
+- MS-PL -> CC-BY-3.0: newly added with "Unknown"
+
+# Changes in 2023-03-09T03:09:00+00:00
+
+
 # Changes in 2023-03-08T03:07:00+00:00
 
 - Apache-1.0 -> ImageMagick: newly added with "Yes"
 - LGPL-2.1-or-later -> OLDAP-2.8: newly added with "Unknown"
 - CC0-1.0 -> ImageMagick: newly added with "Yes"
 - BSD-1-Clause -> OLDAP-2.8: newly added with "Yes"
 - Unicode-DFS-2016 -> ImageMagick: newly added with "Yes"
```

### Comparing `osadl-matrix-2023.3.9.10358/LICENSE.Unlicensed` & `osadl-matrix-2023.6.14.30610/LICENSE.Unlicensed`

 * *Files identical despite different names*

### Comparing `osadl-matrix-2023.3.9.10358/LICENSE.ccby40` & `osadl-matrix-2023.6.14.30610/LICENSE.ccby40`

 * *Files identical despite different names*

### Comparing `osadl-matrix-2023.3.9.10358/PKG-INFO` & `osadl-matrix-2023.6.14.30610/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osadl-matrix
-Version: 2023.3.9.10358
+Version: 2023.6.14.30610
 Summary: OSADL license compatibility matrix
 Home-page: UNKNOWN
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `osadl-matrix-2023.3.9.10358/README.md` & `osadl-matrix-2023.6.14.30610/README.md`

 * *Files identical despite different names*

### Comparing `osadl-matrix-2023.3.9.10358/osadl_matrix/__init__.py` & `osadl-matrix-2023.6.14.30610/osadl_matrix/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2021 Konrad Weihmann
-# SPDX-FileCopyrightText: 2022 Henrik Sandklef
+# SPDX-FileCopyrightText: 2023 Henrik Sandklef
 # SPDX-License-Identifier: Unlicensed
 
-import csv
+import json
 import os
 from enum import Enum, unique
 
 OSADL_MATRIX = os.path.join(os.path.dirname(__file__), 'osadl-matrix.csv')
 OSADL_MATRIX_JSON = os.path.join(os.path.dirname(__file__), 'osadl-matrix.json')
 __osadl_db = {}
 
@@ -39,34 +39,29 @@
 
 
 def __read_db(customdb=None):
     """reads (first call only) matrix file
     """
     global __osadl_db
     if not __osadl_db:
-        with open(customdb or OSADL_MATRIX) as i:
-            _reader = csv.DictReader(i, delimiter=',', quotechar='"')
-            for row in _reader:
-                key = row['Compatibility*']
-                for k, v in row.items():
-                    __osadl_db[(key, k)] = OSADLCompatibility.from_text(v)
-
+        with open(customdb or OSADL_MATRIX_JSON) as i:
+            __osadl_db = json.load(i)
 
 def is_compatible(outbound, inbound, customdb=None):
     """checks if the 'outbound' license is compatible with the 'inbound'
    license. If the licenses can be found in the matrix and the
    licenses are compatible, True is returned. In all other cases False
    is returned.
 
     Args:
         outbound (string): SPDX ID for an outbound license, e.g. the license used for distribution of an application
         inbound (string): SPDX ID for an inbound license, e.g. the license used for a dependency of the application
 
     Returns:
-        [OSADLCompatibility]: True or False
+        True or False
 
     """
     return get_compatibility(outbound, inbound, customdb) == OSADLCompatibility.YES
 
 
 def get_compatibility(outbound, inbound, customdb=None):
     """returns the compatibility status between the 'outbound' and the
@@ -78,22 +73,19 @@
         inbound (string): SPDX ID for an inbound license, e.g. the license used for a dependency of the application
 
     Returns:
         [OSADLCompatibility]: Either yes, no, unknown or undefined
 
     """
     __read_db(customdb=customdb)
-    return __osadl_db.get((outbound, inbound), OSADLCompatibility.UNDEF)
+    try:
+        return OSADLCompatibility.from_text(__osadl_db.get(outbound).get(inbound))
+    except AttributeError:
+        return OSADLCompatibility.UNDEF
 
 
 def supported_licenses(customdb=None):
     """returns the supported licenses (i.e. which licenses for which
     there is a known compatibility status).
     """
     __read_db(customdb=customdb)
-    licenses = set()
-    for row in __osadl_db:
-        key, k = row
-        if k == "Compatibility*":
-            continue
-        licenses.add(k)
-    return licenses
+    return __osadl_db.keys()
```

### Comparing `osadl-matrix-2023.3.9.10358/osadl_matrix/osadl-matrix.csv` & `osadl-matrix-2023.6.14.30610/osadl_matrix/osadl-matrix.csv`

 * *Files 1% similar despite different names*

```diff
@@ -1,92 +1,93 @@
-Compatibility*,0BSD,AFL-2.0,AFL-2.1,AFL-3.0,AGPL-3.0-only,AGPL-3.0-or-later,Apache-1.0,Apache-1.1,Apache-2.0,Artistic-1.0,Artistic-1.0-Perl,Artistic-2.0,BSD-1-Clause,BSD-2-Clause,BSD-2-Clause-Patent,BSD-3-Clause,BSD-4-Clause,BSD-4-Clause-UC,BSD-Source-Code,BSL-1.0,CC0-1.0,CDDL-1.0,CDDL-1.1,CPL-1.0,ECL-2.0,EFL-2.0,EPL-1.0,EPL-2.0,EUPL-1.1,EUPL-1.2,FSFAP,FSFULLR,FTL,GPL-1.0-only,GPL-1.0-or-later,GPL-2.0-only,GPL-2.0-only WITH Classpath-exception-2.0,GPL-2.0-or-later,GPL-3.0-only,GPL-3.0-or-later,HPND,IBM-pibs,ICU,IJG,IPL-1.0,ISC,ImageMagick,Info-ZIP,LGPL-2.1-only,LGPL-2.1-or-later,LGPL-3.0-only,LGPL-3.0-or-later,Libpng,MIT,MIT-CMU,MPL-1.1,MPL-2.0,MPL-2.0-no-copyleft-exception,MS-PL,MS-RL,MirOS,NBPL-1.0,NTP,OLDAP-2.8,OSL-3.0,OpenSSL,PHP-3.01,PostgreSQL,Python-2.0,Qhull,RSA-MD,Sleepycat,SunPro,UPL-1.0,Unicode-DFS-2015,Unicode-DFS-2016,Unlicense,W3C,W3C-19980720,W3C-20150513,WTFPL,X11,XFree86-1.1,ZPL-2.0,Zlib,blessing,bzip2-1.0.5,bzip2-1.0.6,curl,libtiff,zlib-acknowledgement
-0BSD,Same,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-AFL-2.0,Yes,Same,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-AFL-2.1,Yes,Yes,Same,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-AFL-3.0,Yes,Yes,Yes,Same,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-AGPL-3.0-only,Unknown,Unknown,Unknown,Unknown,Same,Yes,No,No,Yes,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,No,No,Check dependency,No,No,Check dependency,Check dependency,Check dependency,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,Check dependency,Check dependency,Check dependency,Check dependency,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
-AGPL-3.0-or-later,Unknown,Unknown,Unknown,Unknown,No,Same,No,No,Yes,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,No,No,Check dependency,No,No,Check dependency,Check dependency,Check dependency,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,Check dependency,Check dependency,Check dependency,Check dependency,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
-Apache-1.0,Yes,Yes,Yes,Yes,No,No,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-Apache-1.1,Yes,Yes,Yes,Yes,No,No,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-Apache-2.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-Artistic-1.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-Artistic-1.0-Perl,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-Artistic-2.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-BSD-1-Clause,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-BSD-2-Clause,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-BSD-2-Clause-Patent,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-BSD-3-Clause,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-BSD-4-Clause,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-BSD-4-Clause-UC,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-BSD-Source-Code,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-BSL-1.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-CC0-1.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-CDDL-1.0,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Yes,Same,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
-CDDL-1.1,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,Same,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
-CPL-1.0,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,No,Same,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,Yes,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
-ECL-2.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Same,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-EFL-2.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Same,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-EPL-1.0,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,No,Yes,Unknown,Yes,Same,No,Yes,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,Yes,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
-EPL-2.0,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,No,Yes,Unknown,Yes,Yes,Same,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
-EUPL-1.1,Unknown,Unknown,Unknown,Unknown,No,No,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,No,Same,No,Yes,Yes,No,No,No,No,No,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
-EUPL-1.2,Unknown,Unknown,Unknown,Unknown,No,No,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,No,No,Same,Yes,Yes,No,No,No,No,No,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,Unknown,No
-FSFAP,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Same,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-FSFULLR,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Same,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-FTL,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Same,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-GPL-1.0-only,Unknown,Unknown,Unknown,Unknown,No,No,No,No,No,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,No,Same,Yes,No,No,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
-GPL-1.0-or-later,Unknown,Unknown,Unknown,Unknown,Check dependency,Check dependency,No,No,No,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,Check dependency,Check dependency,No,Yes,Yes,No,No,Same,No,No,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,Check dependency,Check dependency,No,No,Yes,Yes,Unknown,No,Check dependency,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
-GPL-2.0-only,Unknown,Unknown,Unknown,Unknown,No,No,No,No,No,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,Check dependency,Yes,No,Yes,Yes,No,No,Yes,Same,Yes,Yes,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,Yes,Yes,No,No,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,Yes,Unknown,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
-GPL-2.0-only WITH Classpath-exception-2.0,Unknown,Unknown,Unknown,Unknown,No,No,No,No,No,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,Check dependency,Yes,No,Yes,Yes,No,No,No,No,Same,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
-GPL-2.0-or-later,Unknown,Unknown,Unknown,Unknown,Check dependency,Check dependency,No,No,No,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,Check dependency,Yes,No,Yes,Yes,No,No,Yes,No,No,Same,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,Yes,Yes,No,No,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
-GPL-3.0-only,Unknown,Unknown,Unknown,Unknown,Check dependency,Check dependency,No,No,Yes,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,Check dependency,No,No,Yes,Yes,No,No,Yes,No,No,Yes,Same,Yes,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
-GPL-3.0-or-later,Unknown,Unknown,Unknown,Unknown,Check dependency,Check dependency,No,No,Yes,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,Check dependency,No,No,Yes,Yes,No,No,Yes,No,No,Yes,No,Same,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,Yes,Yes,No,Yes,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
-HPND,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Same,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-IBM-pibs,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Same,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-ICU,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Same,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-IJG,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Same,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-IPL-1.0,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,No,Yes,Unknown,Yes,Yes,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,Same,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
-ISC,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Same,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-ImageMagick,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Same,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-Info-ZIP,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Same,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-LGPL-2.1-only,Unknown,Unknown,Unknown,Unknown,Check dependency,Check dependency,No,No,No,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,Check dependency,No,No,Yes,Yes,No,No,No,No,No,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,Same,Yes,No,No,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
-LGPL-2.1-or-later,Unknown,Unknown,Unknown,Unknown,Check dependency,Check dependency,No,No,No,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,Check dependency,No,No,Yes,Yes,No,No,No,No,No,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,No,Same,No,No,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
-LGPL-3.0-only,Unknown,Unknown,Unknown,Unknown,Check dependency,Check dependency,No,No,Yes,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,Check dependency,No,No,Yes,Yes,No,No,No,No,No,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,No,Yes,Same,Yes,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
-LGPL-3.0-or-later,Unknown,Unknown,Unknown,Unknown,Check dependency,Check dependency,No,No,Yes,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,Check dependency,No,No,Yes,Yes,No,No,No,No,No,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,No,Yes,No,Same,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
-Libpng,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Same,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-MIT,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Same,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-MIT-CMU,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Same,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-MPL-1.1,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,Same,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
-MPL-2.0,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,Same,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
-MPL-2.0-no-copyleft-exception,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,Yes,Same,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
-MS-PL,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Same,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
-MS-RL,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,Same,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
-MirOS,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Same,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-NBPL-1.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Same,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-NTP,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Same,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-OLDAP-2.8,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Same,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-OSL-3.0,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,No,Yes,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,Same,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
-OpenSSL,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Same,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
-PHP-3.01,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Same,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-PostgreSQL,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Same,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-Python-2.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Same,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-Qhull,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Same,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-RSA-MD,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Same,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-Sleepycat,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Same,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
-SunPro,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-UPL-1.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-Unicode-DFS-2015,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-Unicode-DFS-2016,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-Unlicense,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-W3C,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-W3C-19980720,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-W3C-20150513,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-WTFPL,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-X11,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-XFree86-1.1,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-ZPL-2.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes
-Zlib,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes
-blessing,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes
-bzip2-1.0.5,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes
-bzip2-1.0.6,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes
-curl,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes
-libtiff,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes
-zlib-acknowledgement,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same
+Compatibility*,0BSD,AFL-2.0,AFL-2.1,AFL-3.0,AGPL-3.0-only,AGPL-3.0-or-later,Apache-1.0,Apache-1.1,Apache-2.0,Artistic-1.0,Artistic-1.0-Perl,Artistic-2.0,BSD-1-Clause,BSD-2-Clause,BSD-2-Clause-Patent,BSD-3-Clause,BSD-4-Clause,BSD-4-Clause-UC,BSD-Source-Code,BSL-1.0,CC-BY-3.0,CC0-1.0,CDDL-1.0,CDDL-1.1,CPL-1.0,ECL-2.0,EFL-2.0,EPL-1.0,EPL-2.0,EUPL-1.1,EUPL-1.2,FSFAP,FSFULLR,FTL,GPL-1.0-only,GPL-1.0-or-later,GPL-2.0-only,GPL-2.0-only WITH Classpath-exception-2.0,GPL-2.0-or-later,GPL-3.0-only,GPL-3.0-or-later,HPND,IBM-pibs,ICU,IJG,IPL-1.0,ISC,ImageMagick,Info-ZIP,LGPL-2.1-only,LGPL-2.1-or-later,LGPL-3.0-only,LGPL-3.0-or-later,Libpng,MIT,MIT-CMU,MPL-1.1,MPL-2.0,MPL-2.0-no-copyleft-exception,MS-PL,MS-RL,MirOS,NBPL-1.0,NTP,OLDAP-2.8,OSL-3.0,OpenSSL,PHP-3.01,PostgreSQL,Python-2.0,Qhull,RSA-MD,Sleepycat,SunPro,UPL-1.0,Unicode-DFS-2015,Unicode-DFS-2016,Unlicense,W3C,W3C-19980720,W3C-20150513,WTFPL,X11,XFree86-1.1,ZPL-2.0,Zlib,blessing,bzip2-1.0.5,bzip2-1.0.6,curl,libtiff,zlib-acknowledgement
+0BSD,Same,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+AFL-2.0,Yes,Same,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+AFL-2.1,Yes,Yes,Same,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+AFL-3.0,Yes,Yes,Yes,Same,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+AGPL-3.0-only,Unknown,Unknown,Unknown,Unknown,Same,Yes,No,No,Yes,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,No,No,Check dependency,No,No,Check dependency,Check dependency,Check dependency,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,Check dependency,Check dependency,Check dependency,Check dependency,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
+AGPL-3.0-or-later,Unknown,Unknown,Unknown,Unknown,No,Same,No,No,Yes,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,No,No,Check dependency,No,No,Check dependency,Check dependency,Check dependency,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,Check dependency,Check dependency,Check dependency,Check dependency,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
+Apache-1.0,Yes,Yes,Yes,Yes,No,No,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+Apache-1.1,Yes,Yes,Yes,Yes,No,No,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+Apache-2.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+Artistic-1.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+Artistic-1.0-Perl,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+Artistic-2.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+BSD-1-Clause,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+BSD-2-Clause,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+BSD-2-Clause-Patent,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+BSD-3-Clause,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+BSD-4-Clause,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+BSD-4-Clause-UC,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+BSD-Source-Code,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+BSL-1.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+CC-BY-3.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+CC0-1.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+CDDL-1.0,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Unknown,Yes,Same,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
+CDDL-1.1,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Unknown,Yes,No,Same,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
+CPL-1.0,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Unknown,Yes,No,No,Same,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,Yes,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
+ECL-2.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Same,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+EFL-2.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Same,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+EPL-1.0,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Unknown,Yes,No,No,Yes,Unknown,Yes,Same,No,Yes,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,Yes,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
+EPL-2.0,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Unknown,Yes,No,No,Yes,Unknown,Yes,Yes,Same,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
+EUPL-1.1,Unknown,Unknown,Unknown,Unknown,No,No,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,No,Same,No,Yes,Yes,No,No,No,No,No,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
+EUPL-1.2,Unknown,Unknown,Unknown,Unknown,No,No,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,No,No,Same,Yes,Yes,No,No,No,No,No,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,Unknown,No
+FSFAP,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Same,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+FSFULLR,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Same,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+FTL,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Same,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+GPL-1.0-only,Unknown,Unknown,Unknown,Unknown,No,No,No,No,No,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,No,Same,Yes,No,No,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
+GPL-1.0-or-later,Unknown,Unknown,Unknown,Unknown,Check dependency,Check dependency,No,No,No,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,Check dependency,Check dependency,No,Yes,Yes,No,No,Same,No,No,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,Check dependency,Check dependency,No,No,Yes,Yes,Unknown,No,Check dependency,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
+GPL-2.0-only,Unknown,Unknown,Unknown,Unknown,No,No,No,No,No,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,Check dependency,Yes,No,Yes,Yes,No,No,Yes,Same,Yes,Yes,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,Yes,Yes,No,No,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,Yes,Unknown,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
+GPL-2.0-only WITH Classpath-exception-2.0,Unknown,Unknown,Unknown,Unknown,No,No,No,No,No,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,Check dependency,Yes,No,Yes,Yes,No,No,No,No,Same,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
+GPL-2.0-or-later,Unknown,Unknown,Unknown,Unknown,Check dependency,Check dependency,No,No,No,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,Check dependency,Yes,No,Yes,Yes,No,No,Yes,No,No,Same,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,Yes,Yes,No,No,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
+GPL-3.0-only,Unknown,Unknown,Unknown,Unknown,Check dependency,Check dependency,No,No,Yes,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,Check dependency,No,No,Yes,Yes,No,No,Yes,No,No,Yes,Same,Yes,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
+GPL-3.0-or-later,Unknown,Unknown,Unknown,Unknown,Check dependency,Check dependency,No,No,Yes,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,Check dependency,No,No,Yes,Yes,No,No,Yes,No,No,Yes,No,Same,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,Yes,Yes,No,Yes,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
+HPND,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Same,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+IBM-pibs,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Same,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+ICU,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Same,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+IJG,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Same,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+IPL-1.0,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Unknown,Yes,No,No,Yes,Unknown,Yes,Yes,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,Same,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
+ISC,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Same,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+ImageMagick,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Same,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+Info-ZIP,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Same,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+LGPL-2.1-only,Unknown,Unknown,Unknown,Unknown,Check dependency,Check dependency,No,No,No,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,Check dependency,No,No,Yes,Yes,No,No,No,No,No,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,Same,Yes,No,No,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
+LGPL-2.1-or-later,Unknown,Unknown,Unknown,Unknown,Check dependency,Check dependency,No,No,No,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,Check dependency,No,No,Yes,Yes,No,No,No,No,No,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,No,Same,No,No,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
+LGPL-3.0-only,Unknown,Unknown,Unknown,Unknown,Check dependency,Check dependency,No,No,Yes,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,Check dependency,No,No,Yes,Yes,No,No,No,No,No,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,No,Yes,Same,Yes,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
+LGPL-3.0-or-later,Unknown,Unknown,Unknown,Unknown,Check dependency,Check dependency,No,No,Yes,Unknown,Unknown,Yes,Unknown,Yes,Yes,Yes,No,No,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,Check dependency,No,No,Yes,Yes,No,No,No,No,No,No,No,No,Unknown,Yes,Yes,No,No,Yes,Unknown,Unknown,No,Yes,No,Same,Yes,Yes,Unknown,No,Yes,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,No
+Libpng,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Same,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+MIT,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Same,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+MIT-CMU,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Same,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+MPL-1.1,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,No,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,Same,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
+MPL-2.0,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,Same,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
+MPL-2.0-no-copyleft-exception,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,Yes,Same,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
+MS-PL,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Same,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
+MS-RL,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,Same,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
+MirOS,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Same,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+NBPL-1.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Same,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+NTP,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Same,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+OLDAP-2.8,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Same,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+OSL-3.0,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,No,Yes,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,Same,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
+OpenSSL,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Same,Unknown,Unknown,Unknown,Unknown,Unknown,No,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Yes,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
+PHP-3.01,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Same,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+PostgreSQL,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Same,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+Python-2.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Same,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+Qhull,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Same,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+RSA-MD,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Same,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+Sleepycat,Unknown,Unknown,Unknown,Unknown,No,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Yes,Yes,Yes,Unknown,Unknown,Unknown,Yes,Unknown,Yes,No,No,No,Unknown,Yes,No,No,No,No,Yes,Yes,Unknown,No,No,No,No,No,No,No,Unknown,Yes,Yes,Unknown,No,Yes,Unknown,Unknown,No,No,No,No,Yes,Yes,Unknown,No,No,No,Unknown,No,Unknown,Unknown,Yes,Unknown,No,Unknown,Unknown,Unknown,Unknown,Unknown,Unknown,Same,Unknown,Yes,Unknown,Unknown,Yes,Unknown,Unknown,Unknown,Yes,Yes,Unknown,Unknown,Yes,Yes,Yes,Yes,Yes,Unknown,Unknown
+SunPro,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+UPL-1.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+Unicode-DFS-2015,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+Unicode-DFS-2016,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+Unlicense,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+W3C,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+W3C-19980720,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+W3C-20150513,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+WTFPL,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+X11,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+XFree86-1.1,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+ZPL-2.0,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes,Yes
+Zlib,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes,Yes
+blessing,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes,Yes
+bzip2-1.0.5,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes,Yes
+bzip2-1.0.6,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes,Yes
+curl,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes,Yes
+libtiff,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same,Yes
+zlib-acknowledgement,Yes,Yes,Yes,Yes,No,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,No,No,No,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,No,No,No,No,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,No,No,No,No,Yes,Yes,Yes,No,No,No,Unknown,No,Yes,Yes,Yes,Yes,No,Unknown,Yes,Yes,Yes,Yes,Yes,No,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Yes,Same
```

### Comparing `osadl-matrix-2023.3.9.10358/osadl_matrix/osadl-matrix.json` & `osadl-matrix-2023.6.14.30610/osadl_matrix/osadl-matrix.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787812210915802%*

 * *Differences: {"'0BSD'": "{'CC-BY-3.0': 'Yes'}",*

 * * "'AFL-2.0'": "{'CC-BY-3.0': 'Yes'}",*

 * * "'AFL-2.1'": "{'CC-BY-3.0': 'Yes'}",*

 * * "'AFL-3.0'": "{'CC-BY-3.0': 'Yes'}",*

 * * "'AGPL-3.0-only'": "{'CC-BY-3.0': 'Unknown'}",*

 * * "'AGPL-3.0-or-later'": "{'CC-BY-3.0': 'Unknown'}",*

 * * "'Apache-1.0'": "{'CC-BY-3.0': 'Yes'}",*

 * * "'Apache-1.1'": "{'CC-BY-3.0': 'Yes'}",*

 * * "'Apache-2.0'": "{'CC-BY-3.0': 'Yes'}",*

 * * "'Artistic-1.0'": "{'CC-BY-3.0': 'Yes'}",*

 * * "'Artistic-1.0-Perl'": "{'CC-BY-3.0': 'Yes'}",*

 * * "'Artistic-2.0'": "{'CC-BY-3.0': 'Yes'}",*

 * * "'BSD […]*

```diff
@@ -16,14 +16,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -109,14 +110,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -202,14 +204,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -295,14 +298,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -388,14 +392,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "No",
         "BSD-4-Clause-UC": "No",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -481,14 +486,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "No",
         "BSD-4-Clause-UC": "No",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -574,14 +580,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -667,14 +674,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -760,14 +768,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -853,14 +862,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -946,14 +956,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -1039,14 +1050,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -1132,14 +1144,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -1225,14 +1238,15 @@
         "BSD-2-Clause": "Same",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -1318,14 +1332,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Same",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -1411,14 +1426,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Same",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -1504,14 +1520,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Same",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -1597,14 +1614,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Same",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -1690,14 +1708,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Same",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -1783,14 +1802,109 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Same",
+        "CC-BY-3.0": "Yes",
+        "CC0-1.0": "Yes",
+        "CDDL-1.0": "No",
+        "CDDL-1.1": "No",
+        "CPL-1.0": "No",
+        "ECL-2.0": "Yes",
+        "EFL-2.0": "Yes",
+        "EPL-1.0": "No",
+        "EPL-2.0": "No",
+        "EUPL-1.1": "No",
+        "EUPL-1.2": "No",
+        "FSFAP": "Yes",
+        "FSFULLR": "Yes",
+        "FTL": "Yes",
+        "GPL-1.0-only": "No",
+        "GPL-1.0-or-later": "No",
+        "GPL-2.0-only": "No",
+        "GPL-2.0-only WITH Classpath-exception-2.0": "No",
+        "GPL-2.0-or-later": "No",
+        "GPL-3.0-only": "No",
+        "GPL-3.0-or-later": "No",
+        "HPND": "Yes",
+        "IBM-pibs": "Yes",
+        "ICU": "Yes",
+        "IJG": "Yes",
+        "IPL-1.0": "No",
+        "ISC": "Yes",
+        "ImageMagick": "Yes",
+        "Info-ZIP": "Yes",
+        "LGPL-2.1-only": "No",
+        "LGPL-2.1-or-later": "No",
+        "LGPL-3.0-only": "No",
+        "LGPL-3.0-or-later": "No",
+        "Libpng": "Yes",
+        "MIT": "Yes",
+        "MIT-CMU": "Yes",
+        "MPL-1.1": "No",
+        "MPL-2.0": "No",
+        "MPL-2.0-no-copyleft-exception": "No",
+        "MS-PL": "Unknown",
+        "MS-RL": "No",
+        "MirOS": "Yes",
+        "NBPL-1.0": "Yes",
+        "NTP": "Yes",
+        "OLDAP-2.8": "Yes",
+        "OSL-3.0": "No",
+        "OpenSSL": "Unknown",
+        "PHP-3.01": "Yes",
+        "PostgreSQL": "Yes",
+        "Python-2.0": "Yes",
+        "Qhull": "Yes",
+        "RSA-MD": "Yes",
+        "Sleepycat": "No",
+        "SunPro": "Yes",
+        "UPL-1.0": "Yes",
+        "Unicode-DFS-2015": "Yes",
+        "Unicode-DFS-2016": "Yes",
+        "Unlicense": "Yes",
+        "W3C": "Yes",
+        "W3C-19980720": "Yes",
+        "W3C-20150513": "Yes",
+        "WTFPL": "Yes",
+        "X11": "Yes",
+        "XFree86-1.1": "Yes",
+        "ZPL-2.0": "Yes",
+        "Zlib": "Yes",
+        "blessing": "Yes",
+        "bzip2-1.0.5": "Yes",
+        "bzip2-1.0.6": "Yes",
+        "curl": "Yes",
+        "libtiff": "Yes",
+        "zlib-acknowledgement": "Yes"
+    },
+    "CC-BY-3.0": {
+        "0BSD": "Yes",
+        "AFL-2.0": "Yes",
+        "AFL-2.1": "Yes",
+        "AFL-3.0": "Yes",
+        "AGPL-3.0-only": "No",
+        "AGPL-3.0-or-later": "No",
+        "Apache-1.0": "Yes",
+        "Apache-1.1": "Yes",
+        "Apache-2.0": "Yes",
+        "Artistic-1.0": "Yes",
+        "Artistic-1.0-Perl": "Yes",
+        "Artistic-2.0": "Yes",
+        "BSD-1-Clause": "Yes",
+        "BSD-2-Clause": "Yes",
+        "BSD-2-Clause-Patent": "Yes",
+        "BSD-3-Clause": "Yes",
+        "BSD-4-Clause": "Yes",
+        "BSD-4-Clause-UC": "Yes",
+        "BSD-Source-Code": "Yes",
+        "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Same",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -1876,14 +1990,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Same",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -1969,14 +2084,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Unknown",
         "BSD-4-Clause-UC": "Unknown",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "Same",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -2062,14 +2178,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Unknown",
         "BSD-4-Clause-UC": "Unknown",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "Same",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -2155,14 +2272,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Unknown",
         "BSD-4-Clause-UC": "Unknown",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "Same",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -2248,14 +2366,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Same",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -2341,14 +2460,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Same",
         "EPL-1.0": "No",
@@ -2434,14 +2554,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Unknown",
         "BSD-4-Clause-UC": "Unknown",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "Yes",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "Same",
@@ -2527,14 +2648,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Unknown",
         "BSD-4-Clause-UC": "Unknown",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "Yes",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "Yes",
@@ -2620,14 +2742,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "No",
         "BSD-4-Clause-UC": "No",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -2713,14 +2836,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "No",
         "BSD-4-Clause-UC": "No",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -2806,14 +2930,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -2899,14 +3024,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -2992,14 +3118,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -3085,14 +3212,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "No",
         "BSD-4-Clause-UC": "No",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -3178,14 +3306,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "No",
         "BSD-4-Clause-UC": "No",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -3271,14 +3400,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "No",
         "BSD-4-Clause-UC": "No",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -3364,14 +3494,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "No",
         "BSD-4-Clause-UC": "No",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -3457,14 +3588,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "No",
         "BSD-4-Clause-UC": "No",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -3550,14 +3682,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "No",
         "BSD-4-Clause-UC": "No",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -3643,14 +3776,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "No",
         "BSD-4-Clause-UC": "No",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -3736,14 +3870,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -3829,14 +3964,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -3922,14 +4058,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -4015,14 +4152,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -4108,14 +4246,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Unknown",
         "BSD-4-Clause-UC": "Unknown",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "Yes",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "Yes",
@@ -4201,14 +4340,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -4294,14 +4434,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -4387,14 +4528,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -4480,14 +4622,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "No",
         "BSD-4-Clause-UC": "No",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -4573,14 +4716,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "No",
         "BSD-4-Clause-UC": "No",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -4666,14 +4810,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "No",
         "BSD-4-Clause-UC": "No",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -4759,14 +4904,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "No",
         "BSD-4-Clause-UC": "No",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -4852,14 +4998,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -4945,14 +5092,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -5038,14 +5186,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -5131,14 +5280,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Unknown",
         "BSD-4-Clause-UC": "Unknown",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -5224,14 +5374,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Unknown",
         "BSD-4-Clause-UC": "Unknown",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -5317,14 +5468,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Unknown",
         "BSD-4-Clause-UC": "Unknown",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -5410,14 +5562,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -5503,14 +5656,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Unknown",
         "BSD-4-Clause-UC": "Unknown",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -5596,14 +5750,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -5689,14 +5844,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -5782,14 +5938,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -5875,14 +6032,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -5968,14 +6126,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Unknown",
         "BSD-4-Clause-UC": "Unknown",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -6061,14 +6220,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -6154,14 +6314,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -6247,14 +6408,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -6340,14 +6502,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -6433,14 +6596,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -6526,14 +6690,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -6619,14 +6784,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Unknown",
         "BSD-4-Clause-UC": "Unknown",
         "BSD-Source-Code": "Unknown",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Unknown",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Unknown",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -6712,14 +6878,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -6805,14 +6972,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -6898,14 +7066,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -6991,14 +7160,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -7084,14 +7254,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -7177,14 +7348,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -7270,14 +7442,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -7363,14 +7536,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -7456,14 +7630,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -7549,14 +7724,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -7642,14 +7818,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -7735,14 +7912,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -7828,14 +8006,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -7921,14 +8100,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -8014,14 +8194,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -8107,14 +8288,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -8200,14 +8382,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -8293,14 +8476,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
@@ -8366,15 +8550,15 @@
         "bzip2-1.0.5": "Yes",
         "bzip2-1.0.6": "Yes",
         "curl": "Yes",
         "libtiff": "Same",
         "zlib-acknowledgement": "Yes"
     },
     "timeformat": "%Y-%m-%dT%H:%M:%S%z",
-    "timestamp": "2023-03-08T03:07:00+00:00",
+    "timestamp": "2023-06-13T02:08:00+00:00",
     "zlib-acknowledgement": {
         "0BSD": "Yes",
         "AFL-2.0": "Yes",
         "AFL-2.1": "Yes",
         "AFL-3.0": "Yes",
         "AGPL-3.0-only": "No",
         "AGPL-3.0-or-later": "No",
@@ -8388,14 +8572,15 @@
         "BSD-2-Clause": "Yes",
         "BSD-2-Clause-Patent": "Yes",
         "BSD-3-Clause": "Yes",
         "BSD-4-Clause": "Yes",
         "BSD-4-Clause-UC": "Yes",
         "BSD-Source-Code": "Yes",
         "BSL-1.0": "Yes",
+        "CC-BY-3.0": "Yes",
         "CC0-1.0": "Yes",
         "CDDL-1.0": "No",
         "CDDL-1.1": "No",
         "CPL-1.0": "No",
         "ECL-2.0": "Yes",
         "EFL-2.0": "Yes",
         "EPL-1.0": "No",
```

### Comparing `osadl-matrix-2023.3.9.10358/osadl_matrix.egg-info/PKG-INFO` & `osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osadl-matrix
-Version: 2023.3.9.10358
+Version: 2023.6.14.30610
 Summary: OSADL license compatibility matrix
 Home-page: UNKNOWN
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `osadl-matrix-2023.3.9.10358/osadl_matrix.egg-info/requires.txt` & `osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 
 [dev]
-deepdiff~=6.2
-dlint==0.14.0
-flake8-2020==1.7.0
+deepdiff~=6.3
+dlint==0.14.1
+flake8-2020==1.8.1
 flake8-bandit==4.1.1
-flake8-broken-line==0.6.0
-flake8-bugbear==23.2.13
+flake8-broken-line==1.0.0
+flake8-bugbear==23.3.12
 flake8-builtins==2.1.0
 flake8-coding==1.3.2
 flake8-commas==2.1.0
-flake8-comprehensions==3.10.1
+flake8-comprehensions==3.12.0
 flake8-debugger==4.1.2
 flake8-docstrings==1.7.0
-flake8-eradicate==1.4.0
+flake8-eradicate==1.5.0
 flake8-executable==2.1.3
 flake8-fixme==1.1.1
-flake8-functions==0.0.7
+flake8-functions==0.0.8
 flake8-isort==6.0.0
 flake8-logging-format==0.9.0
 flake8-mutable==1.2.0
 flake8-pep3101==2.0.0
 flake8-print==5.0.0
 flake8-quotes==3.3.2
-flake8-requirements==1.7.7
+flake8-requirements==1.7.8
 flake8-string-format==0.3.0
 flake8-variables-names==0.0.5
 flake8==5.0.4
-pytest-cov==4.0.0
+pytest-cov==4.1.0
 pytest-forked==1.6.0
 pytest-icdiff==0.6
 pytest-random-order==1.1.0
 pytest-socket==0.6.0
-pytest-sugar==0.9.6
+pytest-sugar==0.9.7
 pytest-tldr==0.2.5
-pytest==7.2.2
-requests==2.28.2
+pytest==7.3.2
+requests==2.31.0
 twine==4.0.2
-urllib3==1.26.14
+urllib3==1.26.15
```

### Comparing `osadl-matrix-2023.3.9.10358/requirements-dev.txt` & `osadl-matrix-2023.6.14.30610/requirements-dev.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-deepdiff ~= 6.2
-dlint == 0.14.0
+deepdiff ~= 6.3
+dlint == 0.14.1
 flake8 == 5.0.4
-flake8-2020 == 1.7.0
+flake8-2020 == 1.8.1
 flake8-bandit == 4.1.1
-flake8-broken-line == 0.6.0
-flake8-bugbear == 23.2.13
+flake8-broken-line == 1.0.0
+flake8-bugbear == 23.3.12
 flake8-builtins == 2.1.0
 flake8-coding == 1.3.2
 flake8-commas == 2.1.0
-flake8-comprehensions == 3.10.1
+flake8-comprehensions == 3.12.0
 flake8-debugger == 4.1.2
 flake8-docstrings == 1.7.0
-flake8-eradicate == 1.4.0
+flake8-eradicate == 1.5.0
 flake8-executable == 2.1.3
 flake8-fixme == 1.1.1
-flake8-functions == 0.0.7
+flake8-functions == 0.0.8
 flake8-isort == 6.0.0
 flake8-logging-format == 0.9.0
 flake8-mutable == 1.2.0
 flake8-pep3101 == 2.0.0
 flake8-print == 5.0.0
 flake8-quotes == 3.3.2
-flake8-requirements == 1.7.7
+flake8-requirements == 1.7.8
 flake8-string-format == 0.3.0
 flake8-variables-names == 0.0.5
-pytest == 7.2.2
-pytest-cov == 4.0.0
+pytest == 7.3.2
+pytest-cov == 4.1.0
 pytest-forked == 1.6.0
 pytest-icdiff == 0.6
 pytest-random-order == 1.1.0
 pytest-socket == 0.6.0
-pytest-sugar == 0.9.6
+pytest-sugar == 0.9.7
 pytest-tldr == 0.2.5
-requests == 2.28.2
+requests == 2.31.0
 twine == 4.0.2
-urllib3 == 1.26.14
+urllib3 == 1.26.15
```

### Comparing `osadl-matrix-2023.3.9.10358/setup.py` & `osadl-matrix-2023.6.14.30610/setup.py`

 * *Files identical despite different names*

