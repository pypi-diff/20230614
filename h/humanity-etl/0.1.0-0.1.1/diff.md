# Comparing `tmp/humanity_etl-0.1.0.tar.gz` & `tmp/humanity_etl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humanity_etl-0.1.0.tar", last modified: Wed Jun 14 17:29:39 2023, max compression
+gzip compressed data, was "humanity_etl-0.1.1.tar", last modified: Wed Jun 14 17:49:56 2023, max compression
```

## Comparing `humanity_etl-0.1.0.tar` & `humanity_etl-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:29:39.709748 humanity_etl-0.1.0/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 humanity_etl-0.1.0/MANIFEST.in
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1743 2023-06-14 17:29:39.709748 humanity_etl-0.1.0/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1235 2023-06-14 17:17:02.000000 humanity_etl-0.1.0/README_PUBLIC.md
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:29:39.709748 humanity_etl-0.1.0/humanity_etl/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       22 2023-06-14 17:28:48.000000 humanity_etl-0.1.0/humanity_etl/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      155 2023-06-14 17:18:21.000000 humanity_etl-0.1.0/humanity_etl/__main__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      329 2023-06-14 17:18:21.000000 humanity_etl-0.1.0/humanity_etl/humanity_etl.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:29:39.709748 humanity_etl-0.1.0/humanity_etl/libs/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 humanity_etl-0.1.0/humanity_etl/libs/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4840 2023-06-14 17:18:21.000000 humanity_etl-0.1.0/humanity_etl/libs/cnst.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-06-14 17:18:21.000000 humanity_etl-0.1.0/humanity_etl/libs/dbg.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      548 2023-06-14 17:18:21.000000 humanity_etl-0.1.0/humanity_etl/libs/network.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     5986 2023-06-14 17:19:56.000000 humanity_etl-0.1.0/humanity_etl/libs/transform.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:29:39.709748 humanity_etl-0.1.0/humanity_etl/tables/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 humanity_etl-0.1.0/humanity_etl/tables/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4572 2023-06-14 17:18:21.000000 humanity_etl-0.1.0/humanity_etl/tables/timeclocks.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:29:39.709748 humanity_etl-0.1.0/humanity_etl.egg-info/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1743 2023-06-14 17:29:39.000000 humanity_etl-0.1.0/humanity_etl.egg-info/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      530 2023-06-14 17:29:39.000000 humanity_etl-0.1.0/humanity_etl.egg-info/SOURCES.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-14 17:29:39.000000 humanity_etl-0.1.0/humanity_etl.egg-info/dependency_links.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       75 2023-06-14 17:29:39.000000 humanity_etl-0.1.0/humanity_etl.egg-info/requires.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-14 17:29:39.000000 humanity_etl-0.1.0/humanity_etl.egg-info/top_level.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      426 2023-06-14 17:29:39.709748 humanity_etl-0.1.0/setup.cfg
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      987 2023-06-14 17:28:48.000000 humanity_etl-0.1.0/setup.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:29:39.709748 humanity_etl-0.1.0/tests/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 humanity_etl-0.1.0/tests/__init__.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:49:56.715183 humanity_etl-0.1.1/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 humanity_etl-0.1.1/MANIFEST.in
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1743 2023-06-14 17:49:56.715183 humanity_etl-0.1.1/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1235 2023-06-14 17:17:02.000000 humanity_etl-0.1.1/README_PUBLIC.md
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:49:56.711183 humanity_etl-0.1.1/humanity_etl/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       22 2023-06-14 17:49:14.000000 humanity_etl-0.1.1/humanity_etl/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      155 2023-06-14 17:18:21.000000 humanity_etl-0.1.1/humanity_etl/__main__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      329 2023-06-14 17:18:21.000000 humanity_etl-0.1.1/humanity_etl/humanity_etl.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:49:56.715183 humanity_etl-0.1.1/humanity_etl/libs/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 humanity_etl-0.1.1/humanity_etl/libs/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4840 2023-06-14 17:18:21.000000 humanity_etl-0.1.1/humanity_etl/libs/cnst.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-06-14 17:18:21.000000 humanity_etl-0.1.1/humanity_etl/libs/dbg.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      548 2023-06-14 17:18:21.000000 humanity_etl-0.1.1/humanity_etl/libs/network.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     5987 2023-06-14 17:44:05.000000 humanity_etl-0.1.1/humanity_etl/libs/transform.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:49:56.715183 humanity_etl-0.1.1/humanity_etl/tables/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 humanity_etl-0.1.1/humanity_etl/tables/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4572 2023-06-14 17:18:21.000000 humanity_etl-0.1.1/humanity_etl/tables/timeclocks.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:49:56.711183 humanity_etl-0.1.1/humanity_etl.egg-info/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1743 2023-06-14 17:49:56.000000 humanity_etl-0.1.1/humanity_etl.egg-info/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      530 2023-06-14 17:49:56.000000 humanity_etl-0.1.1/humanity_etl.egg-info/SOURCES.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-14 17:49:56.000000 humanity_etl-0.1.1/humanity_etl.egg-info/dependency_links.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       75 2023-06-14 17:49:56.000000 humanity_etl-0.1.1/humanity_etl.egg-info/requires.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-14 17:49:56.000000 humanity_etl-0.1.1/humanity_etl.egg-info/top_level.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      426 2023-06-14 17:49:56.715183 humanity_etl-0.1.1/setup.cfg
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1050 2023-06-14 17:49:14.000000 humanity_etl-0.1.1/setup.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:49:56.715183 humanity_etl-0.1.1/tests/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 humanity_etl-0.1.1/tests/__init__.py
```

### Comparing `humanity_etl-0.1.0/PKG-INFO` & `humanity_etl-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humanity_etl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Replicate humanity data in databricks
 Home-page: https://github.com/neofinancial/humanity_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `humanity_etl-0.1.0/README_PUBLIC.md` & `humanity_etl-0.1.1/README_PUBLIC.md`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.1.0/humanity_etl/libs/cnst.py` & `humanity_etl-0.1.1/humanity_etl/libs/cnst.py`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.1.0/humanity_etl/libs/dbg.py` & `humanity_etl-0.1.1/humanity_etl/libs/dbg.py`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.1.0/humanity_etl/libs/network.py` & `humanity_etl-0.1.1/humanity_etl/libs/network.py`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.1.0/humanity_etl/libs/transform.py` & `humanity_etl-0.1.1/humanity_etl/libs/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     return change
 
 
 def merge_related_dfs(df_dict: Dict[str, PandasDF]) -> Dict[str, PandasDF]:
     """
     Union the employees and disabled employess associated dataframes
     """
