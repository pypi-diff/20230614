# Comparing `tmp/Samay-0.0.2.tar.gz` & `tmp/Samay-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Samay-0.0.2.tar", last modified: Tue Nov 29 13:42:42 2022, max compression
+gzip compressed data, was "Samay-0.0.3.tar", last modified: Tue Nov 29 14:08:32 2022, max compression
```

## Comparing `Samay-0.0.2.tar` & `Samay-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-11-29 13:42:42.675114 Samay-0.0.2/
--rw-rw-rw-   0        0        0     1101 2022-11-27 04:59:06.000000 Samay-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      760 2022-11-29 13:42:42.673845 Samay-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2022-11-29 09:22:34.000000 Samay-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-11-29 13:42:42.642847 Samay-0.0.2/Samay/
--rw-rw-rw-   0        0        0     2555 2022-11-27 05:37:34.000000 Samay-0.0.2/Samay/Samay.py
--rw-rw-rw-   0        0        0        0 2022-11-29 09:00:39.000000 Samay-0.0.2/Samay/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-29 13:42:42.672031 Samay-0.0.2/Samay.egg-info/
--rw-rw-rw-   0        0        0      760 2022-11-29 13:42:42.000000 Samay-0.0.2/Samay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2022-11-29 13:42:42.000000 Samay-0.0.2/Samay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-29 13:42:42.000000 Samay-0.0.2/Samay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-11-29 13:42:42.000000 Samay-0.0.2/Samay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-29 13:42:42.675114 Samay-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1022 2022-11-29 13:41:57.000000 Samay-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-29 14:08:32.873051 Samay-0.0.3/
+-rw-rw-rw-   0        0        0     1101 2022-11-27 04:59:06.000000 Samay-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      769 2022-11-29 14:08:32.871014 Samay-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1042 2022-11-29 09:22:34.000000 Samay-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2022-11-29 14:08:32.851047 Samay-0.0.3/Samay/
+-rw-rw-rw-   0        0        0     2555 2022-11-27 05:37:34.000000 Samay-0.0.3/Samay/Samay.py
+-rw-rw-rw-   0        0        0        0 2022-11-29 09:00:39.000000 Samay-0.0.3/Samay/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-29 14:08:32.869028 Samay-0.0.3/Samay.egg-info/
+-rw-rw-rw-   0        0        0      769 2022-11-29 14:08:32.000000 Samay-0.0.3/Samay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2022-11-29 14:08:32.000000 Samay-0.0.3/Samay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-29 14:08:32.000000 Samay-0.0.3/Samay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2022-11-29 14:08:32.000000 Samay-0.0.3/Samay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-11-29 14:08:32.873051 Samay-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2022-11-29 14:07:39.000000 Samay-0.0.3/setup.py
```

### Comparing `Samay-0.0.2/LICENSE` & `Samay-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Samay-0.0.2/PKG-INFO` & `Samay-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Samay
-Version: 0.0.2
+Version: 0.0.3
 Summary: Samay
 Home-page: UNKNOWN
 Author: Saurav Sharma
 Author-email: sv19projects@gmail.com
 License: UNKNOWN
 Description: A packay to find out execution time of a function, or compare two function with respect to execution time.
 Keywords: Samay,samay,time,execution,execution time,run time,runtime,function runtime,function execution time,compare function
 Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `Samay-0.0.2/README.md` & `Samay-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Samay-0.0.2/Samay/Samay.py` & `Samay-0.0.3/Samay/Samay.py`

 * *Files identical despite different names*

### Comparing `Samay-0.0.2/Samay.egg-info/PKG-INFO` & `Samay-0.0.3/Samay.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Samay
-Version: 0.0.2
+Version: 0.0.3
 Summary: Samay
 Home-page: UNKNOWN
 Author: Saurav Sharma
 Author-email: sv19projects@gmail.com
 License: UNKNOWN
 Description: A packay to find out execution time of a function, or compare two function with respect to execution time.
 Keywords: Samay,samay,time,execution,execution time,run time,runtime,function runtime,function execution time,compare function
 Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `Samay-0.0.2/setup.py` & `Samay-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "Samay"
 LONG_DESCRIPTION = "A packay to find out execution time of a function, or compare two function with respect to execution time."
 
 # Setting up
 setup(
     name="Samay",
     version=VERSION,
@@ -15,15 +15,15 @@
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[""],
     keywords=["Samay","samay","time","execution","execution time","run time","runtime","function runtime","function execution time","compare function"],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

