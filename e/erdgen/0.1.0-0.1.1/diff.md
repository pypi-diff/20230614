# Comparing `tmp/erdgen-0.1.0.tar.gz` & `tmp/erdgen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erdgen-0.1.0.tar", last modified: Wed Jun 14 16:34:35 2023, max compression
+gzip compressed data, was "erdgen-0.1.1.tar", last modified: Wed Jun 14 17:07:57 2023, max compression
```

## Comparing `erdgen-0.1.0.tar` & `erdgen-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 16:34:35.280174 erdgen-0.1.0/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1068 2023-06-06 22:11:44.000000 erdgen-0.1.0/LICENSE
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      197 2023-06-06 22:11:44.000000 erdgen-0.1.0/MANIFEST.in
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4665 2023-06-14 16:34:35.280174 erdgen-0.1.0/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4089 2023-06-14 16:33:45.000000 erdgen-0.1.0/README.md
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 16:34:35.280174 erdgen-0.1.0/erdgen/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       22 2023-06-14 16:31:33.000000 erdgen-0.1.0/erdgen/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       87 2023-06-06 22:11:44.000000 erdgen-0.1.0/erdgen/__main__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      425 2023-06-14 16:09:02.000000 erdgen-0.1.0/erdgen/erdgen.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 16:34:35.280174 erdgen-0.1.0/erdgen/src/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:11:44.000000 erdgen-0.1.0/erdgen/src/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     3005 2023-06-14 16:09:02.000000 erdgen-0.1.0/erdgen/src/erdgen.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 16:34:35.280174 erdgen-0.1.0/erdgen.egg-info/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4665 2023-06-14 16:34:35.000000 erdgen-0.1.0/erdgen.egg-info/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      335 2023-06-14 16:34:35.000000 erdgen-0.1.0/erdgen.egg-info/SOURCES.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-14 16:34:35.000000 erdgen-0.1.0/erdgen.egg-info/dependency_links.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-14 16:34:35.000000 erdgen-0.1.0/erdgen.egg-info/requires.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        7 2023-06-14 16:34:35.000000 erdgen-0.1.0/erdgen.egg-info/top_level.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      420 2023-06-14 16:34:35.280174 erdgen-0.1.0/setup.cfg
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      985 2023-06-14 16:31:33.000000 erdgen-0.1.0/setup.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 16:34:35.280174 erdgen-0.1.0/tests/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:11:44.000000 erdgen-0.1.0/tests/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2322 2023-06-14 16:09:03.000000 erdgen-0.1.0/tests/test_erdgen.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:07:57.671481 erdgen-0.1.1/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1068 2023-06-06 22:11:44.000000 erdgen-0.1.1/LICENSE
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      197 2023-06-06 22:11:44.000000 erdgen-0.1.1/MANIFEST.in
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4715 2023-06-14 17:07:57.671481 erdgen-0.1.1/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4139 2023-06-14 16:58:10.000000 erdgen-0.1.1/README.md
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:07:57.671481 erdgen-0.1.1/erdgen/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       22 2023-06-14 17:07:45.000000 erdgen-0.1.1/erdgen/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       87 2023-06-06 22:11:44.000000 erdgen-0.1.1/erdgen/__main__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      425 2023-06-14 16:09:02.000000 erdgen-0.1.1/erdgen/erdgen.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:07:57.671481 erdgen-0.1.1/erdgen/src/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:11:44.000000 erdgen-0.1.1/erdgen/src/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     3005 2023-06-14 16:09:02.000000 erdgen-0.1.1/erdgen/src/erdgen.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:07:57.671481 erdgen-0.1.1/erdgen.egg-info/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4715 2023-06-14 17:07:57.000000 erdgen-0.1.1/erdgen.egg-info/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      335 2023-06-14 17:07:57.000000 erdgen-0.1.1/erdgen.egg-info/SOURCES.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-14 17:07:57.000000 erdgen-0.1.1/erdgen.egg-info/dependency_links.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-14 17:07:57.000000 erdgen-0.1.1/erdgen.egg-info/requires.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        7 2023-06-14 17:07:57.000000 erdgen-0.1.1/erdgen.egg-info/top_level.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      420 2023-06-14 17:07:57.671481 erdgen-0.1.1/setup.cfg
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      985 2023-06-14 17:07:45.000000 erdgen-0.1.1/setup.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:07:57.671481 erdgen-0.1.1/tests/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:11:44.000000 erdgen-0.1.1/tests/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2322 2023-06-14 16:50:49.000000 erdgen-0.1.1/tests/test_erdgen.py
```

### Comparing `erdgen-0.1.0/LICENSE` & `erdgen-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `erdgen-0.1.0/PKG-INFO` & `erdgen-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erdgen
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generate a DBML ERD from DBT YML relationships
 Home-page: https://github.com/neo-andrew-moss/erdgen
 Author: Andrew Moss
 Author-email: andrew.moss@neofinancial.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -118,40 +118,50 @@
 
 ### Install Packages
 
 ```bash
 pip install -r requirements.txt
 ```
 
-## Test
+### Test
 
 ```bash
 make test
 ```
 
-## Format
+### Format
 
 ```bash
 make format
 ```
 
 ```bash
 make lint
 ```
 
-## Version & Release
+### Version & Release
 
 ```bash
 bump2version <major/minor/patch>
 ```
 
 ```bash
 make release
 ```
 
-## TODO
+**note** Don't forget to `git push` with `--tags`
 
-- Add better error handling and reporting
-- Perhaps add a debug/verbose mode
-- make it less jank
+### pre-commit
+
+#### Setup
+
+```bash
+pre-commit install
+```
+
+#### Run all
+
+```bash
+make pre-commit
+```
```

