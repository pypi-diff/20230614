# Comparing `tmp/rad-tools-0.7.8.tar.gz` & `tmp/rad-tools-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-tools-0.7.8.tar", last modified: Wed Jun 14 14:31:24 2023, max compression
+gzip compressed data, was "rad-tools-0.7.9.tar", last modified: Wed Jun 14 14:49:53 2023, max compression
```

## Comparing `rad-tools-0.7.8.tar` & `rad-tools-0.7.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.319087 rad-tools-0.7.8/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.7.8/LICENSE.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 14:31:24.317509 rad-tools-0.7.8/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2139 2023-06-08 15:38:54.000000 rad-tools-0.7.8/README.rst
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.279630 rad-tools-0.7.8/rad_tools.egg-info/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 14:31:24.000000 rad-tools-0.7.8/rad_tools.egg-info/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1137 2023-06-14 14:31:24.000000 rad-tools-0.7.8/rad_tools.egg-info/SOURCES.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-14 14:31:24.000000 rad-tools-0.7.8/rad_tools.egg-info/dependency_links.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 14:31:24.000000 rad-tools-0.7.8/rad_tools.egg-info/requires.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-06-14 14:31:24.000000 rad-tools-0.7.8/rad_tools.egg-info/top_level.txt
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.284740 rad-tools-0.7.8/radtools/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      560 2023-06-14 14:29:18.000000 rad-tools-0.7.8/radtools/__init__.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.294096 rad-tools-0.7.8/radtools/crystal/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      353 2023-06-13 11:44:25.000000 rad-tools-0.7.8/radtools/crystal/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     7405 2023-06-13 11:44:25.000000 rad-tools-0.7.8/radtools/crystal/atom.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1183 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/crystal/atom_types.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    87365 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/crystal/bravais_lattice.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    18380 2023-06-13 13:58:51.000000 rad-tools-0.7.8/radtools/crystal/crystal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    23756 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/crystal/identify.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    36933 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/crystal/lattice.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4754 2023-06-13 11:44:25.000000 rad-tools-0.7.8/radtools/crystal/properties.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.298590 rad-tools-0.7.8/radtools/dos/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/dos/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    22119 2023-06-14 14:29:09.000000 rad-tools-0.7.8/radtools/dos/dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    24681 2023-06-14 14:29:09.000000 rad-tools-0.7.8/radtools/dos/pdos.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.303419 rad-tools-0.7.8/radtools/exchange/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      299 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/exchange/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    50003 2023-06-13 11:44:25.000000 rad-tools-0.7.8/radtools/exchange/hamiltonian.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    12330 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/exchange/parameter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/exchange/template.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.305635 rad-tools-0.7.8/radtools/io/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      421 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/io/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1929 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/io/internal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     5485 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/io/tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/map.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    18633 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/routines.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.309883 rad-tools-0.7.8/radtools/score/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1639 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/score/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4506 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/score/extract_tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/score/identify_wannier_centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4692 2023-06-13 11:44:25.000000 rad-tools-0.7.8/radtools/score/make_template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    23804 2023-06-14 14:30:58.000000 rad-tools-0.7.8/radtools/score/plot_dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     9914 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/score/plot_tb2j.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.316965 rad-tools-0.7.8/scripts/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.7.8/scripts/compute-energies.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.7.8/scripts/phonopy-plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-06-08 15:38:54.000000 rad-tools-0.7.8/scripts/rad-extract-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-06-08 15:38:54.000000 rad-tools-0.7.8/scripts/rad-identify-wannier-centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-06-08 15:38:54.000000 rad-tools-0.7.8/scripts/rad-make-template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-06-08 15:38:54.000000 rad-tools-0.7.8/scripts/rad-plot-dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-08 15:38:54.000000 rad-tools-0.7.8/scripts/rad-plot-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 14:31:24.319282 rad-tools-0.7.8/setup.cfg
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1411 2023-06-08 15:39:52.000000 rad-tools-0.7.8/setup.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:49:53.896320 rad-tools-0.7.9/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.7.9/LICENSE.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 14:49:53.895838 rad-tools-0.7.9/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2139 2023-06-08 15:38:54.000000 rad-tools-0.7.9/README.rst
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:49:53.859494 rad-tools-0.7.9/rad_tools.egg-info/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 14:49:53.000000 rad-tools-0.7.9/rad_tools.egg-info/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1137 2023-06-14 14:49:53.000000 rad-tools-0.7.9/rad_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-14 14:49:53.000000 rad-tools-0.7.9/rad_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 14:49:53.000000 rad-tools-0.7.9/rad_tools.egg-info/requires.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-06-14 14:49:53.000000 rad-tools-0.7.9/rad_tools.egg-info/top_level.txt
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:49:53.861436 rad-tools-0.7.9/radtools/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      560 2023-06-14 14:42:46.000000 rad-tools-0.7.9/radtools/__init__.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:49:53.873128 rad-tools-0.7.9/radtools/crystal/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      353 2023-06-13 11:44:25.000000 rad-tools-0.7.9/radtools/crystal/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     7405 2023-06-13 11:44:25.000000 rad-tools-0.7.9/radtools/crystal/atom.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1183 2023-06-08 15:38:54.000000 rad-tools-0.7.9/radtools/crystal/atom_types.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    87365 2023-06-08 15:38:54.000000 rad-tools-0.7.9/radtools/crystal/bravais_lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18380 2023-06-13 13:58:51.000000 rad-tools-0.7.9/radtools/crystal/crystal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    23756 2023-06-08 15:38:54.000000 rad-tools-0.7.9/radtools/crystal/identify.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    36933 2023-06-08 15:38:54.000000 rad-tools-0.7.9/radtools/crystal/lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4754 2023-06-13 11:44:25.000000 rad-tools-0.7.9/radtools/crystal/properties.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:49:53.875794 rad-tools-0.7.9/radtools/dos/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-08 15:38:54.000000 rad-tools-0.7.9/radtools/dos/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    22119 2023-06-14 14:29:09.000000 rad-tools-0.7.9/radtools/dos/dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    24685 2023-06-14 14:43:57.000000 rad-tools-0.7.9/radtools/dos/pdos.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:49:53.879711 rad-tools-0.7.9/radtools/exchange/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      299 2023-06-08 15:38:54.000000 rad-tools-0.7.9/radtools/exchange/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    50003 2023-06-13 11:44:25.000000 rad-tools-0.7.9/radtools/exchange/hamiltonian.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    12330 2023-06-08 15:38:54.000000 rad-tools-0.7.9/radtools/exchange/parameter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-08 15:38:54.000000 rad-tools-0.7.9/radtools/exchange/template.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:49:53.881869 rad-tools-0.7.9/radtools/io/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      421 2023-06-08 15:38:54.000000 rad-tools-0.7.9/radtools/io/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1929 2023-06-08 15:38:54.000000 rad-tools-0.7.9/radtools/io/internal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     5485 2023-06-08 15:38:54.000000 rad-tools-0.7.9/radtools/io/tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-08 15:38:54.000000 rad-tools-0.7.9/radtools/map.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18633 2023-06-08 15:38:54.000000 rad-tools-0.7.9/radtools/routines.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:49:53.885906 rad-tools-0.7.9/radtools/score/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1639 2023-06-08 15:38:54.000000 rad-tools-0.7.9/radtools/score/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4506 2023-06-08 15:38:54.000000 rad-tools-0.7.9/radtools/score/extract_tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-08 15:38:54.000000 rad-tools-0.7.9/radtools/score/identify_wannier_centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4692 2023-06-13 11:44:25.000000 rad-tools-0.7.9/radtools/score/make_template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    23827 2023-06-14 14:41:09.000000 rad-tools-0.7.9/radtools/score/plot_dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     9914 2023-06-08 15:38:54.000000 rad-tools-0.7.9/radtools/score/plot_tb2j.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:49:53.894883 rad-tools-0.7.9/scripts/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.7.9/scripts/compute-energies.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.7.9/scripts/phonopy-plotter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-06-08 15:38:54.000000 rad-tools-0.7.9/scripts/rad-extract-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-06-08 15:38:54.000000 rad-tools-0.7.9/scripts/rad-identify-wannier-centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-06-08 15:38:54.000000 rad-tools-0.7.9/scripts/rad-make-template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-06-08 15:38:54.000000 rad-tools-0.7.9/scripts/rad-plot-dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-08 15:38:54.000000 rad-tools-0.7.9/scripts/rad-plot-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 14:49:53.896469 rad-tools-0.7.9/setup.cfg
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1411 2023-06-08 15:39:52.000000 rad-tools-0.7.9/setup.py
```

### Comparing `rad-tools-0.7.8/LICENSE.txt` & `rad-tools-0.7.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/PKG-INFO` & `rad-tools-0.7.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.7.8
+Version: 0.7.9
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.7.8/README.rst` & `rad-tools-0.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/rad_tools.egg-info/PKG-INFO` & `rad-tools-0.7.9/rad_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.7.8
+Version: 0.7.9
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.7.8/rad_tools.egg-info/SOURCES.txt` & `rad-tools-0.7.9/rad_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/__init__.py` & `rad-tools-0.7.9/radtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 r"""
 All tools from the package.
 
 
 |version|
 """
 
