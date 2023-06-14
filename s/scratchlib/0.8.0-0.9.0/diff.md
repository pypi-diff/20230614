# Comparing `tmp/scratchlib-0.8.0.tar.gz` & `tmp/scratchlib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchlib-0.8.0.tar", last modified: Sun Feb 19 15:15:19 2023, max compression
+gzip compressed data, was "scratchlib-0.9.0.tar", last modified: Sat Feb 25 16:54:44 2023, max compression
```

## Comparing `scratchlib-0.8.0.tar` & `scratchlib-0.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 gagarinten  (1002) gagarinten  (1002)        0 2023-02-19 15:15:19.087088 scratchlib-0.8.0/
--rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)      219 2023-02-19 15:15:19.087088 scratchlib-0.8.0/PKG-INFO
--rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)      171 2022-12-03 08:36:44.000000 scratchlib-0.8.0/README.md
-drwxrwxr-x   0 gagarinten  (1002) gagarinten  (1002)        0 2023-02-19 15:15:19.087088 scratchlib-0.8.0/scratchlib/
--rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)       21 2023-02-17 16:30:10.000000 scratchlib-0.8.0/scratchlib/__init__.py
-drwxrwxr-x   0 gagarinten  (1002) gagarinten  (1002)        0 2023-02-19 15:15:19.087088 scratchlib-0.8.0/scratchlib.egg-info/
--rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)      219 2023-02-19 15:15:19.000000 scratchlib-0.8.0/scratchlib.egg-info/PKG-INFO
--rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)      220 2023-02-19 15:15:19.000000 scratchlib-0.8.0/scratchlib.egg-info/SOURCES.txt
--rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)        1 2023-02-19 15:15:19.000000 scratchlib-0.8.0/scratchlib.egg-info/dependency_links.txt
--rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)        1 2023-02-17 16:31:25.000000 scratchlib-0.8.0/scratchlib.egg-info/not-zip-safe
--rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)       11 2023-02-19 15:15:19.000000 scratchlib-0.8.0/scratchlib.egg-info/top_level.txt
--rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)       38 2023-02-19 15:15:19.087088 scratchlib-0.8.0/setup.cfg
--rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)      260 2023-02-19 15:13:46.000000 scratchlib-0.8.0/setup.py
+drwxrwxr-x   0 gagarinten  (1002) gagarinten  (1002)        0 2023-02-25 16:54:44.782643 scratchlib-0.9.0/
+-rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)      219 2023-02-25 16:54:44.782643 scratchlib-0.9.0/PKG-INFO
+-rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)      171 2022-12-03 08:36:44.000000 scratchlib-0.9.0/README.md
+drwxrwxr-x   0 gagarinten  (1002) gagarinten  (1002)        0 2023-02-25 16:54:44.782643 scratchlib-0.9.0/scratchlib/
+-rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)       21 2023-02-17 16:30:10.000000 scratchlib-0.9.0/scratchlib/__init__.py
+drwxrwxr-x   0 gagarinten  (1002) gagarinten  (1002)        0 2023-02-25 16:54:44.782643 scratchlib-0.9.0/scratchlib.egg-info/
+-rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)      219 2023-02-25 16:54:44.000000 scratchlib-0.9.0/scratchlib.egg-info/PKG-INFO
+-rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)      220 2023-02-25 16:54:44.000000 scratchlib-0.9.0/scratchlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)        1 2023-02-25 16:54:44.000000 scratchlib-0.9.0/scratchlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)        1 2023-02-17 16:31:25.000000 scratchlib-0.9.0/scratchlib.egg-info/not-zip-safe
+-rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)       11 2023-02-25 16:54:44.000000 scratchlib-0.9.0/scratchlib.egg-info/top_level.txt
+-rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)       38 2023-02-25 16:54:44.786643 scratchlib-0.9.0/setup.cfg
+-rw-rw-r--   0 gagarinten  (1002) gagarinten  (1002)      260 2023-02-25 16:49:50.000000 scratchlib-0.9.0/setup.py
```