### Comparing `erdgen-0.1.0/README.md` & `erdgen-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -100,38 +100,48 @@
 
 ### Install Packages
 
 ```bash
 pip install -r requirements.txt
 ```
 
-## Test
+### Test
 
 ```bash
 make test
 ```
 
-## Format
+### Format
 
 ```bash
 make format
 ```
 
 ```bash
 make lint
 ```
 
-## Version & Release
+### Version & Release
 
 ```bash
 bump2version <major/minor/patch>
 ```
 
 ```bash
 make release
 ```
 
-## TODO
+**note** Don't forget to `git push` with `--tags`
 
-- Add better error handling and reporting
-- Perhaps add a debug/verbose mode
-- make it less jank
+### pre-commit
+
+#### Setup
+
+```bash
+pre-commit install
+```
+
+#### Run all
+
+```bash
+make pre-commit
+```
```

### Comparing `erdgen-0.1.0/erdgen/src/erdgen.py` & `erdgen-0.1.1/erdgen/src/erdgen.py`

 * *Files identical despite different names*

### Comparing `erdgen-0.1.0/erdgen.egg-info/PKG-INFO` & `erdgen-0.1.1/erdgen.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erdgen
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generate a DBML ERD from DBT YML relationships
 Home-page: https://github.com/neo-andrew-moss/erdgen
 Author: Andrew Moss
 Author-email: andrew.moss@neofinancial.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -118,40 +118,50 @@
 
 ### Install Packages
 
 ```bash
 pip install -r requirements.txt
 ```
 
-## Test
+### Test
 
 ```bash
 make test
 ```
 
-## Format
+### Format
 
 ```bash
 make format
 ```
 
 ```bash
 make lint
 ```
 
-## Version & Release
+### Version & Release
 
 ```bash
 bump2version <major/minor/patch>
 ```
 
 ```bash
 make release
 ```
 
-## TODO
+**note** Don't forget to `git push` with `--tags`
 
-- Add better error handling and reporting
-- Perhaps add a debug/verbose mode
-- make it less jank
+### pre-commit
+
+#### Setup
+
+```bash
+pre-commit install
+```
+
+#### Run all
+
+```bash
+make pre-commit
+```
```

### Comparing `erdgen-0.1.0/setup.py` & `erdgen-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     author="Andrew Moss",
     author_email="andrew.moss@neofinancial.com",
     python_requires=">=3.6",
     name="erdgen",
-    version="0.1.0",
+    version="0.1.1",
     description="Generate a DBML ERD from DBT YML relationships",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
```

### Comparing `erdgen-0.1.0/tests/test_erdgen.py` & `erdgen-0.1.1/tests/test_erdgen.py`

 * *Files identical despite different names*

