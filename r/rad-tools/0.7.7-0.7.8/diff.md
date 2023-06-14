# Comparing `tmp/rad-tools-0.7.7.tar.gz` & `tmp/rad-tools-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-tools-0.7.7.tar", last modified: Wed Jun 14 14:01:29 2023, max compression
+gzip compressed data, was "rad-tools-0.7.8.tar", last modified: Wed Jun 14 14:31:24 2023, max compression
```

## Comparing `rad-tools-0.7.7.tar` & `rad-tools-0.7.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.809830 rad-tools-0.7.7/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.7.7/LICENSE.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 14:01:29.806487 rad-tools-0.7.7/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2139 2023-06-08 15:38:54.000000 rad-tools-0.7.7/README.rst
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.781861 rad-tools-0.7.7/rad_tools.egg-info/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 14:01:29.000000 rad-tools-0.7.7/rad_tools.egg-info/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1137 2023-06-14 14:01:29.000000 rad-tools-0.7.7/rad_tools.egg-info/SOURCES.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-14 14:01:29.000000 rad-tools-0.7.7/rad_tools.egg-info/dependency_links.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 14:01:29.000000 rad-tools-0.7.7/rad_tools.egg-info/requires.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-06-14 14:01:29.000000 rad-tools-0.7.7/rad_tools.egg-info/top_level.txt
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.783934 rad-tools-0.7.7/radtools/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      560 2023-06-14 13:59:25.000000 rad-tools-0.7.7/radtools/__init__.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.789471 rad-tools-0.7.7/radtools/crystal/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      353 2023-06-13 11:44:25.000000 rad-tools-0.7.7/radtools/crystal/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     7405 2023-06-13 11:44:25.000000 rad-tools-0.7.7/radtools/crystal/atom.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1183 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/crystal/atom_types.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    87365 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/crystal/bravais_lattice.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    18380 2023-06-13 13:58:51.000000 rad-tools-0.7.7/radtools/crystal/crystal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    23756 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/crystal/identify.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    36933 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/crystal/lattice.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4754 2023-06-13 11:44:25.000000 rad-tools-0.7.7/radtools/crystal/properties.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.793503 rad-tools-0.7.7/radtools/dos/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/dos/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    21650 2023-06-14 01:04:15.000000 rad-tools-0.7.7/radtools/dos/dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    24258 2023-06-14 13:52:27.000000 rad-tools-0.7.7/radtools/dos/pdos.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.796613 rad-tools-0.7.7/radtools/exchange/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      299 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/exchange/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    50003 2023-06-13 11:44:25.000000 rad-tools-0.7.7/radtools/exchange/hamiltonian.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    12330 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/exchange/parameter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/exchange/template.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.798201 rad-tools-0.7.7/radtools/io/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      421 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/io/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1929 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/io/internal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     5485 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/io/tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/map.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    18633 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/routines.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.801562 rad-tools-0.7.7/radtools/score/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1639 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/score/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4506 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/score/extract_tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/score/identify_wannier_centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4692 2023-06-13 11:44:25.000000 rad-tools-0.7.7/radtools/score/make_template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    21504 2023-06-14 13:57:25.000000 rad-tools-0.7.7/radtools/score/plot_dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     9914 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/score/plot_tb2j.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.805363 rad-tools-0.7.7/scripts/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.7.7/scripts/compute-energies.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.7.7/scripts/phonopy-plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-06-08 15:38:54.000000 rad-tools-0.7.7/scripts/rad-extract-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-06-08 15:38:54.000000 rad-tools-0.7.7/scripts/rad-identify-wannier-centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-06-08 15:38:54.000000 rad-tools-0.7.7/scripts/rad-make-template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-06-08 15:38:54.000000 rad-tools-0.7.7/scripts/rad-plot-dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-08 15:38:54.000000 rad-tools-0.7.7/scripts/rad-plot-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 14:01:29.809984 rad-tools-0.7.7/setup.cfg
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1411 2023-06-08 15:39:52.000000 rad-tools-0.7.7/setup.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.319087 rad-tools-0.7.8/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.7.8/LICENSE.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 14:31:24.317509 rad-tools-0.7.8/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2139 2023-06-08 15:38:54.000000 rad-tools-0.7.8/README.rst
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.279630 rad-tools-0.7.8/rad_tools.egg-info/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 14:31:24.000000 rad-tools-0.7.8/rad_tools.egg-info/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1137 2023-06-14 14:31:24.000000 rad-tools-0.7.8/rad_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-14 14:31:24.000000 rad-tools-0.7.8/rad_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 14:31:24.000000 rad-tools-0.7.8/rad_tools.egg-info/requires.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-06-14 14:31:24.000000 rad-tools-0.7.8/rad_tools.egg-info/top_level.txt
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.284740 rad-tools-0.7.8/radtools/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      560 2023-06-14 14:29:18.000000 rad-tools-0.7.8/radtools/__init__.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.294096 rad-tools-0.7.8/radtools/crystal/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      353 2023-06-13 11:44:25.000000 rad-tools-0.7.8/radtools/crystal/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     7405 2023-06-13 11:44:25.000000 rad-tools-0.7.8/radtools/crystal/atom.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1183 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/crystal/atom_types.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    87365 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/crystal/bravais_lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18380 2023-06-13 13:58:51.000000 rad-tools-0.7.8/radtools/crystal/crystal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    23756 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/crystal/identify.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    36933 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/crystal/lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4754 2023-06-13 11:44:25.000000 rad-tools-0.7.8/radtools/crystal/properties.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.298590 rad-tools-0.7.8/radtools/dos/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/dos/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    22119 2023-06-14 14:29:09.000000 rad-tools-0.7.8/radtools/dos/dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    24681 2023-06-14 14:29:09.000000 rad-tools-0.7.8/radtools/dos/pdos.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.303419 rad-tools-0.7.8/radtools/exchange/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      299 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/exchange/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    50003 2023-06-13 11:44:25.000000 rad-tools-0.7.8/radtools/exchange/hamiltonian.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    12330 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/exchange/parameter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/exchange/template.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.305635 rad-tools-0.7.8/radtools/io/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      421 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/io/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1929 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/io/internal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     5485 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/io/tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/map.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18633 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/routines.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.309883 rad-tools-0.7.8/radtools/score/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1639 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/score/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4506 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/score/extract_tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/score/identify_wannier_centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4692 2023-06-13 11:44:25.000000 rad-tools-0.7.8/radtools/score/make_template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    23804 2023-06-14 14:30:58.000000 rad-tools-0.7.8/radtools/score/plot_dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     9914 2023-06-08 15:38:54.000000 rad-tools-0.7.8/radtools/score/plot_tb2j.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:31:24.316965 rad-tools-0.7.8/scripts/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.7.8/scripts/compute-energies.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.7.8/scripts/phonopy-plotter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-06-08 15:38:54.000000 rad-tools-0.7.8/scripts/rad-extract-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-06-08 15:38:54.000000 rad-tools-0.7.8/scripts/rad-identify-wannier-centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-06-08 15:38:54.000000 rad-tools-0.7.8/scripts/rad-make-template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-06-08 15:38:54.000000 rad-tools-0.7.8/scripts/rad-plot-dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-08 15:38:54.000000 rad-tools-0.7.8/scripts/rad-plot-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 14:31:24.319282 rad-tools-0.7.8/setup.cfg
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1411 2023-06-08 15:39:52.000000 rad-tools-0.7.8/setup.py
```

### Comparing `rad-tools-0.7.7/LICENSE.txt` & `rad-tools-0.7.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/PKG-INFO` & `rad-tools-0.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.7.7
+Version: 0.7.8
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.7.7/README.rst` & `rad-tools-0.7.8/README.rst`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/rad_tools.egg-info/PKG-INFO` & `rad-tools-0.7.8/rad_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.7.7
+Version: 0.7.8
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.7.7/rad_tools.egg-info/SOURCES.txt` & `rad-tools-0.7.8/rad_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/__init__.py` & `rad-tools-0.7.8/radtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 r"""
 All tools from the package.
 
 
 |version|
 """
 
-__version__ = "0.7.7"
+__version__ = "0.7.8"
 
 from . import crystal, dos, exchange, io, score
 from .crystal import *
 from .dos import *
 from .exchange import *
 from .io import *
 from .routines import *
```

