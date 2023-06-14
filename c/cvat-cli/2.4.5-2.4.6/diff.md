# Comparing `tmp/cvat-cli-2.4.5.tar.gz` & `tmp/cvat-cli-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat-cli-2.4.5.tar", last modified: Wed Jun 14 19:52:03 2023, max compression
+gzip compressed data, was "cvat-cli-2.4.6.tar", last modified: Wed Jun 14 19:57:32 2023, max compression
```

## Comparing `cvat-cli-2.4.5.tar` & `cvat-cli-2.4.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:52:03.297405 cvat-cli-2.4.5/
--rw-r--r--   0 andrey    (1000) andrey    (1000)       47 2022-11-18 08:29:30.000000 cvat-cli-2.4.5/MANIFEST.in
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-06-14 19:52:03.297405 cvat-cli-2.4.5/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1981 2022-11-18 08:29:30.000000 cvat-cli-2.4.5/README.md
--rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-11-18 08:29:30.000000 cvat-cli-2.4.5/pyproject.toml
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:52:03.297405 cvat-cli-2.4.5/requirements/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      114 2023-04-14 14:12:32.000000 cvat-cli-2.4.5/requirements/base.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-06-14 19:52:03.297405 cvat-cli-2.4.5/setup.cfg
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1969 2022-11-18 08:29:30.000000 cvat-cli-2.4.5/setup.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:52:03.297405 cvat-cli-2.4.5/src/
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:52:03.297405 cvat-cli-2.4.5/src/cvat_cli/
--rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2022-11-18 08:29:30.000000 cvat-cli-2.4.5/src/cvat_cli/__init__.py
--rwxr-xr-x   0 andrey    (1000) andrey    (1000)     2151 2022-11-18 08:29:30.000000 cvat-cli-2.4.5/src/cvat_cli/__main__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     4805 2023-04-05 10:02:25.000000 cvat-cli-2.4.5/src/cvat_cli/cli.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13103 2023-04-05 10:02:25.000000 cvat-cli-2.4.5/src/cvat_cli/parser.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-06-14 19:46:20.000000 cvat-cli-2.4.5/src/cvat_cli/version.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:52:03.297405 cvat-cli-2.4.5/src/cvat_cli.egg-info/
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-06-14 19:52:03.000000 cvat-cli-2.4.5/src/cvat_cli.egg-info/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)      402 2023-06-14 19:52:03.000000 cvat-cli-2.4.5/src/cvat_cli.egg-info/SOURCES.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-06-14 19:52:03.000000 cvat-cli-2.4.5/src/cvat_cli.egg-info/dependency_links.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       52 2023-06-14 19:52:03.000000 cvat-cli-2.4.5/src/cvat_cli.egg-info/entry_points.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       49 2023-06-14 19:52:03.000000 cvat-cli-2.4.5/src/cvat_cli.egg-info/requires.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-06-14 19:52:03.000000 cvat-cli-2.4.5/src/cvat_cli.egg-info/top_level.txt
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:57:32.167224 cvat-cli-2.4.6/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       47 2022-11-18 08:29:30.000000 cvat-cli-2.4.6/MANIFEST.in
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-06-14 19:57:32.167224 cvat-cli-2.4.6/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1981 2022-11-18 08:29:30.000000 cvat-cli-2.4.6/README.md
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-11-18 08:29:30.000000 cvat-cli-2.4.6/pyproject.toml
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:57:32.167224 cvat-cli-2.4.6/requirements/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      114 2023-04-14 14:12:32.000000 cvat-cli-2.4.6/requirements/base.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-06-14 19:57:32.167224 cvat-cli-2.4.6/setup.cfg
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1969 2022-11-18 08:29:30.000000 cvat-cli-2.4.6/setup.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:57:32.167224 cvat-cli-2.4.6/src/
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:57:32.167224 cvat-cli-2.4.6/src/cvat_cli/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2022-11-18 08:29:30.000000 cvat-cli-2.4.6/src/cvat_cli/__init__.py
+-rwxr-xr-x   0 andrey    (1000) andrey    (1000)     2151 2022-11-18 08:29:30.000000 cvat-cli-2.4.6/src/cvat_cli/__main__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     4805 2023-04-05 10:02:25.000000 cvat-cli-2.4.6/src/cvat_cli/cli.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13103 2023-04-05 10:02:25.000000 cvat-cli-2.4.6/src/cvat_cli/parser.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-06-14 19:53:41.000000 cvat-cli-2.4.6/src/cvat_cli/version.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:57:32.167224 cvat-cli-2.4.6/src/cvat_cli.egg-info/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-06-14 19:57:32.000000 cvat-cli-2.4.6/src/cvat_cli.egg-info/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      402 2023-06-14 19:57:32.000000 cvat-cli-2.4.6/src/cvat_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-06-14 19:57:32.000000 cvat-cli-2.4.6/src/cvat_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       52 2023-06-14 19:57:32.000000 cvat-cli-2.4.6/src/cvat_cli.egg-info/entry_points.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       49 2023-06-14 19:57:32.000000 cvat-cli-2.4.6/src/cvat_cli.egg-info/requires.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-06-14 19:57:32.000000 cvat-cli-2.4.6/src/cvat_cli.egg-info/top_level.txt
```

### Comparing `cvat-cli-2.4.5/PKG-INFO` & `cvat-cli-2.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat-cli
-Version: 2.4.5
+Version: 2.4.6
 Summary: Command-line client for CVAT
 Home-page: https://github.com/cvat-ai/cvat/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cvat-cli-2.4.5/README.md` & `cvat-cli-2.4.6/README.md`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.4.5/setup.py` & `cvat-cli-2.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.4.5/src/cvat_cli/__main__.py` & `cvat-cli-2.4.6/src/cvat_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.4.5/src/cvat_cli/cli.py` & `cvat-cli-2.4.6/src/cvat_cli/cli.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.4.5/src/cvat_cli/parser.py` & `cvat-cli-2.4.6/src/cvat_cli/parser.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.4.5/src/cvat_cli.egg-info/PKG-INFO` & `cvat-cli-2.4.6/src/cvat_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat-cli
-Version: 2.4.5
+Version: 2.4.6
 Summary: Command-line client for CVAT
 Home-page: https://github.com/cvat-ai/cvat/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

