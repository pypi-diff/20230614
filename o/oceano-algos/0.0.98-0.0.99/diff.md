# Comparing `tmp/oceano_algos-0.0.98.tar.gz` & `tmp/oceano_algos-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceano_algos-0.0.98.tar", last modified: Mon Apr 10 08:47:52 2023, max compression
+gzip compressed data, was "oceano_algos-0.0.99.tar", last modified: Sun Apr 23 10:20:58 2023, max compression
```

## Comparing `oceano_algos-0.0.98.tar` & `oceano_algos-0.0.99.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1001)        0 2023-04-10 08:47:52.150232 oceano_algos-0.0.98/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      110 2023-01-17 20:50:26.000000 oceano_algos-0.0.98/MANIFEST.in
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      119 2023-04-10 08:47:52.150232 oceano_algos-0.0.98/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      886 2023-01-22 15:00:56.000000 oceano_algos-0.0.98/README.md
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1001)        0 2023-04-10 08:47:52.150232 oceano_algos-0.0.98/oceano_algos/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)       23 2023-04-10 08:47:46.000000 oceano_algos-0.0.98/oceano_algos/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)     2800 2023-04-10 08:47:46.000000 oceano_algos-0.0.98/oceano_algos/_nbdev.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      209 2023-04-10 08:47:46.000000 oceano_algos-0.0.98/oceano_algos/core.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)    11617 2023-04-10 08:47:46.000000 oceano_algos-0.0.98/oceano_algos/hh_parser.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)    10162 2023-04-10 08:47:46.000000 oceano_algos-0.0.98/oceano_algos/notificator.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)    32653 2023-04-10 08:47:46.000000 oceano_algos-0.0.98/oceano_algos/parser.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)     7049 2023-04-10 08:47:46.000000 oceano_algos-0.0.98/oceano_algos/postgres.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)     2492 2023-04-10 08:47:46.000000 oceano_algos-0.0.98/oceano_algos/preprocessor.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1001)        0 2023-04-10 08:47:52.150232 oceano_algos-0.0.98/oceano_algos.egg-info/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      119 2023-04-10 08:47:52.000000 oceano_algos-0.0.98/oceano_algos.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      422 2023-04-10 08:47:52.000000 oceano_algos-0.0.98/oceano_algos.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)        1 2023-04-10 08:47:52.000000 oceano_algos-0.0.98/oceano_algos.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      200 2023-04-10 08:47:52.000000 oceano_algos-0.0.98/oceano_algos.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)       13 2023-04-10 08:47:52.000000 oceano_algos-0.0.98/oceano_algos.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      651 2023-04-10 08:44:41.000000 oceano_algos-0.0.98/settings.ini
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)       38 2023-04-10 08:47:52.150232 oceano_algos-0.0.98/setup.cfg
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      670 2023-04-10 08:47:47.000000 oceano_algos-0.0.98/setup.py
+drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1001)        0 2023-04-23 10:20:58.582902 oceano_algos-0.0.99/
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      110 2023-01-17 20:50:26.000000 oceano_algos-0.0.99/MANIFEST.in
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      119 2023-04-23 10:20:58.582902 oceano_algos-0.0.99/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      886 2023-01-22 15:00:56.000000 oceano_algos-0.0.99/README.md
+drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1001)        0 2023-04-23 10:20:58.582902 oceano_algos-0.0.99/oceano_algos/
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)       23 2023-04-23 10:20:51.000000 oceano_algos-0.0.99/oceano_algos/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)     1318 2023-04-23 10:20:51.000000 oceano_algos-0.0.99/oceano_algos/_nbdev.py
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      209 2023-04-23 10:20:51.000000 oceano_algos-0.0.99/oceano_algos/core.py
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)    11617 2023-04-23 10:20:51.000000 oceano_algos-0.0.99/oceano_algos/hh_parser.py
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)    10162 2023-04-23 10:20:51.000000 oceano_algos-0.0.99/oceano_algos/notificator.py
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)    32653 2023-04-23 10:20:51.000000 oceano_algos-0.0.99/oceano_algos/parser.py
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)     7049 2023-04-23 10:20:51.000000 oceano_algos-0.0.99/oceano_algos/postgres.py
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)     2492 2023-04-23 10:20:51.000000 oceano_algos-0.0.99/oceano_algos/preprocessor.py
+drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1001)        0 2023-04-23 10:20:58.582902 oceano_algos-0.0.99/oceano_algos.egg-info/
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      119 2023-04-23 10:20:58.000000 oceano_algos-0.0.99/oceano_algos.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      422 2023-04-23 10:20:58.000000 oceano_algos-0.0.99/oceano_algos.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)        1 2023-04-23 10:20:58.000000 oceano_algos-0.0.99/oceano_algos.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      200 2023-04-23 10:20:58.000000 oceano_algos-0.0.99/oceano_algos.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)       13 2023-04-23 10:20:58.000000 oceano_algos-0.0.99/oceano_algos.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      651 2023-04-23 10:19:36.000000 oceano_algos-0.0.99/settings.ini
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)       38 2023-04-23 10:20:58.582902 oceano_algos-0.0.99/setup.cfg
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      670 2023-04-23 10:20:53.000000 oceano_algos-0.0.99/setup.py
```

### Comparing `oceano_algos-0.0.98/README.md` & `oceano_algos-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `oceano_algos-0.0.98/oceano_algos/hh_parser.py` & `oceano_algos-0.0.99/oceano_algos/hh_parser.py`

 * *Files identical despite different names*

### Comparing `oceano_algos-0.0.98/oceano_algos/notificator.py` & `oceano_algos-0.0.99/oceano_algos/notificator.py`

 * *Files identical despite different names*

### Comparing `oceano_algos-0.0.98/oceano_algos/parser.py` & `oceano_algos-0.0.99/oceano_algos/parser.py`

 * *Files identical despite different names*

### Comparing `oceano_algos-0.0.98/oceano_algos/postgres.py` & `oceano_algos-0.0.99/oceano_algos/postgres.py`

 * *Files identical despite different names*

### Comparing `oceano_algos-0.0.98/oceano_algos/preprocessor.py` & `oceano_algos-0.0.99/oceano_algos/preprocessor.py`

 * *Files identical despite different names*

### Comparing `oceano_algos-0.0.98/settings.ini` & `oceano_algos-0.0.99/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 description = A description of your project
 long_description = Long description text
 keywords = some keywords for pypi search
 author = mrtweety123
 author_email = mrtweety123@proton.me
 copyright = some copyright information
 branch = main
-version = 0.0.98
+version = 0.0.99
 min_python = 3.6
 audience = Developers
 language = English
 custom_sidebar = False
 license = some license
 status = 2
 nbs_path = nbs
```

### Comparing `oceano_algos-0.0.98/setup.py` & `oceano_algos-0.0.99/setup.py`

 * *Files identical despite different names*

