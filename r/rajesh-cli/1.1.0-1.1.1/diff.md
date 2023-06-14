# Comparing `tmp/rajesh_cli-1.1.0.tar.gz` & `tmp/rajesh_cli-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rajesh_cli-1.1.0.tar", last modified: Wed Jun 14 11:12:26 2023, max compression
+gzip compressed data, was "rajesh_cli-1.1.1.tar", last modified: Wed Jun 14 11:13:27 2023, max compression
```

## Comparing `rajesh_cli-1.1.0.tar` & `rajesh_cli-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rajesh    (1000) rajesh    (1000)        0 2023-06-14 11:12:26.400062 rajesh_cli-1.1.0/
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       54 2023-06-14 11:12:26.400062 rajesh_cli-1.1.0/PKG-INFO
-drwxrwxr-x   0 rajesh    (1000) rajesh    (1000)        0 2023-06-14 11:12:26.400062 rajesh_cli-1.1.0/rajesh_cli.egg-info/
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       54 2023-06-14 11:12:26.000000 rajesh_cli-1.1.0/rajesh_cli.egg-info/PKG-INFO
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)      241 2023-06-14 11:12:26.000000 rajesh_cli-1.1.0/rajesh_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        1 2023-06-14 11:12:26.000000 rajesh_cli-1.1.0/rajesh_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       60 2023-06-14 11:12:26.000000 rajesh_cli-1.1.0/rajesh_cli.egg-info/entry_points.txt
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        9 2023-06-14 11:12:26.000000 rajesh_cli-1.1.0/rajesh_cli.egg-info/requires.txt
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        4 2023-06-14 11:12:26.000000 rajesh_cli-1.1.0/rajesh_cli.egg-info/top_level.txt
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       38 2023-06-14 11:12:26.400062 rajesh_cli-1.1.0/setup.cfg
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)      299 2023-06-14 11:11:59.000000 rajesh_cli-1.1.0/setup.py
-drwxrwxr-x   0 rajesh    (1000) rajesh    (1000)        0 2023-06-14 11:12:26.400062 rajesh_cli-1.1.0/src/
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        0 2023-06-14 11:10:06.000000 rajesh_cli-1.1.0/src/__init__.py
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)     1681 2023-06-14 11:10:26.000000 rajesh_cli-1.1.0/src/cli.py
+drwxrwxr-x   0 rajesh    (1000) rajesh    (1000)        0 2023-06-14 11:13:27.412062 rajesh_cli-1.1.1/
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       54 2023-06-14 11:13:27.412062 rajesh_cli-1.1.1/PKG-INFO
+drwxrwxr-x   0 rajesh    (1000) rajesh    (1000)        0 2023-06-14 11:13:27.412062 rajesh_cli-1.1.1/rajesh_cli.egg-info/
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       54 2023-06-14 11:13:27.000000 rajesh_cli-1.1.1/rajesh_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)      241 2023-06-14 11:13:27.000000 rajesh_cli-1.1.1/rajesh_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        1 2023-06-14 11:13:27.000000 rajesh_cli-1.1.1/rajesh_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       49 2023-06-14 11:13:27.000000 rajesh_cli-1.1.1/rajesh_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        9 2023-06-14 11:13:27.000000 rajesh_cli-1.1.1/rajesh_cli.egg-info/requires.txt
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        4 2023-06-14 11:13:27.000000 rajesh_cli-1.1.1/rajesh_cli.egg-info/top_level.txt
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       38 2023-06-14 11:13:27.412062 rajesh_cli-1.1.1/setup.cfg
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)      288 2023-06-14 11:13:26.000000 rajesh_cli-1.1.1/setup.py
+drwxrwxr-x   0 rajesh    (1000) rajesh    (1000)        0 2023-06-14 11:13:27.412062 rajesh_cli-1.1.1/src/
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        0 2023-06-14 11:10:06.000000 rajesh_cli-1.1.1/src/__init__.py
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)     1681 2023-06-14 11:10:26.000000 rajesh_cli-1.1.1/src/cli.py
```

### Comparing `rajesh_cli-1.1.0/src/cli.py` & `rajesh_cli-1.1.1/src/cli.py`

 * *Files identical despite different names*