-    merged_dfs: Dict[str,PandasDF] = {}
+    merged_dfs: Dict[str, PandasDF] = {}
     for key, df in df_dict.items():
         if key.endswith("_employees") or key.endswith("_employees_disabled"):
             # Get the prefix of the key
             prefix = (
                 key.rsplit("_", 1)[0]
                 if key.endswith("_employees")
                 else key.rsplit("_", 2)[0]
```

### Comparing `humanity_etl-0.1.0/humanity_etl/tables/timeclocks.py` & `humanity_etl-0.1.1/humanity_etl/tables/timeclocks.py`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.1.0/humanity_etl.egg-info/PKG-INFO` & `humanity_etl-0.1.1/humanity_etl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humanity-etl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Replicate humanity data in databricks
 Home-page: https://github.com/neofinancial/humanity_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `humanity_etl-0.1.0/humanity_etl.egg-info/SOURCES.txt` & `humanity_etl-0.1.1/humanity_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.1.0/setup.py` & `humanity_etl-0.1.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,24 +6,32 @@
     long_description = fh.read()
 
 setup(
     author="Neo Financial",
     author_email="engineering@neofinancial.com",
     python_requires=">=3.6",
     name="humanity_etl",
-    version="0.1.0",
+    version="0.1.1",
     description="Replicate humanity data in databricks",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
     ],
     license="UNLICENSED",
     packages=find_packages(include=["humanity_etl", "humanity_etl.*"]),
     url="https://github.com/neofinancial/humanity_etl",
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=["click", "pandas>=1,<2", "requests", "pyspark", "loguru", "python-dotenv", "typing_extensions"],
+    install_requires=[
+        "click",
+        "pandas>=1,<2",
+        "requests",
+        "pyspark",
+        "loguru",
+        "python-dotenv",
+        "typing_extensions",
+    ],
     tests_require=["pytest"],
 )
```

