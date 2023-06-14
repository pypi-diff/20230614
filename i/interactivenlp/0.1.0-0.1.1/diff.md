# Comparing `tmp/interactivenlp-0.1.0.tar.gz` & `tmp/interactivenlp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactivenlp-0.1.0.tar", last modified: Wed Jun 14 20:37:56 2023, max compression
+gzip compressed data, was "interactivenlp-0.1.1.tar", last modified: Wed Jun 14 20:49:06 2023, max compression
```

## Comparing `interactivenlp-0.1.0.tar` & `interactivenlp-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 20:37:56.457948 interactivenlp-0.1.0/
--rw-rw-rw-   0        0        0     1093 2023-06-14 20:18:06.000000 interactivenlp-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      358 2023-06-14 20:37:56.456944 interactivenlp-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-05-18 19:26:55.000000 interactivenlp-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-14 20:37:56.436398 interactivenlp-0.1.0/interactivenlp/
--rw-rw-rw-   0        0        0      211 2023-05-18 20:43:07.000000 interactivenlp-0.1.0/interactivenlp/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-06-14 20:34:18.000000 interactivenlp-0.1.0/interactivenlp/server.py
--rw-rw-rw-   0        0        0     2184 2023-06-14 20:33:38.000000 interactivenlp-0.1.0/interactivenlp/types.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:37:56.456009 interactivenlp-0.1.0/interactivenlp.egg-info/
--rw-rw-rw-   0        0        0      358 2023-06-14 20:37:56.000000 interactivenlp-0.1.0/interactivenlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-06-14 20:37:56.000000 interactivenlp-0.1.0/interactivenlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 20:37:56.000000 interactivenlp-0.1.0/interactivenlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-14 20:37:56.000000 interactivenlp-0.1.0/interactivenlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-14 20:37:56.000000 interactivenlp-0.1.0/interactivenlp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 20:37:56.457948 interactivenlp-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      616 2023-06-14 20:36:16.000000 interactivenlp-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:49:06.316816 interactivenlp-0.1.1/
+-rw-rw-rw-   0        0        0     1093 2023-06-14 20:18:06.000000 interactivenlp-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      358 2023-06-14 20:49:06.308065 interactivenlp-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-05-18 19:26:55.000000 interactivenlp-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-14 20:49:06.292070 interactivenlp-0.1.1/interactivenlp/
+-rw-rw-rw-   0        0        0      273 2023-06-14 20:47:39.000000 interactivenlp-0.1.1/interactivenlp/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-06-14 20:34:18.000000 interactivenlp-0.1.1/interactivenlp/server.py
+-rw-rw-rw-   0        0        0     2186 2023-06-14 20:48:39.000000 interactivenlp-0.1.1/interactivenlp/types.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:49:06.307066 interactivenlp-0.1.1/interactivenlp.egg-info/
+-rw-rw-rw-   0        0        0      358 2023-06-14 20:49:06.000000 interactivenlp-0.1.1/interactivenlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-06-14 20:49:06.000000 interactivenlp-0.1.1/interactivenlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 20:49:06.000000 interactivenlp-0.1.1/interactivenlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-14 20:49:06.000000 interactivenlp-0.1.1/interactivenlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-14 20:49:06.000000 interactivenlp-0.1.1/interactivenlp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 20:49:06.317341 interactivenlp-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      616 2023-06-14 20:49:03.000000 interactivenlp-0.1.1/setup.py
```

### Comparing `interactivenlp-0.1.0/LICENSE` & `interactivenlp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.1.0/interactivenlp/server.py` & `interactivenlp-0.1.1/interactivenlp/server.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.1.0/interactivenlp/types.py` & `interactivenlp-0.1.1/interactivenlp/types.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -71,8 +71,8 @@
         self.functions = functions
 
     def __dict__(self):
         return {
             "name": self.name,
             "description": self.description,
             "functions": [function.__dict__() for function in self.functions]
-        }
+        }
```

### Comparing `interactivenlp-0.1.0/setup.py` & `interactivenlp-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open('README.rst', "r") as f:
     long_description = f.read()
 
 setup(
     name='interactivenlp',
-    version='0.1.0',
+    version='0.1.1',
     description='Interactive NLP',
     long_description=long_description,
     author="Chunxu Yang",
     author_email="chunxuyang@ucla.edu",
     install_requires=[
         'flask',
         'flask-cors',
```

