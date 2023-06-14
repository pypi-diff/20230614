# Comparing `tmp/adofaipy-0.0.2.tar.gz` & `tmp/adofaipy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adofaipy-0.0.2.tar", last modified: Tue Jun 13 16:24:21 2023, max compression
+gzip compressed data, was "adofaipy-0.0.3.tar", last modified: Wed Jun 14 14:49:34 2023, max compression
```

## Comparing `adofaipy-0.0.2.tar` & `adofaipy-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 16:24:21.850935 adofaipy-0.0.2/
--rw-rw-rw-   0        0        0      171 2023-06-13 16:17:13.000000 adofaipy-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1061 2023-05-28 10:23:16.000000 adofaipy-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-05-28 10:21:05.000000 adofaipy-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2145 2023-06-13 16:24:21.849935 adofaipy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1171 2023-06-13 16:24:06.000000 adofaipy-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 16:24:21.842935 adofaipy-0.0.2/adofaipy/
--rw-rw-rw-   0        0        0    19887 2023-05-28 11:03:21.000000 adofaipy-0.0.2/adofaipy/_init_.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:24:21.848936 adofaipy-0.0.2/adofaipy.egg-info/
--rw-rw-rw-   0        0        0     2145 2023-06-13 16:24:21.000000 adofaipy-0.0.2/adofaipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-06-13 16:24:21.000000 adofaipy-0.0.2/adofaipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 16:24:21.000000 adofaipy-0.0.2/adofaipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 16:24:21.000000 adofaipy-0.0.2/adofaipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 16:24:21.850935 adofaipy-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      733 2023-06-13 16:22:20.000000 adofaipy-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:49:34.732747 adofaipy-0.0.3/
+-rw-rw-rw-   0        0        0      257 2023-06-14 14:49:00.000000 adofaipy-0.0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1061 2023-05-28 10:23:16.000000 adofaipy-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-05-28 10:21:05.000000 adofaipy-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2263 2023-06-14 14:49:34.732747 adofaipy-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1171 2023-06-14 14:48:56.000000 adofaipy-0.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 14:49:34.724748 adofaipy-0.0.3/adofaipy/
+-rw-rw-rw-   0        0        0    19887 2023-06-14 14:48:42.000000 adofaipy-0.0.3/adofaipy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:49:34.730746 adofaipy-0.0.3/adofaipy.egg-info/
+-rw-rw-rw-   0        0        0     2263 2023-06-14 14:49:34.000000 adofaipy-0.0.3/adofaipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-06-14 14:49:34.000000 adofaipy-0.0.3/adofaipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 14:49:34.000000 adofaipy-0.0.3/adofaipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 14:49:34.000000 adofaipy-0.0.3/adofaipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 14:49:34.732747 adofaipy-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-06-14 14:48:46.000000 adofaipy-0.0.3/setup.py
```

### Comparing `adofaipy-0.0.2/LICENSE.txt` & `adofaipy-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adofaipy-0.0.2/PKG-INFO` & `adofaipy-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: adofaipy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library that makes automating events in ADOFAI levels more convenient.
 Home-page: UNKNOWN
 Author: M1n3c4rt
 Author-email: vedicbits@gmail.com
 License: MIT
 Description: This is a library that makes automating events in ADOFAI levels more convenient.
         
@@ -27,14 +27,18 @@
         
         writeToFile(filestring : str, filename : str): writes the modified file string to the file. 
         
         
         Change Log
         ==========
         
+        0.0.3 (2023/06/14)
+        ------------------
+        - Minor bugfix: fixed filename __init__.py
+        
         0.0.2 (2023/06/13)
         ------------------
         - Minor bugfix: 're' is no longer a dependency
         
         0.0.1 (2023/05/28)
         ------------------
         - First Release
```

### Comparing `adofaipy-0.0.2/README.txt` & `adofaipy-0.0.3/README.txt`

 * *Files identical despite different names*

### Comparing `adofaipy-0.0.2/adofaipy/_init_.py` & `adofaipy-0.0.3/adofaipy/__init__.py`

 * *Files identical despite different names*

### Comparing `adofaipy-0.0.2/adofaipy.egg-info/PKG-INFO` & `adofaipy-0.0.3/adofaipy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: adofaipy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library that makes automating events in ADOFAI levels more convenient.
 Home-page: UNKNOWN
 Author: M1n3c4rt
 Author-email: vedicbits@gmail.com
 License: MIT
 Description: This is a library that makes automating events in ADOFAI levels more convenient.
         
@@ -27,14 +27,18 @@
         
         writeToFile(filestring : str, filename : str): writes the modified file string to the file. 
         
         
         Change Log
         ==========
         
+        0.0.3 (2023/06/14)
+        ------------------
+        - Minor bugfix: fixed filename __init__.py
+        
         0.0.2 (2023/06/13)
         ------------------
         - Minor bugfix: 're' is no longer a dependency
         
         0.0.1 (2023/05/28)
         ------------------
         - First Release
```

### Comparing `adofaipy-0.0.2/setup.py` & `adofaipy-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3.11'
 ]
  
 setup(
   name='adofaipy',
-  version='0.0.2',
+  version='0.0.3',
   description='A library that makes automating events in ADOFAI levels more convenient.',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='M1n3c4rt',
   author_email='vedicbits@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

