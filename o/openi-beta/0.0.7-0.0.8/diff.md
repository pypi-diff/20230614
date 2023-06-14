# Comparing `tmp/openi-beta-0.0.7.tar.gz` & `tmp/openi-beta-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-0.0.7.tar", last modified: Thu Jun  8 09:49:37 2023, max compression
+gzip compressed data, was "openi-beta-0.0.8.tar", last modified: Wed Jun 14 08:24:28 2023, max compression
```

## Comparing `openi-beta-0.0.7.tar` & `openi-beta-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 09:49:37.681008 openi-beta-0.0.7/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2103 2023-06-08 09:49:37.680873 openi-beta-0.0.7/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-08 09:39:38.000000 openi-beta-0.0.7/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-08 09:49:37.681073 openi-beta-0.0.7/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)      976 2023-06-08 09:49:30.000000 openi-beta-0.0.7/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 09:49:37.678171 openi-beta-0.0.7/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 09:49:37.678916 openi-beta-0.0.7/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-08 08:37:15.000000 openi-beta-0.0.7/src/openi/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      290 2023-06-08 08:37:15.000000 openi-beta-0.0.7/src/openi/constants.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 09:49:37.679490 openi-beta-0.0.7/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-05-30 08:31:28.000000 openi-beta-0.0.7/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     9661 2023-06-08 09:32:01.000000 openi-beta-0.0.7/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 09:49:37.680646 openi-beta-0.0.7/src/openi_beta.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2103 2023-06-08 09:49:37.000000 openi-beta-0.0.7/src/openi_beta.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      311 2023-06-08 09:49:37.000000 openi-beta-0.0.7/src/openi_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-08 09:49:37.000000 openi-beta-0.0.7/src/openi_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-08 09:49:37.000000 openi-beta-0.0.7/src/openi_beta.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-08 09:49:37.000000 openi-beta-0.0.7/src/openi_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-14 08:24:28.338122 openi-beta-0.0.8/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-14 08:24:28.337989 openi-beta-0.0.8/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-14 08:18:21.000000 openi-beta-0.0.8/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-14 08:24:28.338165 openi-beta-0.0.8/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)      910 2023-06-14 08:23:10.000000 openi-beta-0.0.8/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-14 08:24:28.335952 openi-beta-0.0.8/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-14 08:24:28.336624 openi-beta-0.0.8/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-14 08:18:21.000000 openi-beta-0.0.8/src/openi/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      290 2023-06-14 08:18:21.000000 openi-beta-0.0.8/src/openi/constants.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-14 08:24:28.337091 openi-beta-0.0.8/src/openi/dataset/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-05-30 08:31:28.000000 openi-beta-0.0.8/src/openi/dataset/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     9661 2023-06-14 08:22:19.000000 openi-beta-0.0.8/src/openi/dataset/dataset.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-14 08:24:28.337792 openi-beta-0.0.8/src/openi_beta.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-14 08:24:28.000000 openi-beta-0.0.8/src/openi_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      311 2023-06-14 08:24:28.000000 openi-beta-0.0.8/src/openi_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-14 08:24:28.000000 openi-beta-0.0.8/src/openi_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-14 08:24:28.000000 openi-beta-0.0.8/src/openi_beta.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-14 08:24:28.000000 openi-beta-0.0.8/src/openi_beta.egg-info/top_level.txt
```

### Comparing `openi-beta-0.0.7/PKG-INFO` & `openi-beta-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.0.7
-Summary: A test packages for openi pypi
+Version: 0.0.8
+Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `openi-beta-0.0.7/README.md` & `openi-beta-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `openi-beta-0.0.7/setup.py` & `openi-beta-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-# python setup.py sdist bdist_wheel  
-# twine upload dist/*    
-
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='openi-beta',
-    version='0.0.7',
-    description='A test packages for openi pypi',
+    version='0.0.8',
+    description='A test package for openi pypi',
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi',
     author='chenzh05',
     author_email='chenzh.ds@outlook.com',
     license='MIT',
```

### Comparing `openi-beta-0.0.7/src/openi/dataset/dataset.py` & `openi-beta-0.0.8/src/openi/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `openi-beta-0.0.7/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-0.0.8/src/openi_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.0.7
-Summary: A test packages for openi pypi
+Version: 0.0.8
+Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

