# Comparing `tmp/qub-sherlock-2.2.1.tar.gz` & `tmp/qub-sherlock-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qub-sherlock-2.2.1.tar", last modified: Fri Jan 21 18:28:41 2022, max compression
+gzip compressed data, was "qub-sherlock-2.2.2.tar", last modified: Wed May 18 13:33:57 2022, max compression
```

## Comparing `qub-sherlock-2.2.1.tar` & `qub-sherlock-2.2.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2022-01-21 18:28:41.000000 qub-sherlock-2.2.1/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      413 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/.readthedocs.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4222 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      304 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2739 2022-01-21 18:28:41.000000 qub-sherlock-2.2.1/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1947 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/README.md
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2022-01-21 18:28:41.000000 qub-sherlock-2.2.1/qub_sherlock.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2739 2022-01-21 18:28:41.000000 qub-sherlock-2.2.1/qub_sherlock.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      993 2022-01-21 18:28:41.000000 qub-sherlock-2.2.1/qub_sherlock.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2022-01-21 18:28:41.000000 qub-sherlock-2.2.1/qub_sherlock.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       53 2022-01-21 18:28:41.000000 qub-sherlock-2.2.1/qub_sherlock.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2022-01-21 18:26:32.000000 qub-sherlock-2.2.1/qub_sherlock.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       86 2022-01-21 18:28:41.000000 qub-sherlock-2.2.1/qub_sherlock.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        9 2022-01-21 18:28:41.000000 qub-sherlock-2.2.1/qub_sherlock.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2022-01-21 18:28:41.000000 qub-sherlock-2.2.1/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1987 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/setup.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2022-01-21 18:28:41.000000 qub-sherlock-2.2.1/sherlock/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      371 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10080 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/advanced_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10485 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/catalogue_conesearch.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10399 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2022-01-21 18:28:41.000000 qub-sherlock-2.2.1/sherlock/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      265 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2676 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/commonutils/get_crossmatch_catalogues_column_map.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      411 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/commonutils/getpackagepath.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14272 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/commonutils/update_wiki_pages.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9029 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/database.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    20938 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/database_cleaner.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2666 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/default_settings.yaml
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2022-01-21 18:28:41.000000 qub-sherlock-2.2.1/sherlock/imports/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      174 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/imports/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8961 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/imports/_base_importer.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5686 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/imports/ifs.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    19230 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/imports/ned.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    24917 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/imports/ned_d.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     7195 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/imports/veron.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13936 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/test_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    37494 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/transient_catalogue_crossmatch.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    88151 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/transient_classifier.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3390 2022-01-21 18:25:31.000000 qub-sherlock-2.2.1/sherlock/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2022-05-18 13:33:57.596012 qub-sherlock-2.2.2/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      413 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/.readthedocs.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4316 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      304 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2739 2022-05-18 13:33:57.596012 qub-sherlock-2.2.2/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1947 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/README.md
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2022-05-18 13:33:57.592012 qub-sherlock-2.2.2/qub_sherlock.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2739 2022-05-18 13:33:56.000000 qub-sherlock-2.2.2/qub_sherlock.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      993 2022-05-18 13:33:57.000000 qub-sherlock-2.2.2/qub_sherlock.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2022-05-18 13:33:56.000000 qub-sherlock-2.2.2/qub_sherlock.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       52 2022-05-18 13:33:57.000000 qub-sherlock-2.2.2/qub_sherlock.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2022-05-18 13:31:19.000000 qub-sherlock-2.2.2/qub_sherlock.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       86 2022-05-18 13:33:57.000000 qub-sherlock-2.2.2/qub_sherlock.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        9 2022-05-18 13:33:57.000000 qub-sherlock-2.2.2/qub_sherlock.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2022-05-18 13:33:57.596012 qub-sherlock-2.2.2/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1987 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2022-05-18 13:33:57.592012 qub-sherlock-2.2.2/sherlock/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      371 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10080 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/advanced_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10485 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/catalogue_conesearch.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10399 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2022-05-18 13:33:57.592012 qub-sherlock-2.2.2/sherlock/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      265 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2676 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/commonutils/get_crossmatch_catalogues_column_map.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      411 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/commonutils/getpackagepath.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14272 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/commonutils/update_wiki_pages.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9029 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/database.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    20938 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/database_cleaner.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2666 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/default_settings.yaml
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2022-05-18 13:33:57.596012 qub-sherlock-2.2.2/sherlock/imports/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      174 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/imports/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8961 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/imports/_base_importer.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5669 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/imports/ifs.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    19229 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/imports/ned.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    24917 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/imports/ned_d.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     7195 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/imports/veron.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13936 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/test_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    37494 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/transient_catalogue_crossmatch.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    88470 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/transient_classifier.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3390 2022-05-18 13:29:17.000000 qub-sherlock-2.2.2/sherlock/utKit.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `qub-sherlock-2.2.1/CHANGES.md` & `qub-sherlock-2.2.2/CHANGES.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 
 ## Release Notes
 
+**v2.2.2 - May 18, 2022** 
+
+**FIXED**: NED name parsing errors fixed
+
 **v2.2.1 - January 21, 2022** 
 
-**ENHANCEMENT**: added separate treatment of galaxies which extend > 10 arcmin in the sky. Search radii are reduced to reduce the chance of a background source getting incorrectly associated with these local neighbours.
-**ENHANCEMENT**: added a 'deny list' in settings for galaxies with incorrect morphology reports in NED (only morphology ignored, all other metadata read as usual). So far list members only include "Sagittarius Dwarf Spheroidal" and "WISEA J193037.70-521726.0"
-**REFACTOR**: reduced cl chattiness when verbosity is set to 0.
-**FIXED**: synonym matching was not switched off in hidden settings
-**FIXED**: semi major axis (diameter) now divided by 2 (to get radius) before comparing with separations to determine associations. 
-**FIXED**: typo in 'galaxy radius stretch factor' (was 'galaxy radius stetch factor')
+* **ENHANCEMENT**: added separate treatment of galaxies which extend > 10 arcmin in the sky. Search radii are reduced to reduce the chance of a background source getting incorrectly associated with these local neighbours.  
+* **ENHANCEMENT**: added a 'deny list' in settings for galaxies with incorrect morphology reports in NED (only morphology ignored, all other metadata read as usual). So far list members only include "Sagittarius Dwarf Spheroidal" and "WISEA J193037.70-521726.0"  
+* **REFACTOR**: reduced cl chattiness when verbosity is set to 0.  
+* **FIXED**: synonym matching was not switched off in hidden settings  
+* **FIXED**: semi major axis (diameter) now divided by 2 (to get radius) before comparing with separations to determine associations.   
+* **FIXED**: typo in 'galaxy radius stretch factor' (was 'galaxy radius stetch factor')  
 
 
 **v2.2.0 - August 2, 2021** 
 
 *  **FEATURE**: Default search algorithm now version-controlled and ship alongside code. Users can override the default algorithm if they need to.
 * **FEATURE**: Hidden `database-batch-size` and `cpu-pool-size` settings added - power users can access and change in settings files.
 * **ENHANCEMENT**: Speed improvements (5-10 times processing speed increase).
```

