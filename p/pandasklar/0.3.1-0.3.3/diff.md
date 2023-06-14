# Comparing `tmp/pandasklar-0.3.1.tar.gz` & `tmp/pandasklar-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasklar-0.3.1.tar", last modified: Wed May 31 19:38:45 2023, max compression
+gzip compressed data, was "pandasklar-0.3.3.tar", last modified: Wed Jun 14 04:42:13 2023, max compression
```

## Comparing `pandasklar-0.3.1.tar` & `pandasklar-0.3.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-31 19:38:45.489691 pandasklar-0.3.1/
--rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 pandasklar-0.3.1/LICENSE
--rw-rw-r--   0 me        (1000) me        (1000)     9805 2023-05-31 19:38:45.489691 pandasklar-0.3.1/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)     9297 2023-05-31 19:38:05.000000 pandasklar-0.3.1/README.md
--rw-r--r--   0 me        (1000) me        (1000)     1301 2023-05-31 19:37:55.000000 pandasklar-0.3.1/pyproject.toml
--rw-rw-r--   0 me        (1000) me        (1000)       38 2023-05-31 19:38:45.489691 pandasklar-0.3.1/setup.cfg
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-31 19:38:45.365693 pandasklar-0.3.1/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-31 19:38:45.481691 pandasklar-0.3.1/src/pandasklar/
--rw-r--r--   0 me        (1000) me        (1000)      537 2023-02-13 16:45:54.000000 pandasklar-0.3.1/src/pandasklar/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)      214 2023-02-14 22:57:35.000000 pandasklar-0.3.1/src/pandasklar/__main__.py
--rw-r--r--   0 me        (1000) me        (1000)    19899 2023-05-12 20:23:55.000000 pandasklar-0.3.1/src/pandasklar/aggregate.py
--rw-r--r--   0 me        (1000) me        (1000)    27540 2023-04-11 17:22:24.000000 pandasklar-0.3.1/src/pandasklar/analyse.py
--rw-r--r--   0 me        (1000) me        (1000)    10330 2023-02-12 20:17:03.000000 pandasklar-0.3.1/src/pandasklar/compare.py
--rw-r--r--   0 me        (1000) me        (1000)     1092 2023-02-19 10:51:49.000000 pandasklar-0.3.1/src/pandasklar/config.py
--rw-r--r--   0 me        (1000) me        (1000)    26803 2023-02-20 15:41:11.000000 pandasklar-0.3.1/src/pandasklar/content.py
--rw-r--r--   0 me        (1000) me        (1000)     8710 2023-03-11 11:39:52.000000 pandasklar-0.3.1/src/pandasklar/develop.py
--rw-r--r--   0 me        (1000) me        (1000)    32239 2023-03-16 08:54:51.000000 pandasklar-0.3.1/src/pandasklar/pandas.py
--rw-rw-r--   0 me        (1000) me        (1000)     2613 2023-02-13 21:21:37.000000 pandasklar-0.3.1/src/pandasklar/plot.py
--rw-r--r--   0 me        (1000) me        (1000)     4827 2023-02-08 06:49:03.000000 pandasklar-0.3.1/src/pandasklar/rank.py
--rw-r--r--   0 me        (1000) me        (1000)     8464 2023-02-12 21:40:20.000000 pandasklar-0.3.1/src/pandasklar/scale.py
--rw-r--r--   0 me        (1000) me        (1000)     8975 2023-04-10 20:10:39.000000 pandasklar-0.3.1/src/pandasklar/string.py
--rw-r--r--   0 me        (1000) me        (1000)     8810 2022-11-12 13:55:33.000000 pandasklar-0.3.1/src/pandasklar/subsets.py
--rw-r--r--   0 me        (1000) me        (1000)     5653 2022-11-09 21:26:08.000000 pandasklar-0.3.1/src/pandasklar/type_info.py
--rw-r--r--   0 me        (1000) me        (1000)     5467 2022-11-09 07:00:35.000000 pandasklar-0.3.1/src/pandasklar/values_info.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-31 19:38:45.489691 pandasklar-0.3.1/src/pandasklar.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)     9805 2023-05-31 19:38:45.000000 pandasklar-0.3.1/src/pandasklar.egg-info/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)      677 2023-05-31 19:38:45.000000 pandasklar-0.3.1/src/pandasklar.egg-info/SOURCES.txt
--rw-r--r--   0 me        (1000) me        (1000)        1 2023-05-31 19:38:45.000000 pandasklar-0.3.1/src/pandasklar.egg-info/dependency_links.txt
--rw-r--r--   0 me        (1000) me        (1000)       56 2023-05-31 19:38:45.000000 pandasklar-0.3.1/src/pandasklar.egg-info/entry_points.txt
--rw-r--r--   0 me        (1000) me        (1000)       47 2023-05-31 19:38:45.000000 pandasklar-0.3.1/src/pandasklar.egg-info/requires.txt
--rw-r--r--   0 me        (1000) me        (1000)       11 2023-05-31 19:38:45.000000 pandasklar-0.3.1/src/pandasklar.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 04:42:13.710746 pandasklar-0.3.3/
+-rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 pandasklar-0.3.3/LICENSE
+-rw-rw-r--   0 me        (1000) me        (1000)     9805 2023-06-14 04:42:13.710746 pandasklar-0.3.3/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)     9297 2023-06-14 04:41:46.000000 pandasklar-0.3.3/README.md
+-rw-r--r--   0 me        (1000) me        (1000)     1301 2023-06-14 04:41:35.000000 pandasklar-0.3.3/pyproject.toml
+-rw-rw-r--   0 me        (1000) me        (1000)       38 2023-06-14 04:42:13.710746 pandasklar-0.3.3/setup.cfg
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 04:42:13.706746 pandasklar-0.3.3/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 04:42:13.710746 pandasklar-0.3.3/src/pandasklar/
+-rw-r--r--   0 me        (1000) me        (1000)      537 2023-02-13 16:45:54.000000 pandasklar-0.3.3/src/pandasklar/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)      214 2023-02-14 22:57:35.000000 pandasklar-0.3.3/src/pandasklar/__main__.py
+-rw-r--r--   0 me        (1000) me        (1000)    19899 2023-05-12 20:23:55.000000 pandasklar-0.3.3/src/pandasklar/aggregate.py
+-rw-r--r--   0 me        (1000) me        (1000)    27540 2023-04-11 17:22:24.000000 pandasklar-0.3.3/src/pandasklar/analyse.py
+-rw-r--r--   0 me        (1000) me        (1000)    10330 2023-02-12 20:17:03.000000 pandasklar-0.3.3/src/pandasklar/compare.py
+-rw-r--r--   0 me        (1000) me        (1000)     1092 2023-02-19 10:51:49.000000 pandasklar-0.3.3/src/pandasklar/config.py
+-rw-r--r--   0 me        (1000) me        (1000)    26803 2023-02-20 15:41:11.000000 pandasklar-0.3.3/src/pandasklar/content.py
+-rw-r--r--   0 me        (1000) me        (1000)     8710 2023-03-11 11:39:52.000000 pandasklar-0.3.3/src/pandasklar/develop.py
+-rw-r--r--   0 me        (1000) me        (1000)    32239 2023-03-16 08:54:51.000000 pandasklar-0.3.3/src/pandasklar/pandas.py
+-rw-r--r--   0 me        (1000) me        (1000)     2613 2023-02-13 21:21:37.000000 pandasklar-0.3.3/src/pandasklar/plot.py
+-rw-r--r--   0 me        (1000) me        (1000)     4827 2023-02-08 06:49:03.000000 pandasklar-0.3.3/src/pandasklar/rank.py
+-rw-r--r--   0 me        (1000) me        (1000)     8464 2023-02-12 21:40:20.000000 pandasklar-0.3.3/src/pandasklar/scale.py
+-rw-r--r--   0 me        (1000) me        (1000)     8975 2023-04-10 20:10:39.000000 pandasklar-0.3.3/src/pandasklar/string.py
+-rw-r--r--   0 me        (1000) me        (1000)     8810 2022-11-12 13:55:33.000000 pandasklar-0.3.3/src/pandasklar/subsets.py
+-rw-r--r--   0 me        (1000) me        (1000)     5665 2023-06-09 20:00:34.000000 pandasklar-0.3.3/src/pandasklar/type_info.py
+-rw-r--r--   0 me        (1000) me        (1000)     5467 2022-11-09 07:00:35.000000 pandasklar-0.3.3/src/pandasklar/values_info.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 04:42:13.710746 pandasklar-0.3.3/src/pandasklar.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)     9805 2023-06-14 04:42:13.000000 pandasklar-0.3.3/src/pandasklar.egg-info/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)      677 2023-06-14 04:42:13.000000 pandasklar-0.3.3/src/pandasklar.egg-info/SOURCES.txt
+-rw-r--r--   0 me        (1000) me        (1000)        1 2023-06-14 04:42:13.000000 pandasklar-0.3.3/src/pandasklar.egg-info/dependency_links.txt
+-rw-r--r--   0 me        (1000) me        (1000)       56 2023-06-14 04:42:13.000000 pandasklar-0.3.3/src/pandasklar.egg-info/entry_points.txt
+-rw-r--r--   0 me        (1000) me        (1000)       47 2023-06-14 04:42:13.000000 pandasklar-0.3.3/src/pandasklar.egg-info/requires.txt
+-rw-r--r--   0 me        (1000) me        (1000)       11 2023-06-14 04:42:13.000000 pandasklar-0.3.3/src/pandasklar.egg-info/top_level.txt
```

### Comparing `pandasklar-0.3.1/LICENSE` & `pandasklar-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.1/PKG-INFO` & `pandasklar-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasklar
-Version: 0.3.1
+Version: 0.3.3
 Summary: Toolbox / Ecosystem for data science. Easier handling of pandas, especially when thinking in SQL.
 Author-email: djekra <hopsalla@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/djekra/pandasklar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pandasklar-0.3.1/README.md` & `pandasklar-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.1/pyproject.toml` & `pandasklar-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pyproject.toml
 
 
 [project]
 name            = "pandasklar"