### Comparing `rad-tools-0.7.7/radtools/crystal/atom.py` & `rad-tools-0.7.8/radtools/crystal/atom.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/crystal/atom_types.py` & `rad-tools-0.7.8/radtools/crystal/atom_types.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/crystal/bravais_lattice.py` & `rad-tools-0.7.8/radtools/crystal/bravais_lattice.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/crystal/crystal.py` & `rad-tools-0.7.8/radtools/crystal/crystal.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/crystal/identify.py` & `rad-tools-0.7.8/radtools/crystal/identify.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/crystal/lattice.py` & `rad-tools-0.7.8/radtools/crystal/lattice.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/crystal/properties.py` & `rad-tools-0.7.8/radtools/crystal/properties.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/dos/dos.py` & `rad-tools-0.7.8/radtools/dos/dos.py`

 * *Files 2% similar despite different names*

```diff
@@ -514,14 +514,17 @@
         self,
         output_name,
         interactive=False,
         efermi=0,
         xlim=None,
         ylim=None,
         save_pickle=False,
+        axes_label_fontsize=18,
+        legend_fontsize=12,
+        title_fontsize=18,
     ):
         r"""
         Plot total DOS vs total PDOS.
 
         Parameters
         ----------
         output_name : str
@@ -533,28 +536,34 @@
         xlim : tuple, optional
             Limits for energy scale.
         ylim : tuple, optional
             Limits for dos scale.
         save_pickle : bool, default False
             Whether to save figure as a .pickle file.
             Helps for custom modification of particular figures.
+        axes_label_fontsize : int, default 18
+            Fontsize of the axes labels.
+        legend_fontsize : int, default 12
+            Fontsize of the legend.
+        title_fontsize : int, default 18
+            Title fontsize.
         """
         fig, ax = plt.subplots(figsize=(8, 4))
 
-        ax.set_xlabel("Energy, eV", fontsize=18)
-        ax.set_ylabel("DOS, states/eV", fontsize=18)
+        ax.set_xlabel("Energy, eV", fontsize=axes_label_fontsize)
+        ax.set_ylabel("DOS, states/eV", fontsize=axes_label_fontsize)
         if xlim is None:
             xlim = (np.amin(self.energy), np.amax(self.energy))
         ax.set_xlim(*tuple(xlim))
         if ylim is not None:
             ax.set_ylim(*tuple(ylim))
         if efermi != 0:
-            ax.set_title(f"DOS vs PDOS (0 is Fermi energy)", fontsize=18)
+            ax.set_title(f"DOS vs PDOS (0 is Fermi energy)", fontsize=title_fontsize)
         else:
-            ax.set_title(f"DOS vs PDOS (0 is 0)", fontsize=18)
+            ax.set_title(f"DOS vs PDOS (0 is 0)", fontsize=title_fontsize)
         ax.vlines(
             0,
             0,
             1,
             transform=ax.get_xaxis_transform(),
             color="grey",
             linewidths=0.5,
@@ -657,17 +666,19 @@
                 color="red",
                 alpha=0.7,
                 label="PDOS (down)",
             )
             ncol = 1
 
             if interactive:
-                ax.legend(loc="best", ncol=ncol, draggable=True)
+                ax.legend(
+                    loc="best", ncol=ncol, draggable=True, fontsize=legend_fontsize
+                )
             else:
-                ax.legend(loc="best", ncol=ncol)
+                ax.legend(loc="best", ncol=ncol, fontsize=legend_fontsize)
 
         if interactive:
             plt.show()
         else:
             png_path = f"{output_name}.png"
             plt.savefig(png_path, dpi=600, bbox_inches="tight")
             if save_pickle:
```

