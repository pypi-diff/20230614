# Comparing `tmp/aorta_sirius_dev-0.8.tar.gz` & `tmp/aorta_sirius_dev-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aorta_sirius_dev-0.8.tar", last modified: Sun Jun 11 04:22:13 2023, max compression
+gzip compressed data, was "aorta_sirius_dev-0.9.tar", last modified: Sun Jun 11 04:31:09 2023, max compression
```

## Comparing `aorta_sirius_dev-0.8.tar` & `aorta_sirius_dev-0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:22:13.323422 aorta_sirius_dev-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-11 04:22:13.323422 aorta_sirius_dev-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-11 04:21:57.000000 aorta_sirius_dev-0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 04:22:13.323422 aorta_sirius_dev-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-11 04:21:57.000000 aorta_sirius_dev-0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:22:13.323422 aorta_sirius_dev-0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:22:13.323422 aorta_sirius_dev-0.8/src/aorta_sirius_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-11 04:22:13.000000 aorta_sirius_dev-0.8/src/aorta_sirius_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-11 04:22:13.000000 aorta_sirius_dev-0.8/src/aorta_sirius_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 04:22:13.000000 aorta_sirius_dev-0.8/src/aorta_sirius_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 04:22:13.000000 aorta_sirius_dev-0.8/src/aorta_sirius_dev.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:22:13.323422 aorta_sirius_dev-0.8/src/sirius/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 04:21:57.000000 aorta_sirius_dev-0.8/src/sirius/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:31:09.910041 aorta_sirius_dev-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-11 04:31:09.910041 aorta_sirius_dev-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-11 04:30:53.000000 aorta_sirius_dev-0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 04:31:09.910041 aorta_sirius_dev-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-11 04:30:53.000000 aorta_sirius_dev-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:31:09.910041 aorta_sirius_dev-0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:31:09.910041 aorta_sirius_dev-0.9/src/aorta_sirius_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-11 04:31:09.000000 aorta_sirius_dev-0.9/src/aorta_sirius_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-11 04:31:09.000000 aorta_sirius_dev-0.9/src/aorta_sirius_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 04:31:09.000000 aorta_sirius_dev-0.9/src/aorta_sirius_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 04:31:09.000000 aorta_sirius_dev-0.9/src/aorta_sirius_dev.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:31:09.910041 aorta_sirius_dev-0.9/src/sirius/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 04:30:53.000000 aorta_sirius_dev-0.9/src/sirius/__init__.py
```

### Comparing `aorta_sirius_dev-0.8/setup.py` & `aorta_sirius_dev-0.9/setup.py`

 * *Files identical despite different names*

