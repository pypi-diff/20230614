# Comparing `tmp/UAutoml-0.0.3.tar.gz` & `tmp/UAutoml-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UAutoml-0.0.3.tar", last modified: Tue Jun 13 16:56:27 2023, max compression
+gzip compressed data, was "UAutoml-0.0.4.tar", last modified: Wed Jun 14 07:26:49 2023, max compression
```

## Comparing `UAutoml-0.0.3.tar` & `UAutoml-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-13 16:56:27.188339 UAutoml-0.0.3/
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1073 2023-06-13 15:50:26.000000 UAutoml-0.0.3/LICENSE.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     2227 2023-06-13 16:56:27.187501 UAutoml-0.0.3/PKG-INFO
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1678 2023-06-13 16:55:19.000000 UAutoml-0.0.3/README.md
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)       38 2023-06-13 16:56:27.188581 UAutoml-0.0.3/setup.cfg
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      880 2023-06-13 16:55:52.000000 UAutoml-0.0.3/setup.py
-drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-13 16:56:27.182656 UAutoml-0.0.3/src/
-drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-13 16:56:27.186418 UAutoml-0.0.3/src/UAutoml.egg-info/
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     2227 2023-06-13 16:56:27.000000 UAutoml-0.0.3/src/UAutoml.egg-info/PKG-INFO
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      219 2023-06-13 16:56:27.000000 UAutoml-0.0.3/src/UAutoml.egg-info/SOURCES.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)        1 2023-06-13 16:56:27.000000 UAutoml-0.0.3/src/UAutoml.egg-info/dependency_links.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)       19 2023-06-13 16:56:27.000000 UAutoml-0.0.3/src/UAutoml.egg-info/requires.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)        8 2023-06-13 16:56:27.000000 UAutoml-0.0.3/src/UAutoml.egg-info/top_level.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)    12183 2023-06-13 15:32:30.000000 UAutoml-0.0.3/src/UAutoml.py
+drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-14 07:26:49.077822 UAutoml-0.0.4/
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1073 2023-06-13 15:50:26.000000 UAutoml-0.0.4/LICENSE.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     2227 2023-06-14 07:26:49.077012 UAutoml-0.0.4/PKG-INFO
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1678 2023-06-13 16:55:19.000000 UAutoml-0.0.4/README.md
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)       38 2023-06-14 07:26:49.078112 UAutoml-0.0.4/setup.cfg
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      880 2023-06-14 07:26:34.000000 UAutoml-0.0.4/setup.py
+drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-14 07:26:49.071817 UAutoml-0.0.4/src/
+drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-14 07:26:49.076055 UAutoml-0.0.4/src/UAutoml.egg-info/
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     2227 2023-06-14 07:26:48.000000 UAutoml-0.0.4/src/UAutoml.egg-info/PKG-INFO
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      219 2023-06-14 07:26:48.000000 UAutoml-0.0.4/src/UAutoml.egg-info/SOURCES.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)        1 2023-06-14 07:26:48.000000 UAutoml-0.0.4/src/UAutoml.egg-info/dependency_links.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)       19 2023-06-14 07:26:48.000000 UAutoml-0.0.4/src/UAutoml.egg-info/requires.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)        8 2023-06-14 07:26:48.000000 UAutoml-0.0.4/src/UAutoml.egg-info/top_level.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)    12183 2023-06-13 15:32:30.000000 UAutoml-0.0.4/src/UAutoml.py
```

### Comparing `UAutoml-0.0.3/LICENSE.txt` & `UAutoml-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `UAutoml-0.0.3/PKG-INFO` & `UAutoml-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: UAutoml
-Version: 0.0.3
-Summary: Automated Machine Learning Framework for Data Analysisr
+Version: 0.0.4
+Summary: Automated Machine Learning Framework for Data Analysis.
 Home-page: https://github.com/ujjwalredd/Automated-Machine-Learning-Framework-for-Data-Analysis
 Author: Ujjwal Reddy K S
 License: UNKNOWN
 Keywords: ML,Auto Data Analysis,models
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `UAutoml-0.0.3/README.md` & `UAutoml-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `UAutoml-0.0.3/setup.py` & `UAutoml-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='UAutoml',
-    version='0.0.3',
-    description='Automated Machine Learning Framework for Data Analysisr',
+    version='0.0.4',
+    description='Automated Machine Learning Framework for Data Analysis.',
     author= 'Ujjwal Reddy K S',
     url = 'https://github.com/ujjwalredd/Automated-Machine-Learning-Framework-for-Data-Analysis',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     keywords=['ML', 'Auto Data Analysis', 'models'],
     classifiers=[
```

### Comparing `UAutoml-0.0.3/src/UAutoml.egg-info/PKG-INFO` & `UAutoml-0.0.4/src/UAutoml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: UAutoml
-Version: 0.0.3
-Summary: Automated Machine Learning Framework for Data Analysisr
+Version: 0.0.4
+Summary: Automated Machine Learning Framework for Data Analysis.
 Home-page: https://github.com/ujjwalredd/Automated-Machine-Learning-Framework-for-Data-Analysis
 Author: Ujjwal Reddy K S
 License: UNKNOWN
 Keywords: ML,Auto Data Analysis,models
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `UAutoml-0.0.3/src/UAutoml.py` & `UAutoml-0.0.4/src/UAutoml.py`

 * *Files identical despite different names*