-version         = "0.3.1"    
+version         = "0.3.3"    
 
 requires-python = ">=3.8"
 dependencies    = ['pandas','numpy','perlin_noise','termcolor','bpyth','blab',]
 
 authors        = [{ name = "djekra", email = "hopsalla@gmail.com" }]
 description     = "Toolbox / Ecosystem for data science. Easier handling of pandas, especially when thinking in SQL."
 readme          = "README.md"
```

### Comparing `pandasklar-0.3.1/src/pandasklar/__init__.py` & `pandasklar-0.3.3/src/pandasklar/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.1/src/pandasklar/aggregate.py` & `pandasklar-0.3.3/src/pandasklar/aggregate.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.1/src/pandasklar/analyse.py` & `pandasklar-0.3.3/src/pandasklar/analyse.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.1/src/pandasklar/compare.py` & `pandasklar-0.3.3/src/pandasklar/compare.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.1/src/pandasklar/config.py` & `pandasklar-0.3.3/src/pandasklar/config.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.1/src/pandasklar/content.py` & `pandasklar-0.3.3/src/pandasklar/content.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.1/src/pandasklar/develop.py` & `pandasklar-0.3.3/src/pandasklar/develop.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.1/src/pandasklar/pandas.py` & `pandasklar-0.3.3/src/pandasklar/pandas.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.1/src/pandasklar/plot.py` & `pandasklar-0.3.3/src/pandasklar/plot.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.1/src/pandasklar/rank.py` & `pandasklar-0.3.3/src/pandasklar/rank.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.1/src/pandasklar/scale.py` & `pandasklar-0.3.3/src/pandasklar/scale.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.1/src/pandasklar/string.py` & `pandasklar-0.3.3/src/pandasklar/string.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.1/src/pandasklar/subsets.py` & `pandasklar-0.3.3/src/pandasklar/subsets.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.1/src/pandasklar/type_info.py` & `pandasklar-0.3.3/src/pandasklar/type_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-import collections, warnings
+import collections.abc, warnings
 
 import numpy  as np
 import pandas as pd
 
 from .config    import Config
 from .pandas    import first_valid_value, last_valid_value
 
