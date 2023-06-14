# Comparing `tmp/charred-0.1.1.tar.gz` & `tmp/charred-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charred-0.1.1.tar", last modified: Wed Jun 14 14:22:03 2023, max compression
+gzip compressed data, was "charred-0.1.11.tar", last modified: Wed Jun 14 14:32:27 2023, max compression
```

## Comparing `charred-0.1.1.tar` & `charred-0.1.11.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxr-x   0 endormi   (1000) endormi   (1000)        0 2023-06-14 14:22:03.724125 charred-0.1.1/
--rw-rw-r--   0 endormi   (1000) endormi   (1000)     1064 2023-06-06 17:20:02.000000 charred-0.1.1/LICENSE
--rw-rw-r--   0 endormi   (1000) endormi   (1000)       26 2023-06-06 16:39:17.000000 charred-0.1.1/MANIFEST.in
--rw-rw-r--   0 endormi   (1000) endormi   (1000)     1356 2023-06-14 14:22:03.724125 charred-0.1.1/PKG-INFO
--rw-rw-r--   0 endormi   (1000) endormi   (1000)      584 2023-06-14 13:18:53.000000 charred-0.1.1/README.md
-drwxrwxr-x   0 endormi   (1000) endormi   (1000)        0 2023-06-14 14:22:03.724125 charred-0.1.1/charred.egg-info/
--rw-rw-r--   0 endormi   (1000) endormi   (1000)     1356 2023-06-14 14:22:03.000000 charred-0.1.1/charred.egg-info/PKG-INFO
--rw-rw-r--   0 endormi   (1000) endormi   (1000)      199 2023-06-14 14:22:03.000000 charred-0.1.1/charred.egg-info/SOURCES.txt
--rw-rw-r--   0 endormi   (1000) endormi   (1000)        1 2023-06-14 14:22:03.000000 charred-0.1.1/charred.egg-info/dependency_links.txt
--rw-rw-r--   0 endormi   (1000) endormi   (1000)        6 2023-06-14 14:22:03.000000 charred-0.1.1/charred.egg-info/top_level.txt
--rw-rw-r--   0 endormi   (1000) endormi   (1000)       38 2023-06-14 14:22:03.724125 charred-0.1.1/setup.cfg
--rw-rw-r--   0 endormi   (1000) endormi   (1000)      628 2023-06-14 14:21:57.000000 charred-0.1.1/setup.py
-drwxrwxr-x   0 endormi   (1000) endormi   (1000)        0 2023-06-14 14:22:03.724125 charred-0.1.1/tests/
--rw-rw-r--   0 endormi   (1000) endormi   (1000)        0 2023-06-06 17:05:07.000000 charred-0.1.1/tests/__init__.py
--rw-rw-r--   0 endormi   (1000) endormi   (1000)      824 2023-06-14 13:21:21.000000 charred-0.1.1/tests/test_char.py
+drwxrwxr-x   0 endormi   (1000) endormi   (1000)        0 2023-06-14 14:32:27.348657 charred-0.1.11/
+-rw-rw-r--   0 endormi   (1000) endormi   (1000)     1064 2023-06-06 17:20:02.000000 charred-0.1.11/LICENSE
+-rw-rw-r--   0 endormi   (1000) endormi   (1000)       26 2023-06-06 16:39:17.000000 charred-0.1.11/MANIFEST.in
+-rw-rw-r--   0 endormi   (1000) endormi   (1000)     1357 2023-06-14 14:32:27.348657 charred-0.1.11/PKG-INFO
+-rw-rw-r--   0 endormi   (1000) endormi   (1000)      584 2023-06-14 13:18:53.000000 charred-0.1.11/README.md
+drwxrwxr-x   0 endormi   (1000) endormi   (1000)        0 2023-06-14 14:32:27.348657 charred-0.1.11/charred/
+-rw-rw-r--   0 endormi   (1000) endormi   (1000)       90 2023-06-14 14:27:15.000000 charred-0.1.11/charred/__init__.py
+-rw-rw-r--   0 endormi   (1000) endormi   (1000)      740 2023-06-14 14:32:19.000000 charred-0.1.11/charred/charred.py
+drwxrwxr-x   0 endormi   (1000) endormi   (1000)        0 2023-06-14 14:32:27.348657 charred-0.1.11/charred.egg-info/
+-rw-rw-r--   0 endormi   (1000) endormi   (1000)     1357 2023-06-14 14:32:27.000000 charred-0.1.11/charred.egg-info/PKG-INFO
+-rw-rw-r--   0 endormi   (1000) endormi   (1000)      238 2023-06-14 14:32:27.000000 charred-0.1.11/charred.egg-info/SOURCES.txt
+-rw-rw-r--   0 endormi   (1000) endormi   (1000)        1 2023-06-14 14:32:27.000000 charred-0.1.11/charred.egg-info/dependency_links.txt
+-rw-rw-r--   0 endormi   (1000) endormi   (1000)       14 2023-06-14 14:32:27.000000 charred-0.1.11/charred.egg-info/top_level.txt
+-rw-rw-r--   0 endormi   (1000) endormi   (1000)       38 2023-06-14 14:32:27.348657 charred-0.1.11/setup.cfg
+-rw-rw-r--   0 endormi   (1000) endormi   (1000)      629 2023-06-14 14:32:12.000000 charred-0.1.11/setup.py
+drwxrwxr-x   0 endormi   (1000) endormi   (1000)        0 2023-06-14 14:32:27.348657 charred-0.1.11/tests/
+-rw-rw-r--   0 endormi   (1000) endormi   (1000)        0 2023-06-06 17:05:07.000000 charred-0.1.11/tests/__init__.py
+-rw-rw-r--   0 endormi   (1000) endormi   (1000)      824 2023-06-14 13:21:21.000000 charred-0.1.11/tests/test_char.py
```

### Comparing `charred-0.1.1/LICENSE` & `charred-0.1.11/LICENSE`

 * *Files identical despite different names*

### Comparing `charred-0.1.1/PKG-INFO` & `charred-0.1.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charred
-Version: 0.1.1
+Version: 0.1.11
 Summary: Very simple char functions
 Home-page: https://github.com/endormi
 Author: Endormi
 Author-email: contactendormi@gmail.com
 License: UNKNOWN
 Description: # Charred
```

### Comparing `charred-0.1.1/README.md` & `charred-0.1.11/README.md`

 * *Files identical despite different names*

### Comparing `charred-0.1.1/charred.egg-info/PKG-INFO` & `charred-0.1.11/charred.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charred
-Version: 0.1.1
+Version: 0.1.11
 Summary: Very simple char functions
 Home-page: https://github.com/endormi
 Author: Endormi
 Author-email: contactendormi@gmail.com
 License: UNKNOWN
 Description: # Charred
```

### Comparing `charred-0.1.1/setup.py` & `charred-0.1.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as pkg:
     long_description = pkg.read()
 
 setuptools.setup(
     name="charred",
-    version="0.1.1",
+    version="0.1.11",
     author="Endormi",
     author_email="contactendormi@gmail.com",
     description="Very simple char functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/endormi",
     packages=setuptools.find_packages(),
```

### Comparing `charred-0.1.1/tests/test_char.py` & `charred-0.1.11/tests/test_char.py`

 * *Files identical despite different names*

