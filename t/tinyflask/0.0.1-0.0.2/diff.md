# Comparing `tmp/tinyflask-0.0.1.tar.gz` & `tmp/tinyflask-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyflask-0.0.1.tar", last modified: Wed Jun 14 19:03:02 2023, max compression
+gzip compressed data, was "tinyflask-0.0.2.tar", last modified: Wed Jun 14 19:14:50 2023, max compression
```

## Comparing `tinyflask-0.0.1.tar` & `tinyflask-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 rvdubey   (1000) rvdubey   (1000)        0 2023-06-14 19:03:02.357656 tinyflask-0.0.1/
--rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)      409 2023-06-14 19:03:02.357656 tinyflask-0.0.1/PKG-INFO
--rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)       38 2023-06-14 19:03:02.357656 tinyflask-0.0.1/setup.cfg
--rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)     1799 2023-06-14 19:02:12.000000 tinyflask-0.0.1/setup.py
-drwxr-xr-x   0 rvdubey   (1000) rvdubey   (1000)        0 2023-06-14 19:03:02.347656 tinyflask-0.0.1/tinyflask/
--rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)        0 2023-06-14 18:40:41.000000 tinyflask-0.0.1/tinyflask/__init__.py
--rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)     3854 2023-06-14 18:41:18.000000 tinyflask-0.0.1/tinyflask/api.py
--rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)      909 2023-06-14 17:40:23.000000 tinyflask-0.0.1/tinyflask/middleware.py
--rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)      981 2023-06-14 18:30:36.000000 tinyflask-0.0.1/tinyflask/response.py
-drwxr-xr-x   0 rvdubey   (1000) rvdubey   (1000)        0 2023-06-14 19:03:02.357656 tinyflask-0.0.1/tinyflask.egg-info/
--rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)      409 2023-06-14 19:03:02.000000 tinyflask-0.0.1/tinyflask.egg-info/PKG-INFO
--rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)      257 2023-06-14 19:03:02.000000 tinyflask-0.0.1/tinyflask.egg-info/SOURCES.txt
--rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)        1 2023-06-14 19:03:02.000000 tinyflask-0.0.1/tinyflask.egg-info/dependency_links.txt
--rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)      105 2023-06-14 19:03:02.000000 tinyflask-0.0.1/tinyflask.egg-info/requires.txt
--rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)       10 2023-06-14 19:03:02.000000 tinyflask-0.0.1/tinyflask.egg-info/top_level.txt
+drwxr-xr-x   0 rvdubey   (1000) rvdubey   (1000)        0 2023-06-14 19:14:50.507656 tinyflask-0.0.2/
+-rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)     4068 2023-06-14 19:14:50.507656 tinyflask-0.0.2/PKG-INFO
+-rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)     3717 2023-06-14 19:12:55.000000 tinyflask-0.0.2/README.md
+-rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)       38 2023-06-14 19:14:50.507656 tinyflask-0.0.2/setup.cfg
+-rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)     1799 2023-06-14 19:13:56.000000 tinyflask-0.0.2/setup.py
+drwxr-xr-x   0 rvdubey   (1000) rvdubey   (1000)        0 2023-06-14 19:14:50.507656 tinyflask-0.0.2/tinyflask/
+-rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)        0 2023-06-14 18:40:41.000000 tinyflask-0.0.2/tinyflask/__init__.py
+-rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)     3854 2023-06-14 18:41:18.000000 tinyflask-0.0.2/tinyflask/api.py
+-rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)      909 2023-06-14 17:40:23.000000 tinyflask-0.0.2/tinyflask/middleware.py
+-rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)      981 2023-06-14 18:30:36.000000 tinyflask-0.0.2/tinyflask/response.py
+drwxr-xr-x   0 rvdubey   (1000) rvdubey   (1000)        0 2023-06-14 19:14:50.507656 tinyflask-0.0.2/tinyflask.egg-info/
+-rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)     4068 2023-06-14 19:14:50.000000 tinyflask-0.0.2/tinyflask.egg-info/PKG-INFO
+-rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)      267 2023-06-14 19:14:50.000000 tinyflask-0.0.2/tinyflask.egg-info/SOURCES.txt
+-rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)        1 2023-06-14 19:14:50.000000 tinyflask-0.0.2/tinyflask.egg-info/dependency_links.txt
+-rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)      105 2023-06-14 19:14:50.000000 tinyflask-0.0.2/tinyflask.egg-info/requires.txt
+-rw-r--r--   0 rvdubey   (1000) rvdubey   (1000)       10 2023-06-14 19:14:50.000000 tinyflask-0.0.2/tinyflask.egg-info/top_level.txt
```

### Comparing `tinyflask-0.0.1/setup.py` & `tinyflask-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Package meta-data.
 NAME = "tinyflask"
 DESCRIPTION = "tinyflask Python Web Framework built for learning purposes."
 EMAIL = "rahuldubey.vjti@gmail.com"
 AUTHOR = "Rahul Dubey"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 # Which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.2",
     "parse==1.19.0",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

### Comparing `tinyflask-0.0.1/tinyflask/api.py` & `tinyflask-0.0.2/tinyflask/api.py`

 * *Files identical despite different names*

### Comparing `tinyflask-0.0.1/tinyflask/middleware.py` & `tinyflask-0.0.2/tinyflask/middleware.py`

 * *Files identical despite different names*

### Comparing `tinyflask-0.0.1/tinyflask/response.py` & `tinyflask-0.0.2/tinyflask/response.py`

 * *Files identical despite different names*

