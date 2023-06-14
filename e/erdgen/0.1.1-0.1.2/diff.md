# Comparing `tmp/erdgen-0.1.1.tar.gz` & `tmp/erdgen-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erdgen-0.1.1.tar", last modified: Wed Jun 14 17:07:57 2023, max compression
+gzip compressed data, was "erdgen-0.1.2.tar", last modified: Wed Jun 14 17:53:08 2023, max compression
```

## Comparing `erdgen-0.1.1.tar` & `erdgen-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:07:57.671481 erdgen-0.1.1/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1068 2023-06-06 22:11:44.000000 erdgen-0.1.1/LICENSE
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      197 2023-06-06 22:11:44.000000 erdgen-0.1.1/MANIFEST.in
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4715 2023-06-14 17:07:57.671481 erdgen-0.1.1/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4139 2023-06-14 16:58:10.000000 erdgen-0.1.1/README.md
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:07:57.671481 erdgen-0.1.1/erdgen/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       22 2023-06-14 17:07:45.000000 erdgen-0.1.1/erdgen/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       87 2023-06-06 22:11:44.000000 erdgen-0.1.1/erdgen/__main__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      425 2023-06-14 16:09:02.000000 erdgen-0.1.1/erdgen/erdgen.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:07:57.671481 erdgen-0.1.1/erdgen/src/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:11:44.000000 erdgen-0.1.1/erdgen/src/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     3005 2023-06-14 16:09:02.000000 erdgen-0.1.1/erdgen/src/erdgen.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:07:57.671481 erdgen-0.1.1/erdgen.egg-info/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4715 2023-06-14 17:07:57.000000 erdgen-0.1.1/erdgen.egg-info/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      335 2023-06-14 17:07:57.000000 erdgen-0.1.1/erdgen.egg-info/SOURCES.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-14 17:07:57.000000 erdgen-0.1.1/erdgen.egg-info/dependency_links.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-14 17:07:57.000000 erdgen-0.1.1/erdgen.egg-info/requires.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        7 2023-06-14 17:07:57.000000 erdgen-0.1.1/erdgen.egg-info/top_level.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      420 2023-06-14 17:07:57.671481 erdgen-0.1.1/setup.cfg
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      985 2023-06-14 17:07:45.000000 erdgen-0.1.1/setup.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:07:57.671481 erdgen-0.1.1/tests/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:11:44.000000 erdgen-0.1.1/tests/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2322 2023-06-14 16:50:49.000000 erdgen-0.1.1/tests/test_erdgen.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:53:08.737327 erdgen-0.1.2/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1068 2023-06-06 22:11:44.000000 erdgen-0.1.2/LICENSE
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      197 2023-06-06 22:11:44.000000 erdgen-0.1.2/MANIFEST.in
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4715 2023-06-14 17:53:08.737327 erdgen-0.1.2/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4139 2023-06-14 16:58:10.000000 erdgen-0.1.2/README.md
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:53:08.737327 erdgen-0.1.2/erdgen/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       22 2023-06-14 17:52:59.000000 erdgen-0.1.2/erdgen/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       87 2023-06-06 22:11:44.000000 erdgen-0.1.2/erdgen/__main__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      425 2023-06-14 16:09:02.000000 erdgen-0.1.2/erdgen/erdgen.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:53:08.737327 erdgen-0.1.2/erdgen/src/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:11:44.000000 erdgen-0.1.2/erdgen/src/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     3027 2023-06-14 17:52:18.000000 erdgen-0.1.2/erdgen/src/erdgen.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:53:08.737327 erdgen-0.1.2/erdgen.egg-info/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4715 2023-06-14 17:53:08.000000 erdgen-0.1.2/erdgen.egg-info/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      335 2023-06-14 17:53:08.000000 erdgen-0.1.2/erdgen.egg-info/SOURCES.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-14 17:53:08.000000 erdgen-0.1.2/erdgen.egg-info/dependency_links.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-14 17:53:08.000000 erdgen-0.1.2/erdgen.egg-info/requires.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        7 2023-06-14 17:53:08.000000 erdgen-0.1.2/erdgen.egg-info/top_level.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      420 2023-06-14 17:53:08.737327 erdgen-0.1.2/setup.cfg
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      985 2023-06-14 17:52:59.000000 erdgen-0.1.2/setup.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:53:08.737327 erdgen-0.1.2/tests/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:11:44.000000 erdgen-0.1.2/tests/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2322 2023-06-14 16:50:49.000000 erdgen-0.1.2/tests/test_erdgen.py
```

### Comparing `erdgen-0.1.1/LICENSE` & `erdgen-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `erdgen-0.1.1/PKG-INFO` & `erdgen-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erdgen
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generate a DBML ERD from DBT YML relationships
 Home-page: https://github.com/neo-andrew-moss/erdgen
 Author: Andrew Moss
 Author-email: andrew.moss@neofinancial.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `erdgen-0.1.1/README.md` & `erdgen-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `erdgen-0.1.1/erdgen/src/erdgen.py` & `erdgen-0.1.2/erdgen/src/erdgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def load_yml(file: str) -> Dict:
     """load_yml"""
     with open(file, "r") as stream:
         try:
             return yaml.safe_load(stream)
         except yaml.YAMLError as err:
             print(err)
+            raise err
 
 
 def extract_columns(
     file: str, include_non_join_keys: bool = False
 ) -> List[Tuple[str, str]]:
     """extract_columns"""
     data = load_yml(file)
```

### Comparing `erdgen-0.1.1/erdgen.egg-info/PKG-INFO` & `erdgen-0.1.2/erdgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erdgen
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generate a DBML ERD from DBT YML relationships
 Home-page: https://github.com/neo-andrew-moss/erdgen
 Author: Andrew Moss
 Author-email: andrew.moss@neofinancial.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `erdgen-0.1.1/setup.py` & `erdgen-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 setup(
     author="Andrew Moss",
     author_email="andrew.moss@neofinancial.com",
     python_requires=">=3.6",
     name="erdgen",
-    version="0.1.1",
+    version="0.1.2",
     description="Generate a DBML ERD from DBT YML relationships",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
```

### Comparing `erdgen-0.1.1/tests/test_erdgen.py` & `erdgen-0.1.2/tests/test_erdgen.py`

 * *Files identical despite different names*

