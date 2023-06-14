# Comparing `tmp/drf-simplejwt-additions-1.0.0.tar.gz` & `tmp/drf-simplejwt-additions-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-simplejwt-additions-1.0.0.tar", last modified: Wed Jun 14 05:39:55 2023, max compression
+gzip compressed data, was "drf-simplejwt-additions-1.0.1.tar", last modified: Wed Jun 14 06:03:02 2023, max compression
```

## Comparing `drf-simplejwt-additions-1.0.0.tar` & `drf-simplejwt-additions-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-14 05:39:55.929319 drf-simplejwt-additions-1.0.0/
--rw-r--r--   0 rustam     (501) staff       (20)       33 2023-06-14 05:28:46.000000 drf-simplejwt-additions-1.0.0/MANIFEST.in
--rw-r--r--   0 rustam     (501) staff       (20)     1140 2023-06-14 05:39:55.929425 drf-simplejwt-additions-1.0.0/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)       25 2023-06-14 05:33:49.000000 drf-simplejwt-additions-1.0.0/README.md
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-14 05:39:55.900141 drf-simplejwt-additions-1.0.0/drf_simplejwt_additions/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2023-06-14 05:29:58.000000 drf-simplejwt-additions-1.0.0/drf_simplejwt_additions/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)      581 2023-06-14 05:37:54.000000 drf-simplejwt-additions-1.0.0/drf_simplejwt_additions/serializers.py
--rw-r--r--   0 rustam     (501) staff       (20)      272 2023-06-14 05:37:54.000000 drf-simplejwt-additions-1.0.0/drf_simplejwt_additions/views.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-14 05:39:55.929110 drf-simplejwt-additions-1.0.0/drf_simplejwt_additions.egg-info/
--rw-r--r--   0 rustam     (501) staff       (20)     1140 2023-06-14 05:39:55.000000 drf-simplejwt-additions-1.0.0/drf_simplejwt_additions.egg-info/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)      382 2023-06-14 05:39:55.000000 drf-simplejwt-additions-1.0.0/drf_simplejwt_additions.egg-info/SOURCES.txt
--rw-r--r--   0 rustam     (501) staff       (20)        1 2023-06-14 05:39:55.000000 drf-simplejwt-additions-1.0.0/drf_simplejwt_additions.egg-info/dependency_links.txt
--rw-r--r--   0 rustam     (501) staff       (20)       62 2023-06-14 05:39:55.000000 drf-simplejwt-additions-1.0.0/drf_simplejwt_additions.egg-info/requires.txt
--rw-r--r--   0 rustam     (501) staff       (20)       24 2023-06-14 05:39:55.000000 drf-simplejwt-additions-1.0.0/drf_simplejwt_additions.egg-info/top_level.txt
--rw-r--r--   0 rustam     (501) staff       (20)     1079 2023-06-14 05:39:55.929877 drf-simplejwt-additions-1.0.0/setup.cfg
--rw-r--r--   0 rustam     (501) staff       (20)      195 2023-06-14 05:28:46.000000 drf-simplejwt-additions-1.0.0/setup.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-14 06:03:02.055307 drf-simplejwt-additions-1.0.1/
+-rw-r--r--   0 rustam     (501) staff       (20)       33 2023-06-14 05:28:46.000000 drf-simplejwt-additions-1.0.1/MANIFEST.in
+-rw-r--r--   0 rustam     (501) staff       (20)     2559 2023-06-14 06:03:02.055428 drf-simplejwt-additions-1.0.1/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)     1444 2023-06-14 06:02:14.000000 drf-simplejwt-additions-1.0.1/README.md
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-14 06:03:02.028419 drf-simplejwt-additions-1.0.1/drf_simplejwt_additions/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2023-06-14 05:29:58.000000 drf-simplejwt-additions-1.0.1/drf_simplejwt_additions/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)      581 2023-06-14 05:37:54.000000 drf-simplejwt-additions-1.0.1/drf_simplejwt_additions/serializers.py
+-rw-r--r--   0 rustam     (501) staff       (20)      272 2023-06-14 05:37:54.000000 drf-simplejwt-additions-1.0.1/drf_simplejwt_additions/views.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-14 06:03:02.055051 drf-simplejwt-additions-1.0.1/drf_simplejwt_additions.egg-info/
+-rw-r--r--   0 rustam     (501) staff       (20)     2559 2023-06-14 06:03:02.000000 drf-simplejwt-additions-1.0.1/drf_simplejwt_additions.egg-info/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)      382 2023-06-14 06:03:02.000000 drf-simplejwt-additions-1.0.1/drf_simplejwt_additions.egg-info/SOURCES.txt
+-rw-r--r--   0 rustam     (501) staff       (20)        1 2023-06-14 06:03:02.000000 drf-simplejwt-additions-1.0.1/drf_simplejwt_additions.egg-info/dependency_links.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       62 2023-06-14 06:03:02.000000 drf-simplejwt-additions-1.0.1/drf_simplejwt_additions.egg-info/requires.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       24 2023-06-14 06:03:02.000000 drf-simplejwt-additions-1.0.1/drf_simplejwt_additions.egg-info/top_level.txt
+-rw-r--r--   0 rustam     (501) staff       (20)     1079 2023-06-14 06:03:02.055956 drf-simplejwt-additions-1.0.1/setup.cfg
+-rw-r--r--   0 rustam     (501) staff       (20)      195 2023-06-14 05:28:46.000000 drf-simplejwt-additions-1.0.1/setup.py
```

### Comparing `drf-simplejwt-additions-1.0.0/drf_simplejwt_additions/serializers.py` & `drf-simplejwt-additions-1.0.1/drf_simplejwt_additions/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-simplejwt-additions-1.0.0/setup.cfg` & `drf-simplejwt-additions-1.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = drf-simplejwt-additions
-version = 1.0.0
+version = 1.0.1
 description = Additions for Django Rest Framework Simple JWT
 url = https://github.com/AllYouZombies/drf-simplejwt-additions
 author = Astafeev Rustam
 author_email = rustam@astafeev.dev
 license = MIT License
 classifiers = 
 	Environment :: Web Environment
```

