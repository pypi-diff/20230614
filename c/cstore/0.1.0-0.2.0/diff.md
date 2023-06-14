# Comparing `tmp/cstore-0.1.0.tar.gz` & `tmp/cstore-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cstore-0.1.0.tar", last modified: Wed Jun 14 08:19:59 2023, max compression
+gzip compressed data, was "cstore-0.2.0.tar", last modified: Wed Jun 14 09:20:43 2023, max compression
```

## Comparing `cstore-0.1.0.tar` & `cstore-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 08:19:59.822520 cstore-0.1.0/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1073 2023-06-14 08:18:09.000000 cstore-0.1.0/LICENSE
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1318 2023-06-14 08:19:59.822520 cstore-0.1.0/PKG-INFO
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      665 2023-06-14 08:11:19.000000 cstore-0.1.0/README.md
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 08:19:59.822520 cstore-0.1.0/cstore/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       40 2023-06-14 07:25:51.000000 cstore-0.1.0/cstore/__init__.py
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 08:19:59.822520 cstore-0.1.0/cstore.egg-info/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1318 2023-06-14 08:19:59.000000 cstore-0.1.0/cstore.egg-info/PKG-INFO
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      238 2023-06-14 08:19:59.000000 cstore-0.1.0/cstore.egg-info/SOURCES.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        1 2023-06-14 08:19:59.000000 cstore-0.1.0/cstore.egg-info/dependency_links.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        1 2023-06-14 08:17:12.000000 cstore-0.1.0/cstore.egg-info/not-zip-safe
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        5 2023-06-14 08:19:59.000000 cstore-0.1.0/cstore.egg-info/requires.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        7 2023-06-14 08:19:59.000000 cstore-0.1.0/cstore.egg-info/top_level.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      641 2023-06-14 08:18:28.000000 cstore-0.1.0/pyproject.toml
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       38 2023-06-14 08:19:59.822520 cstore-0.1.0/setup.cfg
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      459 2023-06-14 07:43:34.000000 cstore-0.1.0/setup.py
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 09:20:43.045067 cstore-0.2.0/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1073 2023-06-14 08:18:09.000000 cstore-0.2.0/LICENSE
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-14 09:20:43.045067 cstore-0.2.0/PKG-INFO
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      115 2023-06-14 08:22:10.000000 cstore-0.2.0/README.md
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 09:20:43.045067 cstore-0.2.0/cstore/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       40 2023-06-14 09:15:54.000000 cstore-0.2.0/cstore/__init__.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       79 2023-06-14 09:16:00.000000 cstore-0.2.0/cstore/__main__.py
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 09:20:43.045067 cstore-0.2.0/cstore.egg-info/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-14 09:20:43.000000 cstore-0.2.0/cstore.egg-info/PKG-INFO
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      252 2023-06-14 09:20:43.000000 cstore-0.2.0/cstore.egg-info/SOURCES.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        1 2023-06-14 09:20:43.000000 cstore-0.2.0/cstore.egg-info/dependency_links.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       38 2023-06-14 09:20:43.000000 cstore-0.2.0/cstore.egg-info/entry_points.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        5 2023-06-14 09:20:43.000000 cstore-0.2.0/cstore.egg-info/requires.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        7 2023-06-14 09:20:43.000000 cstore-0.2.0/cstore.egg-info/top_level.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      713 2023-06-14 09:20:30.000000 cstore-0.2.0/pyproject.toml
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       38 2023-06-14 09:20:43.045067 cstore-0.2.0/setup.cfg
```

### Comparing `cstore-0.1.0/LICENSE` & `cstore-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cstore-0.1.0/pyproject.toml` & `cstore-0.2.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0", "rich"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cstore"
-version = "0.1.0"
+version = "0.2.0"
+dependencies = [
+    "rich",
+]
 authors = [
   { name="Navid Arabi", email="navidved@gmail.com" },
 ]
 description = "A tools to store and recall useful commands, specifically created to assist forgetful individuals"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/navidved/ctore"
-"Bug Tracker" = "https://github.com/navidved/ctore/issues"
+"Bug Tracker" = "https://github.com/navidved/ctore/issues"
+
+[project.scripts]
+cstore = "cstore.run"
```

