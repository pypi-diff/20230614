# Comparing `tmp/masterthermconnect-2.2.4.tar.gz` & `tmp/masterthermconnect-2.2.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masterthermconnect-2.2.4.tar", last modified: Tue Jun 13 19:06:34 2023, max compression
+gzip compressed data, was "masterthermconnect-2.2.5b0.tar", last modified: Wed Jun 14 12:11:26 2023, max compression
```

## Comparing `masterthermconnect-2.2.4.tar` & `masterthermconnect-2.2.5b0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:06:34.231447 masterthermconnect-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-06-13 19:06:34.231447 masterthermconnect-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:06:34.231447 masterthermconnect-2.2.4/masterthermconnect/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21627 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    27399 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    15138 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/datamapread.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/datamapwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/masterthermconnect/special.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:06:34.231447 masterthermconnect-2.2.4/masterthermconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-06-13 19:06:34.000000 masterthermconnect-2.2.4/masterthermconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-13 19:06:34.000000 masterthermconnect-2.2.4/masterthermconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:06:34.000000 masterthermconnect-2.2.4/masterthermconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-13 19:06:34.000000 masterthermconnect-2.2.4/masterthermconnect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-13 19:06:34.000000 masterthermconnect-2.2.4/masterthermconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 19:06:34.000000 masterthermconnect-2.2.4/masterthermconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-13 19:06:34.235447 masterthermconnect-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:06:34.231447 masterthermconnect-2.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/tests/test_api_new.py
--rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/tests/test_api_old.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/tests/test_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29214 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-06-13 19:05:59.000000 masterthermconnect-2.2.4/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:11:26.777562 masterthermconnect-2.2.5b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-06-14 12:11:26.777562 masterthermconnect-2.2.5b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:11:26.777562 masterthermconnect-2.2.5b0/masterthermconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21627 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27399 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15173 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/datamapread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/datamapwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/special.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:11:26.777562 masterthermconnect-2.2.5b0/masterthermconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-06-14 12:11:26.000000 masterthermconnect-2.2.5b0/masterthermconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-14 12:11:26.000000 masterthermconnect-2.2.5b0/masterthermconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:11:26.000000 masterthermconnect-2.2.5b0/masterthermconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-14 12:11:26.000000 masterthermconnect-2.2.5b0/masterthermconnect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 12:11:26.000000 masterthermconnect-2.2.5b0/masterthermconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-14 12:11:26.000000 masterthermconnect-2.2.5b0/masterthermconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-14 12:11:26.777562 masterthermconnect-2.2.5b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:11:26.777562 masterthermconnect-2.2.5b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/tests/test_api_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/tests/test_api_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/tests/test_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29214 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/tests/test_main.py
```

### Comparing `masterthermconnect-2.2.4/LICENSE` & `masterthermconnect-2.2.5b0/LICENSE`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.4/PKG-INFO` & `masterthermconnect-2.2.5b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterthermconnect
-Version: 2.2.4
+Version: 2.2.5b0
 Summary: Python 3 API wrapper for Mastertherm API
 Author-email: Richard Holmes <richard@shedc.uk>
 License: MIT License
         
         Copyright (c) 2021 shedc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: masterthermconnect Version: 2.2.4 Summary: Python 3
-API wrapper for Mastertherm API Author-email: Richard Holmes
+Metadata-Version: 2.1 Name: masterthermconnect Version: 2.2.5b0 Summary: Python
+3 API wrapper for Mastertherm API Author-email: Richard Holmes
 shedc.uk> License: MIT License Copyright (c) 2021 shedc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
```

