# Comparing `tmp/podval-3.3.tar.gz` & `tmp/podval-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\podval-3.3.tar", last modified: Wed Jun 14 09:58:22 2023, max compression
+gzip compressed data, was "dist\podval-3.4.tar", last modified: Wed Jun 14 10:37:19 2023, max compression
```

## Comparing `podval-3.3.tar` & `podval-3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 09:58:22.000000 podval-3.3/
--rw-rw-rw-   0        0        0      188 2023-06-14 09:58:22.000000 podval-3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 09:58:22.000000 podval-3.3/podval/
--rw-rw-rw-   0        0        0        0 2023-06-14 09:57:54.000000 podval-3.3/podval/__init__.py
--rw-rw-rw-   0        0        0    28965 2023-06-14 09:28:18.000000 podval-3.3/podval/exam.py
--rw-rw-rw-   0        0        0   111373 2023-06-04 19:49:44.000000 podval-3.3/podval/podval.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:58:22.000000 podval-3.3/podval.egg-info/
--rw-rw-rw-   0        0        0      188 2023-06-14 09:58:22.000000 podval-3.3/podval.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-06-14 09:58:22.000000 podval-3.3/podval.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 09:58:22.000000 podval-3.3/podval.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-03 21:34:23.000000 podval-3.3/podval.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-14 09:58:22.000000 podval-3.3/podval.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 09:58:22.000000 podval-3.3/setup.cfg
--rw-rw-rw-   0        0        0      173 2023-06-14 09:58:12.000000 podval-3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 10:37:19.000000 podval-3.4/
+-rw-rw-rw-   0        0        0      188 2023-06-14 10:37:19.000000 podval-3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 10:37:19.000000 podval-3.4/podval/
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:57:54.000000 podval-3.4/podval/__init__.py
+-rw-rw-rw-   0        0        0    50824 2023-06-14 10:26:28.000000 podval-3.4/podval/exam.py
+-rw-rw-rw-   0        0        0   111373 2023-06-04 19:49:44.000000 podval-3.4/podval/podval.py
+drwxrwxrwx   0        0        0        0 2023-06-14 10:37:19.000000 podval-3.4/podval.egg-info/
+-rw-rw-rw-   0        0        0      188 2023-06-14 10:37:19.000000 podval-3.4/podval.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-06-14 10:37:19.000000 podval-3.4/podval.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 10:37:19.000000 podval-3.4/podval.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-03 21:34:23.000000 podval-3.4/podval.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-14 10:37:19.000000 podval-3.4/podval.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 10:37:19.000000 podval-3.4/setup.cfg
+-rw-rw-rw-   0        0        0      173 2023-06-14 10:33:14.000000 podval-3.4/setup.py
```

### Comparing `podval-3.3/podval/podval.py` & `podval-3.4/podval/podval.py`

 * *Files identical despite different names*

