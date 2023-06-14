# Comparing `tmp/cstore-0.3.0.tar.gz` & `tmp/cstore-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cstore-0.3.0.tar", last modified: Wed Jun 14 11:09:53 2023, max compression
+gzip compressed data, was "cstore-0.3.1.tar", last modified: Wed Jun 14 11:15:49 2023, max compression
```

## Comparing `cstore-0.3.0.tar` & `cstore-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 11:09:53.081736 cstore-0.3.0/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1073 2023-06-14 08:18:09.000000 cstore-0.3.0/LICENSE
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-14 11:09:53.081736 cstore-0.3.0/PKG-INFO
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      115 2023-06-14 08:22:10.000000 cstore-0.3.0/README.md
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      836 2023-06-14 11:07:29.000000 cstore-0.3.0/pyproject.toml
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       38 2023-06-14 11:09:53.081736 cstore-0.3.0/setup.cfg
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 11:09:53.081736 cstore-0.3.0/src/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       40 2023-06-14 09:15:54.000000 cstore-0.3.0/src/__init__.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      148 2023-06-14 09:54:08.000000 cstore-0.3.0/src/cli_module.py
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 11:09:53.081736 cstore-0.3.0/src/cstore.egg-info/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-14 11:09:53.000000 cstore-0.3.0/src/cstore.egg-info/PKG-INFO
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      272 2023-06-14 11:09:53.000000 cstore-0.3.0/src/cstore.egg-info/SOURCES.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        1 2023-06-14 11:09:53.000000 cstore-0.3.0/src/cstore.egg-info/dependency_links.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       50 2023-06-14 11:09:53.000000 cstore-0.3.0/src/cstore.egg-info/entry_points.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        6 2023-06-14 11:09:53.000000 cstore-0.3.0/src/cstore.egg-info/requires.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       20 2023-06-14 11:09:53.000000 cstore-0.3.0/src/cstore.egg-info/top_level.txt
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 11:15:49.141377 cstore-0.3.1/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1073 2023-06-14 08:18:09.000000 cstore-0.3.1/LICENSE
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-14 11:15:49.141377 cstore-0.3.1/PKG-INFO
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      115 2023-06-14 08:22:10.000000 cstore-0.3.1/README.md
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      828 2023-06-14 11:15:35.000000 cstore-0.3.1/pyproject.toml
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       38 2023-06-14 11:15:49.141377 cstore-0.3.1/setup.cfg
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 11:15:49.141377 cstore-0.3.1/src/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 11:12:45.000000 cstore-0.3.1/src/__init__.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      148 2023-06-14 09:54:08.000000 cstore-0.3.1/src/cli.py
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 11:15:49.141377 cstore-0.3.1/src/cstore.egg-info/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-14 11:15:49.000000 cstore-0.3.1/src/cstore.egg-info/PKG-INFO
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      265 2023-06-14 11:15:49.000000 cstore-0.3.1/src/cstore.egg-info/SOURCES.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        1 2023-06-14 11:15:49.000000 cstore-0.3.1/src/cstore.egg-info/dependency_links.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       42 2023-06-14 11:15:49.000000 cstore-0.3.1/src/cstore.egg-info/entry_points.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        6 2023-06-14 11:15:49.000000 cstore-0.3.1/src/cstore.egg-info/requires.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       13 2023-06-14 11:15:49.000000 cstore-0.3.1/src/cstore.egg-info/top_level.txt
```

### Comparing `cstore-0.3.0/LICENSE` & `cstore-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cstore-0.3.0/PKG-INFO` & `cstore-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cstore
-Version: 0.3.0
+Version: 0.3.1
 Summary: A tools to store and recall useful commands, specifically created to assist forgetful individuals
 Author-email: Navid Arabi <navidved@gmail.com>
 Project-URL: Homepage, https://github.com/navidved/ctore
 Project-URL: Bug Tracker, https://github.com/navidved/ctore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cstore-0.3.0/pyproject.toml` & `cstore-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "rich"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cstore"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
     "typer",
 ]
 authors = [
   { name="Navid Arabi", email="navidved@gmail.com" },
 ]
 description = "A tools to store and recall useful commands, specifically created to assist forgetful individuals"
@@ -29,8 +29,8 @@
 zip_safe = true
 include_package_data = true
 
 [options.packages.find]
 where="src"
 
 [project.scripts]
-cstore = "cstore.cli_module:main"
+cstore = "cstore.cli:app"
```

### Comparing `cstore-0.3.0/src/cstore.egg-info/PKG-INFO` & `cstore-0.3.1/src/cstore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cstore
-Version: 0.3.0
+Version: 0.3.1
 Summary: A tools to store and recall useful commands, specifically created to assist forgetful individuals
 Author-email: Navid Arabi <navidved@gmail.com>
 Project-URL: Homepage, https://github.com/navidved/ctore
 Project-URL: Bug Tracker, https://github.com/navidved/ctore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

