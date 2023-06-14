# Comparing `tmp/dassana-0.8.4.tar.gz` & `tmp/dassana-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dassana-0.8.4.tar", last modified: Thu Apr  6 13:39:56 2023, max compression
+gzip compressed data, was "dassana-0.8.5.tar", last modified: Thu Jun  8 12:37:01 2023, max compression
```

## Comparing `dassana-0.8.4.tar` & `dassana-0.8.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:39:56.337264 dassana-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-06 13:39:56.337264 dassana-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-06 13:39:44.000000 dassana-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:39:56.337264 dassana-0.8.4/dassana/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-06 13:39:44.000000 dassana-0.8.4/dassana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-06 13:39:44.000000 dassana-0.8.4/dassana/dassana_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-04-06 13:39:44.000000 dassana-0.8.4/dassana/data_pipes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-04-06 13:39:44.000000 dassana-0.8.4/dassana/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:39:56.337264 dassana-0.8.4/dassana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-06 13:39:56.000000 dassana-0.8.4/dassana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-06 13:39:56.000000 dassana-0.8.4/dassana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 13:39:56.000000 dassana-0.8.4/dassana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 13:39:56.000000 dassana-0.8.4/dassana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-06 13:39:56.000000 dassana-0.8.4/dassana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-06 13:39:56.000000 dassana-0.8.4/dassana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 13:39:56.337264 dassana-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-06 13:39:44.000000 dassana-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:37:01.519464 dassana-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-08 12:37:01.519464 dassana-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 12:36:51.000000 dassana-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:37:01.519464 dassana-0.8.5/dassana/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-08 12:36:51.000000 dassana-0.8.5/dassana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-06-08 12:36:51.000000 dassana-0.8.5/dassana/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-08 12:36:51.000000 dassana-0.8.5/dassana/dassana_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-06-08 12:36:51.000000 dassana-0.8.5/dassana/data_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-06-08 12:36:51.000000 dassana-0.8.5/dassana/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:37:01.519464 dassana-0.8.5/dassana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-08 12:37:01.000000 dassana-0.8.5/dassana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-08 12:37:01.000000 dassana-0.8.5/dassana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:37:01.000000 dassana-0.8.5/dassana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:37:01.000000 dassana-0.8.5/dassana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 12:37:01.000000 dassana-0.8.5/dassana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 12:37:01.000000 dassana-0.8.5/dassana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 12:37:01.519464 dassana-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-08 12:36:51.000000 dassana-0.8.5/setup.py
```

### Comparing `dassana-0.8.4/dassana/dassana_env.py` & `dassana-0.8.5/dassana/dassana_env.py`

 * *Files identical despite different names*

### Comparing `dassana-0.8.4/dassana/data_pipes.py` & `dassana-0.8.5/dassana/data_pipes.py`

 * *Files identical despite different names*

### Comparing `dassana-0.8.4/dassana/rest.py` & `dassana-0.8.5/dassana/rest.py`

 * *Files identical despite different names*

