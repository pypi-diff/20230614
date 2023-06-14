# Comparing `tmp/bmw-lobster-0.9.4.tar.gz` & `tmp/bmw-lobster-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-0.9.4.tar", last modified: Tue Jun 13 09:18:58 2023, max compression
+gzip compressed data, was "bmw-lobster-0.9.5.tar", last modified: Wed Jun 14 14:03:21 2023, max compression
```

## Comparing `bmw-lobster-0.9.4.tar` & `bmw-lobster-0.9.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:58.397266 bmw-lobster-0.9.4/
--rw-r--r--   0 florian   (1000) florian   (1000)     2079 2023-06-13 09:18:58.397266 bmw-lobster-0.9.4/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1142 2023-06-13 09:17:37.000000 bmw-lobster-0.9.4/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:58.397266 bmw-lobster-0.9.4/bmw_lobster.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     2079 2023-06-13 09:18:58.000000 bmw-lobster-0.9.4/bmw_lobster.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      192 2023-06-13 09:18:58.000000 bmw-lobster-0.9.4/bmw_lobster.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-13 09:18:58.000000 bmw-lobster-0.9.4/bmw_lobster.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      223 2023-06-13 09:18:58.000000 bmw-lobster-0.9.4/bmw_lobster.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-13 09:18:58.000000 bmw-lobster-0.9.4/bmw_lobster.egg-info/top_level.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-13 09:18:58.397266 bmw-lobster-0.9.4/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2334 2023-06-13 09:17:37.000000 bmw-lobster-0.9.4/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:21.265671 bmw-lobster-0.9.5/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2079 2023-06-14 14:03:21.265671 bmw-lobster-0.9.5/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1142 2023-06-13 09:17:37.000000 bmw-lobster-0.9.5/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:21.265671 bmw-lobster-0.9.5/bmw_lobster.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2079 2023-06-14 14:03:21.000000 bmw-lobster-0.9.5/bmw_lobster.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      192 2023-06-14 14:03:21.000000 bmw-lobster-0.9.5/bmw_lobster.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-14 14:03:21.000000 bmw-lobster-0.9.5/bmw_lobster.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      223 2023-06-14 14:03:21.000000 bmw-lobster-0.9.5/bmw_lobster.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-14 14:03:21.000000 bmw-lobster-0.9.5/bmw_lobster.egg-info/top_level.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-14 14:03:21.265671 bmw-lobster-0.9.5/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2334 2023-06-13 09:17:37.000000 bmw-lobster-0.9.5/setup.py
```

### Comparing `bmw-lobster-0.9.4/PKG-INFO` & `bmw-lobster-0.9.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster
-Version: 0.9.4
+Version: 0.9.5
 Summary: Metapackage to install all LOBSTER Tools
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-0.9.4/README.md` & `bmw-lobster-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-0.9.4/bmw_lobster.egg-info/PKG-INFO` & `bmw-lobster-0.9.5/bmw_lobster.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster
-Version: 0.9.4
+Version: 0.9.5
 Summary: Metapackage to install all LOBSTER Tools
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-0.9.4/setup.py` & `bmw-lobster-0.9.5/setup.py`

 * *Files identical despite different names*

