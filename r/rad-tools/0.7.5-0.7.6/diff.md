# Comparing `tmp/rad-tools-0.7.5.tar.gz` & `tmp/rad-tools-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-tools-0.7.5.tar", last modified: Wed Jun 14 01:09:47 2023, max compression
+gzip compressed data, was "rad-tools-0.7.6.tar", last modified: Wed Jun 14 12:18:55 2023, max compression
```

## Comparing `rad-tools-0.7.5.tar` & `rad-tools-0.7.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.367844 rad-tools-0.7.5/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.7.5/LICENSE.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 01:09:47.367150 rad-tools-0.7.5/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2139 2023-06-08 15:38:54.000000 rad-tools-0.7.5/README.rst
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.338437 rad-tools-0.7.5/rad_tools.egg-info/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 01:09:47.000000 rad-tools-0.7.5/rad_tools.egg-info/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1137 2023-06-14 01:09:47.000000 rad-tools-0.7.5/rad_tools.egg-info/SOURCES.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-14 01:09:47.000000 rad-tools-0.7.5/rad_tools.egg-info/dependency_links.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 01:09:47.000000 rad-tools-0.7.5/rad_tools.egg-info/requires.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-06-14 01:09:47.000000 rad-tools-0.7.5/rad_tools.egg-info/top_level.txt
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.340706 rad-tools-0.7.5/radtools/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      560 2023-06-14 01:04:27.000000 rad-tools-0.7.5/radtools/__init__.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.347323 rad-tools-0.7.5/radtools/crystal/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      353 2023-06-13 11:44:25.000000 rad-tools-0.7.5/radtools/crystal/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     7405 2023-06-13 11:44:25.000000 rad-tools-0.7.5/radtools/crystal/atom.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1183 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/crystal/atom_types.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    87365 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/crystal/bravais_lattice.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    18380 2023-06-13 13:58:51.000000 rad-tools-0.7.5/radtools/crystal/crystal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    23756 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/crystal/identify.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    36933 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/crystal/lattice.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4754 2023-06-13 11:44:25.000000 rad-tools-0.7.5/radtools/crystal/properties.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.350879 rad-tools-0.7.5/radtools/dos/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/dos/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    21650 2023-06-14 01:04:15.000000 rad-tools-0.7.5/radtools/dos/dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    23738 2023-06-14 01:04:15.000000 rad-tools-0.7.5/radtools/dos/pdos.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.354023 rad-tools-0.7.5/radtools/exchange/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      299 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/exchange/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    50003 2023-06-13 11:44:25.000000 rad-tools-0.7.5/radtools/exchange/hamiltonian.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    12330 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/exchange/parameter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/exchange/template.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.356072 rad-tools-0.7.5/radtools/io/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      421 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/io/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1929 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/io/internal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     5485 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/io/tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/map.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    18633 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/routines.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.359214 rad-tools-0.7.5/radtools/score/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1639 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/score/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4506 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/score/extract_tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/score/identify_wannier_centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4692 2023-06-13 11:44:25.000000 rad-tools-0.7.5/radtools/score/make_template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    19943 2023-06-14 01:04:15.000000 rad-tools-0.7.5/radtools/score/plot_dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     9914 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/score/plot_tb2j.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.366300 rad-tools-0.7.5/scripts/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.7.5/scripts/compute-energies.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.7.5/scripts/phonopy-plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-06-08 15:38:54.000000 rad-tools-0.7.5/scripts/rad-extract-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-06-08 15:38:54.000000 rad-tools-0.7.5/scripts/rad-identify-wannier-centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-06-08 15:38:54.000000 rad-tools-0.7.5/scripts/rad-make-template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-06-08 15:38:54.000000 rad-tools-0.7.5/scripts/rad-plot-dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-08 15:38:54.000000 rad-tools-0.7.5/scripts/rad-plot-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 01:09:47.368005 rad-tools-0.7.5/setup.cfg
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1411 2023-06-08 15:39:52.000000 rad-tools-0.7.5/setup.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.115363 rad-tools-0.7.6/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.7.6/LICENSE.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 12:18:55.114431 rad-tools-0.7.6/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2139 2023-06-08 15:38:54.000000 rad-tools-0.7.6/README.rst
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.011779 rad-tools-0.7.6/rad_tools.egg-info/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 12:18:54.000000 rad-tools-0.7.6/rad_tools.egg-info/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1137 2023-06-14 12:18:54.000000 rad-tools-0.7.6/rad_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-14 12:18:54.000000 rad-tools-0.7.6/rad_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 12:18:54.000000 rad-tools-0.7.6/rad_tools.egg-info/requires.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-06-14 12:18:54.000000 rad-tools-0.7.6/rad_tools.egg-info/top_level.txt
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.014784 rad-tools-0.7.6/radtools/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      560 2023-06-14 12:16:09.000000 rad-tools-0.7.6/radtools/__init__.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.028049 rad-tools-0.7.6/radtools/crystal/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      353 2023-06-13 11:44:25.000000 rad-tools-0.7.6/radtools/crystal/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     7405 2023-06-13 11:44:25.000000 rad-tools-0.7.6/radtools/crystal/atom.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1183 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/crystal/atom_types.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    87365 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/crystal/bravais_lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18380 2023-06-13 13:58:51.000000 rad-tools-0.7.6/radtools/crystal/crystal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    23756 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/crystal/identify.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    36933 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/crystal/lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4754 2023-06-13 11:44:25.000000 rad-tools-0.7.6/radtools/crystal/properties.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.034568 rad-tools-0.7.6/radtools/dos/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/dos/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    21650 2023-06-14 01:04:15.000000 rad-tools-0.7.6/radtools/dos/dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    23738 2023-06-14 01:04:15.000000 rad-tools-0.7.6/radtools/dos/pdos.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.041204 rad-tools-0.7.6/radtools/exchange/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      299 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/exchange/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    50003 2023-06-13 11:44:25.000000 rad-tools-0.7.6/radtools/exchange/hamiltonian.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    12330 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/exchange/parameter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/exchange/template.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.043738 rad-tools-0.7.6/radtools/io/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      421 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/io/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1929 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/io/internal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     5485 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/io/tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/map.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18633 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/routines.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.068563 rad-tools-0.7.6/radtools/score/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1639 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/score/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4506 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/score/extract_tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/score/identify_wannier_centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4692 2023-06-13 11:44:25.000000 rad-tools-0.7.6/radtools/score/make_template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    21069 2023-06-14 12:15:54.000000 rad-tools-0.7.6/radtools/score/plot_dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     9914 2023-06-08 15:38:54.000000 rad-tools-0.7.6/radtools/score/plot_tb2j.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 12:18:55.113901 rad-tools-0.7.6/scripts/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.7.6/scripts/compute-energies.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.7.6/scripts/phonopy-plotter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-06-08 15:38:54.000000 rad-tools-0.7.6/scripts/rad-extract-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-06-08 15:38:54.000000 rad-tools-0.7.6/scripts/rad-identify-wannier-centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-06-08 15:38:54.000000 rad-tools-0.7.6/scripts/rad-make-template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-06-08 15:38:54.000000 rad-tools-0.7.6/scripts/rad-plot-dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-08 15:38:54.000000 rad-tools-0.7.6/scripts/rad-plot-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 12:18:55.115492 rad-tools-0.7.6/setup.cfg
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1411 2023-06-08 15:39:52.000000 rad-tools-0.7.6/setup.py
```

### Comparing `rad-tools-0.7.5/LICENSE.txt` & `rad-tools-0.7.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/PKG-INFO` & `rad-tools-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.7.5
+Version: 0.7.6
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.7.5/README.rst` & `rad-tools-0.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/rad_tools.egg-info/PKG-INFO` & `rad-tools-0.7.6/rad_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.7.5
+Version: 0.7.6
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.7.5/rad_tools.egg-info/SOURCES.txt` & `rad-tools-0.7.6/rad_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/__init__.py` & `rad-tools-0.7.6/radtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 r"""
 All tools from the package.
 
 
 |version|
 """
 