### Comparing `rad-tools-0.7.7/radtools/dos/pdos.py` & `rad-tools-0.7.8/radtools/dos/pdos.py`

 * *Files 3% similar despite different names*

```diff
@@ -532,14 +532,17 @@
     ylim=None,
     relative=False,
     normalize=False,
     interactive=False,
     save_pickle=False,
     colours=COLOURS,
     total_label="default",
+    axes_label_fontsize=14,
+    legend_fontsize=12,
+    title_fontsize=18,
 ):
     r"""
     Plot PDOS.
 
     Parameters
     ----------
     pdos : :py:class:`.PDOS`
@@ -563,14 +566,20 @@
     save_pickle : bool, default False
         Whether to save figure as a .pickle file.
         Helps for custom modification of particular figures.
     colours : list
         List of colours to be used. values are passed directly to matplotlib
     total_label : str or ``None``, default "default"
         Label for the total data. If None , then the label is not added
+    axes_label_fontsize : int, default 14
+        Fontsize of the axes labels.
+    legend_fontsize : int, default 12
+        Fontsize of the legend.
+    title_fontsize : int, default 18
+        Fontsize of the title
     """
 
     n = len(pdos.projectors)
     pdos = pdos.squeezed()
 
     if relative:
         fig, ax = plt.subplots(figsize=(9, 4))
@@ -578,19 +587,19 @@
         fig, axs = plt.subplots(n, 1, figsize=(9, n * 2))
         if n == 1:
             axs = [axs]
     fig.subplots_adjust(hspace=0)
 
     def set_up_axis(ax, i):
         if normalize:
-            ax.set_ylabel("PDOS / LDOS", fontsize=15)
+            ax.set_ylabel("PDOS / LDOS", fontsize=axes_label_fontsize)
         else:
-            ax.set_ylabel("DOS, states/eV", fontsize=15)
+            ax.set_ylabel("DOS, states/eV", fontsize=axes_label_fontsize)
         if i == n - 1:
-            ax.set_xlabel("E, ev", fontsize=15)
+            ax.set_xlabel("E, ev", fontsize=axes_label_fontsize)
         else:
             ax.axes.get_xaxis().set_visible(False)
         if ylim is not None:
             ax.set_ylim(*tuple(ylim))
         if xlim is not None:
             ax.set_xlim(*tuple(xlim))
         else:
@@ -601,15 +610,15 @@
             1,
             transform=ax.get_xaxis_transform(),
             color="grey",
             linewidths=0.5,
             linestyles="dashed",
         )
         if title is not None and (i == 0 or relative):
-            ax.set_title(title)
+            ax.set_title(title, fontsize=title_fontsize)
 
     if normalize:
         pdos = pdos.normalized()
 
     if relative:
         set_up_axis(ax, n - 1)
         ax.hlines(
@@ -754,22 +763,24 @@
                     label=projector,
                 )
         if interactive:
             ax.legend(
                 loc=(1.025, 0.2),
                 bbox_transform=ax.transAxes,
                 draggable=True,
-                fontsize=12,
+                fontsize=legend_fontsize,
             )
         else:
-            ax.legend(loc=(1.025, 0.2), bbox_transform=ax.transAxes, fontsize=12)
+            ax.legend(
+                loc=(1.025, 0.2), bbox_transform=ax.transAxes, fontsize=legend_fontsize
+            )
 
     if interactive:
         plt.show()
     else:
-        plt.savefig(f"{output_name}.png", dpi=400, bbox_inches="tight")
+        plt.savefig(f"{output_name}.png", dpi=600, bbox_inches="tight")
         if save_pickle:
             import pickle
 
             with open(f"{output_name}.png.pickle", "wb") as file:
                 pickle.dump(fig, file)
     plt.close()
```

