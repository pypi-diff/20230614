# Comparing `tmp/current_events_magnifier-0.1.0.tar.gz` & `tmp/current_events_magnifier-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/current_events_magnifier-0.1.0.tar", last modified: Wed Jun 14 08:59:40 2023, max compression
+gzip compressed data, was "dist/current_events_magnifier-0.1.1.tar", last modified: Wed Jun 14 09:06:23 2023, max compression
```

## Comparing `current_events_magnifier-0.1.0.tar` & `current_events_magnifier-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 08:59:40.558520 current_events_magnifier-0.1.0/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.1.0/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6066 2023-06-14 08:59:40.558520 current_events_magnifier-0.1.0/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5456 2023-06-14 08:59:36.000000 current_events_magnifier-0.1.0/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 08:59:40.558520 current_events_magnifier-0.1.0/current_events_magnifier.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6066 2023-06-14 08:59:40.000000 current_events_magnifier-0.1.0/current_events_magnifier.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      265 2023-06-14 08:59:40.000000 current_events_magnifier-0.1.0/current_events_magnifier.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 08:59:40.000000 current_events_magnifier-0.1.0/current_events_magnifier.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       69 2023-06-14 08:59:40.000000 current_events_magnifier-0.1.0/current_events_magnifier.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 08:59:40.000000 current_events_magnifier-0.1.0/current_events_magnifier.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-14 08:59:40.558520 current_events_magnifier-0.1.0/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      984 2023-06-14 08:52:28.000000 current_events_magnifier-0.1.0/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 09:06:23.937013 current_events_magnifier-0.1.1/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.1.1/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6066 2023-06-14 09:06:23.937013 current_events_magnifier-0.1.1/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5456 2023-06-14 08:59:36.000000 current_events_magnifier-0.1.1/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 09:06:23.937013 current_events_magnifier-0.1.1/current_events_magnifier.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6066 2023-06-14 09:06:23.000000 current_events_magnifier-0.1.1/current_events_magnifier.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      265 2023-06-14 09:06:23.000000 current_events_magnifier-0.1.1/current_events_magnifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 09:06:23.000000 current_events_magnifier-0.1.1/current_events_magnifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       69 2023-06-14 09:06:23.000000 current_events_magnifier-0.1.1/current_events_magnifier.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 09:06:23.000000 current_events_magnifier-0.1.1/current_events_magnifier.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-14 09:06:23.937013 current_events_magnifier-0.1.1/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      984 2023-06-14 09:05:46.000000 current_events_magnifier-0.1.1/setup.py
```

### Comparing `current_events_magnifier-0.1.0/LICENSE` & `current_events_magnifier-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.1.0/PKG-INFO` & `current_events_magnifier-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current_events_magnifier
-Version: 0.1.0
+Version: 0.1.1
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.1.0/README.md` & `current_events_magnifier-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.1.0/current_events_magnifier.egg-info/PKG-INFO` & `current_events_magnifier-0.1.1/current_events_magnifier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current-events-magnifier
-Version: 0.1.0
+Version: 0.1.1
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.1.0/setup.py` & `current_events_magnifier-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="current_events_magnifier",
-    version="0.1.0",
+    version="0.1.1",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
```