-__version__ = "0.7.5"
+__version__ = "0.7.6"
 
 from . import crystal, dos, exchange, io, score
 from .crystal import *
 from .dos import *
 from .exchange import *
 from .io import *
 from .routines import *
```

### Comparing `rad-tools-0.7.5/radtools/crystal/atom.py` & `rad-tools-0.7.6/radtools/crystal/atom.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/crystal/atom_types.py` & `rad-tools-0.7.6/radtools/crystal/atom_types.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/crystal/bravais_lattice.py` & `rad-tools-0.7.6/radtools/crystal/bravais_lattice.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/crystal/crystal.py` & `rad-tools-0.7.6/radtools/crystal/crystal.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/crystal/identify.py` & `rad-tools-0.7.6/radtools/crystal/identify.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/crystal/lattice.py` & `rad-tools-0.7.6/radtools/crystal/lattice.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/crystal/properties.py` & `rad-tools-0.7.6/radtools/crystal/properties.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/dos/dos.py` & `rad-tools-0.7.6/radtools/dos/dos.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/dos/pdos.py` & `rad-tools-0.7.6/radtools/dos/pdos.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/exchange/hamiltonian.py` & `rad-tools-0.7.6/radtools/exchange/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/exchange/parameter.py` & `rad-tools-0.7.6/radtools/exchange/parameter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/exchange/template.py` & `rad-tools-0.7.6/radtools/exchange/template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/io/internal.py` & `rad-tools-0.7.6/radtools/io/internal.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/io/tb2j.py` & `rad-tools-0.7.6/radtools/io/tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/map.py` & `rad-tools-0.7.6/radtools/map.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/routines.py` & `rad-tools-0.7.6/radtools/routines.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/score/__init__.py` & `rad-tools-0.7.6/radtools/score/__init__.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/score/extract_tb2j.py` & `rad-tools-0.7.6/radtools/score/extract_tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/score/identify_wannier_centres.py` & `rad-tools-0.7.6/radtools/score/identify_wannier_centres.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/score/make_template.py` & `rad-tools-0.7.6/radtools/score/make_template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/radtools/score/plot_dos.py` & `rad-tools-0.7.6/radtools/score/plot_dos.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,78 +282,98 @@
     relative=False,
     normalize=False,
     interactive=False,
     save_pickle=False,
     save_txt=False,
     background_total=False,
     colours=COLOURS,
