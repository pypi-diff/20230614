# Comparing `tmp/egcst-0.0.1.tar.gz` & `tmp/egcst-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "egcst-0.0.1.tar", last modified: Tue Jun 13 23:58:01 2023, max compression
+gzip compressed data, was "egcst-0.0.2.tar", last modified: Wed Jun 14 00:32:06 2023, max compression
```

## Comparing `egcst-0.0.1.tar` & `egcst-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-13 23:58:01.214239 egcst-0.0.1/
--rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-13 23:58:01.214424 egcst-0.0.1/PKG-INFO
--rw-r--r--   0 sasha      (502) staff       (20)       85 2023-06-13 23:55:24.000000 egcst-0.0.1/README.md
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-13 23:58:01.209449 egcst-0.0.1/egcst/
--rw-r--r--   0 sasha      (502) staff       (20)       25 2023-06-13 23:54:54.000000 egcst-0.0.1/egcst/__init__.py
--rw-r--r--   0 sasha      (502) staff       (20)    10467 2023-06-13 23:11:39.000000 egcst-0.0.1/egcst/core.py
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-13 23:58:01.213749 egcst-0.0.1/egcst.egg-info/
--rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-13 23:58:00.000000 egcst-0.0.1/egcst.egg-info/PKG-INFO
--rw-r--r--   0 sasha      (502) staff       (20)      204 2023-06-13 23:58:00.000000 egcst-0.0.1/egcst.egg-info/SOURCES.txt
--rw-r--r--   0 sasha      (502) staff       (20)        1 2023-06-13 23:58:00.000000 egcst-0.0.1/egcst.egg-info/dependency_links.txt
--rw-r--r--   0 sasha      (502) staff       (20)       41 2023-06-13 23:58:00.000000 egcst-0.0.1/egcst.egg-info/requires.txt
--rw-r--r--   0 sasha      (502) staff       (20)        6 2023-06-13 23:58:00.000000 egcst-0.0.1/egcst.egg-info/top_level.txt
--rw-r--r--   0 sasha      (502) staff       (20)      103 2023-06-13 23:58:01.216767 egcst-0.0.1/setup.cfg
--rw-r--r--   0 sasha      (502) staff       (20)      578 2023-06-13 23:54:14.000000 egcst-0.0.1/setup.py
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 00:32:06.971191 egcst-0.0.2/
+-rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-14 00:32:06.971401 egcst-0.0.2/PKG-INFO
+-rw-r--r--   0 sasha      (502) staff       (20)     2192 2023-06-14 00:30:49.000000 egcst-0.0.2/README.md
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 00:32:06.966257 egcst-0.0.2/egcst/
+-rw-r--r--   0 sasha      (502) staff       (20)       25 2023-06-13 23:54:54.000000 egcst-0.0.2/egcst/__init__.py
+-rw-r--r--   0 sasha      (502) staff       (20)    10467 2023-06-13 23:11:39.000000 egcst-0.0.2/egcst/core.py
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 00:32:06.970550 egcst-0.0.2/egcst.egg-info/
+-rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-14 00:32:06.000000 egcst-0.0.2/egcst.egg-info/PKG-INFO
+-rw-r--r--   0 sasha      (502) staff       (20)      204 2023-06-14 00:32:06.000000 egcst-0.0.2/egcst.egg-info/SOURCES.txt
+-rw-r--r--   0 sasha      (502) staff       (20)        1 2023-06-14 00:32:06.000000 egcst-0.0.2/egcst.egg-info/dependency_links.txt
+-rw-r--r--   0 sasha      (502) staff       (20)       37 2023-06-14 00:32:06.000000 egcst-0.0.2/egcst.egg-info/requires.txt
+-rw-r--r--   0 sasha      (502) staff       (20)        6 2023-06-14 00:32:06.000000 egcst-0.0.2/egcst.egg-info/top_level.txt
+-rw-r--r--   0 sasha      (502) staff       (20)      103 2023-06-14 00:32:06.972303 egcst-0.0.2/setup.cfg
+-rw-r--r--   0 sasha      (502) staff       (20)      571 2023-06-14 00:25:57.000000 egcst-0.0.2/setup.py
```

### Comparing `egcst-0.0.1/egcst/core.py` & `egcst-0.0.2/egcst/core.py`

 * *Files identical despite different names*

### Comparing `egcst-0.0.1/setup.py` & `egcst-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 setup(
     name = 'egcst',
     packages = ['egcst'],
-    version = '0.0.1',
+    version = '0.0.2',
     license = 'MIT',
     description = 'This package performs triangulation for engineering geological cross-sections',
     url = 'https://github.com/yuryatin/egcst',
-    download_url = 'https://github.com/yuryatin/egcst/archive/refs/tags/v0.0.1.tar.gz',
+    download_url = 'https://github.com/yuryatin/egcst/archive/refs/tags/v0.0.2.tar.gz',
     keywords = ['engineering', 'geological', 'cross', 'sections', 'mapping', 'triangulation', 'delaunay'],
     classifiers = [],
-    install_requires = ['sys', 'numpy', 'matplotlib', 'shapely', 'ground', 'sect']
+    install_requires = ['numpy', 'matplotlib', 'shapely', 'ground', 'sect']
 )
```

