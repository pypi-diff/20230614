# Comparing `tmp/selis-1.9.tar.gz` & `tmp/selis-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-1.9.tar", last modified: Wed Jun 14 16:03:25 2023, max compression
+gzip compressed data, was "selis-2.0.tar", last modified: Wed Jun 14 16:14:41 2023, max compression
```

## Comparing `selis-1.9.tar` & `selis-2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 16:03:25.659547 selis-1.9/
--rw-r--r--   0 client     (501) staff       (20)       47 2023-06-14 16:03:25.659414 selis-1.9/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 16:03:25.658298 selis-1.9/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-1.9/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     3837 2023-06-14 16:01:52.000000 selis-1.9/selis/client.py
--rw-r--r--   0 client     (501) staff       (20)     1466 2023-06-14 16:02:20.000000 selis-1.9/selis/selis.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 16:03:25.659239 selis-1.9/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)       47 2023-06-14 16:03:25.000000 selis-1.9/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      233 2023-06-14 16:03:25.000000 selis-1.9/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-06-14 16:03:25.000000 selis-1.9/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       43 2023-06-14 16:03:25.000000 selis-1.9/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)        9 2023-06-14 16:03:25.000000 selis-1.9/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-06-14 16:03:25.000000 selis-1.9/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-06-14 16:03:25.659588 selis-1.9/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      254 2023-06-14 16:02:27.000000 selis-1.9/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 16:14:41.946236 selis-2.0/
+-rw-r--r--   0 client     (501) staff       (20)       47 2023-06-14 16:14:41.946097 selis-2.0/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 16:14:41.944686 selis-2.0/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-2.0/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     3837 2023-06-14 16:01:52.000000 selis-2.0/selis/client.py
+-rw-r--r--   0 client     (501) staff       (20)     1472 2023-06-14 16:14:33.000000 selis-2.0/selis/selis.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 16:14:41.945845 selis-2.0/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)       47 2023-06-14 16:14:41.000000 selis-2.0/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      233 2023-06-14 16:14:41.000000 selis-2.0/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-06-14 16:14:41.000000 selis-2.0/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       43 2023-06-14 16:14:41.000000 selis-2.0/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)        9 2023-06-14 16:14:41.000000 selis-2.0/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-06-14 16:14:41.000000 selis-2.0/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-06-14 16:14:41.946310 selis-2.0/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      254 2023-06-14 16:14:21.000000 selis-2.0/setup.py
```

### Comparing `selis-1.9/selis/client.py` & `selis-2.0/selis/client.py`

 * *Files identical despite different names*

### Comparing `selis-1.9/selis/selis.py` & `selis-2.0/selis/selis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import getpass
 import sys
 
 from optparse import OptionParser
-from client import Client
+from selis.client import Client
 
 
 def return_arguments():
     parser = OptionParser()
     parser.add_option("-p", "--port", dest="port", help="Connect to sever through this port")
     parser.add_option("-r", "--root", dest="root", help="Use root [on/off] to become the admin")
     parser.add_option("-n", "--nickname", dest="nickname", help="Choose your name or a nickname")
```

