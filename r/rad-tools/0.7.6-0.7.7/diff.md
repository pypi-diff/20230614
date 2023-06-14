# Comparing `tmp/rad-tools-0.7.6.tar.gz` & `tmp/rad-tools-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-tools-0.7.6.tar", last modified: Wed Jun 14 12:18:55 2023, max compression
+gzip compressed data, was "rad-tools-0.7.7.tar", last modified: Wed Jun 14 14:01:29 2023, max compression
```

## Comparing `rad-tools-0.7.6.tar` & `rad-tools-0.7.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.115363 rad-tools-0.7.6/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.7.6/LICENSE.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 12:18:55.114431 rad-tools-0.7.6/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2139 2023-06-08 15:38:54.000000 rad-tools-0.7.6/README.rst
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.011779 rad-tools-0.7.6/rad_tools.egg-info/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 12:18:54.000000 rad-tools-0.7.6/rad_tools.egg-info/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1137 2023-06-14 12:18:54.000000 rad-tools-0.7.6/rad_tools.egg-info/SOURCES.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-14 12:18:54.000000 rad-tools-0.7.6/rad_tools.egg-info/dependency_links.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 12:18:54.000000 rad-tools-0.7.6/rad_tools.egg-info/requires.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-06-14 12:18:54.000000 rad-tools-0.7.6/rad_tools.egg-info/top_level.txt
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.014784 rad-tools-0.7.6/radtools/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      560 2023-06-14 12:16:09.000000 rad-tools-0.7.6/radtools/__init__.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.028049 rad-tools-0.7.6/radtools/crystal/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      353 2023-06-13 11:44:25.000000 rad-tools-0.7.6/radtools/crystal/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     7405 2023-06-13 11:44:25.000000 rad-tools-0.7.6/radtools/crystal/atom.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1183 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/crystal/atom_types.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    87365 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/crystal/bravais_lattice.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    18380 2023-06-13 13:58:51.000000 rad-tools-0.7.6/radtools/crystal/crystal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    23756 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/crystal/identify.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    36933 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/crystal/lattice.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4754 2023-06-13 11:44:25.000000 rad-tools-0.7.6/radtools/crystal/properties.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.034568 rad-tools-0.7.6/radtools/dos/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/dos/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    21650 2023-06-14 01:04:15.000000 rad-tools-0.7.6/radtools/dos/dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    23738 2023-06-14 01:04:15.000000 rad-tools-0.7.6/radtools/dos/pdos.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.041204 rad-tools-0.7.6/radtools/exchange/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      299 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/exchange/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    50003 2023-06-13 11:44:25.000000 rad-tools-0.7.6/radtools/exchange/hamiltonian.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    12330 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/exchange/parameter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/exchange/template.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.043738 rad-tools-0.7.6/radtools/io/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      421 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/io/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1929 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/io/internal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     5485 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/io/tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/map.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    18633 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/routines.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.068563 rad-tools-0.7.6/radtools/score/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1639 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/score/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4506 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/score/extract_tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/score/identify_wannier_centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4692 2023-06-13 11:44:25.000000 rad-tools-0.7.6/radtools/score/make_template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    21069 2023-06-14 12:15:54.000000 rad-tools-0.7.6/radtools/score/plot_dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     9914 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/score/plot_tb2j.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.113901 rad-tools-0.7.6/scripts/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.7.6/scripts/compute-energies.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.7.6/scripts/phonopy-plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-06-08 15:38:54.000000 rad-tools-0.7.6/scripts/rad-extract-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-06-08 15:38:54.000000 rad-tools-0.7.6/scripts/rad-identify-wannier-centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-06-08 15:38:54.000000 rad-tools-0.7.6/scripts/rad-make-template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-06-08 15:38:54.000000 rad-tools-0.7.6/scripts/rad-plot-dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-08 15:38:54.000000 rad-tools-0.7.6/scripts/rad-plot-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 12:18:55.115492 rad-tools-0.7.6/setup.cfg
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1411 2023-06-08 15:39:52.000000 rad-tools-0.7.6/setup.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.809830 rad-tools-0.7.7/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.7.7/LICENSE.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 14:01:29.806487 rad-tools-0.7.7/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2139 2023-06-08 15:38:54.000000 rad-tools-0.7.7/README.rst
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.781861 rad-tools-0.7.7/rad_tools.egg-info/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 14:01:29.000000 rad-tools-0.7.7/rad_tools.egg-info/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1137 2023-06-14 14:01:29.000000 rad-tools-0.7.7/rad_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-14 14:01:29.000000 rad-tools-0.7.7/rad_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 14:01:29.000000 rad-tools-0.7.7/rad_tools.egg-info/requires.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-06-14 14:01:29.000000 rad-tools-0.7.7/rad_tools.egg-info/top_level.txt
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.783934 rad-tools-0.7.7/radtools/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      560 2023-06-14 13:59:25.000000 rad-tools-0.7.7/radtools/__init__.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.789471 rad-tools-0.7.7/radtools/crystal/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      353 2023-06-13 11:44:25.000000 rad-tools-0.7.7/radtools/crystal/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     7405 2023-06-13 11:44:25.000000 rad-tools-0.7.7/radtools/crystal/atom.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1183 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/crystal/atom_types.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    87365 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/crystal/bravais_lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18380 2023-06-13 13:58:51.000000 rad-tools-0.7.7/radtools/crystal/crystal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    23756 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/crystal/identify.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    36933 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/crystal/lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4754 2023-06-13 11:44:25.000000 rad-tools-0.7.7/radtools/crystal/properties.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.793503 rad-tools-0.7.7/radtools/dos/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/dos/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    21650 2023-06-14 01:04:15.000000 rad-tools-0.7.7/radtools/dos/dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    24258 2023-06-14 13:52:27.000000 rad-tools-0.7.7/radtools/dos/pdos.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.796613 rad-tools-0.7.7/radtools/exchange/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      299 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/exchange/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    50003 2023-06-13 11:44:25.000000 rad-tools-0.7.7/radtools/exchange/hamiltonian.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    12330 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/exchange/parameter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/exchange/template.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.798201 rad-tools-0.7.7/radtools/io/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      421 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/io/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1929 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/io/internal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     5485 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/io/tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/map.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18633 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/routines.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.801562 rad-tools-0.7.7/radtools/score/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1639 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/score/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4506 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/score/extract_tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/score/identify_wannier_centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4692 2023-06-13 11:44:25.000000 rad-tools-0.7.7/radtools/score/make_template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    21504 2023-06-14 13:57:25.000000 rad-tools-0.7.7/radtools/score/plot_dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     9914 2023-06-08 15:38:54.000000 rad-tools-0.7.7/radtools/score/plot_tb2j.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 14:01:29.805363 rad-tools-0.7.7/scripts/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.7.7/scripts/compute-energies.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.7.7/scripts/phonopy-plotter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-06-08 15:38:54.000000 rad-tools-0.7.7/scripts/rad-extract-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-06-08 15:38:54.000000 rad-tools-0.7.7/scripts/rad-identify-wannier-centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-06-08 15:38:54.000000 rad-tools-0.7.7/scripts/rad-make-template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-06-08 15:38:54.000000 rad-tools-0.7.7/scripts/rad-plot-dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-08 15:38:54.000000 rad-tools-0.7.7/scripts/rad-plot-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 14:01:29.809984 rad-tools-0.7.7/setup.cfg
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1411 2023-06-08 15:39:52.000000 rad-tools-0.7.7/setup.py
```

### Comparing `rad-tools-0.7.6/LICENSE.txt` & `rad-tools-0.7.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/PKG-INFO` & `rad-tools-0.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.7.6
+Version: 0.7.7
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.7.6/README.rst` & `rad-tools-0.7.7/README.rst`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/rad_tools.egg-info/PKG-INFO` & `rad-tools-0.7.7/rad_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.7.6
+Version: 0.7.7
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.7.6/rad_tools.egg-info/SOURCES.txt` & `rad-tools-0.7.7/rad_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/__init__.py` & `rad-tools-0.7.7/radtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 r"""
 All tools from the package.
 
 
 |version|
 """
 
-__version__ = "0.7.6"
+__version__ = "0.7.7"
 
 from . import crystal, dos, exchange, io, score
 from .crystal import *
 from .dos import *
 from .exchange import *
 from .io import *
 from .routines import *
```

