# Comparing `tmp/anomalies-0.2.5.tar.gz` & `tmp/anomalies-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anomalies-0.2.5.tar", last modified: Tue Sep  6 23:31:07 2022, max compression
+gzip compressed data, was "anomalies-0.2.6.tar", last modified: Wed Jun 14 07:02:43 2023, max compression
```

## Comparing `anomalies-0.2.5.tar` & `anomalies-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 23:31:07.100986 anomalies-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-09-06 23:30:58.000000 anomalies-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-09-06 23:31:07.100986 anomalies-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-09-06 23:30:58.000000 anomalies-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 23:31:07.100986 anomalies-0.2.5/anomalies/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-06 23:30:58.000000 anomalies-0.2.5/anomalies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1724 2022-09-06 23:30:58.000000 anomalies-0.2.5/anomalies/anomaly.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 23:31:07.100986 anomalies-0.2.5/anomalies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-09-06 23:31:07.000000 anomalies-0.2.5/anomalies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-09-06 23:31:07.000000 anomalies-0.2.5/anomalies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 23:31:07.000000 anomalies-0.2.5/anomalies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-09-06 23:31:07.000000 anomalies-0.2.5/anomalies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-06 23:31:07.000000 anomalies-0.2.5/anomalies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-06 23:31:07.100986 anomalies-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-09-06 23:30:58.000000 anomalies-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:02:43.872858 anomalies-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-14 07:02:32.000000 anomalies-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-14 07:02:43.872858 anomalies-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-14 07:02:32.000000 anomalies-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:02:43.872858 anomalies-0.2.6/anomalies/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 07:02:32.000000 anomalies-0.2.6/anomalies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-14 07:02:32.000000 anomalies-0.2.6/anomalies/anomaly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:02:43.872858 anomalies-0.2.6/anomalies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-14 07:02:43.000000 anomalies-0.2.6/anomalies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-14 07:02:43.000000 anomalies-0.2.6/anomalies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:02:43.000000 anomalies-0.2.6/anomalies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-14 07:02:43.000000 anomalies-0.2.6/anomalies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 07:02:43.000000 anomalies-0.2.6/anomalies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 07:02:43.872858 anomalies-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-14 07:02:32.000000 anomalies-0.2.6/setup.py
```

### Comparing `anomalies-0.2.5/LICENSE` & `anomalies-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `anomalies-0.2.5/PKG-INFO` & `anomalies-0.2.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anomalies
-Version: 0.2.5
+Version: 0.2.6
 Summary: Anomaly cancellation
 Home-page: https://github.com/restrepo/anomalies
 Author: restrepo
 Author-email: restrepo@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -39,8 +39,8 @@
 >>> anomaly.free.gcd
 3
 >>> anomaly.free.simplified
 array([ 1,  1,  1, -4, -4,  5])
 ```
 
 ## Example
-A sample for `4<N<13` with integers until `|30|` with `~400 000` chiral solutions can be download from [here](https://github.com/restrepo/anomaly/raw/main/solutions.json.gz) [JSON]
+A sample for `4<N<13` with integers until `|30|` with `~400 000` chiral solutions can be download from: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7380817.svg)](https://doi.org/10.5281/zenodo.7380817) [JSON]
```

### Comparing `anomalies-0.2.5/README.md` & `anomalies-0.2.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 >>> anomaly.free.gcd
 3
 >>> anomaly.free.simplified
 array([ 1,  1,  1, -4, -4,  5])
 ```
 
 ## Example
-A sample for `4<N<13` with integers until `|30|` with `~400 000` chiral solutions can be download from [here](https://github.com/restrepo/anomaly/raw/main/solutions.json.gz) [JSON]
+A sample for `4<N<13` with integers until `|30|` with `~400 000` chiral solutions can be download from: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7380817.svg)](https://doi.org/10.5281/zenodo.7380817) [JSON]
```

### Comparing `anomalies-0.2.5/anomalies/anomaly.py` & `anomalies-0.2.6/anomalies/anomaly.py`

 * *Files identical despite different names*

### Comparing `anomalies-0.2.5/anomalies.egg-info/PKG-INFO` & `anomalies-0.2.6/anomalies.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anomalies
-Version: 0.2.5
+Version: 0.2.6
 Summary: Anomaly cancellation
 Home-page: https://github.com/restrepo/anomalies
 Author: restrepo
 Author-email: restrepo@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -39,8 +39,8 @@
 >>> anomaly.free.gcd
 3
 >>> anomaly.free.simplified
 array([ 1,  1,  1, -4, -4,  5])
 ```
 
 ## Example
-A sample for `4<N<13` with integers until `|30|` with `~400 000` chiral solutions can be download from [here](https://github.com/restrepo/anomaly/raw/main/solutions.json.gz) [JSON]
+A sample for `4<N<13` with integers until `|30|` with `~400 000` chiral solutions can be download from: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7380817.svg)](https://doi.org/10.5281/zenodo.7380817) [JSON]
```

### Comparing `anomalies-0.2.5/setup.py` & `anomalies-0.2.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 def main():
     setup(
         # Application name:
         name="anomalies",
 
         # Version number (initial):
-        version="0.2.5",
+        version="0.2.6",
 
         # Application author details:
         author="restrepo",
         author_email="restrepo@udea.edu.co",
 
         # Packages
         packages=find_packages(exclude=['tests']),
```

