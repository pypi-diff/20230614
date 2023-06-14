# Comparing `tmp/poplar_logging-1.2.1.tar.gz` & `tmp/poplar_logging-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poplar_logging-1.2.1.tar", last modified: Wed Jun 14 20:00:48 2023, max compression
+gzip compressed data, was "poplar_logging-1.2.2.tar", last modified: Wed Jun 14 20:11:15 2023, max compression
```

## Comparing `poplar_logging-1.2.1.tar` & `poplar_logging-1.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-14 20:00:48.435016 poplar_logging-1.2.1/
--rw-r--r--   0 odai       (501) staff       (20)     1070 2023-06-12 04:45:07.000000 poplar_logging-1.2.1/LICENSE
--rw-r--r--   0 odai       (501) staff       (20)      861 2023-06-14 20:00:48.434906 poplar_logging-1.2.1/PKG-INFO
--rw-r--r--   0 odai       (501) staff       (20)      427 2023-06-14 19:59:52.000000 poplar_logging-1.2.1/README.md
--rw-r--r--   0 odai       (501) staff       (20)      427 2023-06-14 20:00:38.000000 poplar_logging-1.2.1/pyproject.toml
--rw-r--r--   0 odai       (501) staff       (20)       38 2023-06-14 20:00:48.435048 poplar_logging-1.2.1/setup.cfg
-drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-14 20:00:48.433420 poplar_logging-1.2.1/src/
-drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-14 20:00:48.434269 poplar_logging-1.2.1/src/poplar_logging/
--rw-r--r--   0 odai       (501) staff       (20)       26 2023-06-14 19:58:40.000000 poplar_logging-1.2.1/src/poplar_logging/__init__.py
--rw-r--r--   0 odai       (501) staff       (20)     1507 2023-06-14 19:58:23.000000 poplar_logging-1.2.1/src/poplar_logging/logger.py
-drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-14 20:00:48.434781 poplar_logging-1.2.1/src/poplar_logging.egg-info/
--rw-r--r--   0 odai       (501) staff       (20)      861 2023-06-14 20:00:48.000000 poplar_logging-1.2.1/src/poplar_logging.egg-info/PKG-INFO
--rw-r--r--   0 odai       (501) staff       (20)      260 2023-06-14 20:00:48.000000 poplar_logging-1.2.1/src/poplar_logging.egg-info/SOURCES.txt
--rw-r--r--   0 odai       (501) staff       (20)        1 2023-06-14 20:00:48.000000 poplar_logging-1.2.1/src/poplar_logging.egg-info/dependency_links.txt
--rw-r--r--   0 odai       (501) staff       (20)       15 2023-06-14 20:00:48.000000 poplar_logging-1.2.1/src/poplar_logging.egg-info/top_level.txt
+drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-14 20:11:15.816734 poplar_logging-1.2.2/
+-rw-r--r--   0 odai       (501) staff       (20)     1070 2023-06-12 04:45:07.000000 poplar_logging-1.2.2/LICENSE
+-rw-r--r--   0 odai       (501) staff       (20)      861 2023-06-14 20:11:15.816601 poplar_logging-1.2.2/PKG-INFO
+-rw-r--r--   0 odai       (501) staff       (20)      427 2023-06-14 19:59:52.000000 poplar_logging-1.2.2/README.md
+-rw-r--r--   0 odai       (501) staff       (20)      427 2023-06-14 20:09:38.000000 poplar_logging-1.2.2/pyproject.toml
+-rw-r--r--   0 odai       (501) staff       (20)       38 2023-06-14 20:11:15.816769 poplar_logging-1.2.2/setup.cfg
+drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-14 20:11:15.814608 poplar_logging-1.2.2/src/
+drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-14 20:11:15.815609 poplar_logging-1.2.2/src/poplar_logging/
+-rw-r--r--   0 odai       (501) staff       (20)       40 2023-06-14 20:05:23.000000 poplar_logging-1.2.2/src/poplar_logging/__init__.py
+-rw-r--r--   0 odai       (501) staff       (20)     1507 2023-06-14 19:58:23.000000 poplar_logging-1.2.2/src/poplar_logging/logger.py
+drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-14 20:11:15.816424 poplar_logging-1.2.2/src/poplar_logging.egg-info/
+-rw-r--r--   0 odai       (501) staff       (20)      861 2023-06-14 20:11:15.000000 poplar_logging-1.2.2/src/poplar_logging.egg-info/PKG-INFO
+-rw-r--r--   0 odai       (501) staff       (20)      260 2023-06-14 20:11:15.000000 poplar_logging-1.2.2/src/poplar_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 odai       (501) staff       (20)        1 2023-06-14 20:11:15.000000 poplar_logging-1.2.2/src/poplar_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 odai       (501) staff       (20)       15 2023-06-14 20:11:15.000000 poplar_logging-1.2.2/src/poplar_logging.egg-info/top_level.txt
```

### Comparing `poplar_logging-1.2.1/LICENSE` & `poplar_logging-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poplar_logging-1.2.1/PKG-INFO` & `poplar_logging-1.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poplar_logging
-Version: 1.2.1
+Version: 1.2.2
 Summary: Simple Python logging library
 Author-email: Odai Athamneh <heyodai@gmail.com>
 Project-URL: Homepage, https://github.com/heyodai/poplar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `poplar_logging-1.2.1/src/poplar_logging/logger.py` & `poplar_logging-1.2.2/src/poplar_logging/logger.py`

 * *Files identical despite different names*

### Comparing `poplar_logging-1.2.1/src/poplar_logging.egg-info/PKG-INFO` & `poplar_logging-1.2.2/src/poplar_logging.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poplar-logging
-Version: 1.2.1
+Version: 1.2.2
 Summary: Simple Python logging library
 Author-email: Odai Athamneh <heyodai@gmail.com>
 Project-URL: Homepage, https://github.com/heyodai/poplar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

