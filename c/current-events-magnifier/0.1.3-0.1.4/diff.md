# Comparing `tmp/current_events_magnifier-0.1.3.tar.gz` & `tmp/current_events_magnifier-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/current_events_magnifier-0.1.3.tar", last modified: Wed Jun 14 09:23:04 2023, max compression
+gzip compressed data, was "dist/current_events_magnifier-0.1.4.tar", last modified: Wed Jun 14 09:26:23 2023, max compression
```

## Comparing `current_events_magnifier-0.1.3.tar` & `current_events_magnifier-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 09:23:04.060936 current_events_magnifier-0.1.3/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6044 2023-06-14 09:23:04.060936 current_events_magnifier-0.1.3/PKG-INFO
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 09:23:04.060936 current_events_magnifier-0.1.3/current_events_magnifier.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6044 2023-06-14 09:23:04.000000 current_events_magnifier-0.1.3/current_events_magnifier.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      275 2023-06-14 09:23:04.000000 current_events_magnifier-0.1.3/current_events_magnifier.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 09:23:04.000000 current_events_magnifier-0.1.3/current_events_magnifier.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       69 2023-06-14 09:23:04.000000 current_events_magnifier-0.1.3/current_events_magnifier.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 09:23:04.000000 current_events_magnifier-0.1.3/current_events_magnifier.egg-info/top_level.txt
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     5760 2023-06-14 09:21:54.000000 current_events_magnifier-0.1.3/current_events_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-14 09:23:04.060936 current_events_magnifier-0.1.3/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1032 2023-06-14 09:22:55.000000 current_events_magnifier-0.1.3/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 09:26:23.182361 current_events_magnifier-0.1.4/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6044 2023-06-14 09:26:23.182361 current_events_magnifier-0.1.4/PKG-INFO
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 09:26:23.182361 current_events_magnifier-0.1.4/current_events_magnifier.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6044 2023-06-14 09:26:23.000000 current_events_magnifier-0.1.4/current_events_magnifier.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      275 2023-06-14 09:26:23.000000 current_events_magnifier-0.1.4/current_events_magnifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 09:26:23.000000 current_events_magnifier-0.1.4/current_events_magnifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       69 2023-06-14 09:26:23.000000 current_events_magnifier-0.1.4/current_events_magnifier.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 09:26:23.000000 current_events_magnifier-0.1.4/current_events_magnifier.egg-info/top_level.txt
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     5760 2023-06-14 09:21:54.000000 current_events_magnifier-0.1.4/current_events_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-14 09:26:23.182361 current_events_magnifier-0.1.4/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1032 2023-06-14 09:26:21.000000 current_events_magnifier-0.1.4/setup.py
```

### Comparing `current_events_magnifier-0.1.3/PKG-INFO` & `current_events_magnifier-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current_events_magnifier
-Version: 0.1.3
+Version: 0.1.4
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.1.3/current_events_magnifier.egg-info/PKG-INFO` & `current_events_magnifier-0.1.4/current_events_magnifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current-events-magnifier
-Version: 0.1.3
+Version: 0.1.4
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.1.3/current_events_magnifier.py` & `current_events_magnifier-0.1.4/current_events_magnifier.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.1.3/setup.py` & `current_events_magnifier-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("../README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="current_events_magnifier",
-    version="0.1.3",
+    version="0.1.4",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
```

