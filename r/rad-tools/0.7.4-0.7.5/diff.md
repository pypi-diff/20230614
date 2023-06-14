# Comparing `tmp/rad-tools-0.7.4.tar.gz` & `tmp/rad-tools-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-tools-0.7.4.tar", last modified: Tue Jun 13 17:36:53 2023, max compression
+gzip compressed data, was "rad-tools-0.7.5.tar", last modified: Wed Jun 14 01:09:47 2023, max compression
```

## Comparing `rad-tools-0.7.4.tar` & `rad-tools-0.7.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 17:36:53.783584 rad-tools-0.7.4/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.7.4/LICENSE.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-13 17:36:53.782750 rad-tools-0.7.4/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2139 2023-06-08 15:38:54.000000 rad-tools-0.7.4/README.rst
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 17:36:53.753558 rad-tools-0.7.4/rad_tools.egg-info/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-13 17:36:53.000000 rad-tools-0.7.4/rad_tools.egg-info/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1137 2023-06-13 17:36:53.000000 rad-tools-0.7.4/rad_tools.egg-info/SOURCES.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-13 17:36:53.000000 rad-tools-0.7.4/rad_tools.egg-info/dependency_links.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-13 17:36:53.000000 rad-tools-0.7.4/rad_tools.egg-info/requires.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-06-13 17:36:53.000000 rad-tools-0.7.4/rad_tools.egg-info/top_level.txt
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 17:36:53.756154 rad-tools-0.7.4/radtools/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      560 2023-06-13 17:36:25.000000 rad-tools-0.7.4/radtools/__init__.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 17:36:53.764947 rad-tools-0.7.4/radtools/crystal/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      353 2023-06-13 11:44:25.000000 rad-tools-0.7.4/radtools/crystal/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     7405 2023-06-13 11:44:25.000000 rad-tools-0.7.4/radtools/crystal/atom.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1183 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/crystal/atom_types.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    87365 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/crystal/bravais_lattice.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    18380 2023-06-13 13:58:51.000000 rad-tools-0.7.4/radtools/crystal/crystal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    23756 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/crystal/identify.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    36933 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/crystal/lattice.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4754 2023-06-13 11:44:25.000000 rad-tools-0.7.4/radtools/crystal/properties.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 17:36:53.767758 rad-tools-0.7.4/radtools/dos/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/dos/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    21701 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/dos/dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    22429 2023-06-13 17:36:25.000000 rad-tools-0.7.4/radtools/dos/pdos.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 17:36:53.769928 rad-tools-0.7.4/radtools/exchange/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      299 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/exchange/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    50003 2023-06-13 11:44:25.000000 rad-tools-0.7.4/radtools/exchange/hamiltonian.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    12330 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/exchange/parameter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/exchange/template.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 17:36:53.771508 rad-tools-0.7.4/radtools/io/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      421 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/io/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1929 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/io/internal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     5485 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/io/tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/map.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    18633 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/routines.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 17:36:53.775039 rad-tools-0.7.4/radtools/score/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1639 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/score/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4506 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/score/extract_tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/score/identify_wannier_centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4692 2023-06-13 11:44:25.000000 rad-tools-0.7.4/radtools/score/make_template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    13280 2023-06-13 16:17:28.000000 rad-tools-0.7.4/radtools/score/plot_dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     9914 2023-06-08 15:38:54.000000 rad-tools-0.7.4/radtools/score/plot_tb2j.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 17:36:53.781253 rad-tools-0.7.4/scripts/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.7.4/scripts/compute-energies.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.7.4/scripts/phonopy-plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-06-08 15:38:54.000000 rad-tools-0.7.4/scripts/rad-extract-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-06-08 15:38:54.000000 rad-tools-0.7.4/scripts/rad-identify-wannier-centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-06-08 15:38:54.000000 rad-tools-0.7.4/scripts/rad-make-template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-06-08 15:38:54.000000 rad-tools-0.7.4/scripts/rad-plot-dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-08 15:38:54.000000 rad-tools-0.7.4/scripts/rad-plot-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-13 17:36:53.783754 rad-tools-0.7.4/setup.cfg
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1411 2023-06-08 15:39:52.000000 rad-tools-0.7.4/setup.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.367844 rad-tools-0.7.5/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.7.5/LICENSE.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 01:09:47.367150 rad-tools-0.7.5/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2139 2023-06-08 15:38:54.000000 rad-tools-0.7.5/README.rst
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.338437 rad-tools-0.7.5/rad_tools.egg-info/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-14 01:09:47.000000 rad-tools-0.7.5/rad_tools.egg-info/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1137 2023-06-14 01:09:47.000000 rad-tools-0.7.5/rad_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-14 01:09:47.000000 rad-tools-0.7.5/rad_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 01:09:47.000000 rad-tools-0.7.5/rad_tools.egg-info/requires.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-06-14 01:09:47.000000 rad-tools-0.7.5/rad_tools.egg-info/top_level.txt
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.340706 rad-tools-0.7.5/radtools/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      560 2023-06-14 01:04:27.000000 rad-tools-0.7.5/radtools/__init__.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.347323 rad-tools-0.7.5/radtools/crystal/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      353 2023-06-13 11:44:25.000000 rad-tools-0.7.5/radtools/crystal/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     7405 2023-06-13 11:44:25.000000 rad-tools-0.7.5/radtools/crystal/atom.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1183 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/crystal/atom_types.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    87365 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/crystal/bravais_lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18380 2023-06-13 13:58:51.000000 rad-tools-0.7.5/radtools/crystal/crystal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    23756 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/crystal/identify.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    36933 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/crystal/lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4754 2023-06-13 11:44:25.000000 rad-tools-0.7.5/radtools/crystal/properties.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.350879 rad-tools-0.7.5/radtools/dos/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/dos/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    21650 2023-06-14 01:04:15.000000 rad-tools-0.7.5/radtools/dos/dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    23738 2023-06-14 01:04:15.000000 rad-tools-0.7.5/radtools/dos/pdos.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.354023 rad-tools-0.7.5/radtools/exchange/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      299 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/exchange/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    50003 2023-06-13 11:44:25.000000 rad-tools-0.7.5/radtools/exchange/hamiltonian.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    12330 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/exchange/parameter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/exchange/template.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.356072 rad-tools-0.7.5/radtools/io/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      421 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/io/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1929 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/io/internal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     5485 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/io/tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/map.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18633 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/routines.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.359214 rad-tools-0.7.5/radtools/score/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1639 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/score/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4506 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/score/extract_tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/score/identify_wannier_centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4692 2023-06-13 11:44:25.000000 rad-tools-0.7.5/radtools/score/make_template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    19943 2023-06-14 01:04:15.000000 rad-tools-0.7.5/radtools/score/plot_dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     9914 2023-06-08 15:38:54.000000 rad-tools-0.7.5/radtools/score/plot_tb2j.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-14 01:09:47.366300 rad-tools-0.7.5/scripts/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.7.5/scripts/compute-energies.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.7.5/scripts/phonopy-plotter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-06-08 15:38:54.000000 rad-tools-0.7.5/scripts/rad-extract-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-06-08 15:38:54.000000 rad-tools-0.7.5/scripts/rad-identify-wannier-centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-06-08 15:38:54.000000 rad-tools-0.7.5/scripts/rad-make-template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-06-08 15:38:54.000000 rad-tools-0.7.5/scripts/rad-plot-dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-08 15:38:54.000000 rad-tools-0.7.5/scripts/rad-plot-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-14 01:09:47.368005 rad-tools-0.7.5/setup.cfg
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1411 2023-06-08 15:39:52.000000 rad-tools-0.7.5/setup.py
```

### Comparing `rad-tools-0.7.4/LICENSE.txt` & `rad-tools-0.7.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/PKG-INFO` & `rad-tools-0.7.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.7.4
+Version: 0.7.5
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.7.4/README.rst` & `rad-tools-0.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/rad_tools.egg-info/PKG-INFO` & `rad-tools-0.7.5/rad_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.7.4
+Version: 0.7.5
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.7.4/rad_tools.egg-info/SOURCES.txt` & `rad-tools-0.7.5/rad_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/__init__.py` & `rad-tools-0.7.5/radtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 r"""
 All tools from the package.
 
 
 |version|
 """
 