### Comparing `rad-tools-0.7.7/radtools/exchange/hamiltonian.py` & `rad-tools-0.7.8/radtools/exchange/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/exchange/parameter.py` & `rad-tools-0.7.8/radtools/exchange/parameter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/exchange/template.py` & `rad-tools-0.7.8/radtools/exchange/template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/io/internal.py` & `rad-tools-0.7.8/radtools/io/internal.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/io/tb2j.py` & `rad-tools-0.7.8/radtools/io/tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/map.py` & `rad-tools-0.7.8/radtools/map.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/routines.py` & `rad-tools-0.7.8/radtools/routines.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/score/__init__.py` & `rad-tools-0.7.8/radtools/score/__init__.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/score/extract_tb2j.py` & `rad-tools-0.7.8/radtools/score/extract_tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/score/identify_wannier_centres.py` & `rad-tools-0.7.8/radtools/score/identify_wannier_centres.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/score/make_template.py` & `rad-tools-0.7.8/radtools/score/make_template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/radtools/score/plot_dos.py` & `rad-tools-0.7.8/radtools/score/plot_dos.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,14 +56,17 @@
     relative=False,
     normalize=False,
     interactive=False,
     save_pickle=False,
     save_txt=False,
     background_total=False,
     colours=COLOURS,
+    legend_fontsize=12,
+    axes_labels_fontsize=14,
+    title_fontsize=18,
 ):
     cprint("Orbital-resolved PDOS:", "green")
     local_output = join(output_root, "orbital-resolved")
     makedirs(local_output, exist_ok=True)
     data = {}
     for atom, atom_number, wfc, wfc_number in dos:
         if atom not in data:
