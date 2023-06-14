# Comparing `tmp/erdgen-0.0.1rc4.tar.gz` & `tmp/erdgen-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erdgen-0.0.1rc4.tar", last modified: Mon Jun  5 16:13:15 2023, max compression
+gzip compressed data, was "erdgen-0.1.0.tar", last modified: Wed Jun 14 16:34:35 2023, max compression
```

## Comparing `erdgen-0.0.1rc4.tar` & `erdgen-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-05 16:13:15.302172 erdgen-0.0.1rc4/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1068 2023-06-02 00:24:03.000000 erdgen-0.0.1rc4/LICENSE
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      197 2023-06-05 16:12:49.000000 erdgen-0.0.1rc4/MANIFEST.in
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     4578 2023-06-05 16:13:15.302172 erdgen-0.0.1rc4/PKG-INFO
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     3995 2023-06-05 16:12:49.000000 erdgen-0.0.1rc4/README.md
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-05 16:13:15.302172 erdgen-0.0.1rc4/erdgen/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:24:03.000000 erdgen-0.0.1rc4/erdgen/__init__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       87 2023-06-02 00:24:03.000000 erdgen-0.0.1rc4/erdgen/__main__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      419 2023-06-02 00:24:03.000000 erdgen-0.0.1rc4/erdgen/erdgen.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-05 16:13:15.302172 erdgen-0.0.1rc4/erdgen/src/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     3004 2023-06-02 18:44:51.000000 erdgen-0.0.1rc4/erdgen/src/_.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:24:03.000000 erdgen-0.0.1rc4/erdgen/src/__init__.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-05 16:13:15.302172 erdgen-0.0.1rc4/erdgen.egg-info/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     4578 2023-06-05 16:13:15.000000 erdgen-0.0.1rc4/erdgen.egg-info/PKG-INFO
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      320 2023-06-05 16:13:15.000000 erdgen-0.0.1rc4/erdgen.egg-info/SOURCES.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        1 2023-06-05 16:13:15.000000 erdgen-0.0.1rc4/erdgen.egg-info/dependency_links.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       38 2023-06-05 16:13:15.000000 erdgen-0.0.1rc4/erdgen.egg-info/requires.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        7 2023-06-05 16:13:15.000000 erdgen-0.0.1rc4/erdgen.egg-info/top_level.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       38 2023-06-05 16:13:15.302172 erdgen-0.0.1rc4/setup.cfg
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      992 2023-06-05 16:12:49.000000 erdgen-0.0.1rc4/setup.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-05 16:13:15.302172 erdgen-0.0.1rc4/tests/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-04 00:27:25.000000 erdgen-0.0.1rc4/tests/__init__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2315 2023-06-05 16:12:49.000000 erdgen-0.0.1rc4/tests/test_erdgen.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 16:34:35.280174 erdgen-0.1.0/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1068 2023-06-06 22:11:44.000000 erdgen-0.1.0/LICENSE
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      197 2023-06-06 22:11:44.000000 erdgen-0.1.0/MANIFEST.in
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4665 2023-06-14 16:34:35.280174 erdgen-0.1.0/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4089 2023-06-14 16:33:45.000000 erdgen-0.1.0/README.md
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 16:34:35.280174 erdgen-0.1.0/erdgen/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       22 2023-06-14 16:31:33.000000 erdgen-0.1.0/erdgen/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       87 2023-06-06 22:11:44.000000 erdgen-0.1.0/erdgen/__main__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      425 2023-06-14 16:09:02.000000 erdgen-0.1.0/erdgen/erdgen.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 16:34:35.280174 erdgen-0.1.0/erdgen/src/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:11:44.000000 erdgen-0.1.0/erdgen/src/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     3005 2023-06-14 16:09:02.000000 erdgen-0.1.0/erdgen/src/erdgen.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 16:34:35.280174 erdgen-0.1.0/erdgen.egg-info/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4665 2023-06-14 16:34:35.000000 erdgen-0.1.0/erdgen.egg-info/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      335 2023-06-14 16:34:35.000000 erdgen-0.1.0/erdgen.egg-info/SOURCES.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-14 16:34:35.000000 erdgen-0.1.0/erdgen.egg-info/dependency_links.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-14 16:34:35.000000 erdgen-0.1.0/erdgen.egg-info/requires.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        7 2023-06-14 16:34:35.000000 erdgen-0.1.0/erdgen.egg-info/top_level.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      420 2023-06-14 16:34:35.280174 erdgen-0.1.0/setup.cfg
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      985 2023-06-14 16:31:33.000000 erdgen-0.1.0/setup.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 16:34:35.280174 erdgen-0.1.0/tests/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:11:44.000000 erdgen-0.1.0/tests/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2322 2023-06-14 16:09:03.000000 erdgen-0.1.0/tests/test_erdgen.py
```

### Comparing `erdgen-0.0.1rc4/LICENSE` & `erdgen-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erdgen-0.0.1rc4/PKG-INFO` & `erdgen-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: erdgen
-Version: 0.0.1rc4
+Version: 0.1.0
 Summary: Generate a DBML ERD from DBT YML relationships
 Home-page: https://github.com/neo-andrew-moss/erdgen
 Author: Andrew Moss
 Author-email: andrew.moss@neofinancial.com
 License: MIT license
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -134,14 +134,24 @@
 make format
 ```
 
 ```bash
 make lint
 ```
 
+## Version & Release
+
+```bash
+bump2version <major/minor/patch>
+```
+
+```bash
+make release
+```
+
 ## TODO
 
 - Add better error handling and reporting
 - Perhaps add a debug/verbose mode
 - make it less jank
```

