# Comparing `tmp/egcst-0.0.2.tar.gz` & `tmp/egcst-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "egcst-0.0.2.tar", last modified: Wed Jun 14 00:32:06 2023, max compression
+gzip compressed data, was "egcst-0.0.3.tar", last modified: Wed Jun 14 00:46:51 2023, max compression
```

## Comparing `egcst-0.0.2.tar` & `egcst-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 00:32:06.971191 egcst-0.0.2/
--rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-14 00:32:06.971401 egcst-0.0.2/PKG-INFO
--rw-r--r--   0 sasha      (502) staff       (20)     2192 2023-06-14 00:30:49.000000 egcst-0.0.2/README.md
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 00:32:06.966257 egcst-0.0.2/egcst/
--rw-r--r--   0 sasha      (502) staff       (20)       25 2023-06-13 23:54:54.000000 egcst-0.0.2/egcst/__init__.py
--rw-r--r--   0 sasha      (502) staff       (20)    10467 2023-06-13 23:11:39.000000 egcst-0.0.2/egcst/core.py
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 00:32:06.970550 egcst-0.0.2/egcst.egg-info/
--rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-14 00:32:06.000000 egcst-0.0.2/egcst.egg-info/PKG-INFO
--rw-r--r--   0 sasha      (502) staff       (20)      204 2023-06-14 00:32:06.000000 egcst-0.0.2/egcst.egg-info/SOURCES.txt
--rw-r--r--   0 sasha      (502) staff       (20)        1 2023-06-14 00:32:06.000000 egcst-0.0.2/egcst.egg-info/dependency_links.txt
--rw-r--r--   0 sasha      (502) staff       (20)       37 2023-06-14 00:32:06.000000 egcst-0.0.2/egcst.egg-info/requires.txt
--rw-r--r--   0 sasha      (502) staff       (20)        6 2023-06-14 00:32:06.000000 egcst-0.0.2/egcst.egg-info/top_level.txt
--rw-r--r--   0 sasha      (502) staff       (20)      103 2023-06-14 00:32:06.972303 egcst-0.0.2/setup.cfg
--rw-r--r--   0 sasha      (502) staff       (20)      571 2023-06-14 00:25:57.000000 egcst-0.0.2/setup.py
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 00:46:51.212230 egcst-0.0.3/
+-rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-14 00:46:51.212406 egcst-0.0.3/PKG-INFO
+-rw-r--r--   0 sasha      (502) staff       (20)     2319 2023-06-14 00:46:10.000000 egcst-0.0.3/README.md
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 00:46:51.207759 egcst-0.0.3/egcst/
+-rw-r--r--   0 sasha      (502) staff       (20)       25 2023-06-13 23:54:54.000000 egcst-0.0.3/egcst/__init__.py
+-rw-r--r--   0 sasha      (502) staff       (20)    10467 2023-06-13 23:11:39.000000 egcst-0.0.3/egcst/core.py
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 00:46:51.211834 egcst-0.0.3/egcst.egg-info/
+-rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-14 00:46:50.000000 egcst-0.0.3/egcst.egg-info/PKG-INFO
+-rw-r--r--   0 sasha      (502) staff       (20)      204 2023-06-14 00:46:51.000000 egcst-0.0.3/egcst.egg-info/SOURCES.txt
+-rw-r--r--   0 sasha      (502) staff       (20)        1 2023-06-14 00:46:50.000000 egcst-0.0.3/egcst.egg-info/dependency_links.txt
+-rw-r--r--   0 sasha      (502) staff       (20)       37 2023-06-14 00:46:50.000000 egcst-0.0.3/egcst.egg-info/requires.txt
+-rw-r--r--   0 sasha      (502) staff       (20)        6 2023-06-14 00:46:50.000000 egcst-0.0.3/egcst.egg-info/top_level.txt
+-rw-r--r--   0 sasha      (502) staff       (20)      103 2023-06-14 00:46:51.213116 egcst-0.0.3/setup.cfg
+-rw-r--r--   0 sasha      (502) staff       (20)      571 2023-06-14 00:45:11.000000 egcst-0.0.3/setup.py
```

### Comparing `egcst-0.0.2/README.md` & `egcst-0.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -9,11 +9,13 @@
 
 # Dependencies
 This package depends on the standard Python module `sys` as well as the non-standard Python modules `numpy`, `matplotlib`, `shapely`, `ground`, and `sect`.
 
 # How to use it
 Very easy. The package has only one class `CrossSection()`, which is initiated with the input text file containing the coordinates for the polygons of the  engineering geological cross-section. This class has only 5 'public' methods: `.draw_blank()`, `.triangulate()`, `.save_triangles()`, `.draw_triangles()`, `.do_everything()`, which (except for the last one) are expected to be called in this order (and never repeated for the same object).<br/> The illustration of how to use this package can be found in the attached file [egcst_illustration.ipybn](https://github.com/yuryatin/egcst/blob/main/egcst_illustration.ipynb) .<br/> Briefly this can be expressed like this:
 ```python
-import egcst
+from egcst import CrossSection
 cs = CrossSection(input_file_name="input.txt", min_step=1.0)
 cs.do_everything()
 ```
+![output_triangles](https://github.com/yuryatin/egcst/assets/14263965/b549f8e7-071c-406c-b515-7ae984076e8f)
+
```

### Comparing `egcst-0.0.2/egcst/core.py` & `egcst-0.0.3/egcst/core.py`

 * *Files identical despite different names*

### Comparing `egcst-0.0.2/setup.py` & `egcst-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 setup(
     name = 'egcst',
     packages = ['egcst'],
-    version = '0.0.2',
+    version = '0.0.3',
     license = 'MIT',
     description = 'This package performs triangulation for engineering geological cross-sections',
     url = 'https://github.com/yuryatin/egcst',
-    download_url = 'https://github.com/yuryatin/egcst/archive/refs/tags/v0.0.2.tar.gz',
+    download_url = 'https://github.com/yuryatin/egcst/archive/refs/tags/v0.0.3.tar.gz',
     keywords = ['engineering', 'geological', 'cross', 'sections', 'mapping', 'triangulation', 'delaunay'],
     classifiers = [],
     install_requires = ['numpy', 'matplotlib', 'shapely', 'ground', 'sect']
 )
```