-__version__ = "0.7.4"
+__version__ = "0.7.5"
 
 from . import crystal, dos, exchange, io, score
 from .crystal import *
 from .dos import *
 from .exchange import *
 from .io import *
 from .routines import *
```

### Comparing `rad-tools-0.7.4/radtools/crystal/atom.py` & `rad-tools-0.7.5/radtools/crystal/atom.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/crystal/atom_types.py` & `rad-tools-0.7.5/radtools/crystal/atom_types.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/crystal/bravais_lattice.py` & `rad-tools-0.7.5/radtools/crystal/bravais_lattice.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/crystal/crystal.py` & `rad-tools-0.7.5/radtools/crystal/crystal.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/crystal/identify.py` & `rad-tools-0.7.5/radtools/crystal/identify.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/crystal/lattice.py` & `rad-tools-0.7.5/radtools/crystal/lattice.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/crystal/properties.py` & `rad-tools-0.7.5/radtools/crystal/properties.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/dos/dos.py` & `rad-tools-0.7.5/radtools/dos/dos.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,14 +268,15 @@
 
         If DOS is k resolved, then sum over k points.
 
         Parameters
         ----------
         squeeze : bool, default False
             Whether to sum over k points. Ignored if DOS is not k resolved.
+        Whether to fix updown in the noncollinear, non spin-orbit case.
 
         Returns
         -------
         total_dos : :numpy:`ndarray`
             Shape :math:`(2, n_e)` if DOS is collinear, spin-polarized;
             :math:`(n_e)` otherwise.
         """
@@ -305,15 +306,15 @@
                     / self.nkpoints
                 )[self.energy_window[0] : self.energy_window[1]]
             return dos[2].reshape((self.nkpoints, self.nepoints))[
                 :, self.energy_window[0] : self.energy_window[1]
             ]
         return dos[1][self.energy_window[0] : self.energy_window[1]]
 
-    def total_pdos(self, squeeze=False, fix_updown=False):
+    def total_pdos(self, squeeze=False):
         r"""
         Total partial density of states.
 
         If DOS is k resolved, then sum over k points.
 
         Parameters
         ----------
@@ -355,18 +356,15 @@
                         / self.nkpoints
                     )[:, self.energy_window[0] : self.energy_window[1]]
 
                 total_pdos = dos[3:5].reshape((2, self.nkpoints, self.nepoints))[
                     :, :, self.energy_window[0] : self.energy_window[1]
                 ]
             total_pdos = dos[2:4][:, self.energy_window[0] : self.energy_window[1]]
-            if fix_updown:
-                return np.array([total_pdos, total_pdos])
-            else:
-                return total_pdos
+            return total_pdos
 
         if self.k_resolved:
             if squeeze:
                 return (
                     np.sum(dos[3].reshape((self.nkpoints, self.nepoints)), axis=0)
                     / self.nkpoints
                 )[self.energy_window[0] : self.energy_window[1]]
