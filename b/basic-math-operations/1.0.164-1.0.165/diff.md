# Comparing `tmp/basic_math_operations-1.0.164.tar.gz` & `tmp/basic_math_operations-1.0.165.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic_math_operations-1.0.164.tar", last modified: Wed Jun 14 15:06:52 2023, max compression
+gzip compressed data, was "basic_math_operations-1.0.165.tar", last modified: Wed Jun 14 15:55:22 2023, max compression
```

## Comparing `basic_math_operations-1.0.164.tar` & `basic_math_operations-1.0.165.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:06:52.575944 basic_math_operations-1.0.164/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 15:06:25.000000 basic_math_operations-1.0.164/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-14 15:06:52.575944 basic_math_operations-1.0.164/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-14 15:06:25.000000 basic_math_operations-1.0.164/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:06:52.575944 basic_math_operations-1.0.164/basic_math_operations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-14 15:06:52.000000 basic_math_operations-1.0.164/basic_math_operations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-14 15:06:52.000000 basic_math_operations-1.0.164/basic_math_operations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:06:52.000000 basic_math_operations-1.0.164/basic_math_operations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-14 15:06:52.000000 basic_math_operations-1.0.164/basic_math_operations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 15:06:52.575944 basic_math_operations-1.0.164/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-14 15:06:25.000000 basic_math_operations-1.0.164/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:06:52.571944 basic_math_operations-1.0.164/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:06:52.575944 basic_math_operations-1.0.164/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)    75528 2023-06-14 15:06:52.000000 basic_math_operations-1.0.164/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-14 15:06:25.000000 basic_math_operations-1.0.164/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 15:06:52.000000 basic_math_operations-1.0.164/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:55:22.735604 basic_math_operations-1.0.165/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 15:55:06.000000 basic_math_operations-1.0.165/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-14 15:55:22.735604 basic_math_operations-1.0.165/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-14 15:55:06.000000 basic_math_operations-1.0.165/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:55:22.731604 basic_math_operations-1.0.165/basic_math_operations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-14 15:55:22.000000 basic_math_operations-1.0.165/basic_math_operations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-14 15:55:22.000000 basic_math_operations-1.0.165/basic_math_operations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:55:22.000000 basic_math_operations-1.0.165/basic_math_operations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-14 15:55:22.000000 basic_math_operations-1.0.165/basic_math_operations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 15:55:22.735604 basic_math_operations-1.0.165/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-14 15:55:06.000000 basic_math_operations-1.0.165/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:55:22.731604 basic_math_operations-1.0.165/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:55:22.735604 basic_math_operations-1.0.165/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)    75528 2023-06-14 15:55:22.000000 basic_math_operations-1.0.165/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-14 15:55:06.000000 basic_math_operations-1.0.165/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 15:55:22.000000 basic_math_operations-1.0.165/src/python-module/version.txt
```

### Comparing `basic_math_operations-1.0.164/LICENSE` & `basic_math_operations-1.0.165/LICENSE`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.164/README.md` & `basic_math_operations-1.0.165/README.md`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.164/setup.py` & `basic_math_operations-1.0.165/setup.py`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.164/src/python-module/libbasic_math_operations.a` & `basic_math_operations-1.0.165/src/python-module/libbasic_math_operations.a`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.164/src/python-module/module.c` & `basic_math_operations-1.0.165/src/python-module/module.c`

 * *Files identical despite different names*