### Comparing `masterthermconnect-2.2.4/README.md` & `masterthermconnect-2.2.5b0/README.md`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.4/masterthermconnect/__init__.py` & `masterthermconnect-2.2.5b0/masterthermconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.4/masterthermconnect/__main__.py` & `masterthermconnect-2.2.5b0/masterthermconnect/__main__.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.4/masterthermconnect/api.py` & `masterthermconnect-2.2.5b0/masterthermconnect/api.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.4/masterthermconnect/const.py` & `masterthermconnect-2.2.5b0/masterthermconnect/const.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.4/masterthermconnect/controller.py` & `masterthermconnect-2.2.5b0/masterthermconnect/controller.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.4/masterthermconnect/datamapread.py` & `masterthermconnect-2.2.5b0/masterthermconnect/datamapread.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,16 +292,16 @@
     "operating_mode": [
         Special(str, Special.FORMULA),
         [
             (
                 "'dhw' if {0} else "
                 "'pool' if {1} else "
                 "'aux_heater' if not ({2} or {3}) and ({4} or {5}) else "
-                "'dpc' if {6} else "
-                "'cooling' if {7} or {12} or {13} else"
+                "'cooling_dpc' if {6} and ({7} or {12} or {13}) else "
+                "'cooling' if {7} or {12} or {13} else "
                 "'heating' if {8} or {9} or {10} or {11} else "
                 "'idle'"
             ),
             [
                 [bool, "D_66"],  # 0 - domestic hot water
                 [bool, "D_43"],  # 1 - pool
                 [bool, "D_20"],  # 2 - some_error
```

### Comparing `masterthermconnect-2.2.4/masterthermconnect/datamapwrite.py` & `masterthermconnect-2.2.5b0/masterthermconnect/datamapwrite.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.4/masterthermconnect/exceptions.py` & `masterthermconnect-2.2.5b0/masterthermconnect/exceptions.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.4/masterthermconnect/special.py` & `masterthermconnect-2.2.5b0/masterthermconnect/special.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.4/masterthermconnect.egg-info/PKG-INFO` & `masterthermconnect-2.2.5b0/masterthermconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterthermconnect
-Version: 2.2.4
+Version: 2.2.5b0
 Summary: Python 3 API wrapper for Mastertherm API
 Author-email: Richard Holmes <richard@shedc.uk>
 License: MIT License
         
         Copyright (c) 2021 shedc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: masterthermconnect Version: 2.2.4 Summary: Python 3
-API wrapper for Mastertherm API Author-email: Richard Holmes
+Metadata-Version: 2.1 Name: masterthermconnect Version: 2.2.5b0 Summary: Python
+3 API wrapper for Mastertherm API Author-email: Richard Holmes
 shedc.uk> License: MIT License Copyright (c) 2021 shedc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
```

### Comparing `masterthermconnect-2.2.4/masterthermconnect.egg-info/SOURCES.txt` & `masterthermconnect-2.2.5b0/masterthermconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.4/pyproject.toml` & `masterthermconnect-2.2.5b0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "masterthermconnect"
-version = "2.2.4"
+version = "2.2.5b0"
 description = "Python 3 API wrapper for Mastertherm API"
 readme = "README.md"
 authors = [{ name = "Richard Holmes", email = "richard@shedc.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -24,15 +24,15 @@
 [project.urls]
 Homepage = "https://github.com/sHedC/python-masterthermconnect"
 
 [project.scripts]
 masterthermconnect = "masterthermconnect.__main__:main"
 
 [tool.bumpver]
-current_version = "2.2.4"
+current_version = "2.2.5-b0"
 version_pattern = "MAJOR.MINOR.PATCH[-PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `masterthermconnect-2.2.4/setup.cfg` & `masterthermconnect-2.2.5b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.4/tests/test_api_new.py` & `masterthermconnect-2.2.5b0/tests/test_api_new.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.4/tests/test_api_old.py` & `masterthermconnect-2.2.5b0/tests/test_api_old.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.4/tests/test_config_data.py` & `masterthermconnect-2.2.5b0/tests/test_config_data.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.4/tests/test_controller.py` & `masterthermconnect-2.2.5b0/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.4/tests/test_main.py` & `masterthermconnect-2.2.5b0/tests/test_main.py`

 * *Files identical despite different names*