### Comparing `rad-tools-0.7.6/radtools/crystal/atom.py` & `rad-tools-0.7.7/radtools/crystal/atom.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/crystal/atom_types.py` & `rad-tools-0.7.7/radtools/crystal/atom_types.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/crystal/bravais_lattice.py` & `rad-tools-0.7.7/radtools/crystal/bravais_lattice.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/crystal/crystal.py` & `rad-tools-0.7.7/radtools/crystal/crystal.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/crystal/identify.py` & `rad-tools-0.7.7/radtools/crystal/identify.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/crystal/lattice.py` & `rad-tools-0.7.7/radtools/crystal/lattice.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/crystal/properties.py` & `rad-tools-0.7.7/radtools/crystal/properties.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/dos/dos.py` & `rad-tools-0.7.7/radtools/dos/dos.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/dos/pdos.py` & `rad-tools-0.7.7/radtools/dos/pdos.py`

 * *Files 4% similar despite different names*

```diff
@@ -531,14 +531,15 @@
     xlim=None,
     ylim=None,
     relative=False,
     normalize=False,
     interactive=False,
     save_pickle=False,
     colours=COLOURS,
+    total_label="default",
 ):
     r"""
     Plot PDOS.
 
     Parameters
     ----------
     pdos : :py:class:`.PDOS`
@@ -560,14 +561,16 @@
     interactive : bool, default False
         Whether to use interactive plotting mode.
     save_pickle : bool, default False
         Whether to save figure as a .pickle file.
         Helps for custom modification of particular figures.
     colours : list
         List of colours to be used. values are passed directly to matplotlib
+    total_label : str or ``None``, default "default"
+        Label for the total data. If None , then the label is not added
     """
 
     n = len(pdos.projectors)
     pdos = pdos.squeezed()
 
     if relative:
         fig, ax = plt.subplots(figsize=(9, 4))
@@ -619,33 +622,42 @@
         )
 
     for i, projector in enumerate(pdos):
         if not relative:
             ax = axs[i]
             set_up_axis(ax, i)
         if pdos.spin_pol:
+            if total_label == "default":
+                label_up = f"{pdos.projectors_group} (up)"
+                label_down = f"{pdos.projectors_group} (down)"
+            elif total_label is None:
+                label_up = None
+                label_down = None
+            else:
+                label_up = f"{total_label} (up)"
+                label_down = f"{total_label} (down)"
             if relative:
                 if i == 0:
                     ax.plot(
                         pdos.energy,
                         np.where(pdos.ldos[0] > 1e-5, pdos.ldos[0], None),
                         "-",
                         lw=1,
                         color="blue",
                         alpha=0.8,
-                        label=f"{pdos.projectors_group} (up)",
+                        label=label_up,
                     )
                     ax.plot(
                         pdos.energy,
                         np.where(pdos.ldos[1] > 1e-5, -pdos.ldos[1], None),
                         "-",
                         lw=1,
                         color="red",
                         alpha=0.8,
-                        label=f"{pdos.projectors_group} (down)",
+                        label=label_down,
                     )
                 ax.fill_between(
                     pdos.energy,
                     np.sum(pdos[:i], axis=0)[0],
                     np.sum(pdos[: i + 1], axis=0)[0],
                     lw=0,
                     color=colours[i % len(colours)],
@@ -664,24 +676,24 @@
                 ax.fill_between(
                     pdos.energy,
                     0,
                     pdos.ldos[0],
                     lw=0,
                     color="blue",
                     alpha=0.2,
-                    label=f"{pdos.projectors_group} (up)",
+                    label=label_up,
                 )
                 ax.fill_between(
                     pdos.energy,
                     0,
                     -pdos.ldos[1],
                     lw=0,
                     color="red",
                     alpha=0.2,
-                    label=f"{pdos.projectors_group} (down)",
+                    label=label_down,
                 )
 
                 ax.plot(
                     pdos.energy,
                     pdos[projector][0],
                     "-",
                     lw=0.8,
@@ -695,24 +707,26 @@
                     "-",
                     lw=0.8,
                     color="red",
                     alpha=0.8,
                     label=f"{projector} (down)",
                 )
         else:
+            if total_label == "default":
+                total_label = pdos.projectors_group
             if relative:
                 if i == 0:
                     ax.plot(
                         pdos.energy,
                         np.where(pdos.ldos > 1e-5, pdos.ldos, None),
                         "-",
                         lw=1,
                         color="black",
                         alpha=0.8,
-                        label=pdos.projectors_group,
+                        label=total_label,
                     )
                 ax.fill_between(
                     pdos.energy,
                     np.sum(pdos[:i], axis=0),
                     np.sum(pdos[: i + 1], axis=0),
                     lw=0,
                     color=colours[i % len(colours)],
@@ -724,15 +738,15 @@
                 ax.fill_between(
                     pdos.energy,
                     0,
                     pdos.ldos,
                     lw=0,
                     color="black",
                     alpha=0.3,
-                    label=pdos.projectors_group,
+                    label=total_label,
                 )
                 ax.plot(
                     pdos.energy,
                     pdos[projector],
                     "-",
                     lw=0.8,
                     color="black",
```