@@ -113,14 +116,17 @@
                     xlim=energy_window,
                     ylim=dos_window,
                     relative=relative,
                     normalize=normalize,
                     interactive=interactive,
                     save_pickle=save_pickle,
                     colours=colours,
+                    legend_fontsize=legend_fontsize,
+                    axes_labels_fontsize=axes_labels_fontsize,
+                    title_fontsize=title_fontsize,
                 )
     cprint(f"Results are in {abspath(local_output)}", "blue")
 
 
 def plot_atom_resolved(
     dos,
     output_root=".",
@@ -131,14 +137,17 @@
     relative=False,
     normalize=False,
     interactive=False,
     save_pickle=False,
     save_txt=False,
     background_total=False,
     colours=COLOURS,
+    legend_fontsize=12,
+    axes_labels_fontsize=14,
+    title_fontsize=18,
 ):
     cprint("Orbital's contribution for each atom.", "green")
     local_output = join(output_root, "atom-resolved")
     makedirs(local_output, exist_ok=True)
 
     for atom in dos.atoms:
         if separate:
@@ -188,14 +197,17 @@
                 xlim=energy_window,
                 ylim=dos_window,
                 relative=relative,
                 normalize=normalize,
                 interactive=interactive,
                 save_pickle=save_pickle,
                 colours=colours,
+                legend_fontsize=legend_fontsize,
+                axes_labels_fontsize=axes_labels_fontsize,
+                title_fontsize=title_fontsize,
             )
     cprint(f"Results are in {abspath(local_output)}", "blue")
 
 
 def plot_atom_to_total(
     dos,
     output_root=".",
@@ -206,14 +218,17 @@
     relative=False,
     normalize=False,
     interactive=False,
     save_pickle=False,
     save_txt=False,
     background_total=False,
     colours=COLOURS,
+    legend_fontsize=12,
+    axes_labels_fontsize=14,
+    title_fontsize=18,
 ):
     cprint("Atom's contributions into total PDOS:", "green")
     projectors = []
     pdos = []
     for atom in dos.atoms:
         if separate:
             atom_numbers = dos.atom_numbers(atom)
@@ -264,14 +279,17 @@
         xlim=energy_window,
         ylim=dos_window,
         relative=relative,
         normalize=normalize,
         interactive=interactive,
         save_pickle=save_pickle,
         colours=colours,
