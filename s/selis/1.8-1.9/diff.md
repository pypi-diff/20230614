# Comparing `tmp/selis-1.8.tar.gz` & `tmp/selis-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-1.8.tar", last modified: Wed Jun 14 09:42:48 2023, max compression
+gzip compressed data, was "selis-1.9.tar", last modified: Wed Jun 14 16:03:25 2023, max compression
```

## Comparing `selis-1.8.tar` & `selis-1.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:42:48.557921 selis-1.8/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-14 09:42:48.557823 selis-1.8/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:42:48.556822 selis-1.8/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-1.8/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     5145 2023-06-14 09:42:29.000000 selis-1.8/selis/selis.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 09:42:48.557668 selis-1.8/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-14 09:42:48.000000 selis-1.8/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      217 2023-06-14 09:42:48.000000 selis-1.8/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-06-14 09:42:48.000000 selis-1.8/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       44 2023-06-14 09:42:48.000000 selis-1.8/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)        9 2023-06-14 09:42:48.000000 selis-1.8/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-06-14 09:42:48.000000 selis-1.8/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-06-14 09:42:48.557956 selis-1.8/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      254 2023-06-14 09:42:35.000000 selis-1.8/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 16:03:25.659547 selis-1.9/
+-rw-r--r--   0 client     (501) staff       (20)       47 2023-06-14 16:03:25.659414 selis-1.9/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 16:03:25.658298 selis-1.9/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-1.9/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     3837 2023-06-14 16:01:52.000000 selis-1.9/selis/client.py
+-rw-r--r--   0 client     (501) staff       (20)     1466 2023-06-14 16:02:20.000000 selis-1.9/selis/selis.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 16:03:25.659239 selis-1.9/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)       47 2023-06-14 16:03:25.000000 selis-1.9/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      233 2023-06-14 16:03:25.000000 selis-1.9/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-06-14 16:03:25.000000 selis-1.9/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       43 2023-06-14 16:03:25.000000 selis-1.9/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)        9 2023-06-14 16:03:25.000000 selis-1.9/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-06-14 16:03:25.000000 selis-1.9/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-06-14 16:03:25.659588 selis-1.9/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      254 2023-06-14 16:02:27.000000 selis-1.9/setup.py
```

