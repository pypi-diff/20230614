# Comparing `tmp/dart-tools-0.3.6.tar.gz` & `tmp/dart-tools-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dart-tools-0.3.6.tar", last modified: Tue Jun 13 00:08:00 2023, max compression
+gzip compressed data, was "dart-tools-0.3.7.tar", last modified: Wed Jun 14 01:49:08 2023, max compression
```

## Comparing `dart-tools-0.3.6.tar` & `dart-tools-0.3.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-13 00:08:00.188567 dart-tools-0.3.6/
--rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.3.6/LICENSE
--rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-13 00:08:00.187997 dart-tools-0.3.6/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.3.6/README.md
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-13 00:08:00.182590 dart-tools-0.3.6/dart/
--rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.3.6/dart/__init__.py
--rwxr-xr-x   0 zack       (501) staff       (20)    17148 2023-06-13 00:05:45.000000 dart-tools-0.3.6/dart/dart.py
--rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.3.6/dart/order_manager.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-13 00:08:00.185812 dart-tools-0.3.6/dart_tools.egg-info/
--rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-13 00:08:00.000000 dart-tools-0.3.6/dart_tools.egg-info/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)      339 2023-06-13 00:08:00.000000 dart-tools-0.3.6/dart_tools.egg-info/SOURCES.txt
--rw-r--r--   0 zack       (501) staff       (20)        1 2023-06-13 00:08:00.000000 dart-tools-0.3.6/dart_tools.egg-info/dependency_links.txt
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-13 00:08:00.186657 dart-tools-0.3.6/dart_tools.egg-info/dist/
--rw-r--r--   0 zack       (501) staff       (20)     8788 2023-06-03 08:11:34.000000 dart-tools-0.3.6/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz
--rw-r--r--   0 zack       (501) staff       (20)       34 2023-06-13 00:08:00.000000 dart-tools-0.3.6/dart_tools.egg-info/entry_points.txt
--rw-r--r--   0 zack       (501) staff       (20)       25 2023-06-13 00:08:00.000000 dart-tools-0.3.6/dart_tools.egg-info/requires.txt
--rw-r--r--   0 zack       (501) staff       (20)        5 2023-06-13 00:08:00.000000 dart-tools-0.3.6/dart_tools.egg-info/top_level.txt
--rw-r--r--   0 zack       (501) staff       (20)     1760 2023-06-12 05:46:27.000000 dart-tools-0.3.6/pyproject.toml
--rw-r--r--   0 zack       (501) staff       (20)       38 2023-06-13 00:08:00.188809 dart-tools-0.3.6/setup.cfg
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-14 01:49:08.479313 dart-tools-0.3.7/
+-rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.3.7/LICENSE
+-rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-14 01:49:08.478972 dart-tools-0.3.7/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.3.7/README.md
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-14 01:49:08.473428 dart-tools-0.3.7/dart/
+-rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.3.7/dart/__init__.py
+-rwxr-xr-x   0 zack       (501) staff       (20)    17124 2023-06-14 01:48:05.000000 dart-tools-0.3.7/dart/dart.py
+-rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.3.7/dart/order_manager.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-14 01:49:08.477504 dart-tools-0.3.7/dart_tools.egg-info/
+-rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-14 01:49:08.000000 dart-tools-0.3.7/dart_tools.egg-info/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)      339 2023-06-14 01:49:08.000000 dart-tools-0.3.7/dart_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 zack       (501) staff       (20)        1 2023-06-14 01:49:08.000000 dart-tools-0.3.7/dart_tools.egg-info/dependency_links.txt
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-14 01:49:08.478049 dart-tools-0.3.7/dart_tools.egg-info/dist/
+-rw-r--r--   0 zack       (501) staff       (20)     8788 2023-06-03 08:11:34.000000 dart-tools-0.3.7/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz
+-rw-r--r--   0 zack       (501) staff       (20)       34 2023-06-14 01:49:08.000000 dart-tools-0.3.7/dart_tools.egg-info/entry_points.txt
+-rw-r--r--   0 zack       (501) staff       (20)       25 2023-06-14 01:49:08.000000 dart-tools-0.3.7/dart_tools.egg-info/requires.txt
+-rw-r--r--   0 zack       (501) staff       (20)        5 2023-06-14 01:49:08.000000 dart-tools-0.3.7/dart_tools.egg-info/top_level.txt
+-rw-r--r--   0 zack       (501) staff       (20)     1760 2023-06-14 01:48:17.000000 dart-tools-0.3.7/pyproject.toml
+-rw-r--r--   0 zack       (501) staff       (20)       38 2023-06-14 01:49:08.479432 dart-tools-0.3.7/setup.cfg
```

### Comparing `dart-tools-0.3.6/LICENSE` & `dart-tools-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.6/PKG-INFO` & `dart-tools-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.3.6
+Version: 0.3.7
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.3.6 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.3.7 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.3.6/README.md` & `dart-tools-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.6/dart/dart.py` & `dart-tools-0.3.7/dart/dart.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,14 @@
     status_title=None,
     assignee_emails=None,
     tag_titles=None,
     priority_int=None,
     size_int=None,
     due_at_str=None,
 ):
-    print(priority_int)
     config = _Config()
     session = _Session(config)
 
     user_bundle = _get_full_user_bundle(session)
 
     user = user_bundle["user"]
     user_duid = user["duid"]
```

### Comparing `dart-tools-0.3.6/dart/order_manager.py` & `dart-tools-0.3.7/dart/order_manager.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.6/dart_tools.egg-info/PKG-INFO` & `dart-tools-0.3.7/dart_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.3.6
+Version: 0.3.7
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.3.6 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.3.7 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.3.6/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz` & `dart-tools-0.3.7/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.6/pyproject.toml` & `dart-tools-0.3.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dart-tools"
-version = "0.3.6"
+version = "0.3.7"
 description = "The Dart CLI and Python Library"
 readme = "README.md"
 requires-python = ">=3.8"
 
 license = {file = "LICENSE"}
 keywords = ["dart", "cli", "projectmanagement", "taskmanagement"]
 authors = [
```

