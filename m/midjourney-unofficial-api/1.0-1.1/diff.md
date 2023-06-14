# Comparing `tmp/midjourney_unofficial_api-1.0.tar.gz` & `tmp/midjourney_unofficial_api-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midjourney_unofficial_api-1.0.tar", last modified: Tue Jun 13 20:19:29 2023, max compression
+gzip compressed data, was "midjourney_unofficial_api-1.1.tar", last modified: Wed Jun 14 06:55:29 2023, max compression
```

## Comparing `midjourney_unofficial_api-1.0.tar` & `midjourney_unofficial_api-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 va1ngvarr  (1000) va1ngvarr  (1000)        0 2023-06-13 20:19:29.065438 midjourney_unofficial_api-1.0/
--rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)     1070 2023-06-13 18:34:16.000000 midjourney_unofficial_api-1.0/LICENSE
--rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)      259 2023-06-13 20:19:29.065438 midjourney_unofficial_api-1.0/PKG-INFO
--rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)      797 2023-06-13 19:12:35.000000 midjourney_unofficial_api-1.0/README.md
-drwxr-xr-x   0 va1ngvarr  (1000) va1ngvarr  (1000)        0 2023-06-13 20:19:28.975436 midjourney_unofficial_api-1.0/midjourney/
-drwxr-xr-x   0 va1ngvarr  (1000) va1ngvarr  (1000)        0 2023-06-13 20:19:29.065438 midjourney_unofficial_api-1.0/midjourney/midjourney_unofficial_api.egg-info/
--rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)      259 2023-06-13 20:19:28.000000 midjourney_unofficial_api-1.0/midjourney/midjourney_unofficial_api.egg-info/PKG-INFO
--rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)      335 2023-06-13 20:19:28.000000 midjourney_unofficial_api-1.0/midjourney/midjourney_unofficial_api.egg-info/SOURCES.txt
--rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)        1 2023-06-13 20:19:28.000000 midjourney_unofficial_api-1.0/midjourney/midjourney_unofficial_api.egg-info/dependency_links.txt
--rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)       16 2023-06-13 20:19:28.000000 midjourney_unofficial_api-1.0/midjourney/midjourney_unofficial_api.egg-info/requires.txt
--rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)        1 2023-06-13 20:19:28.000000 midjourney_unofficial_api-1.0/midjourney/midjourney_unofficial_api.egg-info/top_level.txt
--rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)      103 2023-06-13 20:19:29.068771 midjourney_unofficial_api-1.0/setup.cfg
--rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)      429 2023-06-13 20:17:35.000000 midjourney_unofficial_api-1.0/setup.py
+drwxr-xr-x   0 va1ngvarr  (1000) va1ngvarr  (1000)        0 2023-06-14 06:55:29.941316 midjourney_unofficial_api-1.1/
+-rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)     1070 2023-06-14 06:34:36.000000 midjourney_unofficial_api-1.1/LICENSE
+-rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)      259 2023-06-14 06:55:29.941316 midjourney_unofficial_api-1.1/PKG-INFO
+-rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)      976 2023-06-14 06:34:36.000000 midjourney_unofficial_api-1.1/README.md
+drwxr-xr-x   0 va1ngvarr  (1000) va1ngvarr  (1000)        0 2023-06-14 06:55:29.937983 midjourney_unofficial_api-1.1/midjourney/
+drwxr-xr-x   0 va1ngvarr  (1000) va1ngvarr  (1000)        0 2023-06-14 06:55:29.941316 midjourney_unofficial_api-1.1/midjourney/midjourney_unofficial_api.egg-info/
+-rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)      259 2023-06-14 06:55:29.000000 midjourney_unofficial_api-1.1/midjourney/midjourney_unofficial_api.egg-info/PKG-INFO
+-rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)      335 2023-06-14 06:55:29.000000 midjourney_unofficial_api-1.1/midjourney/midjourney_unofficial_api.egg-info/SOURCES.txt
+-rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)        1 2023-06-14 06:55:29.000000 midjourney_unofficial_api-1.1/midjourney/midjourney_unofficial_api.egg-info/dependency_links.txt
+-rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)       16 2023-06-14 06:55:29.000000 midjourney_unofficial_api-1.1/midjourney/midjourney_unofficial_api.egg-info/requires.txt
+-rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)        1 2023-06-14 06:55:29.000000 midjourney_unofficial_api-1.1/midjourney/midjourney_unofficial_api.egg-info/top_level.txt
+-rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)      103 2023-06-14 06:55:29.941316 midjourney_unofficial_api-1.1/setup.cfg
+-rw-r--r--   0 va1ngvarr  (1000) va1ngvarr  (1000)      429 2023-06-14 06:55:26.000000 midjourney_unofficial_api-1.1/setup.py
```

### Comparing `midjourney_unofficial_api-1.0/LICENSE` & `midjourney_unofficial_api-1.1/LICENSE`

 * *Files identical despite different names*