### Comparing `qub-sherlock-2.2.1/LICENSE` & `qub-sherlock-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qub-sherlock-2.2.1/PKG-INFO` & `qub-sherlock-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: qub-sherlock
-Version: 2.2.1
+Version: 2.2.2
 Summary: mine a library of historical and on-going astronomical survey data in an attempt to identify the sources of transient/variable events, and predict their classifications based on crossmatched data
 Home-page: https://github.com/thespacedoctor/sherlock
+Download-URL: https://github.com/thespacedoctor/sherlock/archive/v2.2.2.zip
 Author: David Young
 Author-email: davidrobertyoung@gmail.com
 License: MIT
-Download-URL: https://github.com/thespacedoctor/sherlock/archive/v2.2.1.zip
 Keywords: astronomy, classification, crossmatch, sherlock, transient
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
```

### Comparing `qub-sherlock-2.2.1/README.md` & `qub-sherlock-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `qub-sherlock-2.2.1/qub_sherlock.egg-info/PKG-INFO` & `qub-sherlock-2.2.2/qub_sherlock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: qub-sherlock
-Version: 2.2.1
+Version: 2.2.2
 Summary: mine a library of historical and on-going astronomical survey data in an attempt to identify the sources of transient/variable events, and predict their classifications based on crossmatched data
 Home-page: https://github.com/thespacedoctor/sherlock
+Download-URL: https://github.com/thespacedoctor/sherlock/archive/v2.2.2.zip
 Author: David Young
 Author-email: davidrobertyoung@gmail.com
 License: MIT
-Download-URL: https://github.com/thespacedoctor/sherlock/archive/v2.2.1.zip
 Keywords: astronomy, classification, crossmatch, sherlock, transient
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
```