### Comparing `rad-tools-0.7.6/radtools/exchange/hamiltonian.py` & `rad-tools-0.7.7/radtools/exchange/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/exchange/parameter.py` & `rad-tools-0.7.7/radtools/exchange/parameter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/exchange/template.py` & `rad-tools-0.7.7/radtools/exchange/template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/io/internal.py` & `rad-tools-0.7.7/radtools/io/internal.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/io/tb2j.py` & `rad-tools-0.7.7/radtools/io/tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/map.py` & `rad-tools-0.7.7/radtools/map.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/routines.py` & `rad-tools-0.7.7/radtools/routines.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/score/__init__.py` & `rad-tools-0.7.7/radtools/score/__init__.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/score/extract_tb2j.py` & `rad-tools-0.7.7/radtools/score/extract_tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/score/identify_wannier_centres.py` & `rad-tools-0.7.7/radtools/score/identify_wannier_centres.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/score/make_template.py` & `rad-tools-0.7.7/radtools/score/make_template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/radtools/score/plot_dos.py` & `rad-tools-0.7.7/radtools/score/plot_dos.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,18 +288,32 @@
     colours=COLOURS,
     labels=None,
 ):
     cprint("Plotting custom plot", "green")
     print("Input is understood as:")
     projectors = []
     pdos = []
