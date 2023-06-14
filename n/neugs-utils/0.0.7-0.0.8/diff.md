# Comparing `tmp/neugs_utils-0.0.7.tar.gz` & `tmp/neugs_utils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neugs_utils-0.0.7.tar", last modified: Wed Dec 21 21:28:30 2022, max compression
+gzip compressed data, was "neugs_utils-0.0.8.tar", last modified: Fri Dec 30 18:41:06 2022, max compression
```

## Comparing `neugs_utils-0.0.7.tar` & `neugs_utils-0.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-12-21 21:28:30.755331 neugs_utils-0.0.7/
--rw-rw-rw-   0        0        0     3306 2022-12-13 03:21:59.000000 neugs_utils-0.0.7/.gitignore
--rw-rw-rw-   0        0        0     1103 2022-12-05 05:36:56.000000 neugs_utils-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     4544 2022-12-21 21:28:30.755331 neugs_utils-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2793 2022-12-13 16:43:03.000000 neugs_utils-0.0.7/README.md
--rw-rw-rw-   0        0        0      376 2022-12-13 16:44:31.000000 neugs_utils-0.0.7/TODO.md
-drwxrwxrwx   0        0        0        0 2022-12-21 21:28:30.706800 neugs_utils-0.0.7/neugs_utils/
--rw-rw-rw-   0        0        0     4211 2022-12-20 18:45:14.000000 neugs_utils-0.0.7/neugs_utils/__init__.py
--rw-rw-rw-   0        0        0     1887 2022-12-04 22:55:01.000000 neugs_utils-0.0.7/neugs_utils/common_tests.py
--rw-rw-rw-   0        0        0     1504 2022-12-12 15:56:54.000000 neugs_utils-0.0.7/neugs_utils/context_managers.py
-drwxrwxrwx   0        0        0        0 2022-12-21 21:28:30.723341 neugs_utils-0.0.7/neugs_utils/scripts/
--rw-rw-rw-   0        0        0     3196 2022-12-21 02:33:43.000000 neugs_utils-0.0.7/neugs_utils/scripts/build_autograder.py
-drwxrwxrwx   0        0        0        0 2022-12-21 21:28:30.747525 neugs_utils-0.0.7/neugs_utils/scripts/templates/
--rw-rw-rw-   0        0        0       55 2022-12-13 03:12:58.000000 neugs_utils-0.0.7/neugs_utils/scripts/templates/requirements.txt
--rw-rw-rw-   0        0        0      222 2022-12-21 21:24:01.000000 neugs_utils-0.0.7/neugs_utils/scripts/templates/run_autograder
--rw-rw-rw-   0        0        0      331 2022-12-13 03:13:08.000000 neugs_utils-0.0.7/neugs_utils/scripts/templates/run_tests.py
--rw-rw-rw-   0        0        0      166 2022-12-13 03:13:16.000000 neugs_utils-0.0.7/neugs_utils/scripts/templates/setup.sh
--rw-rw-rw-   0        0        0     2630 2022-12-21 02:49:09.000000 neugs_utils-0.0.7/neugs_utils/scripts/test_utils.py
--rw-rw-rw-   0        0        0     4614 2022-12-16 23:20:04.000000 neugs_utils-0.0.7/neugs_utils/tier_grading.py
-drwxrwxrwx   0        0        0        0 2022-12-21 21:28:30.720340 neugs_utils-0.0.7/neugs_utils.egg-info/
--rw-rw-rw-   0        0        0     4544 2022-12-21 21:28:30.000000 neugs_utils-0.0.7/neugs_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2022-12-21 21:28:30.000000 neugs_utils-0.0.7/neugs_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-21 21:28:30.000000 neugs_utils-0.0.7/neugs_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2022-12-21 21:28:30.000000 neugs_utils-0.0.7/neugs_utils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       42 2022-12-21 21:28:30.000000 neugs_utils-0.0.7/neugs_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-12-21 21:28:30.000000 neugs_utils-0.0.7/neugs_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      824 2022-12-21 02:51:15.000000 neugs_utils-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      357 2022-12-21 21:26:54.000000 neugs_utils-0.0.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-12-21 21:28:30.756336 neugs_utils-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-21 21:28:30.748521 neugs_utils-0.0.7/tests/
-drwxrwxrwx   0        0        0        0 2022-12-21 21:28:30.754029 neugs_utils-0.0.7/tests/examples/
--rw-rw-rw-   0        0        0     1355 2022-12-12 15:58:35.000000 neugs_utils-0.0.7/tests/examples/test_one.py
--rw-rw-rw-   0        0        0      428 2022-12-12 17:02:39.000000 neugs_utils-0.0.7/tests/run_tests.py
+drwxrwxrwx   0        0        0        0 2022-12-30 18:41:06.167060 neugs_utils-0.0.8/
+-rw-rw-rw-   0        0        0     3306 2022-12-13 03:21:59.000000 neugs_utils-0.0.8/.gitignore
+-rw-rw-rw-   0        0        0     1103 2022-12-05 05:36:56.000000 neugs_utils-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     4544 2022-12-30 18:41:06.167060 neugs_utils-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2793 2022-12-13 16:43:03.000000 neugs_utils-0.0.8/README.md
+-rw-rw-rw-   0        0        0      473 2022-12-30 18:39:34.000000 neugs_utils-0.0.8/TODO.md
+drwxrwxrwx   0        0        0        0 2022-12-30 18:41:06.088915 neugs_utils-0.0.8/neugs_utils/
+-rw-rw-rw-   0        0        0     4211 2022-12-20 18:45:14.000000 neugs_utils-0.0.8/neugs_utils/__init__.py
+-rw-rw-rw-   0        0        0     1887 2022-12-04 22:55:01.000000 neugs_utils-0.0.8/neugs_utils/common_tests.py
+-rw-rw-rw-   0        0        0     1504 2022-12-12 15:56:54.000000 neugs_utils-0.0.8/neugs_utils/context_managers.py
+drwxrwxrwx   0        0        0        0 2022-12-30 18:41:06.124059 neugs_utils-0.0.8/neugs_utils/scripts/
+-rw-rw-rw-   0        0        0     3196 2022-12-21 02:33:43.000000 neugs_utils-0.0.8/neugs_utils/scripts/build_autograder.py
+drwxrwxrwx   0        0        0        0 2022-12-30 18:41:06.154059 neugs_utils-0.0.8/neugs_utils/scripts/templates/
+-rw-rw-rw-   0        0        0       55 2022-12-13 03:12:58.000000 neugs_utils-0.0.8/neugs_utils/scripts/templates/requirements.txt
+-rw-rw-rw-   0        0        0      222 2022-12-21 21:24:01.000000 neugs_utils-0.0.8/neugs_utils/scripts/templates/run_autograder
+-rw-rw-rw-   0        0        0      331 2022-12-13 03:13:08.000000 neugs_utils-0.0.8/neugs_utils/scripts/templates/run_tests.py
+-rw-rw-rw-   0        0        0      215 2022-12-30 18:39:05.000000 neugs_utils-0.0.8/neugs_utils/scripts/templates/setup.sh
+-rw-rw-rw-   0        0        0     2630 2022-12-21 02:49:09.000000 neugs_utils-0.0.8/neugs_utils/scripts/test_utils.py
+-rw-rw-rw-   0        0        0     4614 2022-12-16 23:20:04.000000 neugs_utils-0.0.8/neugs_utils/tier_grading.py
+drwxrwxrwx   0        0        0        0 2022-12-30 18:41:06.109920 neugs_utils-0.0.8/neugs_utils.egg-info/
+-rw-rw-rw-   0        0        0     4544 2022-12-30 18:41:05.000000 neugs_utils-0.0.8/neugs_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2022-12-30 18:41:06.000000 neugs_utils-0.0.8/neugs_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-30 18:41:05.000000 neugs_utils-0.0.8/neugs_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2022-12-30 18:41:05.000000 neugs_utils-0.0.8/neugs_utils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       42 2022-12-30 18:41:05.000000 neugs_utils-0.0.8/neugs_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2022-12-30 18:41:05.000000 neugs_utils-0.0.8/neugs_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      824 2022-12-30 18:39:58.000000 neugs_utils-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      357 2022-12-30 18:40:47.000000 neugs_utils-0.0.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2022-12-30 18:41:06.168059 neugs_utils-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-12-30 18:41:06.159058 neugs_utils-0.0.8/tests/
+drwxrwxrwx   0        0        0        0 2022-12-30 18:41:06.165061 neugs_utils-0.0.8/tests/examples/
+-rw-rw-rw-   0        0        0     1355 2022-12-12 15:58:35.000000 neugs_utils-0.0.8/tests/examples/test_one.py
+-rw-rw-rw-   0        0        0      428 2022-12-12 17:02:39.000000 neugs_utils-0.0.8/tests/run_tests.py
```

### Comparing `neugs_utils-0.0.7/.gitignore` & `neugs_utils-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `neugs_utils-0.0.7/LICENSE` & `neugs_utils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `neugs_utils-0.0.7/PKG-INFO` & `neugs_utils-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neugs_utils
-Version: 0.0.7
+Version: 0.0.8
 Summary: Alternative Grading Options for Gradescope autograder
 Author-email: Albert Lionelle <lionelle+neugs-utils@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2022 Albert Lionelle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `neugs_utils-0.0.7/README.md` & `neugs_utils-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `neugs_utils-0.0.7/neugs_utils/__init__.py` & `neugs_utils-0.0.8/neugs_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neugs_utils-0.0.7/neugs_utils/common_tests.py` & `neugs_utils-0.0.8/neugs_utils/common_tests.py`

 * *Files identical despite different names*

### Comparing `neugs_utils-0.0.7/neugs_utils/context_managers.py` & `neugs_utils-0.0.8/neugs_utils/context_managers.py`

 * *Files identical despite different names*

### Comparing `neugs_utils-0.0.7/neugs_utils/scripts/build_autograder.py` & `neugs_utils-0.0.8/neugs_utils/scripts/build_autograder.py`

 * *Files identical despite different names*

### Comparing `neugs_utils-0.0.7/neugs_utils/scripts/test_utils.py` & `neugs_utils-0.0.8/neugs_utils/scripts/test_utils.py`

 * *Files identical despite different names*

### Comparing `neugs_utils-0.0.7/neugs_utils/tier_grading.py` & `neugs_utils-0.0.8/neugs_utils/tier_grading.py`

 * *Files identical despite different names*

### Comparing `neugs_utils-0.0.7/neugs_utils.egg-info/PKG-INFO` & `neugs_utils-0.0.8/neugs_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neugs-utils
-Version: 0.0.7
+Version: 0.0.8
 Summary: Alternative Grading Options for Gradescope autograder
 Author-email: Albert Lionelle <lionelle+neugs-utils@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2022 Albert Lionelle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `neugs_utils-0.0.7/neugs_utils.egg-info/SOURCES.txt` & `neugs_utils-0.0.8/neugs_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neugs_utils-0.0.7/pyproject.toml` & `neugs_utils-0.0.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "gradescope-utils >= 0.3.1", 
     "pycodestyle",
     "click",
 ]
 
 name = "neugs_utils"
 description = "Alternative Grading Options for Gradescope autograder"
-version = "0.0.7"
+version = "0.0.8"
 authors = [{name = "Albert Lionelle", email = "lionelle+neugs-utils@gmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
```

### Comparing `neugs_utils-0.0.7/tests/examples/test_one.py` & `neugs_utils-0.0.8/tests/examples/test_one.py`

 * *Files identical despite different names*

