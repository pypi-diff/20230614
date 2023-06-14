# Comparing `tmp/simple_aws_ec2-0.1.4.tar.gz` & `tmp/simple_aws_ec2-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_aws_ec2-0.1.4.tar", last modified: Sat May  6 21:10:40 2023, max compression
+gzip compressed data, was "simple_aws_ec2-0.2.1.tar", last modified: Wed Jun 14 14:25:59 2023, max compression
```

## Comparing `simple_aws_ec2-0.1.4.tar` & `simple_aws_ec2-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 21:10:40.511444 simple_aws_ec2-0.1.4/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.4/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.4/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.4/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4922 2023-05-06 21:10:40.511266 simple_aws_ec2-0.1.4/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3860 2023-05-03 16:06:52.000000 simple_aws_ec2-0.1.4/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1165 2023-05-06 21:09:45.000000 simple_aws_ec2-0.1.4/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.4/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.4/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-05-03 14:53:32.000000 simple_aws_ec2-0.1.4/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       76 2023-05-03 14:58:41.000000 simple_aws_ec2-0.1.4/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-06 21:10:40.511500 simple_aws_ec2-0.1.4/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7513 2023-05-03 14:54:47.000000 simple_aws_ec2-0.1.4/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 21:10:40.508868 simple_aws_ec2-0.1.4/simple_aws_ec2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      398 2023-05-03 16:05:44.000000 simple_aws_ec2-0.1.4/simple_aws_ec2/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-06 21:06:30.000000 simple_aws_ec2-0.1.4/simple_aws_ec2/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      116 2023-05-03 16:04:16.000000 simple_aws_ec2-0.1.4/simple_aws_ec2/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 21:10:40.510024 simple_aws_ec2-0.1.4/simple_aws_ec2/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.4/simple_aws_ec2/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6864 2023-05-06 21:10:23.000000 simple_aws_ec2-0.1.4/simple_aws_ec2/ec2.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 21:10:40.509872 simple_aws_ec2-0.1.4/simple_aws_ec2.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4922 2023-05-06 21:10:40.000000 simple_aws_ec2-0.1.4/simple_aws_ec2.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      511 2023-05-06 21:10:40.000000 simple_aws_ec2-0.1.4/simple_aws_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-06 21:10:40.000000 simple_aws_ec2-0.1.4/simple_aws_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      257 2023-05-06 21:10:40.000000 simple_aws_ec2-0.1.4/simple_aws_ec2.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-05-06 21:10:40.000000 simple_aws_ec2-0.1.4/simple_aws_ec2.egg-info/top_level.txt
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 21:10:40.510903 simple_aws_ec2-0.1.4/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      315 2023-05-03 16:04:16.000000 simple_aws_ec2-0.1.4/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3457 2023-05-03 15:15:52.000000 simple_aws_ec2-0.1.4/tests/test_ec2.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 14:25:59.384306 simple_aws_ec2-0.2.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-03 14:52:18.000000 simple_aws_ec2-0.2.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 14:52:18.000000 simple_aws_ec2-0.2.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 14:52:18.000000 simple_aws_ec2-0.2.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5098 2023-06-14 14:25:59.384151 simple_aws_ec2-0.2.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4036 2023-06-14 13:43:26.000000 simple_aws_ec2-0.2.1/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1606 2023-06-14 13:42:31.000000 simple_aws_ec2-0.2.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 14:52:18.000000 simple_aws_ec2-0.2.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 14:52:18.000000 simple_aws_ec2-0.2.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-14 13:05:19.000000 simple_aws_ec2-0.2.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       48 2023-06-14 12:12:36.000000 simple_aws_ec2-0.2.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-14 14:25:59.384350 simple_aws_ec2-0.2.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7513 2023-05-03 14:54:47.000000 simple_aws_ec2-0.2.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 14:25:59.381888 simple_aws_ec2-0.2.1/simple_aws_ec2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      398 2023-05-03 16:05:44.000000 simple_aws_ec2-0.2.1/simple_aws_ec2/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-14 14:25:25.000000 simple_aws_ec2-0.2.1/simple_aws_ec2/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1034 2023-06-14 14:00:30.000000 simple_aws_ec2-0.2.1/simple_aws_ec2/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 14:25:59.383211 simple_aws_ec2-0.2.1/simple_aws_ec2/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 14:52:18.000000 simple_aws_ec2-0.2.1/simple_aws_ec2/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    18508 2023-06-14 13:50:05.000000 simple_aws_ec2-0.2.1/simple_aws_ec2/ec2.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 14:25:59.383078 simple_aws_ec2-0.2.1/simple_aws_ec2.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5098 2023-06-14 14:25:59.000000 simple_aws_ec2-0.2.1/simple_aws_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      511 2023-06-14 14:25:59.000000 simple_aws_ec2-0.2.1/simple_aws_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-14 14:25:59.000000 simple_aws_ec2-0.2.1/simple_aws_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      264 2023-06-14 14:25:59.000000 simple_aws_ec2-0.2.1/simple_aws_ec2.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-14 14:25:59.000000 simple_aws_ec2-0.2.1/simple_aws_ec2.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 14:25:59.383838 simple_aws_ec2-0.2.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      315 2023-05-03 16:04:16.000000 simple_aws_ec2-0.2.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6793 2023-06-14 13:58:57.000000 simple_aws_ec2-0.2.1/tests/test_ec2.py
```

### Comparing `simple_aws_ec2-0.1.4/LICENSE.txt` & `simple_aws_ec2-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.1.4/PKG-INFO` & `simple_aws_ec2-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simple_aws_ec2
-Version: 0.1.4
+Version: 0.2.1
 Summary: Simple AWS EC2 devtool.
 Home-page: https://github.com/MacHu-GWU/simple_aws_ec2-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.1.4#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -45,14 +45,17 @@
 
 .. image:: https://img.shields.io/pypi/l/simple_aws_ec2.svg
     :target: https://pypi.python.org/pypi/simple_aws_ec2
 
 .. image:: https://img.shields.io/pypi/pyversions/simple_aws_ec2.svg
     :target: https://pypi.python.org/pypi/simple_aws_ec2
 