@@ -67,15 +67,15 @@
             else: 
                 self.name_instance = 'mix'
                 
         # is_hashable
         if self.name_instance == 'mix':
             self.is_hashable = False    
         else:
-            self.is_hashable = isinstance(self.instance1, collections.Hashable)  and  isinstance(self.instance2, collections.Hashable)
+            self.is_hashable = isinstance(self.instance1, collections.abc.Hashable)  and  isinstance(self.instance2, collections.abc.Hashable)
             
         # name_short
         if '.' in search:
             self.name_short = search.split('.')[-1]
         self.name_short = self.name_short.replace("<class '","").replace("'>","").replace("numpy.","").replace("Dtype","")
```

### Comparing `pandasklar-0.3.1/src/pandasklar/values_info.py` & `pandasklar-0.3.3/src/pandasklar/values_info.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.1/src/pandasklar.egg-info/PKG-INFO` & `pandasklar-0.3.3/src/pandasklar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasklar
-Version: 0.3.1
+Version: 0.3.3
 Summary: Toolbox / Ecosystem for data science. Easier handling of pandas, especially when thinking in SQL.
 Author-email: djekra <hopsalla@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/djekra/pandasklar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pandasklar-0.3.1/src/pandasklar.egg-info/SOURCES.txt` & `pandasklar-0.3.3/src/pandasklar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

