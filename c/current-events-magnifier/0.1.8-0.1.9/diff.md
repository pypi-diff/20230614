# Comparing `tmp/current_events_magnifier-0.1.8.tar.gz` & `tmp/current_events_magnifier-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "current_events_magnifier-0.1.8.tar", last modified: Wed Jun 14 10:41:03 2023, max compression
+gzip compressed data, was "dist/current_events_magnifier-0.1.9.tar", last modified: Wed Jun 14 10:43:42 2023, max compression
```

## Comparing `current_events_magnifier-0.1.8.tar` & `current_events_magnifier-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 10:41:03.550828 current_events_magnifier-0.1.8/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.1.8/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6103 2023-06-14 10:41:03.550828 current_events_magnifier-0.1.8/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5456 2023-06-14 08:59:36.000000 current_events_magnifier-0.1.8/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 10:41:03.550828 current_events_magnifier-0.1.8/current_events_magnifier.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6103 2023-06-14 10:41:03.000000 current_events_magnifier-0.1.8/current_events_magnifier.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      418 2023-06-14 10:41:03.000000 current_events_magnifier-0.1.8/current_events_magnifier.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 10:41:03.000000 current_events_magnifier-0.1.8/current_events_magnifier.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       69 2023-06-14 10:41:03.000000 current_events_magnifier-0.1.8/current_events_magnifier.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        4 2023-06-14 10:41:03.000000 current_events_magnifier-0.1.8/current_events_magnifier.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-14 10:41:03.550828 current_events_magnifier-0.1.8/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1029 2023-06-14 10:39:17.000000 current_events_magnifier-0.1.8/setup.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 10:41:03.550828 current_events_magnifier-0.1.8/src/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       74 2023-06-14 10:40:40.000000 current_events_magnifier-0.1.8/src/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.1.8/src/cm_utils.py
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     5760 2023-06-14 09:21:54.000000 current_events_magnifier-0.1.8/src/current_events_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.1.8/src/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7487 2023-06-14 08:32:18.000000 current_events_magnifier-0.1.8/src/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9117 2023-06-14 05:39:22.000000 current_events_magnifier-0.1.8/src/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13350 2023-06-14 09:18:43.000000 current_events_magnifier-0.1.8/src/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 10:43:42.612044 current_events_magnifier-0.1.9/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.1.9/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6066 2023-06-14 10:43:42.612044 current_events_magnifier-0.1.9/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5456 2023-06-14 08:59:36.000000 current_events_magnifier-0.1.9/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 10:43:42.612044 current_events_magnifier-0.1.9/current_events_magnifier/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       95 2023-06-14 10:43:38.000000 current_events_magnifier-0.1.9/current_events_magnifier/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.1.9/current_events_magnifier/cm_utils.py
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     5760 2023-06-14 09:21:54.000000 current_events_magnifier-0.1.9/current_events_magnifier/current_events_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.1.9/current_events_magnifier/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7487 2023-06-14 08:32:18.000000 current_events_magnifier-0.1.9/current_events_magnifier/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9117 2023-06-14 05:39:22.000000 current_events_magnifier-0.1.9/current_events_magnifier/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13350 2023-06-14 09:18:43.000000 current_events_magnifier-0.1.9/current_events_magnifier/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 10:43:42.612044 current_events_magnifier-0.1.9/current_events_magnifier.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6066 2023-06-14 10:43:42.000000 current_events_magnifier-0.1.9/current_events_magnifier.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      565 2023-06-14 10:43:42.000000 current_events_magnifier-0.1.9/current_events_magnifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 10:43:42.000000 current_events_magnifier-0.1.9/current_events_magnifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       69 2023-06-14 10:43:42.000000 current_events_magnifier-0.1.9/current_events_magnifier.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-14 10:43:42.000000 current_events_magnifier-0.1.9/current_events_magnifier.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-14 10:43:42.612044 current_events_magnifier-0.1.9/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1054 2023-06-14 10:43:38.000000 current_events_magnifier-0.1.9/setup.py
```

### Comparing `current_events_magnifier-0.1.8/LICENSE` & `current_events_magnifier-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.1.8/PKG-INFO` & `current_events_magnifier-0.1.9/current_events_magnifier.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
-Name: current_events_magnifier
-Version: 0.1.8
+Name: current-events-magnifier
+Version: 0.1.9
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -126,9 +124,7 @@
 
 ```
 
 
 
 
 
-
-
```

### Comparing `current_events_magnifier-0.1.8/README.md` & `current_events_magnifier-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.1.8/current_events_magnifier.egg-info/PKG-INFO` & `current_events_magnifier-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
-Name: current-events-magnifier
-Version: 0.1.8
+Name: current_events_magnifier
+Version: 0.1.9
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -126,9 +124,7 @@
 
 ```
 
 
 
 
 
-
-
```

### Comparing `current_events_magnifier-0.1.8/setup.py` & `current_events_magnifier-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="current_events_magnifier",
-    version="0.1.8",
+    version="0.1.9",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
@@ -23,9 +23,9 @@
     install_requires=[
         'h5py==3.8.0',
         'numpy>=1.21.6',
         'pandas>=1.1.5',
         'plotnine>=0.8.0',
         'tqdm>=4.62.0',
     ],
-    scripts=['current_events_magnifier.py']
+    scripts=['current_events_magnifier/current_events_magnifier.py']
 )
```

### Comparing `current_events_magnifier-0.1.8/src/cm_utils.py` & `current_events_magnifier-0.1.9/current_events_magnifier/cm_utils.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.1.8/src/current_events_magnifier.py` & `current_events_magnifier-0.1.9/current_events_magnifier/current_events_magnifier.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.1.8/src/normalization.py` & `current_events_magnifier-0.1.9/current_events_magnifier/normalization.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.1.8/src/plot.py` & `current_events_magnifier-0.1.9/current_events_magnifier/plot.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.1.8/src/read_f5c_resquiggle.py` & `current_events_magnifier-0.1.9/current_events_magnifier/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.1.8/src/read_tombo_resquiggle.py` & `current_events_magnifier-0.1.9/current_events_magnifier/read_tombo_resquiggle.py`

 * *Files identical despite different names*