-__version__ = "0.7.8"
+__version__ = "0.7.9"
 
 from . import crystal, dos, exchange, io, score
 from .crystal import *
 from .dos import *
 from .exchange import *
 from .io import *
 from .routines import *
```

### Comparing `rad-tools-0.7.8/radtools/crystal/atom.py` & `rad-tools-0.7.9/radtools/crystal/atom.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/crystal/atom_types.py` & `rad-tools-0.7.9/radtools/crystal/atom_types.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/crystal/bravais_lattice.py` & `rad-tools-0.7.9/radtools/crystal/bravais_lattice.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/crystal/crystal.py` & `rad-tools-0.7.9/radtools/crystal/crystal.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/crystal/identify.py` & `rad-tools-0.7.9/radtools/crystal/identify.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/crystal/lattice.py` & `rad-tools-0.7.9/radtools/crystal/lattice.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/crystal/properties.py` & `rad-tools-0.7.9/radtools/crystal/properties.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/dos/dos.py` & `rad-tools-0.7.9/radtools/dos/dos.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/dos/pdos.py` & `rad-tools-0.7.9/radtools/dos/pdos.py`

 * *Files 2% similar despite different names*

```diff
@@ -532,15 +532,15 @@
     ylim=None,
     relative=False,
     normalize=False,
     interactive=False,
     save_pickle=False,
     colours=COLOURS,
     total_label="default",