+    labels=None,
 ):
     cprint("Plotting custom plot", "green")
     print("Input is understood as:")
     projectors = []
     pdos = []
-    for entry in custom:
-        projectors.append(entry)
+    if labels is not None and len(labels) != len(custom):
+        raise ValueError(
+            f"Got {len(labels)} labels, but {len(custom)} PDOS, have to be the same."
+        )
+    for i_e, entry in enumerate(custom):
+        if labels is not None:
+            projectors.append(labels[i_e])
+        else:
+            projectors.append(entry)
         cprint(f'"{entry}":', "green")
         entry = entry.replace(" ", "").replace(")", "")
-        tmp = entry.split("(")[0]
-        atom = tmp.split("#")[0]
-        print(f"  * Atom type is {atom}")
-        if "#" in tmp:
-            atom_numbers = list(map(int, tmp.split("#")[1:]))
-        else:
-            atom_numbers = dos.atom_numbers(atom)
-
-        print(f"  * PDOS is summed among the following atoms:", end="\n      ")
-        for i, number in enumerate(atom_numbers):
-            print(f"{atom}#{number}", end="")
-            if i != len(atom_numbers) - 1:
-                print(end=", ")
+        subentries = entry.split(";")
+        pdos_element = None
+        for subentry in subentries:
+            atom_part = subentry.split("(")[0]
+            atom = atom_part.split("#")[0]
+            if "#" in subentry:
+                atom_numbers = list(map(int, atom_part.split("#")[1:]))
             else:
-                print()
-        if "(" in entry:
-            tmp = entry.split("(")[1].split(",")
-            wfcs = []
-            for i in tmp:
-                wfc = i.split("#")[0]
-                if "#" in i:
-                    tmp_numbers = list(map(int, i.split("#")[1:]))
-                    for number in tmp_numbers:
-                        wfcs.append((wfc, number))
+                atom_numbers = dos.atom_numbers(atom)
+
+            cprint(
+                f"  * PDOS is summed among the following {atom} atoms:",
+                "green",
+                end="\n      ",
+            )
+            for i, number in enumerate(atom_numbers):
+                print(f"{atom}#{number}", end="")
+                if i != len(atom_numbers) - 1:
+                    print(end=", ")
                 else:
-                    wfc_list = dos.wfcs(atom)
-                    for name, number in wfc_list:
-                        if name == wfc:
-                            wfcs.append((wfc, number))
-        else:
-            wfcs = dos.wfcs(atom)
+                    print()
 
-        print(
-            "  * For each atom PDOS is summed among the following projections:",
-            end="\n      ",
-        )
-        for i, (name, number) in enumerate(wfcs):
-            print(f"{name}#{number}", end="")
-            if i != len(wfcs) - 1:
-                print(end=", ")
+            if "(" in subentry:
+                wfc_parts = subentry.split("(")[1].split(",")
+                wfcs = []
+                for wfc_part in wfc_parts:
+                    wfc = wfc_part.split("#")[0]
+                    if "#" in wfc_part:
+                        wfc_numbers = list(map(int, wfc_part.split("#")[1:]))
+                        for number in wfc_numbers:
+                            wfcs.append((wfc, number))
+                    else:
+                        wfc_list = dos.wfcs(atom)
+                        for name, number in wfc_list:
+                            if name == wfc:
+                                wfcs.append((wfc, number))
             else:
-                print()
+                wfcs = dos.wfcs(atom)
 
-        tmp = None
-        for name, number in wfcs:
-            if tmp is None:
-                tmp = dos.pdos(
-                    atom=atom, wfc=name, wfc_number=number, atom_numbers=atom_numbers
-                ).ldos
-            else:
-                tmp += dos.pdos(
-                    atom=atom, wfc=name, wfc_number=number, atom_numbers=atom_numbers
-                ).ldos
+            print(
+                f"  * For each {atom} atom PDOS is summed among the following projections:",
+                end="\n      ",
+            )
+            for i, (name, number) in enumerate(wfcs):
+                print(f"{name}#{number}", end="")
+                if i != len(wfcs) - 1:
+                    print(end=", ")
+                else:
+                    print()
+
+            for name, number in wfcs:
+                if pdos_element is None:
+                    pdos_element = dos.pdos(
+                        atom=atom,
+                        wfc=name,
+                        wfc_number=number,
+                        atom_numbers=atom_numbers,
+                    ).ldos
+                else:
+                    pdos_element += dos.pdos(
+                        atom=atom,
+                        wfc=name,
+                        wfc_number=number,
+                        atom_numbers=atom_numbers,
+                    ).ldos
 
-        pdos.append(tmp)
+        pdos.append(pdos_element)
 
     if background_total:
         pdos = PDOS(
             energy=dos.energy,
             pdos=pdos,
             ldos=dos.total_pdos(),
             projectors_group="Total PDOS",
@@ -407,14 +427,15 @@
     verbose=False,
     interactive=False,
     save_pickle=False,
     save_txt=False,
     background_total=False,
     custom=None,
     colours=None,
+    labels=None,
 ):
     r"""
     ``rad-plot-dos.py`` script.
 
     Full documentation on the behaviour is available in the
     :ref:`User Guide <rad-plot-dos>`.
     Parameters of the function directly
@@ -534,14 +555,15 @@
                 relative=relative,
                 normalize=normalize,
                 interactive=interactive,
                 save_pickle=save_pickle,
                 save_txt=save_txt,
                 background_total=background_total,
                 colours=colours,
+                labels=labels,
             )
 
 
 def create_parser():
     parser = ArgumentParser(
         description="Script for visualisation of density of states."
     )
@@ -666,9 +688,18 @@
         "--colours",
         type=str,
         metavar="colours",
         default=None,
         nargs="*",
         help="Colours for the relative and custom plots.",
     )
+    parser.add_argument(
+        "-lbs",
+        "--labels",
+        type=str,
+        metavar="labels",
+        default=None,
+        nargs="*",
+        help="Labels for the custom plots.",
+    )
 
     return parser
```

### Comparing `rad-tools-0.7.5/radtools/score/plot_tb2j.py` & `rad-tools-0.7.6/radtools/score/plot_tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/scripts/compute-energies.py` & `rad-tools-0.7.6/scripts/compute-energies.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/scripts/phonopy-plotter.py` & `rad-tools-0.7.6/scripts/phonopy-plotter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.5/setup.py` & `rad-tools-0.7.6/setup.py`

 * *Files identical despite different names*

