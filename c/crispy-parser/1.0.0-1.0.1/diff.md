# Comparing `tmp/crispy-parser-1.0.0.tar.gz` & `tmp/crispy-parser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crispy-parser-1.0.0.tar", last modified: Tue Jun 13 11:35:05 2023, max compression
+gzip compressed data, was "crispy-parser-1.0.1.tar", last modified: Wed Jun 14 18:35:57 2023, max compression
```

## Comparing `crispy-parser-1.0.0.tar` & `crispy-parser-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 ferit     (1000) ferit     (1000)        0 2023-06-13 11:35:05.200687 crispy-parser-1.0.0/
--rw-r--r--   0 ferit     (1000) ferit     (1000)    26526 2023-06-12 15:03:30.000000 crispy-parser-1.0.0/LICENSE
--rw-r--r--   0 ferit     (1000) ferit     (1000)      304 2023-06-13 11:35:05.200687 crispy-parser-1.0.0/PKG-INFO
--rw-r--r--   0 ferit     (1000) ferit     (1000)      161 2023-06-13 10:57:17.000000 crispy-parser-1.0.0/README.md
-drwxr-xr-x   0 ferit     (1000) ferit     (1000)        0 2023-06-13 11:35:05.199687 crispy-parser-1.0.0/crispy/
--rw-r--r--   0 ferit     (1000) ferit     (1000)      280 2023-06-13 10:56:05.000000 crispy-parser-1.0.0/crispy/__init__.py
--rw-r--r--   0 ferit     (1000) ferit     (1000)     4373 2023-06-13 10:57:17.000000 crispy-parser-1.0.0/crispy/crispy.py
--rw-r--r--   0 ferit     (1000) ferit     (1000)      238 2023-06-13 05:54:04.000000 crispy-parser-1.0.0/crispy/duplicate_name_exception.py
--rw-r--r--   0 ferit     (1000) ferit     (1000)      236 2023-06-13 05:57:19.000000 crispy-parser-1.0.0/crispy/missing_value_exception.py
--rw-r--r--   0 ferit     (1000) ferit     (1000)      234 2023-06-13 05:56:04.000000 crispy-parser-1.0.0/crispy/no_arguments_exception.py
-drwxr-xr-x   0 ferit     (1000) ferit     (1000)        0 2023-06-13 11:35:05.199687 crispy-parser-1.0.0/crispy/tests/
--rw-r--r--   0 ferit     (1000) ferit     (1000)        0 2023-06-12 16:22:44.000000 crispy-parser-1.0.0/crispy/tests/__init__.py
--rw-r--r--   0 ferit     (1000) ferit     (1000)     1636 2023-06-13 10:57:17.000000 crispy-parser-1.0.0/crispy/tests/test_add_variable.py
--rw-r--r--   0 ferit     (1000) ferit     (1000)      990 2023-06-13 10:57:17.000000 crispy-parser-1.0.0/crispy/tests/test_crispy.py
--rw-r--r--   0 ferit     (1000) ferit     (1000)     4233 2023-06-13 10:57:17.000000 crispy-parser-1.0.0/crispy/tests/test_parse_arguments.py
--rw-r--r--   0 ferit     (1000) ferit     (1000)      547 2023-06-13 10:57:17.000000 crispy-parser-1.0.0/crispy/tests/test_parse_string.py
--rw-r--r--   0 ferit     (1000) ferit     (1000)      873 2023-06-13 10:57:17.000000 crispy-parser-1.0.0/crispy/tests/test_show_keys.py
--rw-r--r--   0 ferit     (1000) ferit     (1000)      836 2023-06-13 10:57:17.000000 crispy-parser-1.0.0/crispy/tests/test_try_parse.py
--rw-r--r--   0 ferit     (1000) ferit     (1000)      248 2023-06-13 05:58:00.000000 crispy-parser-1.0.0/crispy/unexpected_argument_exception.py
-drwxr-xr-x   0 ferit     (1000) ferit     (1000)        0 2023-06-13 11:35:05.200687 crispy-parser-1.0.0/crispy_parser.egg-info/
--rw-r--r--   0 ferit     (1000) ferit     (1000)      304 2023-06-13 11:35:05.000000 crispy-parser-1.0.0/crispy_parser.egg-info/PKG-INFO
--rw-r--r--   0 ferit     (1000) ferit     (1000)      572 2023-06-13 11:35:05.000000 crispy-parser-1.0.0/crispy_parser.egg-info/SOURCES.txt
--rw-r--r--   0 ferit     (1000) ferit     (1000)        1 2023-06-13 11:35:05.000000 crispy-parser-1.0.0/crispy_parser.egg-info/dependency_links.txt
--rw-r--r--   0 ferit     (1000) ferit     (1000)        7 2023-06-13 11:35:05.000000 crispy-parser-1.0.0/crispy_parser.egg-info/top_level.txt
--rw-r--r--   0 ferit     (1000) ferit     (1000)       38 2023-06-13 11:35:05.200687 crispy-parser-1.0.0/setup.cfg
--rw-r--r--   0 ferit     (1000) ferit     (1000)      383 2023-06-13 11:32:43.000000 crispy-parser-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:35:57.633542 crispy-parser-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-14 18:35:57.633542 crispy-parser-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:35:57.633542 crispy-parser-1.0.1/crispy/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/crispy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/duplicate_name_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/missing_value_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/no_arguments_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:35:57.633542 crispy-parser-1.0.1/crispy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/tests/test_add_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/tests/test_crispy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/tests/test_parse_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/tests/test_parse_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/tests/test_show_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/tests/test_try_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/unexpected_argument_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:35:57.633542 crispy-parser-1.0.1/crispy_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-14 18:35:57.000000 crispy-parser-1.0.1/crispy_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-14 18:35:57.000000 crispy-parser-1.0.1/crispy_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 18:35:57.000000 crispy-parser-1.0.1/crispy_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 18:35:57.000000 crispy-parser-1.0.1/crispy_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 18:35:57.633542 crispy-parser-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/setup.py
```

### Comparing `crispy-parser-1.0.0/LICENSE` & `crispy-parser-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crispy-parser-1.0.0/crispy/crispy.py` & `crispy-parser-1.0.1/crispy/crispy.py`

 * *Files identical despite different names*

### Comparing `crispy-parser-1.0.0/crispy/tests/test_add_variable.py` & `crispy-parser-1.0.1/crispy/tests/test_add_variable.py`

 * *Files identical despite different names*

### Comparing `crispy-parser-1.0.0/crispy/tests/test_crispy.py` & `crispy-parser-1.0.1/crispy/tests/test_crispy.py`

 * *Files identical despite different names*

### Comparing `crispy-parser-1.0.0/crispy/tests/test_parse_arguments.py` & `crispy-parser-1.0.1/crispy/tests/test_parse_arguments.py`

 * *Files identical despite different names*

### Comparing `crispy-parser-1.0.0/crispy/tests/test_parse_string.py` & `crispy-parser-1.0.1/crispy/tests/test_parse_string.py`

 * *Files identical despite different names*

### Comparing `crispy-parser-1.0.0/crispy/tests/test_show_keys.py` & `crispy-parser-1.0.1/crispy/tests/test_show_keys.py`

 * *Files identical despite different names*

### Comparing `crispy-parser-1.0.0/crispy/tests/test_try_parse.py` & `crispy-parser-1.0.1/crispy/tests/test_try_parse.py`

 * *Files identical despite different names*

### Comparing `crispy-parser-1.0.0/crispy_parser.egg-info/SOURCES.txt` & `crispy-parser-1.0.1/crispy_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