### Comparing `erdgen-0.0.1rc4/README.md` & `erdgen-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -116,12 +116,22 @@
 make format
 ```
 
 ```bash
 make lint
 ```
 
+## Version & Release
+
+```bash
+bump2version <major/minor/patch>
+```
+
+```bash
+make release
+```
+
 ## TODO
 
 - Add better error handling and reporting
 - Perhaps add a debug/verbose mode
 - make it less jank
```

### Comparing `erdgen-0.0.1rc4/erdgen/src/_.py` & `erdgen-0.1.0/erdgen/src/erdgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """src"""
 import os
 from functools import reduce
-from typing import List, Tuple, Dict, Union
+from typing import Dict, List, Tuple, Union
+
 import yaml
 from jinja2 import Template
 
 
 def load_yml(file: str) -> Dict:
     """load_yml"""
     with open(file, "r") as stream:
```

### Comparing `erdgen-0.0.1rc4/erdgen.egg-info/PKG-INFO` & `erdgen-0.1.0/erdgen.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: erdgen
-Version: 0.0.1rc4
+Version: 0.1.0
 Summary: Generate a DBML ERD from DBT YML relationships
 Home-page: https://github.com/neo-andrew-moss/erdgen
 Author: Andrew Moss
 Author-email: andrew.moss@neofinancial.com
 License: MIT license
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -134,14 +134,24 @@
 make format
 ```
 
 ```bash
 make lint
 ```
 
+## Version & Release
+
+```bash
+bump2version <major/minor/patch>
+```
+
+```bash
+make release
+```
+
 ## TODO
 
 - Add better error handling and reporting
 - Perhaps add a debug/verbose mode
 - make it less jank
```

### Comparing `erdgen-0.0.1rc4/setup.py` & `erdgen-0.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     long_description = fh.read()
 
 setup(
     author="Andrew Moss",
     author_email="andrew.moss@neofinancial.com",
     python_requires=">=3.6",
     name="erdgen",
-    version="0.0.1rc4",
+    version="0.1.0",
     description="Generate a DBML ERD from DBT YML relationships",
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
     ],
     license="MIT license",
     packages=find_packages(include=["erdgen", "erdgen.*"]),
```

### Comparing `erdgen-0.0.1rc4/tests/test_erdgen.py` & `erdgen-0.1.0/tests/test_erdgen.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-import pytest
 import os
 from tempfile import TemporaryDirectory
-from erdgen.src._ import (
-    load_yml,
+
+import pytest
+
+from erdgen.src.erdgen import (
+    extract_columns,
+    extract_relationships,
     generate_dbml,
     generate_dbml_schema,
-    extract_relationships,
-    extract_columns,
+    load_yml,
 )
 
 sample_yaml_content = """
 version: 2
 models:
  - name: Computer
    description: beep boop beep
```

