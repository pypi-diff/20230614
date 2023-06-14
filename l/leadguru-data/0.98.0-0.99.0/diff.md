# Comparing `tmp/leadguru_data-0.98.0.tar.gz` & `tmp/leadguru_data-0.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/workspace/python/lgt-data/dist/tmpwxyummhp/leadguru_data-0.98.0.tar", last modified: Thu Jul 15 07:36:38 2021, max compression
+gzip compressed data, was "/workspace/python/lgt-data/dist/tmpcpldmi22/leadguru_data-0.99.0.tar", last modified: Tue Jul 20 07:00:39 2021, max compression
```

## Comparing `leadguru_data-0.98.0.tar` & `leadguru_data-0.99.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 07:36:38.000000 leadguru_data-0.98.0/
--rw-r--r--   0 root         (0) root         (0)       38 2021-07-15 07:35:57.000000 leadguru_data-0.98.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      183 2021-07-15 07:36:38.000000 leadguru_data-0.98.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 07:36:38.000000 leadguru_data-0.98.0/leadguru_data.egg-info/
--rw-r--r--   0 root         (0) root         (0)      183 2021-07-15 07:36:38.000000 leadguru_data-0.98.0/leadguru_data.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      318 2021-07-15 07:36:38.000000 leadguru_data-0.98.0/leadguru_data.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-15 07:36:38.000000 leadguru_data-0.98.0/leadguru_data.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-15 07:36:38.000000 leadguru_data-0.98.0/leadguru_data.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       41 2021-07-15 07:36:38.000000 leadguru_data-0.98.0/leadguru_data.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2021-07-15 07:36:38.000000 leadguru_data-0.98.0/leadguru_data.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-15 07:36:38.000000 leadguru_data-0.98.0/lgt_data/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-15 07:35:57.000000 leadguru_data-0.98.0/lgt_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12319 2021-07-15 07:35:57.000000 leadguru_data-0.98.0/lgt_data/model.py
--rw-r--r--   0 root         (0) root         (0)    30385 2021-07-15 07:35:57.000000 leadguru_data-0.98.0/lgt_data/mongo_repository.py
--rw-r--r--   0 root         (0) root         (0)       38 2021-07-15 07:36:38.000000 leadguru_data-0.98.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      837 2021-07-15 07:35:57.000000 leadguru_data-0.98.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-20 07:00:39.000000 leadguru_data-0.99.0/
+-rw-r--r--   0 root         (0) root         (0)       38 2021-07-20 06:59:58.000000 leadguru_data-0.99.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      183 2021-07-20 07:00:39.000000 leadguru_data-0.99.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-20 07:00:39.000000 leadguru_data-0.99.0/leadguru_data.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      183 2021-07-20 07:00:39.000000 leadguru_data-0.99.0/leadguru_data.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      318 2021-07-20 07:00:39.000000 leadguru_data-0.99.0/leadguru_data.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-07-20 07:00:39.000000 leadguru_data-0.99.0/leadguru_data.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-07-20 07:00:38.000000 leadguru_data-0.99.0/leadguru_data.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       41 2021-07-20 07:00:39.000000 leadguru_data-0.99.0/leadguru_data.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2021-07-20 07:00:39.000000 leadguru_data-0.99.0/leadguru_data.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-20 07:00:39.000000 leadguru_data-0.99.0/lgt_data/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-20 06:59:58.000000 leadguru_data-0.99.0/lgt_data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12319 2021-07-20 06:59:58.000000 leadguru_data-0.99.0/lgt_data/model.py
+-rw-r--r--   0 root         (0) root         (0)    30385 2021-07-20 06:59:58.000000 leadguru_data-0.99.0/lgt_data/mongo_repository.py
+-rw-r--r--   0 root         (0) root         (0)       38 2021-07-20 07:00:39.000000 leadguru_data-0.99.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      837 2021-07-20 06:59:58.000000 leadguru_data-0.99.0/setup.py
```

### Comparing `leadguru_data-0.98.0/lgt_data/model.py` & `leadguru_data-0.99.0/lgt_data/model.py`

 * *Files identical despite different names*

### Comparing `leadguru_data-0.98.0/lgt_data/mongo_repository.py` & `leadguru_data-0.99.0/lgt_data/mongo_repository.py`

 * *Files identical despite different names*

### Comparing `leadguru_data-0.98.0/setup.py` & `leadguru_data-0.99.0/setup.py`

 * *Files identical despite different names*