@@ -635,15 +633,15 @@
             ax.fill_between(
                 self.energy,
                 -self.total_dos(squeeze=True),
                 0,
                 lw=0,
                 color="grey",
                 alpha=0.3,
-                label="-DOS",
+                label="$-$DOS",
             )
 
             ax.plot(
                 self.energy,
                 self.total_pdos(squeeze=True)[0],
                 "-",
                 lw=1,
```

### Comparing `rad-tools-0.7.4/radtools/dos/pdos.py` & `rad-tools-0.7.5/radtools/dos/pdos.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,27 @@
 import re
 from copy import deepcopy
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 
+COLOURS = [
+    "#00FFFF",
+    "#FF9720",
+    "#CD00FF",
+    "#FFFF2B",
+    "#00B9FF",
+    "#FF163D",
+    "#79FF35",
+    "#FF0BEA",
+    "#0200FF",
+]
+
+
 class PDOS:
     r"""
     Partial density of states, projected on arbitrary projections.
 
     Supports k-resolved density of states.
     Support spin-polarised and spin-unpolarised cases.
 
@@ -494,16 +507,17 @@
     ):
         if projectors is not None:
             pass
         elif projectors_group in self._projectors:
             projectors = self._projectors[projectors_group]
         elif re.fullmatch(self._pattern, projectors_group):
             l, j = projectors_group.split("_j")
-            m_j = range(1, 1 + int(2 * float(j) + 1))
-            projectors = [f"{l} ($m_j = {i}$)" for i in m_j]
+            m_j = range(0, int(2 * float(j) + 1))
+            projectors = [f"{l} ($m_J = {i - float(j):>4.1f}$)" for i in m_j]
+            projectors_group = f"{l} (J = {j})"
         else:
             raise ValueError(
                 "Projectors can not be assigned automatically, "
                 + "you have to provide explicit list of projectors. "
                 + f"Projectors group: {projectors_group}"
             )
         super().__init__(energy, pdos, projectors_group, projectors, ldos, spin_pol)
@@ -516,14 +530,15 @@
     title=None,
     xlim=None,
     ylim=None,
     relative=False,
     normalize=False,
     interactive=False,
     save_pickle=False,
+    colours=COLOURS,
 ):
     r"""
     Plot PDOS.
 
     Parameters
     ----------
     pdos : :py:class:`.PDOS`
@@ -543,43 +558,34 @@
     normalize : bool, default False
         Whether to norma;ize relative plot style.
     interactive : bool, default False
         Whether to use interactive plotting mode.
     save_pickle : bool, default False
         Whether to save figure as a .pickle file.
         Helps for custom modification of particular figures.
+    colours : list
+        List of colours to be used. values are passed directly to matplotlib
     """
 
-    colours = [
-        "#0000FF",
-        "#FF0000",
-        "#00FF00",
-        "#FF00FF",
-        "#00FFFF",
-        "#3E3847",
-        "#FFD600",
-        "#366B35",
-        "#FF6F00",
-    ]
     n = len(pdos.projectors)
     pdos = pdos.squeezed()
 
     if relative:
         fig, ax = plt.subplots(figsize=(9, 4))
     else:
         fig, axs = plt.subplots(n, 1, figsize=(9, n * 2))
         if n == 1:
             axs = [axs]
     fig.subplots_adjust(hspace=0)
 
     def set_up_axis(ax, i):
         if normalize:
-            ax.set_ylabel("PDOS / LDOS", fontsize=12)
+            ax.set_ylabel("PDOS / LDOS", fontsize=15)
         else:
-            ax.set_ylabel("DOS, states/eV", fontsize=12)
+            ax.set_ylabel("DOS, states/eV", fontsize=15)
         if i == n - 1:
             ax.set_xlabel("E, ev", fontsize=15)
         else:
             ax.axes.get_xaxis().set_visible(False)
         if ylim is not None:
             ax.set_ylim(*tuple(ylim))
         if xlim is not None:
@@ -614,104 +620,138 @@
 
     for i, projector in enumerate(pdos):
         if not relative:
             ax = axs[i]
             set_up_axis(ax, i)
         if pdos.spin_pol:
             if relative:
+                if i == 0:
+                    ax.plot(
+                        pdos.energy,
+                        np.where(pdos.ldos[0] > 1e-5, pdos.ldos[0], None),
+                        "-",
+                        lw=1,
+                        color="blue",
+                        alpha=0.8,
+                        label=f"{pdos.projectors_group} (up)",
+                    )
+                    ax.plot(
+                        pdos.energy,
+                        np.where(pdos.ldos[1] > 1e-5, -pdos.ldos[1], None),
+                        "-",
+                        lw=1,
+                        color="red",
+                        alpha=0.8,
+                        label=f"{pdos.projectors_group} (down)",
+                    )
                 ax.fill_between(
                     pdos.energy,
                     np.sum(pdos[:i], axis=0)[0],
                     np.sum(pdos[: i + 1], axis=0)[0],
                     lw=0,
                     color=colours[i % len(colours)],
-                    alpha=0.3,
-                    label=f"{projector} (up)",
+                    # alpha=0.5,
+                    label=f"{projector}",
                 )
                 ax.fill_between(
                     pdos.energy,
                     -np.sum(pdos[:i], axis=0)[1],
                     -np.sum(pdos[: i + 1], axis=0)[1],
                     lw=0,
                     color=colours[i % len(colours)],
-                    alpha=0.3,
-                    label=f"{projector} (down)",
+                    # alpha=0.5,
                 )
             else:
                 ax.fill_between(
                     pdos.energy,
                     0,
                     pdos.ldos[0],
                     lw=0,
                     color="blue",
-                    alpha=0.3,
+                    alpha=0.2,
                     label=f"{pdos.projectors_group} (up)",
                 )
                 ax.fill_between(
                     pdos.energy,
                     0,
                     -pdos.ldos[1],
                     lw=0,
                     color="red",
-                    alpha=0.3,
+                    alpha=0.2,
                     label=f"{pdos.projectors_group} (down)",
                 )
 
                 ax.plot(
                     pdos.energy,
                     pdos[projector][0],
                     "-",
-                    lw=0.5,
+                    lw=0.8,
                     color="blue",
                     alpha=0.8,
                     label=f"{projector} (up)",
                 )
                 ax.plot(
                     pdos.energy,
                     -pdos[projector][1],
                     "-",
-                    lw=0.5,
+                    lw=0.8,
                     color="red",
                     alpha=0.8,
                     label=f"{projector} (down)",
                 )
         else:
             if relative:
+                if i == 0:
+                    ax.plot(
+                        pdos.energy,
+                        np.where(pdos.ldos > 1e-5, pdos.ldos, None),
+                        "-",
+                        lw=1,
+                        color="black",
+                        alpha=0.8,
+                        label=pdos.projectors_group,
+                    )
                 ax.fill_between(
                     pdos.energy,
                     np.sum(pdos[:i], axis=0),
                     np.sum(pdos[: i + 1], axis=0),
                     lw=0,
                     color=colours[i % len(colours)],
-                    alpha=0.3,
+                    # alpha=0.5,
                     label=projector,
                 )
+
             else:
                 ax.fill_between(
                     pdos.energy,
                     0,
                     pdos.ldos,
                     lw=0,
                     color="black",
                     alpha=0.3,
                     label=pdos.projectors_group,
                 )
                 ax.plot(
                     pdos.energy,
                     pdos[projector],
                     "-",
-                    lw=0.5,
+                    lw=0.8,
                     color="black",
                     alpha=0.8,
                     label=projector,
                 )
         if interactive:
-            ax.legend(loc=(1.025, 0.2), bbox_transform=ax.transAxes, draggable=True)
+            ax.legend(
+                loc=(1.025, 0.2),
+                bbox_transform=ax.transAxes,
+                draggable=True,
+                fontsize=12,
+            )
         else:
-            ax.legend(loc=(1.025, 0.2), bbox_transform=ax.transAxes)
+            ax.legend(loc=(1.025, 0.2), bbox_transform=ax.transAxes, fontsize=12)
 
     if interactive:
         plt.show()
     else:
         plt.savefig(f"{output_name}.png", dpi=400, bbox_inches="tight")
         if save_pickle:
             import pickle
```

### Comparing `rad-tools-0.7.4/radtools/exchange/hamiltonian.py` & `rad-tools-0.7.5/radtools/exchange/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/exchange/parameter.py` & `rad-tools-0.7.5/radtools/exchange/parameter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/exchange/template.py` & `rad-tools-0.7.5/radtools/exchange/template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/io/internal.py` & `rad-tools-0.7.5/radtools/io/internal.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/io/tb2j.py` & `rad-tools-0.7.5/radtools/io/tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/map.py` & `rad-tools-0.7.5/radtools/map.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/routines.py` & `rad-tools-0.7.5/radtools/routines.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/score/__init__.py` & `rad-tools-0.7.5/radtools/score/__init__.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/score/extract_tb2j.py` & `rad-tools-0.7.5/radtools/score/extract_tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/score/identify_wannier_centres.py` & `rad-tools-0.7.5/radtools/score/identify_wannier_centres.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/score/make_template.py` & `rad-tools-0.7.5/radtools/score/make_template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/radtools/score/plot_dos.py` & `rad-tools-0.7.5/radtools/score/plot_dos.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # TODO Fix background total + non-colinear-nonspin-orbit
 
 import re
 from argparse import ArgumentParser
 from os import makedirs, walk
-from os.path import abspath, join
+from os.path import abspath, join, isfile
 
 from termcolor import cprint
 from tqdm import tqdm
 
 from radtools.dos.dos import DOSQE
-from radtools.dos.pdos import PDOS, plot_projected
+from radtools.dos.pdos import PDOS, plot_projected, COLOURS
 
 
 def detect_seednames(input_path):
     r"""
     Analyze input folder, detects seednames for the dos output files.
 
     Parameters
@@ -42,14 +42,362 @@
         elif re.match(f".*{pattern}$", file):
             seednames.add(re.split(f"{pattern}$", file)[0])
     seednames = list(seednames)
 
     return seednames
 
 
+def plot_orbital_resolved(
+    dos,
+    output_root=".",
+    energy_window=None,
+    dos_window=None,
+    efermi=0.0,
+    separate=False,
+    relative=False,
+    normalize=False,
+    interactive=False,
+    save_pickle=False,
+    save_txt=False,
+    background_total=False,
+    colours=COLOURS,
+):
+    cprint("Orbital-resolved PDOS:", "green")
+    local_output = join(output_root, "orbital-resolved")
+    makedirs(local_output, exist_ok=True)
+    data = {}
+    for atom, atom_number, wfc, wfc_number in dos:
+        if atom not in data:
+            data[atom] = []
+        data[atom].append((wfc, wfc_number))
+
+    # Avoid repetitions
+    for atom in data:
+        data[atom] = list(set(data[atom]))
+
+    for atom in data:
+        for wfc, wfc_number in data[atom]:
+            if separate:
+                atom_numbers = dos.atom_numbers(atom)
+            else:
+                atom_numbers = [None]
+
+            for atom_number in tqdm(atom_numbers, desc=f"  {atom} {wfc} #{wfc_number}"):
+                if separate:
+                    atom_name = f"{atom}#{atom_number}"
+                else:
+                    atom_name = atom
+
+                if efermi == 0:
+                    title = f"PDOS for {atom_name} ({wfc} #{wfc_number}) (0 is 0)"
+                else:
+                    title = f"PDOS for {atom_name} ({wfc} #{wfc_number}) (0 is Fermi energy)"
+
+                pdos = dos.pdos(
+                    atom=atom,
+                    wfc=wfc,
+                    wfc_number=wfc_number,
+                    atom_numbers=atom_number,
+                    background_total=background_total,
+                )
+                if background_total:
+                    pdos.projectors_group = "Total PDOS"
+                if save_txt:
+                    pdos.dump_txt(
+                        join(local_output, f"{atom_name}_{wfc}#{wfc_number}.txt")
+                    )
+                plot_projected(
+                    pdos=pdos,
+                    efermi=efermi,
+                    output_name=join(local_output, f"{atom_name}_{wfc}#{wfc_number}"),
+                    title=title,
+                    xlim=energy_window,
+                    ylim=dos_window,
+                    relative=relative,
+                    normalize=normalize,
+                    interactive=interactive,
+                    save_pickle=save_pickle,
+                    colours=colours,
+                )
+    cprint(f"Results are in {abspath(local_output)}", "blue")
+
+
+def plot_atom_resolved(
+    dos,
+    output_root=".",
+    energy_window=None,
+    dos_window=None,
+    efermi=0.0,
+    separate=False,
+    relative=False,
+    normalize=False,
+    interactive=False,
+    save_pickle=False,
+    save_txt=False,
+    background_total=False,
+    colours=COLOURS,
+):
+    cprint("Orbital's contribution for each atom.", "green")
+    local_output = join(output_root, "atom-resolved")
+    makedirs(local_output, exist_ok=True)
+
+    for atom in dos.atoms:
+        if separate:
+            atom_numbers = dos.atom_numbers(atom)
+        else:
+            atom_numbers = [None]
+        for atom_number in tqdm(atom_numbers, desc=f"  {atom}"):
+            if separate:
+                atom_name = f"{atom}#{atom_number}"
+            else:
+                atom_name = atom
+            projectors = []
+            pdos = []
+            for wfc, wfc_number in dos.wfcs(atom, atom_number):
+                projectors.append(f"{wfc} #{wfc_number}")
+                pdos.append(dos.pdos(atom, wfc, wfc_number, atom_number).ldos)
+
+            if background_total:
+                pdos = PDOS(
+                    energy=dos.energy,
+                    pdos=pdos,
+                    ldos=dos.total_pdos(),
+                    projectors_group=atom_name,
+                    projectors=projectors,
+                    spin_pol=dos.case in [2, 3],
+                )
+                pdos.projectors_group = "Total PDOS"
+            else:
+                pdos = PDOS(
+                    energy=dos.energy,
+                    pdos=pdos,
+                    projectors_group=atom_name,
+                    projectors=projectors,
+                    spin_pol=dos.case in [2, 3],
+                )
+            if efermi == 0:
+                title = f"PDOS for {atom_name} (0 is 0)"
+            else:
+                title = f"PDOS for {atom_name} (0 is Fermi energy)"
+            if save_txt:
+                pdos.dump_txt(join(local_output, f"{atom_name}.txt"))
+            plot_projected(
+                pdos=pdos,
+                efermi=efermi,
+                output_name=join(local_output, atom_name),
+                title=title,
+                xlim=energy_window,
+                ylim=dos_window,
+                relative=relative,
+                normalize=normalize,
+                interactive=interactive,
+                save_pickle=save_pickle,
+                colours=colours,
+            )
+    cprint(f"Results are in {abspath(local_output)}", "blue")
+
+
+def plot_atom_to_total(
+    dos,
+    output_root=".",
+    energy_window=None,
+    dos_window=None,
+    efermi=0.0,
+    separate=False,
+    relative=False,
+    normalize=False,
+    interactive=False,
+    save_pickle=False,
+    save_txt=False,
+    background_total=False,
+    colours=COLOURS,
+):
+    cprint("Atom's contributions into total PDOS:", "green")
+    projectors = []
+    pdos = []
+    for atom in dos.atoms:
+        if separate:
+            atom_numbers = dos.atom_numbers(atom)
+        else:
+            atom_numbers = [None]
+        for atom_number in atom_numbers:
+            if separate:
+                atom_name = f"{atom}#{atom_number}"
+            else:
+                atom_name = atom
+            projectors.append(atom_name)
+            for i, (wfc, wfc_number) in enumerate(dos.wfcs(atom, atom_number)):
+                if i == 0:
+                    ldos = dos.pdos(atom, wfc, wfc_number, atom_number).ldos
+                else:
+                    ldos += dos.pdos(atom, wfc, wfc_number, atom_number).ldos
+            pdos.append(ldos)
+    if background_total:
+        pdos = PDOS(
+            energy=dos.energy,
+            pdos=pdos,
+            ldos=dos.total_pdos(),
+            projectors_group="Total PDOS",
+            projectors=projectors,
+            spin_pol=dos.case in [2, 3],
+        )
+        pdos.projectors_group = "Total PDOS"
+    else:
+        pdos = PDOS(
+            energy=dos.energy,
+            pdos=pdos,
+            projectors_group="Total PDOS",
+            projectors=projectors,
+            spin_pol=dos.case in [2, 3],
+        )
+
+    if efermi == 0:
+        title = f"Atom contribution in PDOS (0 is 0)"
+    else:
+        title = f"Atom contribution in PDOS (0 is Fermi energy)"
+    if save_txt:
+        pdos.dump_txt(join(output_root, "atomic-contributions.txt"))
+    plot_projected(
+        pdos=pdos,
+        efermi=efermi,
+        output_name=join(output_root, "atomic-contributions"),
+        title=title,
+        xlim=energy_window,
+        ylim=dos_window,
+        relative=relative,
+        normalize=normalize,
+        interactive=interactive,
+        save_pickle=save_pickle,
+        colours=colours,
+    )
+    cprint(f"Result is in {abspath(output_root)}", "blue")
+
+
+def plot_custom(
+    dos,
+    custom,
+    output_root=".",
+    energy_window=None,
+    dos_window=None,
+    efermi=0.0,
+    relative=False,
+    normalize=False,
+    interactive=False,
+    save_pickle=False,
+    save_txt=False,
+    background_total=False,
+    colours=COLOURS,
+):
+    cprint("Plotting custom plot", "green")
+    print("Input is understood as:")
+    projectors = []
+    pdos = []
+    for entry in custom:
+        projectors.append(entry)
+        cprint(f'"{entry}":', "green")
+        entry = entry.replace(" ", "").replace(")", "")
+        tmp = entry.split("(")[0]
+        atom = tmp.split("#")[0]
+        print(f"  * Atom type is {atom}")
+        if "#" in tmp:
+            atom_numbers = list(map(int, tmp.split("#")[1:]))
+        else:
+            atom_numbers = dos.atom_numbers(atom)
+
+        print(f"  * PDOS is summed among the following atoms:", end="\n      ")
+        for i, number in enumerate(atom_numbers):
+            print(f"{atom}#{number}", end="")
+            if i != len(atom_numbers) - 1:
+                print(end=", ")
+            else:
+                print()
+        if "(" in entry:
+            tmp = entry.split("(")[1].split(",")
+            wfcs = []
+            for i in tmp:
+                wfc = i.split("#")[0]
+                if "#" in i:
+                    tmp_numbers = list(map(int, i.split("#")[1:]))
+                    for number in tmp_numbers:
+                        wfcs.append((wfc, number))
+                else:
+                    wfc_list = dos.wfcs(atom)
+                    for name, number in wfc_list:
+                        if name == wfc:
+                            wfcs.append((wfc, number))
+        else:
+            wfcs = dos.wfcs(atom)
+
+        print(
+            "  * For each atom PDOS is summed among the following projections:",
+            end="\n      ",
+        )
+        for i, (name, number) in enumerate(wfcs):
+            print(f"{name}#{number}", end="")
+            if i != len(wfcs) - 1:
+                print(end=", ")
+            else:
+                print()
+
+        tmp = None
+        for name, number in wfcs:
+            if tmp is None:
+                tmp = dos.pdos(
+                    atom=atom, wfc=name, wfc_number=number, atom_numbers=atom_numbers
+                ).ldos
+            else:
+                tmp += dos.pdos(
+                    atom=atom, wfc=name, wfc_number=number, atom_numbers=atom_numbers
+                ).ldos
+
+        pdos.append(tmp)
+
+    if background_total:
+        pdos = PDOS(
+            energy=dos.energy,
+            pdos=pdos,
+            ldos=dos.total_pdos(),
+            projectors_group="Total PDOS",
+            projectors=projectors,
+            spin_pol=dos.case in [2, 3],
+        )
+    else:
+        pdos = PDOS(
+            energy=dos.energy,
+            pdos=pdos,
+            projectors_group="Total (sum)",
+            projectors=projectors,
+            spin_pol=dos.case in [2, 3],
+        )
+
+    if isfile(join(output_root, "custom.png")):
+        i = 1
+        while isfile(join(output_root, f"custom{i}.png")):
+            i += 1
+        output_name = f"custom{i}"
+    else:
+        output_name = "custom"
+
+    if save_txt:
+        pdos.dump_txt(join(output_root, f"{output_name}.txt"))
+    plot_projected(
+        pdos=pdos,
+        efermi=efermi,
+        output_name=join(output_root, output_name),
+        xlim=energy_window,
+        ylim=dos_window,
+        relative=relative,
+        normalize=normalize,
+        interactive=interactive,
+        save_pickle=save_pickle,
+        colours=colours,
+    )
+    cprint(f"Result is in {abspath(join(output_root, f'{output_name}.png'))}", "blue")
+
+
 def manager(
     input_path,
     seedname=None,
     output_path=".",
     energy_window=None,
     dos_window=None,
     efermi=0.0,
@@ -57,23 +405,27 @@
     relative=False,
     normalize=False,
     verbose=False,
     interactive=False,
     save_pickle=False,
     save_txt=False,
     background_total=False,
+    custom=None,
+    colours=None,
 ):
     r"""
     ``rad-plot-dos.py`` script.
 
     Full documentation on the behaviour is available in the
     :ref:`User Guide <rad-plot-dos>`.
     Parameters of the function directly
     correspond to the arguments of the script.
     """
+    if colours is None:
+        colours = COLOURS
     makedirs(output_path, exist_ok=True)
 
     suffix = ""
     if relative:
         suffix += "-relative"
     if normalize:
         suffix += "-normalized"
@@ -83,228 +435,115 @@
         suffix += "-vstotal"
 
     # Detect seednames if not provided.
     if seedname is None:
         seednames = detect_seednames(input_path)
         print(f"Following DOS seednames (filpdos) are detected:")
         for item in seednames:
-            cprint(f"   * {item}", "green")
+            cprint(f"   * {item}", "green", attrs=["bold"])
     else:
         seednames = [seedname]
 
     # Work with each seedname.
     for s_i, seedname in enumerate(seednames):
         cprint(
             f"({s_i + 1}/{len(seednames)}) Start to work with {seedname} seedname",
-            "green",
+            "yellow",
+            attrs=["bold"],
         )
         # Preparations
         output_root = join(output_path, f"{seedname}{suffix}")
         makedirs(output_root, exist_ok=True)
 
         # Load DOS data.
         dos = DOSQE(seedname, input_path, energy_window=energy_window, efermi=efermi)
         print(f"{dos.casename} case detected.")
         for atom in dos.atoms:
-            print(f"    {len(dos.atom_numbers(atom))} of {atom} detected")
-
-        # Plot PDOS vs DOS
-        cprint("Total DOS vs total PDOS", "green")
-        dos.plot_pdos_tot(
-            output_name=join(output_root, "pdos-vs-dos"),
-            interactive=interactive,
-            efermi=efermi,
-            xlim=energy_window,
-            ylim=dos_window,
-            save_pickle=save_pickle,
-        )
-        print(f"  Result is in {join(output_root, 'pdos-vs-dos')}")
-
-        # Plot PDOS for each atom/wfc
-        cprint("Orbital-resolved PDOS:", "green")
-        local_output = join(output_root, "orbital-resolved")
-        makedirs(local_output, exist_ok=True)
-        data = {}
-        for atom, atom_number, wfc, wfc_number in dos:
-            if atom not in data:
-                data[atom] = []
-            data[atom].append((wfc, wfc_number))
-
-        # Avoid repetitions
-        for atom in data:
-            data[atom] = list(set(data[atom]))
-
-        for atom in data:
-            for wfc, wfc_number in data[atom]:
-                if separate:
-                    atom_numbers = dos.atom_numbers(atom)
-                else:
-                    atom_numbers = [None]
+            print(f"  {len(dos.atom_numbers(atom))} {atom} detected")
 
-                for atom_number in tqdm(
-                    atom_numbers, desc=f"  {atom} {wfc} #{wfc_number}"
-                ):
-                    if separate:
-                        atom_name = f"{atom}#{atom_number}"
-                    else:
-                        atom_name = atom
-
-                    if efermi == 0:
-                        title = f"PDOS for {atom_name} ({wfc} #{wfc_number}) (0 is 0)"
-                    else:
-                        title = f"PDOS for {atom_name} ({wfc} #{wfc_number}) (0 is Fermi energy)"
-
-                    pdos = dos.pdos(
-                        atom=atom,
-                        wfc=wfc,
-                        wfc_number=wfc_number,
-                        atom_numbers=atom_number,
-                        background_total=background_total,
-                    )
-                    if background_total:
-                        pdos.projectors_group = "Total PDOS"
-                    if save_txt:
-                        pdos.dump_txt(
-                            join(local_output, f"{atom_name}_{wfc}#{wfc_number}.txt")
-                        )
-                    plot_projected(
-                        pdos=pdos,
-                        efermi=efermi,
-                        output_name=join(
-                            local_output, f"{atom_name}_{wfc}#{wfc_number}"
-                        ),
-                        title=title,
-                        xlim=energy_window,
-                        ylim=dos_window,
-                        relative=relative,
-                        normalize=normalize,
-                        interactive=interactive,
-                        save_pickle=save_pickle,
-                    )
-        print(f"  Results are in {abspath(local_output)}")
-
-        # Plot wfc contribution into each atom
-        cprint("Orbital's contribution for each atom.", "green")
-        local_output = join(output_root, "atom-resolved")
-        makedirs(local_output, exist_ok=True)
+        if custom is None:
+            # Plot PDOS vs DOS
+            cprint("Total DOS vs total PDOS", "green")
+            dos.plot_pdos_tot(
+                output_name=join(output_root, "pdos-vs-dos"),
+                interactive=interactive,
+                efermi=efermi,
+                xlim=energy_window,
+                ylim=dos_window,
+                save_pickle=save_pickle,
+            )
+            cprint(f"Result is in {join(output_root, 'pdos-vs-dos')}", "blue")
 
-        for atom in dos.atoms:
-            if separate:
-                atom_numbers = dos.atom_numbers(atom)
-            else:
-                atom_numbers = [None]
-            for atom_number in tqdm(atom_numbers, desc=f"  {atom}"):
-                if separate:
-                    atom_name = f"{atom}#{atom_number}"
-                else:
-                    atom_name = atom
-                projectors = []
-                pdos = []
-                for wfc, wfc_number in dos.wfcs(atom, atom_number):
-                    projectors.append(f"{wfc} #{wfc_number}")
-                    pdos.append(dos.pdos(atom, wfc, wfc_number, atom_number).ldos)
+            # Plot PDOS for each atom/wfc
+            plot_orbital_resolved(
+                dos=dos,
+                output_root=output_root,
+                energy_window=energy_window,
+                dos_window=dos_window,
+                efermi=efermi,
+                separate=separate,
+                relative=relative,
+                normalize=normalize,
+                interactive=interactive,
+                save_pickle=save_pickle,
+                save_txt=save_txt,
+                background_total=background_total,
+                colours=colours,
+            )
 
-                if background_total:
-                    pdos = PDOS(
-                        energy=dos.energy,
-                        pdos=pdos,
-                        ldos=dos.total_pdos(fix_updown=True),
-                        projectors_group=atom_name,
-                        projectors=projectors,
-                        spin_pol=dos.case in [2, 3],
-                    )
-                    pdos.projectors_group = "Total PDOS"
-                else:
-                    pdos = PDOS(
-                        energy=dos.energy,
-                        pdos=pdos,
-                        projectors_group=atom_name,
-                        projectors=projectors,
-                        spin_pol=dos.case in [2, 3],
-                    )
-                if efermi == 0:
-                    title = f"PDOS for {atom_name} (0 is 0)"
-                else:
-                    title = f"PDOS for {atom_name} (0 is Fermi energy)"
-                if save_txt:
-                    pdos.dump_txt(join(local_output, f"{atom_name}.txt"))
-                plot_projected(
-                    pdos=pdos,
-                    efermi=efermi,
-                    output_name=join(local_output, atom_name),
-                    title=title,
-                    xlim=energy_window,
-                    ylim=dos_window,
-                    relative=relative,
-                    normalize=normalize,
-                    interactive=interactive,
-                    save_pickle=save_pickle,
-                )
-        print(f"  Results are in {abspath(local_output)}")
+            # Plot wfc contribution into each atom
+            plot_atom_resolved(
+                dos=dos,
+                output_root=output_root,
+                energy_window=energy_window,
+                dos_window=dos_window,
+                efermi=efermi,
+                separate=separate,
+                relative=relative,
+                normalize=normalize,
+                interactive=interactive,
+                save_pickle=save_pickle,
+                save_txt=save_txt,
+                background_total=background_total,
+                colours=colours,
+            )
 
-        # Plot atom contributions into total PDOS
-        cprint("Atom's contributions into total PDOS:", "green")
-        projectors = []
-        pdos = []
-        for atom in dos.atoms:
-            if separate:
-                atom_numbers = dos.atom_numbers(atom)
-            else:
-                atom_numbers = [None]
-            for atom_number in atom_numbers:
-                if separate:
-                    atom_name = f"{atom}#{atom_number}"
-                else:
-                    atom_name = atom
-                projectors.append(atom_name)
-                for i, (wfc, wfc_number) in enumerate(dos.wfcs(atom, atom_number)):
-                    if i == 0:
-                        ldos = dos.pdos(atom, wfc, wfc_number, atom_number).ldos
-                    else:
-                        ldos += dos.pdos(atom, wfc, wfc_number, atom_number).ldos
-                pdos.append(ldos)
-        if background_total:
-            pdos = PDOS(
-                energy=dos.energy,
-                pdos=pdos,
-                ldos=dos.total_pdos(fix_updown=True),
-                projectors_group="Total PDOS",
-                projectors=projectors,
-                spin_pol=dos.case in [2, 3],
+            # Plot atom contributions into total PDOS
+            plot_atom_to_total(
+                dos=dos,
+                output_root=output_root,
+                energy_window=energy_window,
+                dos_window=dos_window,
+                efermi=efermi,
+                separate=separate,
+                relative=relative,
+                normalize=normalize,
+                interactive=interactive,
+                save_pickle=save_pickle,
+                save_txt=save_txt,
+                background_total=background_total,
+                colours=colours,
             )
-            pdos.projectors_group = "Total PDOS"
         else:
-            pdos = PDOS(
-                energy=dos.energy,
-                pdos=pdos,
-                projectors_group="Total PDOS",
-                projectors=projectors,
-                spin_pol=dos.case in [2, 3],
+            plot_custom(
+                dos=dos,
+                custom=custom,
+                output_root=output_root,
+                energy_window=energy_window,
+                dos_window=dos_window,
+                efermi=efermi,
+                relative=relative,
+                normalize=normalize,
+                interactive=interactive,
+                save_pickle=save_pickle,
+                save_txt=save_txt,
+                background_total=background_total,
+                colours=colours,
             )
 
-        if efermi == 0:
-            title = f"Atom contribution in PDOS (0 is 0)"
-        else:
-            title = f"Atom contribution in PDOS (0 is Fermi energy)"
-        if save_txt:
-            pdos.dump_txt(join(output_root, "atomic-contributions.txt"))
-        plot_projected(
-            pdos=pdos,
-            efermi=efermi,
-            output_name=join(output_root, "atomic-contributions"),
-            title=title,
-            xlim=energy_window,
-            ylim=dos_window,
-            relative=relative,
-            normalize=normalize,
-            interactive=interactive,
-            save_pickle=save_pickle,
-        )
-        print(f"  Result is in {abspath(local_output)}")
-
 
 def create_parser():
     parser = ArgumentParser(
         description="Script for visualisation of density of states."
     )
     parser.add_argument(
         "-ip",
@@ -410,9 +649,26 @@
     parser.add_argument(
         "-bt",
         "--background-total",
         action="store_true",
         default=False,
         help="Whether to use total PDOS as the background for all plots.",
     )
+    parser.add_argument(
+        "--custom",
+        type=str,
+        metavar="description",
+        default=None,
+        nargs="*",
+        help="Custom PDOS plot. See docs for info.",
+    )
+    parser.add_argument(
+        "-cls",
+        "--colours",
+        type=str,
+        metavar="colours",
+        default=None,
+        nargs="*",
+        help="Colours for the relative and custom plots.",
+    )
 
     return parser
```

### Comparing `rad-tools-0.7.4/radtools/score/plot_tb2j.py` & `rad-tools-0.7.5/radtools/score/plot_tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/scripts/compute-energies.py` & `rad-tools-0.7.5/scripts/compute-energies.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/scripts/phonopy-plotter.py` & `rad-tools-0.7.5/scripts/phonopy-plotter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.4/setup.py` & `rad-tools-0.7.5/setup.py`

 * *Files identical despite different names*