-    axes_label_fontsize=14,
+    axes_labels_fontsize=14,
     legend_fontsize=12,
     title_fontsize=18,
 ):
     r"""
     Plot PDOS.
 
     Parameters
@@ -587,19 +587,19 @@
         fig, axs = plt.subplots(n, 1, figsize=(9, n * 2))
         if n == 1:
             axs = [axs]
     fig.subplots_adjust(hspace=0)
 
     def set_up_axis(ax, i):
         if normalize:
-            ax.set_ylabel("PDOS / LDOS", fontsize=axes_label_fontsize)
+            ax.set_ylabel("PDOS / LDOS", fontsize=axes_labels_fontsize)
         else:
-            ax.set_ylabel("DOS, states/eV", fontsize=axes_label_fontsize)
+            ax.set_ylabel("DOS, states/eV", fontsize=axes_labels_fontsize)
         if i == n - 1:
-            ax.set_xlabel("E, ev", fontsize=axes_label_fontsize)
+            ax.set_xlabel("E, ev", fontsize=axes_labels_fontsize)
         else:
             ax.axes.get_xaxis().set_visible(False)
         if ylim is not None:
             ax.set_ylim(*tuple(ylim))
         if xlim is not None:
             ax.set_xlim(*tuple(xlim))
         else:
```

### Comparing `rad-tools-0.7.8/radtools/exchange/hamiltonian.py` & `rad-tools-0.7.9/radtools/exchange/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/exchange/parameter.py` & `rad-tools-0.7.9/radtools/exchange/parameter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/exchange/template.py` & `rad-tools-0.7.9/radtools/exchange/template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/io/internal.py` & `rad-tools-0.7.9/radtools/io/internal.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/io/tb2j.py` & `rad-tools-0.7.9/radtools/io/tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/map.py` & `rad-tools-0.7.9/radtools/map.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/routines.py` & `rad-tools-0.7.9/radtools/routines.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/score/__init__.py` & `rad-tools-0.7.9/radtools/score/__init__.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/score/extract_tb2j.py` & `rad-tools-0.7.9/radtools/score/extract_tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/score/identify_wannier_centres.py` & `rad-tools-0.7.9/radtools/score/identify_wannier_centres.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/score/make_template.py` & `rad-tools-0.7.9/radtools/score/make_template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/radtools/score/plot_dos.py` & `rad-tools-0.7.9/radtools/score/plot_dos.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,15 +317,15 @@
         labels is not None
         and len(labels) != len(custom)
         and len(labels) != len(custom) + 1
     ):
         raise ValueError(
             f"Got {len(labels)} labels, but {len(custom)} PDOS, have to be the same or n custom, n+1 labels."
         )
-    if len(labels) == len(custom) + 1:
+    if labels is not None and len(labels) == len(custom) + 1:
         if labels[0].lower() == "none":
             total_label = None
         elif labels[0].lower() == "default":
             total_label = "default"
         else:
             total_label = labels[0]
         labels = labels[1:]
```

### Comparing `rad-tools-0.7.8/radtools/score/plot_tb2j.py` & `rad-tools-0.7.9/radtools/score/plot_tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/scripts/compute-energies.py` & `rad-tools-0.7.9/scripts/compute-energies.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/scripts/phonopy-plotter.py` & `rad-tools-0.7.9/scripts/phonopy-plotter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.8/setup.py` & `rad-tools-0.7.9/setup.py`

 * *Files identical despite different names*

