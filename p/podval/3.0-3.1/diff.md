# Comparing `tmp/podval-3.0.tar.gz` & `tmp/podval-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\podval-3.0.tar", last modified: Wed Jun 14 09:34:42 2023, max compression
+gzip compressed data, was "dist\podval-3.1.tar", last modified: Wed Jun 14 09:45:14 2023, max compression
```

## Comparing `podval-3.0.tar` & `podval-3.1.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 09:34:42.000000 podval-3.0/
--rw-rw-rw-   0        0        0      188 2023-06-14 09:34:42.000000 podval-3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 09:34:42.000000 podval-3.0/exam/
--rw-rw-rw-   0        0        0    28965 2023-06-14 09:28:18.000000 podval-3.0/exam/exam.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:34:42.000000 podval-3.0/podval/
--rw-rw-rw-   0        0        0    28965 2023-06-14 09:28:18.000000 podval-3.0/podval/exam.py
--rw-rw-rw-   0        0        0   111373 2023-06-04 19:49:44.000000 podval-3.0/podval/podval.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:34:42.000000 podval-3.0/podval.egg-info/
--rw-rw-rw-   0        0        0      188 2023-06-14 09:34:41.000000 podval-3.0/podval.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-06-14 09:34:41.000000 podval-3.0/podval.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 09:34:41.000000 podval-3.0/podval.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-03 21:34:23.000000 podval-3.0/podval.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-06-14 09:34:41.000000 podval-3.0/podval.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 09:34:42.000000 podval-3.0/setup.cfg
--rw-rw-rw-   0        0        0      180 2023-06-14 09:12:11.000000 podval-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:45:14.000000 podval-3.1/
+-rw-rw-rw-   0        0        0      188 2023-06-14 09:45:14.000000 podval-3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 09:45:14.000000 podval-3.1/podval/
+-rw-rw-rw-   0        0        0    28965 2023-06-14 09:28:18.000000 podval-3.1/podval/exam.py
+-rw-rw-rw-   0        0        0   111373 2023-06-04 19:49:44.000000 podval-3.1/podval/podval.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:45:14.000000 podval-3.1/podval.egg-info/
+-rw-rw-rw-   0        0        0      188 2023-06-14 09:45:14.000000 podval-3.1/podval.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-06-14 09:45:14.000000 podval-3.1/podval.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 09:45:14.000000 podval-3.1/podval.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-03 21:34:23.000000 podval-3.1/podval.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-14 09:45:14.000000 podval-3.1/podval.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 09:45:14.000000 podval-3.1/setup.cfg
+-rw-rw-rw-   0        0        0      173 2023-06-14 09:44:56.000000 podval-3.1/setup.py
```

### Comparing `podval-3.0/exam/exam.py` & `podval-3.1/podval/exam.py`

 * *Files identical despite different names*

### Comparing `podval-3.0/podval/podval.py` & `podval-3.1/podval/podval.py`

 * *Files identical despite different names*

