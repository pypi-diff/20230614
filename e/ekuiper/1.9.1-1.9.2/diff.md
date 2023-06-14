# Comparing `tmp/ekuiper-1.9.1.tar.gz` & `tmp/ekuiper-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ekuiper-1.9.1.tar", last modified: Mon Apr 17 10:25:00 2023, max compression
+gzip compressed data, was "ekuiper-1.9.2.tar", last modified: Thu May 18 03:56:50 2023, max compression
```

## Comparing `ekuiper-1.9.1.tar` & `ekuiper-1.9.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:25:00.145509 ekuiper-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 10:24:45.000000 ekuiper-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-17 10:25:00.145509 ekuiper-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-17 10:24:45.000000 ekuiper-1.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:25:00.141509 ekuiper-1.9.1/ekuiper/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-17 10:24:45.000000 ekuiper-1.9.1/ekuiper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-17 10:24:45.000000 ekuiper-1.9.1/ekuiper/function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:25:00.145509 ekuiper-1.9.1/ekuiper/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-17 10:24:45.000000 ekuiper-1.9.1/ekuiper/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-17 10:24:45.000000 ekuiper-1.9.1/ekuiper/runtime/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-17 10:24:45.000000 ekuiper-1.9.1/ekuiper/runtime/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-17 10:24:45.000000 ekuiper-1.9.1/ekuiper/runtime/contextimpl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-17 10:24:45.000000 ekuiper-1.9.1/ekuiper/runtime/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-17 10:24:45.000000 ekuiper-1.9.1/ekuiper/runtime/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-17 10:24:45.000000 ekuiper-1.9.1/ekuiper/runtime/reg.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-17 10:24:45.000000 ekuiper-1.9.1/ekuiper/runtime/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-17 10:24:45.000000 ekuiper-1.9.1/ekuiper/runtime/sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-17 10:24:45.000000 ekuiper-1.9.1/ekuiper/runtime/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-17 10:24:45.000000 ekuiper-1.9.1/ekuiper/runtime/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-17 10:24:45.000000 ekuiper-1.9.1/ekuiper/sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-17 10:24:45.000000 ekuiper-1.9.1/ekuiper/source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:25:00.141509 ekuiper-1.9.1/ekuiper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-17 10:25:00.000000 ekuiper-1.9.1/ekuiper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-17 10:25:00.000000 ekuiper-1.9.1/ekuiper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:25:00.000000 ekuiper-1.9.1/ekuiper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 10:25:00.000000 ekuiper-1.9.1/ekuiper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 10:25:00.000000 ekuiper-1.9.1/ekuiper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 10:25:00.145509 ekuiper-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-17 10:24:59.000000 ekuiper-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:56:50.046679 ekuiper-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 03:56:33.000000 ekuiper-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-18 03:56:50.046679 ekuiper-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-18 03:56:33.000000 ekuiper-1.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:56:50.042678 ekuiper-1.9.2/ekuiper/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-18 03:56:33.000000 ekuiper-1.9.2/ekuiper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-18 03:56:33.000000 ekuiper-1.9.2/ekuiper/function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:56:50.046679 ekuiper-1.9.2/ekuiper/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-18 03:56:33.000000 ekuiper-1.9.2/ekuiper/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-18 03:56:33.000000 ekuiper-1.9.2/ekuiper/runtime/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-18 03:56:33.000000 ekuiper-1.9.2/ekuiper/runtime/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-18 03:56:33.000000 ekuiper-1.9.2/ekuiper/runtime/contextimpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-18 03:56:33.000000 ekuiper-1.9.2/ekuiper/runtime/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-18 03:56:33.000000 ekuiper-1.9.2/ekuiper/runtime/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-18 03:56:33.000000 ekuiper-1.9.2/ekuiper/runtime/reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-18 03:56:33.000000 ekuiper-1.9.2/ekuiper/runtime/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-18 03:56:33.000000 ekuiper-1.9.2/ekuiper/runtime/sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-18 03:56:33.000000 ekuiper-1.9.2/ekuiper/runtime/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-18 03:56:33.000000 ekuiper-1.9.2/ekuiper/runtime/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-18 03:56:33.000000 ekuiper-1.9.2/ekuiper/sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-18 03:56:33.000000 ekuiper-1.9.2/ekuiper/source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:56:50.046679 ekuiper-1.9.2/ekuiper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-18 03:56:50.000000 ekuiper-1.9.2/ekuiper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-18 03:56:50.000000 ekuiper-1.9.2/ekuiper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 03:56:50.000000 ekuiper-1.9.2/ekuiper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 03:56:50.000000 ekuiper-1.9.2/ekuiper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 03:56:50.000000 ekuiper-1.9.2/ekuiper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 03:56:50.046679 ekuiper-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-18 03:56:49.000000 ekuiper-1.9.2/setup.py
```

### Comparing `ekuiper-1.9.1/LICENSE` & `ekuiper-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ekuiper-1.9.1/ekuiper/__init__.py` & `ekuiper-1.9.2/ekuiper/__init__.py`

 * *Files identical despite different names*

### Comparing `ekuiper-1.9.1/ekuiper/function.py` & `ekuiper-1.9.2/ekuiper/function.py`

 * *Files identical despite different names*

### Comparing `ekuiper-1.9.1/ekuiper/runtime/connection.py` & `ekuiper-1.9.2/ekuiper/runtime/connection.py`

 * *Files identical despite different names*

### Comparing `ekuiper-1.9.1/ekuiper/runtime/context.py` & `ekuiper-1.9.2/ekuiper/runtime/context.py`

 * *Files identical despite different names*

### Comparing `ekuiper-1.9.1/ekuiper/runtime/contextimpl.py` & `ekuiper-1.9.2/ekuiper/runtime/contextimpl.py`

 * *Files identical despite different names*

### Comparing `ekuiper-1.9.1/ekuiper/runtime/function.py` & `ekuiper-1.9.2/ekuiper/runtime/function.py`

 * *Files identical despite different names*

### Comparing `ekuiper-1.9.1/ekuiper/runtime/plugin.py` & `ekuiper-1.9.2/ekuiper/runtime/plugin.py`

 * *Files identical despite different names*

### Comparing `ekuiper-1.9.1/ekuiper/runtime/reg.py` & `ekuiper-1.9.2/ekuiper/runtime/reg.py`

 * *Files identical despite different names*

### Comparing `ekuiper-1.9.1/ekuiper/runtime/shared.py` & `ekuiper-1.9.2/ekuiper/runtime/shared.py`

 * *Files identical despite different names*

### Comparing `ekuiper-1.9.1/ekuiper/runtime/sink.py` & `ekuiper-1.9.2/ekuiper/runtime/sink.py`

 * *Files identical despite different names*

### Comparing `ekuiper-1.9.1/ekuiper/runtime/source.py` & `ekuiper-1.9.2/ekuiper/runtime/source.py`

 * *Files identical despite different names*

### Comparing `ekuiper-1.9.1/ekuiper/runtime/symbol.py` & `ekuiper-1.9.2/ekuiper/runtime/symbol.py`

 * *Files identical despite different names*

### Comparing `ekuiper-1.9.1/ekuiper/sink.py` & `ekuiper-1.9.2/ekuiper/sink.py`

 * *Files identical despite different names*

### Comparing `ekuiper-1.9.1/ekuiper/source.py` & `ekuiper-1.9.2/ekuiper/source.py`

 * *Files identical despite different names*

### Comparing `ekuiper-1.9.1/ekuiper.egg-info/SOURCES.txt` & `ekuiper-1.9.2/ekuiper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