+.. image:: https://img.shields.io/badge/Release_History!--None.svg?style=social
+    :target: https://github.com/MacHu-GWU/simple_aws_ec2-project/blob/main/release-history.rst
+
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/simple_aws_ec2-project
 
 ------
 
 
 .. .. image:: https://img.shields.io/badge/Link-Document-blue.svg
```

### Comparing `simple_aws_ec2-0.1.4/README.rst` & `simple_aws_ec2-0.2.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 .. image:: https://img.shields.io/pypi/l/simple_aws_ec2.svg
     :target: https://pypi.python.org/pypi/simple_aws_ec2
 
 .. image:: https://img.shields.io/pypi/pyversions/simple_aws_ec2.svg
     :target: https://pypi.python.org/pypi/simple_aws_ec2
 
+.. image:: https://img.shields.io/badge/Release_History!--None.svg?style=social
+    :target: https://github.com/MacHu-GWU/simple_aws_ec2-project/blob/main/release-history.rst
+
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/simple_aws_ec2-project
 
 ------
 
 
 .. .. image:: https://img.shields.io/badge/Link-Document-blue.svg
```

### Comparing `simple_aws_ec2-0.1.4/requirements-doc.txt` & `simple_aws_ec2-0.2.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.1.4/setup.py` & `simple_aws_ec2-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.1.4/simple_aws_ec2.egg-info/PKG-INFO` & `simple_aws_ec2-0.2.1/simple_aws_ec2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simple-aws-ec2
-Version: 0.1.4
+Version: 0.2.1
 Summary: Simple AWS EC2 devtool.
 Home-page: https://github.com/MacHu-GWU/simple_aws_ec2-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.1.4#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -45,14 +45,17 @@
 
 .. image:: https://img.shields.io/pypi/l/simple_aws_ec2.svg
     :target: https://pypi.python.org/pypi/simple_aws_ec2
 
 .. image:: https://img.shields.io/pypi/pyversions/simple_aws_ec2.svg
     :target: https://pypi.python.org/pypi/simple_aws_ec2
 
+.. image:: https://img.shields.io/badge/Release_History!--None.svg?style=social
+    :target: https://github.com/MacHu-GWU/simple_aws_ec2-project/blob/main/release-history.rst
+
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/simple_aws_ec2-project
 
 ------
 
 
 .. .. image:: https://img.shields.io/badge/Link-Document-blue.svg
```