+        legend_fontsize=legend_fontsize,
+        axes_labels_fontsize=axes_labels_fontsize,
+        title_fontsize=title_fontsize,
     )
     cprint(f"Result is in {abspath(output_root)}", "blue")
 
 
 def plot_custom(
     dos,
     custom,
@@ -283,14 +301,17 @@
     normalize=False,
     interactive=False,
     save_pickle=False,
     save_txt=False,
     background_total=False,
     colours=COLOURS,
     labels=None,
+    legend_fontsize=12,
+    axes_labels_fontsize=14,
+    title_fontsize=18,
 ):
     cprint("Plotting custom plot", "green")
     print("Input is understood as:")
     projectors = []
     pdos = []
     if (
         labels is not None
@@ -421,14 +442,17 @@
         ylim=dos_window,
         relative=relative,
         normalize=normalize,
         interactive=interactive,
         save_pickle=save_pickle,
         colours=colours,
         total_label=total_label,
+        legend_fontsize=legend_fontsize,
+        axes_labels_fontsize=axes_labels_fontsize,
+        title_fontsize=title_fontsize,
     )
     cprint(f"Result is in {abspath(join(output_root, f'{output_name}.png'))}", "blue")
 
 
 def manager(
     input_path,
     seedname=None,
@@ -443,14 +467,17 @@
     interactive=False,
     save_pickle=False,
     save_txt=False,
     background_total=False,
     custom=None,
     colours=None,
     labels=None,
+    legend_fontsize=12,
+    axes_labels_fontsize=14,
+    title_fontsize=18,
 ):
     r"""
     ``rad-plot-dos.py`` script.
 
     Full documentation on the behaviour is available in the
     :ref:`User Guide <rad-plot-dos>`.
     Parameters of the function directly
@@ -502,14 +529,17 @@
             dos.plot_pdos_tot(
                 output_name=join(output_root, "pdos-vs-dos"),
                 interactive=interactive,
                 efermi=efermi,
                 xlim=energy_window,
                 ylim=dos_window,
                 save_pickle=save_pickle,
+                legend_fontsize=legend_fontsize,
+                axes_labels_fontsize=axes_labels_fontsize,
+                title_fontsize=title_fontsize,
             )
             cprint(f"Result is in {join(output_root, 'pdos-vs-dos')}", "blue")
 
             # Plot PDOS for each atom/wfc
             plot_orbital_resolved(
                 dos=dos,
                 output_root=output_root,
@@ -520,14 +550,17 @@
                 relative=relative,
                 normalize=normalize,
                 interactive=interactive,
                 save_pickle=save_pickle,
                 save_txt=save_txt,
                 background_total=background_total,
                 colours=colours,
+                legend_fontsize=legend_fontsize,
+                axes_labels_fontsize=axes_labels_fontsize,
+                title_fontsize=title_fontsize,
             )
 
             # Plot wfc contribution into each atom
             plot_atom_resolved(
                 dos=dos,
                 output_root=output_root,
                 energy_window=energy_window,
@@ -537,14 +570,17 @@
                 relative=relative,
                 normalize=normalize,
                 interactive=interactive,
                 save_pickle=save_pickle,
                 save_txt=save_txt,
                 background_total=background_total,
                 colours=colours,
+                legend_fontsize=legend_fontsize,
+                axes_labels_fontsize=axes_labels_fontsize,
+                title_fontsize=title_fontsize,
             )
 
             # Plot atom contributions into total PDOS
             plot_atom_to_total(
                 dos=dos,
                 output_root=output_root,
                 energy_window=energy_window,
@@ -554,14 +590,17 @@
                 relative=relative,
                 normalize=normalize,
                 interactive=interactive,
                 save_pickle=save_pickle,
                 save_txt=save_txt,
                 background_total=background_total,
                 colours=colours,
+                legend_fontsize=legend_fontsize,
+                axes_labels_fontsize=axes_labels_fontsize,
+                title_fontsize=title_fontsize,
             )
         else:
             plot_custom(
                 dos=dos,
                 custom=custom,
                 output_root=output_root,
                 energy_window=energy_window,
@@ -571,14 +610,17 @@
                 normalize=normalize,
                 interactive=interactive,
                 save_pickle=save_pickle,
                 save_txt=save_txt,
                 background_total=background_total,
                 colours=colours,
                 labels=labels,
+                legend_fontsize=legend_fontsize,
+                axes_labels_fontsize=axes_labels_fontsize,
+                title_fontsize=title_fontsize,
             )
 
 
 def create_parser():
     parser = ArgumentParser(
         description="Script for visualisation of density of states."
     )
@@ -712,9 +754,33 @@
         "--labels",
         type=str,
         metavar="labels",
         default=None,
         nargs="*",
         help="Labels for the custom plots.",
     )
+    parser.add_argument(
+        "-alfs",
+        "--axes-labels-fontsize",
+        type=int,
+        default=14,
+        metavar="fontsize",
+        help="Fontsize of the labes of the axes.",
+    )
+    parser.add_argument(
+        "-lfs",
+        "--legend-fontsize",
+        type=int,
+        default=12,
+        metavar="fontsize",
+        help="Fontsize of the legend.",
+    )
+    parser.add_argument(
+        "-tfs",
+        "--title-fontsize",
+        type=int,
+        default=18,
+        metavar="fontsize",
+        help="Fontsize of the title.",
+    )
 
     return parser
```

### Comparing `rad-tools-0.7.7/radtools/score/plot_tb2j.py` & `rad-tools-0.7.8/radtools/score/plot_tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/scripts/compute-energies.py` & `rad-tools-0.7.8/scripts/compute-energies.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/scripts/phonopy-plotter.py` & `rad-tools-0.7.8/scripts/phonopy-plotter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.7/setup.py` & `rad-tools-0.7.8/setup.py`

 * *Files identical despite different names*