### Comparing `qub-sherlock-2.2.1/qub_sherlock.egg-info/SOURCES.txt` & `qub-sherlock-2.2.2/qub_sherlock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qub-sherlock-2.2.1/setup.py` & `qub-sherlock-2.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `qub-sherlock-2.2.1/sherlock/advanced_settings.yaml` & `qub-sherlock-2.2.2/sherlock/advanced_settings.yaml`

 * *Files identical despite different names*

### Comparing `qub-sherlock-2.2.1/sherlock/catalogue_conesearch.py` & `qub-sherlock-2.2.2/sherlock/catalogue_conesearch.py`

 * *Files identical despite different names*

### Comparing `qub-sherlock-2.2.1/sherlock/cl_utils.py` & `qub-sherlock-2.2.2/sherlock/cl_utils.py`

 * *Files identical despite different names*

### Comparing `qub-sherlock-2.2.1/sherlock/commonutils/get_crossmatch_catalogues_column_map.py` & `qub-sherlock-2.2.2/sherlock/commonutils/get_crossmatch_catalogues_column_map.py`

 * *Files identical despite different names*

### Comparing `qub-sherlock-2.2.1/sherlock/commonutils/update_wiki_pages.py` & `qub-sherlock-2.2.2/sherlock/commonutils/update_wiki_pages.py`

 * *Files identical despite different names*

### Comparing `qub-sherlock-2.2.1/sherlock/database.py` & `qub-sherlock-2.2.2/sherlock/database.py`

 * *Files identical despite different names*

### Comparing `qub-sherlock-2.2.1/sherlock/database_cleaner.py` & `qub-sherlock-2.2.2/sherlock/database_cleaner.py`

 * *Files identical despite different names*

### Comparing `qub-sherlock-2.2.1/sherlock/default_settings.yaml` & `qub-sherlock-2.2.2/sherlock/default_settings.yaml`

 * *Files identical despite different names*

### Comparing `qub-sherlock-2.2.1/sherlock/imports/_base_importer.py` & `qub-sherlock-2.2.2/sherlock/imports/_base_importer.py`

 * *Files identical despite different names*

### Comparing `qub-sherlock-2.2.1/sherlock/imports/ifs.py` & `qub-sherlock-2.2.2/sherlock/imports/ifs.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,43 +3,44 @@
 """
 *Import Multi Unit Spectroscopic Explorer (MUSE) IFS galaxy stream into sherlock-catalogues database*
 
 :Author:
     David Young
 """
 from __future__ import print_function
+from ._base_importer import _base_importer
+from fundamentals.download import multiobject_download
+from astrocalc.coords import unit_conversion
+from docopt import docopt
+import re
+import requests
+import string
+import codecs
+import pickle
+import glob
+import readline
 import sys
 import os
 os.environ['TERM'] = 'vt100'
-import readline
-import glob
-import pickle
-import codecs
-import string
-import requests
-import re
-from docopt import docopt
-from astrocalc.coords import unit_conversion
-from fundamentals.download import multiobject_download
-from ._base_importer import _base_importer
+
 
 class ifs(_base_importer):
     """
     *Importer for the Multi Unit Spectroscopic Explorer (MUSE) IFS galaxy catalogue stream*
 
     **Key Arguments**
 
     - ``log`` -- logger
     - ``settings`` -- the settings dictionary
-    
+
 
     **Usage**
 
     To import the IFS catalogue stream into the sherlock-catalogues database, run the following:
-    
+
 
       ```python
       from sherlock.imports import IFS
       ```
 
         stream = IFS(
             log=log,
@@ -58,29 +59,29 @@
         """*Import the IFS catalogue into the sherlock-catalogues database*
 
         The method first generates a list of python dictionaries from the IFS datafile, imports this list of dictionaries into a database table and then generates the HTMIDs for that table. 
 
         **Usage**
 
         See class docstring for usage
-        
+
         """
         self.log.debug('starting the ``get`` method')
 
         self.primaryIdColumnName = "primaryId"
         self.raColName = "raDeg"
         self.declColName = "decDeg"
         self.dbTableName = "tcs_cat_ifs_stream"
         self.databaseInsertbatchSize = 500
 
         dictList = self._create_dictionary_of_IFS()
 
         tableName = self.dbTableName
         createStatement = """
