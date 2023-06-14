# Comparing `tmp/pythorhead-0.0.3.tar.gz` & `tmp/pythorhead-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythorhead-0.0.3.tar", last modified: Wed Jun 14 21:39:58 2023, max compression
+gzip compressed data, was "pythorhead-0.0.4.tar", last modified: Wed Jun 14 21:43:22 2023, max compression
```

## Comparing `pythorhead-0.0.3.tar` & `pythorhead-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:39:58.287478 pythorhead-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:39:58.283478 pythorhead-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:39:58.287478 pythorhead-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-14 21:39:43.000000 pythorhead-0.0.3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-14 21:39:43.000000 pythorhead-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-14 21:39:47.000000 pythorhead-0.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-14 21:39:43.000000 pythorhead-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40688 2023-06-14 21:39:58.287478 pythorhead-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-14 21:39:43.000000 pythorhead-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-14 21:39:43.000000 pythorhead-0.0.3/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-14 21:39:48.000000 pythorhead-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:39:58.287478 pythorhead-0.0.3/pythorhead/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 21:39:43.000000 pythorhead-0.0.3/pythorhead/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-14 21:39:43.000000 pythorhead-0.0.3/pythorhead/lemmy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:39:58.287478 pythorhead-0.0.3/pythorhead.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40688 2023-06-14 21:39:58.000000 pythorhead-0.0.3/pythorhead.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-14 21:39:58.000000 pythorhead-0.0.3/pythorhead.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:39:58.000000 pythorhead-0.0.3/pythorhead.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 21:39:58.000000 pythorhead-0.0.3/pythorhead.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:39:58.287478 pythorhead-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:22.388036 pythorhead-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:22.384036 pythorhead-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:22.388036 pythorhead-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-14 21:42:58.000000 pythorhead-0.0.4/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-14 21:42:58.000000 pythorhead-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-14 21:43:04.000000 pythorhead-0.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-14 21:42:58.000000 pythorhead-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40742 2023-06-14 21:43:22.388036 pythorhead-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-14 21:42:58.000000 pythorhead-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-14 21:42:58.000000 pythorhead-0.0.4/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-14 21:43:04.000000 pythorhead-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:22.388036 pythorhead-0.0.4/pythorhead/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 21:42:58.000000 pythorhead-0.0.4/pythorhead/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-14 21:42:58.000000 pythorhead-0.0.4/pythorhead/lemmy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:22.388036 pythorhead-0.0.4/pythorhead.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40742 2023-06-14 21:43:22.000000 pythorhead-0.0.4/pythorhead.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-14 21:43:22.000000 pythorhead-0.0.4/pythorhead.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:43:22.000000 pythorhead-0.0.4/pythorhead.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 21:43:22.000000 pythorhead-0.0.4/pythorhead.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:43:22.388036 pythorhead-0.0.4/setup.cfg
```

### Comparing `pythorhead-0.0.3/.github/workflows/pypi.yml` & `pythorhead-0.0.4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pythorhead-0.0.3/.gitignore` & `pythorhead-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pythorhead-0.0.3/CHANGELOG.md` & `pythorhead-0.0.4/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## [v0.0.4](https://github.com/db0/pythorhead/tree/v0.0.4) (2023-06-14)
+
+[Full Changelog](https://github.com/db0/pythorhead/compare/v0.0.3...v0.0.4)
+
 ## [v0.0.3](https://github.com/db0/pythorhead/tree/v0.0.3) (2023-06-14)
 
 [Full Changelog](https://github.com/db0/pythorhead/compare/v0.0.2...v0.0.3)
 
 ## [v0.0.2](https://github.com/db0/pythorhead/tree/v0.0.2) (2023-06-14)
 
 [Full Changelog](https://github.com/db0/pythorhead/compare/0.0.1...v0.0.2)
```

### Comparing `pythorhead-0.0.3/LICENSE` & `pythorhead-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pythorhead-0.0.3/PKG-INFO` & `pythorhead-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -675,15 +675,15 @@
 License-File: LICENSE
 License-File: CHANGELOG.md
 
 # Pythörhead
 
 A python library for interacting with Lemmy
 
-![pythorhead logo](logo.png)
+![pythorhead logo](https://raw.githubusercontent.com/db0/pythorhead/main/logo.png)
 
 # Sample Usage
 
 ```python
 from pythorhead import Lemmy
 
 lemmy = Lemmy("https://lemmy.dbzer0.com")
```

### Comparing `pythorhead-0.0.3/logo.png` & `pythorhead-0.0.4/logo.png`

 * *Files identical despite different names*

### Comparing `pythorhead-0.0.3/pyproject.toml` & `pythorhead-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "pythorhead"
 description = "A python library for interacting with Lemmy API"
 authors = [
     {name = "db0", email = "mail@dbzer0.com"},
 ]
-version = "v0.0.3"
+version = "v0.0.4"
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
 license = { file="LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
```

### Comparing `pythorhead-0.0.3/pythorhead/lemmy.py` & `pythorhead-0.0.4/pythorhead/lemmy.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.0.3/pythorhead.egg-info/PKG-INFO` & `pythorhead-0.0.4/pythorhead.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -675,15 +675,15 @@
 License-File: LICENSE
 License-File: CHANGELOG.md
 
 # Pythörhead
 
 A python library for interacting with Lemmy
 
-![pythorhead logo](logo.png)
+![pythorhead logo](https://raw.githubusercontent.com/db0/pythorhead/main/logo.png)
 
 # Sample Usage
 
 ```python
 from pythorhead import Lemmy
 
 lemmy = Lemmy("https://lemmy.dbzer0.com")
```

