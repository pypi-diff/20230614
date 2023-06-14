# Comparing `tmp/rajesh_cli-1.0.5.tar.gz` & `tmp/rajesh_cli-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rajesh_cli-1.0.5.tar", last modified: Wed Jun 14 10:56:17 2023, max compression
+gzip compressed data, was "rajesh_cli-1.0.6.tar", last modified: Wed Jun 14 11:07:40 2023, max compression
```

## Comparing `rajesh_cli-1.0.5.tar` & `rajesh_cli-1.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 rajesh    (1000) rajesh    (1000)        0 2023-06-14 10:56:17.460059 rajesh_cli-1.0.5/
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       54 2023-06-14 10:56:17.460059 rajesh_cli-1.0.5/PKG-INFO
-drwxrwxr-x   0 rajesh    (1000) rajesh    (1000)        0 2023-06-14 10:56:17.460059 rajesh_cli-1.0.5/rajesh_cli.egg-info/
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       54 2023-06-14 10:56:17.000000 rajesh_cli-1.0.5/rajesh_cli.egg-info/PKG-INFO
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)      214 2023-06-14 10:56:17.000000 rajesh_cli-1.0.5/rajesh_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        1 2023-06-14 10:56:17.000000 rajesh_cli-1.0.5/rajesh_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       47 2023-06-14 10:56:17.000000 rajesh_cli-1.0.5/rajesh_cli.egg-info/entry_points.txt
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        9 2023-06-14 10:56:17.000000 rajesh_cli-1.0.5/rajesh_cli.egg-info/requires.txt
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        1 2023-06-14 10:56:17.000000 rajesh_cli-1.0.5/rajesh_cli.egg-info/top_level.txt
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       38 2023-06-14 10:56:17.460059 rajesh_cli-1.0.5/setup.cfg
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)      286 2023-06-14 10:55:43.000000 rajesh_cli-1.0.5/setup.py
+drwxrwxr-x   0 rajesh    (1000) rajesh    (1000)        0 2023-06-14 11:07:40.092061 rajesh_cli-1.0.6/
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       54 2023-06-14 11:07:40.092061 rajesh_cli-1.0.6/PKG-INFO
+drwxrwxr-x   0 rajesh    (1000) rajesh    (1000)        0 2023-06-14 11:07:40.092061 rajesh_cli-1.0.6/rajesh_cli.egg-info/
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       54 2023-06-14 11:07:40.000000 rajesh_cli-1.0.6/rajesh_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)      214 2023-06-14 11:07:40.000000 rajesh_cli-1.0.6/rajesh_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        1 2023-06-14 11:07:40.000000 rajesh_cli-1.0.6/rajesh_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       53 2023-06-14 11:07:40.000000 rajesh_cli-1.0.6/rajesh_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        9 2023-06-14 11:07:40.000000 rajesh_cli-1.0.6/rajesh_cli.egg-info/requires.txt
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        1 2023-06-14 11:07:40.000000 rajesh_cli-1.0.6/rajesh_cli.egg-info/top_level.txt
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       38 2023-06-14 11:07:40.092061 rajesh_cli-1.0.6/setup.cfg
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)      292 2023-06-14 11:07:39.000000 rajesh_cli-1.0.6/setup.py
```

