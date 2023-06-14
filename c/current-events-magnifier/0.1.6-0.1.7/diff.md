# Comparing `tmp/current_events_magnifier-0.1.6.tar.gz` & `tmp/current_events_magnifier-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/current_events_magnifier-0.1.6.tar", last modified: Wed Jun 14 09:36:29 2023, max compression
+gzip compressed data, was "dist/current_events_magnifier-0.1.7.tar", last modified: Wed Jun 14 09:38:02 2023, max compression
```

## Comparing `current_events_magnifier-0.1.6.tar` & `current_events_magnifier-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 09:36:29.363047 current_events_magnifier-0.1.6/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6044 2023-06-14 09:36:29.363047 current_events_magnifier-0.1.6/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5456 2023-06-14 08:59:36.000000 current_events_magnifier-0.1.6/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 09:36:29.363047 current_events_magnifier-0.1.6/current_events_magnifier.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6044 2023-06-14 09:36:29.000000 current_events_magnifier-0.1.6/current_events_magnifier.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      285 2023-06-14 09:36:29.000000 current_events_magnifier-0.1.6/current_events_magnifier.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 09:36:29.000000 current_events_magnifier-0.1.6/current_events_magnifier.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       69 2023-06-14 09:36:29.000000 current_events_magnifier-0.1.6/current_events_magnifier.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 09:36:29.000000 current_events_magnifier-0.1.6/current_events_magnifier.egg-info/top_level.txt
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     5760 2023-06-14 09:21:54.000000 current_events_magnifier-0.1.6/current_events_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-14 09:36:29.363047 current_events_magnifier-0.1.6/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1137 2023-06-14 09:36:16.000000 current_events_magnifier-0.1.6/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 09:38:02.437392 current_events_magnifier-0.1.7/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6044 2023-06-14 09:38:02.437392 current_events_magnifier-0.1.7/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5456 2023-06-14 08:59:36.000000 current_events_magnifier-0.1.7/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 09:38:02.437392 current_events_magnifier-0.1.7/current_events_magnifier.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6044 2023-06-14 09:38:02.000000 current_events_magnifier-0.1.7/current_events_magnifier.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      285 2023-06-14 09:38:02.000000 current_events_magnifier-0.1.7/current_events_magnifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 09:38:02.000000 current_events_magnifier-0.1.7/current_events_magnifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       69 2023-06-14 09:38:02.000000 current_events_magnifier-0.1.7/current_events_magnifier.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 09:38:02.000000 current_events_magnifier-0.1.7/current_events_magnifier.egg-info/top_level.txt
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     5760 2023-06-14 09:21:54.000000 current_events_magnifier-0.1.7/current_events_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-14 09:38:02.437392 current_events_magnifier-0.1.7/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1145 2023-06-14 09:38:01.000000 current_events_magnifier-0.1.7/setup.py
```

### Comparing `current_events_magnifier-0.1.6/PKG-INFO` & `current_events_magnifier-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current_events_magnifier
-Version: 0.1.6
+Version: 0.1.7
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.1.6/README.md` & `current_events_magnifier-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.1.6/current_events_magnifier.egg-info/PKG-INFO` & `current_events_magnifier-0.1.7/current_events_magnifier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current-events-magnifier
-Version: 0.1.6
+Version: 0.1.7
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.1.6/current_events_magnifier.py` & `current_events_magnifier-0.1.7/current_events_magnifier.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.1.6/setup.py` & `current_events_magnifier-0.1.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="current_events_magnifier",
-    version="0.1.6",
+    version="0.1.7",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
-    packages=find_packages(['cm_utils','normalization','plot','read_f5c_resquiggle','read_tombo_reqsuiggle','current_events_magnifier']),
+    packages=find_packages(include=['cm_utils','normalization','plot','read_f5c_resquiggle','read_tombo_reqsuiggle','current_events_magnifier']),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
     install_requires=[
```