-    if labels is not None and len(labels) != len(custom):
+    if (
+        labels is not None
+        and len(labels) != len(custom)
+        and len(labels) != len(custom) + 1
+    ):
         raise ValueError(
-            f"Got {len(labels)} labels, but {len(custom)} PDOS, have to be the same."
+            f"Got {len(labels)} labels, but {len(custom)} PDOS, have to be the same or n custom, n+1 labels."
         )
+    if len(labels) == len(custom) + 1:
+        if labels[0].lower() == "none":
+            total_label = None
+        elif labels[0].lower() == "default":
+            total_label = "default"
+        else:
+            total_label = labels[0]
+        labels = labels[1:]
+    else:
+        total_label = "default"
     for i_e, entry in enumerate(custom):
         if labels is not None:
             projectors.append(labels[i_e])
         else:
             projectors.append(entry)
         cprint(f'"{entry}":', "green")
         entry = entry.replace(" ", "").replace(")", "")
@@ -406,14 +420,15 @@
         xlim=energy_window,
         ylim=dos_window,
         relative=relative,
         normalize=normalize,
         interactive=interactive,
         save_pickle=save_pickle,
         colours=colours,
+        total_label=total_label,
     )
     cprint(f"Result is in {abspath(join(output_root, f'{output_name}.png'))}", "blue")
 
 
 def manager(
     input_path,
     seedname=None,
```

### Comparing `rad-tools-0.7.6/radtools/score/plot_tb2j.py` & `rad-tools-0.7.7/radtools/score/plot_tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/scripts/compute-energies.py` & `rad-tools-0.7.7/scripts/compute-energies.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/scripts/phonopy-plotter.py` & `rad-tools-0.7.7/scripts/phonopy-plotter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.6/setup.py` & `rad-tools-0.7.7/setup.py`

 * *Files identical despite different names*