-    CREATE TABLE `%(tableName)s` (
+    CREATE TABLE IF NOT EXISTS `%(tableName)s` (
       `primaryId` bigint(20) NOT NULL AUTO_INCREMENT COMMENT 'An internal counter',
       `dateCreated` datetime DEFAULT  CURRENT_TIMESTAMP,
       `decDeg` double DEFAULT NULL,
       `name` varchar(100) COLLATE utf8_unicode_ci DEFAULT NULL,
       `raDeg` double DEFAULT NULL,
       `z` double DEFAULT NULL,
       `htm16ID` bigint(20) DEFAULT NULL,
@@ -107,27 +108,27 @@
     def _create_dictionary_of_IFS(
             self):
         """*Generate the list of dictionaries containing all the rows in the IFS stream*
 
         **Return**
 
         - ``dictList`` - a list of dictionaries containing all the rows in the IFS stream
-        
+
 
         **Usage**
 
         ```python
         from sherlock.imports import IFS
         stream = IFS(
             log=log,
             settings=settings
         )
         dictList = stream._create_dictionary_of_IFS()
         ```
-        
+
         """
         self.log.debug(
             'starting the ``_create_dictionary_of_IFS`` method')
 
         # GRAB THE CONTENT OF THE IFS CSV
         try:
             response = requests.get(
```

### Comparing `qub-sherlock-2.2.1/sherlock/imports/ned.py` & `qub-sherlock-2.2.2/sherlock/imports/ned.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 # encoding: utf-8
 """
 *Import ned stream into sherlock-catalogues database*
 
 :Author:
     David Young
 """
-from __future__ import print_function
-from __future__ import division
+from __future__ import print_function, division
+from ._base_importer import _base_importer
+from fundamentals.mysql import directory_script_runner, readquery, writequery
+from fundamentals.renderer import list_of_dictionaries
+from astrocalc.coords import unit_conversion
+from fundamentals.mysql import insert_list_of_dictionaries_into_database_tables
+from HMpTy.mysql import add_htm_ids_to_mysql_database_table
+from neddy import namesearch, conesearch
+from docopt import docopt
+from datetime import datetime, date, time
+import re
+import string
+import codecs
+import pickle
+import glob
+import readline
+
 from past.utils import old_div
 import sys
 import os
 os.environ['TERM'] = 'vt100'
-import readline
-import glob
-import pickle
-import codecs
-import string
-import re
-from datetime import datetime, date, time
-from docopt import docopt
-from neddy import namesearch, conesearch
-from HMpTy.mysql import add_htm_ids_to_mysql_database_table
-from fundamentals.mysql import insert_list_of_dictionaries_into_database_tables
-from astrocalc.coords import unit_conversion
-from fundamentals.renderer import list_of_dictionaries
-from fundamentals.mysql import directory_script_runner, readquery, writequery
-from ._base_importer import _base_importer
 
 
 class ned(_base_importer):
     """
     *Using a list of coordinates, query the online* `NED <https://ned.ipac.caltech.edu/>`_ *database and import sources found within a given search radius of each of the loctions into the sherlock-catalogues database*
 
     The code:
@@ -372,15 +372,15 @@
             log=self.log,
             sqlQuery=sqlQuery,
             dbConn=self.cataloguesDbConn,
             quiet=False
         )
 
         self.theseIds = []
-        self.theseIds[:] = [r["ned_name"] for r in rows]
+        self.theseIds[:] = [r["ned_name"].replace('"', '\\"') for r in rows]
 
         self.log.debug(
             'completed the ``_get_ned_sources_needing_metadata`` method')
 
         return len(self.theseIds)
 
     def _do_ned_namesearch_queries_and_add_resulting_metadata_to_database(
```

### Comparing `qub-sherlock-2.2.1/sherlock/imports/ned_d.py` & `qub-sherlock-2.2.2/sherlock/imports/ned_d.py`

 * *Files identical despite different names*

### Comparing `qub-sherlock-2.2.1/sherlock/imports/veron.py` & `qub-sherlock-2.2.2/sherlock/imports/veron.py`

 * *Files identical despite different names*

### Comparing `qub-sherlock-2.2.1/sherlock/test_settings.yaml` & `qub-sherlock-2.2.2/sherlock/test_settings.yaml`

 * *Files identical despite different names*

### Comparing `qub-sherlock-2.2.1/sherlock/transient_catalogue_crossmatch.py` & `qub-sherlock-2.2.2/sherlock/transient_catalogue_crossmatch.py`

 * *Files identical despite different names*

### Comparing `qub-sherlock-2.2.1/sherlock/transient_classifier.py` & `qub-sherlock-2.2.2/sherlock/transient_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,30 @@
 *classify a set of transients defined by a database query in the sherlock settings file*
 
 :Author:
     David Young
 """
 from __future__ import print_function
 from __future__ import division
+from astrocalc.coords import unit_conversion
+import copy
+from fundamentals.mysql import insert_list_of_dictionaries_into_database_tables
+from fundamentals import fmultiprocess
+import psutil
+from sherlock.commonutils import get_crossmatch_catalogues_column_map
+from sherlock.imports import ned
+from HMpTy.htm import sets
+from HMpTy.mysql import conesearch
+from fundamentals.renderer import list_of_dictionaries
+from fundamentals.mysql import readquery, directory_script_runner, writequery
+from fundamentals import tools
+import numpy as np
+from operator import itemgetter
+from datetime import datetime, date, time, timedelta
+
 from builtins import zip
 from builtins import str
 from builtins import range
 from builtins import object
 from past.utils import old_div
 import sys
 import os
@@ -20,32 +36,14 @@
 import re
 import math
 import time
 import inspect
 import yaml
 from random import randint
 os.environ['TERM'] = 'vt100'
-from datetime import datetime, date, time, timedelta
-from operator import itemgetter
-import numpy as np
-from fundamentals import tools
-from fundamentals.mysql import readquery, directory_script_runner, writequery
-from fundamentals.renderer import list_of_dictionaries
-from HMpTy.mysql import conesearch
-from HMpTy.htm import sets
-from sherlock.imports import ned
-from sherlock.commonutils import get_crossmatch_catalogues_column_map
-import psutil
-from fundamentals import fmultiprocess
-from fundamentals.mysql import insert_list_of_dictionaries_into_database_tables
-import copy
-import psutil
-import copy
-from operator import itemgetter
-from astrocalc.coords import unit_conversion
 
 theseBatches = []
 crossmatchArray = []
 
 
 class transient_classifier(object):
     """
@@ -1940,14 +1938,18 @@
         if "catalogue_object_subtype" not in match:
             match["catalogue_object_subtype"] = None
         catalogue = match["catalogue_table_name"]
         objectId = match["catalogue_object_id"]
         objectType = match["catalogue_object_type"]
         objectSubtype = match["catalogue_object_subtype"]
         catalogueString = catalogue
+        if catalogueString is None:
+            badGuy = match["transient_object_id"]
+            print(f"Issue with object {badGuy}")
+            raise TypeError(f"Issue with object {badGuy}")
         if "catalogue" not in catalogueString.lower():
             catalogueString = catalogue + " catalogue"
         if "/" in catalogueString:
             catalogueString += "s"
 
         if "ned" in catalogue.lower():
             objectId = objectId.replace("+", "%2B")
@@ -2093,16 +2095,20 @@
                 absMag = "%(distance_modulus)0.2f" % locals()
                 absMag = """ A host %(distance)s implies a <em>m - M =</em> %(absMag)s.""" % locals(
                 )
             else:
                 absMag = ""
 
         annotation = "The transient is %(classificationReliability)s with <em>%(objectId)s</em>; %(best_mag_filter)s%(best_mag)smag %(objectType)s found in the %(catalogueString)s. It's located %(location)s.%(absMag)s" % locals()
-        summary = '%(sep)0.1f" from %(objectType)s in %(catalogue)s' % locals(
-        )
+        try:
+            summary = '%(sep)0.1f" from %(objectType)s in %(catalogue)s' % locals()
+        except:
+            badGuy = match["transient_object_id"]
+            print(f"Issue with object {badGuy}")
+            raise TypeError(f"Issue with object {badGuy}")
 
         self.log.debug('completed the ``generate_match_annotation`` method')
         return annotation, summary, sep
 
     # use the tab-trigger below for new method
     # xt-class-method
```

### Comparing `qub-sherlock-2.2.1/sherlock/utKit.py` & `qub-sherlock-2.2.2/sherlock/utKit.py`

 * *Files identical despite different names*

