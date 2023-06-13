# Comparing `tmp/pySailingVLM-1.0.0.tar.gz` & `tmp/pySailingVLM-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pySailingVLM-1.0.0.tar", last modified: Tue Jun 13 12:58:17 2023, max compression
+gzip compressed data, was "pySailingVLM-1.0.1.tar", last modified: Tue Jun 13 22:53:14 2023, max compression
```

## Comparing `pySailingVLM-1.0.0.tar` & `pySailingVLM-1.0.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 12:58:17.518308 pySailingVLM-1.0.0/
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)    11357 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/LICENSE
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     2465 2023-06-13 12:58:17.518308 pySailingVLM-1.0.0/PKG-INFO
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     1397 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/README.md
-drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 12:58:17.502307 pySailingVLM-1.0.0/pySailingVLM/
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)      143 2023-06-13 12:48:20.000000 pySailingVLM-1.0.0/pySailingVLM/__main__.py
-drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 12:58:17.506307 pySailingVLM-1.0.0/pySailingVLM/examples/
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4506 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/examples/rectangle_variables.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4463 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/examples/sweep_variables.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4340 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/examples/variables.py
-drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 12:58:17.506307 pySailingVLM-1.0.0/pySailingVLM/inlet/
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/inlet/__init__.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     1935 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/inlet/inlet_conditions.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     7356 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/inlet/winds.py
-drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 12:58:17.506307 pySailingVLM-1.0.0/pySailingVLM/results/
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/results/__init__.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     9425 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/results/inviscid_flow.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     7231 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/results/save_utils.py
-drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 12:58:17.506307 pySailingVLM-1.0.0/pySailingVLM/rotations/
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/rotations/__init__.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4109 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/rotations/csys_transformations.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     2932 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/rotations/geometry_calc.py
-drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 12:58:17.510307 pySailingVLM-1.0.0/pySailingVLM/runner/
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/runner/__init__.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     5394 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/runner/aircraft.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4395 2023-06-13 12:48:20.000000 pySailingVLM-1.0.0/pySailingVLM/runner/cli.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     5175 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/runner/container.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     8010 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/runner/sail.py
-drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 12:58:17.514308 pySailingVLM-1.0.0/pySailingVLM/solver/
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/solver/__init__.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     6447 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/solver/additional_functions.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     9607 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/solver/coefs.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4209 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/solver/forces.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     1474 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/solver/interpolator.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     2645 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/solver/mesher.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4649 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/solver/panels.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)    15325 2023-06-13 12:48:20.000000 pySailingVLM-1.0.0/pySailingVLM/solver/panels_plotter.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     7608 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/solver/velocity.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4317 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/solver/vlm.py
-drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 12:58:17.514308 pySailingVLM-1.0.0/pySailingVLM/thin_airfoil/
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4107 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/thin_airfoil/vlm_airfoil.py
-drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 12:58:17.518308 pySailingVLM-1.0.0/pySailingVLM/yacht_geometry/
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/yacht_geometry/__init__.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     2422 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/yacht_geometry/hull_geometry.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     3757 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/yacht_geometry/sail_factory.py
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)    10466 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pySailingVLM/yacht_geometry/sail_geometry.py
-drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 12:58:17.502307 pySailingVLM-1.0.0/pySailingVLM.egg-info/
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     2465 2023-06-13 12:58:17.000000 pySailingVLM-1.0.0/pySailingVLM.egg-info/PKG-INFO
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     1458 2023-06-13 12:58:17.000000 pySailingVLM-1.0.0/pySailingVLM.egg-info/SOURCES.txt
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)        1 2023-06-13 12:58:17.000000 pySailingVLM-1.0.0/pySailingVLM.egg-info/dependency_links.txt
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)       62 2023-06-13 12:58:17.000000 pySailingVLM-1.0.0/pySailingVLM.egg-info/entry_points.txt
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)      146 2023-06-13 12:58:17.000000 pySailingVLM-1.0.0/pySailingVLM.egg-info/requires.txt
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)       18 2023-06-13 12:58:17.000000 pySailingVLM-1.0.0/pySailingVLM.egg-info/top_level.txt
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)        1 2023-06-13 11:20:12.000000 pySailingVLM-1.0.0/pySailingVLM.egg-info/zip-safe
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)       80 2023-06-11 17:55:25.000000 pySailingVLM-1.0.0/pyproject.toml
--rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     1740 2023-06-13 12:58:17.518308 pySailingVLM-1.0.0/setup.cfg
+drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 22:53:14.792827 pySailingVLM-1.0.1/
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)    11357 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/LICENSE
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     2394 2023-06-13 22:53:14.792827 pySailingVLM-1.0.1/PKG-INFO
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     1323 2023-06-13 22:25:11.000000 pySailingVLM-1.0.1/README.md
+drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 22:53:14.776826 pySailingVLM-1.0.1/pySailingVLM/
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)      143 2023-06-13 12:48:20.000000 pySailingVLM-1.0.1/pySailingVLM/__main__.py
+drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 22:53:14.780826 pySailingVLM-1.0.1/pySailingVLM/examples/
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4506 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/examples/rectangle_variables.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4463 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/examples/sweep_variables.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4340 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/examples/variables.py
+drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 22:53:14.780826 pySailingVLM-1.0.1/pySailingVLM/inlet/
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/inlet/__init__.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     1935 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/inlet/inlet_conditions.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     7356 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/inlet/winds.py
+drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 22:53:14.780826 pySailingVLM-1.0.1/pySailingVLM/results/
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/results/__init__.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     9425 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/results/inviscid_flow.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     7231 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/results/save_utils.py
+drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 22:53:14.784826 pySailingVLM-1.0.1/pySailingVLM/rotations/
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/rotations/__init__.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4109 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/rotations/csys_transformations.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     2932 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/rotations/geometry_calc.py
+drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 22:53:14.784826 pySailingVLM-1.0.1/pySailingVLM/runner/
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/runner/__init__.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     5394 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/runner/aircraft.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4395 2023-06-13 12:48:20.000000 pySailingVLM-1.0.1/pySailingVLM/runner/cli.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     5175 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/runner/container.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     8010 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/runner/sail.py
+drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 22:53:14.788827 pySailingVLM-1.0.1/pySailingVLM/solver/
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/solver/__init__.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     6447 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/solver/additional_functions.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     9607 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/solver/coefs.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4209 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/solver/forces.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     1474 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/solver/interpolator.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     2645 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/solver/mesher.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4649 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/solver/panels.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)    15325 2023-06-13 12:48:20.000000 pySailingVLM-1.0.1/pySailingVLM/solver/panels_plotter.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     7608 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/solver/velocity.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4317 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/solver/vlm.py
+drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 22:53:14.788827 pySailingVLM-1.0.1/pySailingVLM/thin_airfoil/
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     4107 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/thin_airfoil/vlm_airfoil.py
+drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 22:53:14.792827 pySailingVLM-1.0.1/pySailingVLM/yacht_geometry/
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/yacht_geometry/__init__.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     2422 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/yacht_geometry/hull_geometry.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     3757 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/yacht_geometry/sail_factory.py
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)    10466 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pySailingVLM/yacht_geometry/sail_geometry.py
+drwxrwxr-x   0 zuzanna   (1000) zuzanna   (1000)        0 2023-06-13 22:53:14.780826 pySailingVLM-1.0.1/pySailingVLM.egg-info/
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     2394 2023-06-13 22:53:14.000000 pySailingVLM-1.0.1/pySailingVLM.egg-info/PKG-INFO
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     1458 2023-06-13 22:53:14.000000 pySailingVLM-1.0.1/pySailingVLM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)        1 2023-06-13 22:53:14.000000 pySailingVLM-1.0.1/pySailingVLM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)       62 2023-06-13 22:53:14.000000 pySailingVLM-1.0.1/pySailingVLM.egg-info/entry_points.txt
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)      146 2023-06-13 22:53:14.000000 pySailingVLM-1.0.1/pySailingVLM.egg-info/requires.txt
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)       18 2023-06-13 22:53:14.000000 pySailingVLM-1.0.1/pySailingVLM.egg-info/top_level.txt
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)        1 2023-06-13 11:20:12.000000 pySailingVLM-1.0.1/pySailingVLM.egg-info/zip-safe
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)       80 2023-06-11 17:55:25.000000 pySailingVLM-1.0.1/pyproject.toml
+-rw-rw-r--   0 zuzanna   (1000) zuzanna   (1000)     1753 2023-06-13 22:53:14.792827 pySailingVLM-1.0.1/setup.cfg
```

### Comparing `pySailingVLM-1.0.0/LICENSE` & `pySailingVLM-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/examples/rectangle_variables.py` & `pySailingVLM-1.0.1/pySailingVLM/examples/rectangle_variables.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/examples/sweep_variables.py` & `pySailingVLM-1.0.1/pySailingVLM/examples/sweep_variables.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/examples/variables.py` & `pySailingVLM-1.0.1/pySailingVLM/examples/variables.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/inlet/inlet_conditions.py` & `pySailingVLM-1.0.1/pySailingVLM/inlet/inlet_conditions.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/inlet/winds.py` & `pySailingVLM-1.0.1/pySailingVLM/inlet/winds.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/results/inviscid_flow.py` & `pySailingVLM-1.0.1/pySailingVLM/results/inviscid_flow.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/results/save_utils.py` & `pySailingVLM-1.0.1/pySailingVLM/results/save_utils.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/rotations/csys_transformations.py` & `pySailingVLM-1.0.1/pySailingVLM/rotations/csys_transformations.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/rotations/geometry_calc.py` & `pySailingVLM-1.0.1/pySailingVLM/rotations/geometry_calc.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/runner/aircraft.py` & `pySailingVLM-1.0.1/pySailingVLM/runner/aircraft.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/runner/cli.py` & `pySailingVLM-1.0.1/pySailingVLM/runner/cli.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/runner/container.py` & `pySailingVLM-1.0.1/pySailingVLM/runner/container.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/runner/sail.py` & `pySailingVLM-1.0.1/pySailingVLM/runner/sail.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/solver/additional_functions.py` & `pySailingVLM-1.0.1/pySailingVLM/solver/additional_functions.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/solver/coefs.py` & `pySailingVLM-1.0.1/pySailingVLM/solver/coefs.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/solver/forces.py` & `pySailingVLM-1.0.1/pySailingVLM/solver/forces.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/solver/interpolator.py` & `pySailingVLM-1.0.1/pySailingVLM/solver/interpolator.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/solver/mesher.py` & `pySailingVLM-1.0.1/pySailingVLM/solver/mesher.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/solver/panels.py` & `pySailingVLM-1.0.1/pySailingVLM/solver/panels.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/solver/panels_plotter.py` & `pySailingVLM-1.0.1/pySailingVLM/solver/panels_plotter.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/solver/velocity.py` & `pySailingVLM-1.0.1/pySailingVLM/solver/velocity.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/solver/vlm.py` & `pySailingVLM-1.0.1/pySailingVLM/solver/vlm.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/thin_airfoil/vlm_airfoil.py` & `pySailingVLM-1.0.1/pySailingVLM/thin_airfoil/vlm_airfoil.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/yacht_geometry/hull_geometry.py` & `pySailingVLM-1.0.1/pySailingVLM/yacht_geometry/hull_geometry.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/yacht_geometry/sail_factory.py` & `pySailingVLM-1.0.1/pySailingVLM/yacht_geometry/sail_factory.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM/yacht_geometry/sail_geometry.py` & `pySailingVLM-1.0.1/pySailingVLM/yacht_geometry/sail_geometry.py`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/pySailingVLM.egg-info/SOURCES.txt` & `pySailingVLM-1.0.1/pySailingVLM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pySailingVLM-1.0.0/setup.cfg` & `pySailingVLM-1.0.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 [metadata]
 name = pySailingVLM
-version = 1.0.0
+version = 1.0.1
 author = Grzegorz Gruszczynski, Zuzanna Wieczorek
 url = https://zuza3012.github.io/vlmbook/intro.html
-description = 'Vortex Lattice Method for yacht sailing'
+description = 'Vortex Lattice Method for initial aerodynamic analysis of upwind sails.'
 long_description = file: README.md
 long_description_content_type = text/markdown
-keywords = Vortex Lattice Method, VLM, sailingVLM, yacht, sailing
+keywords = Vortex Lattice Method, VLM, initial sail analysis, yacht engineering
 python_requires = >=3.10
 classifiers = 
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.10
 	Topic :: Software Development
-	Topic :: Scientific/Engineering
+	Topic :: Scientific/Engineering :: Information Analysis
 	Topic :: Scientific/Engineering :: Visualization
 	Topic :: Scientific/Engineering :: Physics
-	Topic :: Scientific/Engineering :: Information Analysis
 	Topic :: Education
 	Framework :: Jupyter
-	Intended Audience :: Science/Research
-	Intended Audience :: Education
 	Intended Audience :: End Users/Desktop
 	Intended Audience :: Developers
+	Intended Audience :: Education
+	Intended Audience :: Science/Research
 	Operating System :: POSIX :: Linux
 
 [options]
 packages = find_namespace:
 zip_safe = True
 include_package_data = True
 install_requires =
```

