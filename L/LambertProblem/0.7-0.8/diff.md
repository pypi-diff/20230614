# Comparing `tmp/LambertProblem-0.7.tar.gz` & `tmp/LambertProblem-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LambertProblem-0.7.tar", last modified: Wed Jun 14 02:22:01 2023, max compression
+gzip compressed data, was "LambertProblem-0.8.tar", last modified: Wed Jun 14 02:40:34 2023, max compression
```

## Comparing `LambertProblem-0.7.tar` & `LambertProblem-0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-14 02:22:01.268388 LambertProblem-0.7/
--rw-r--r--   0 juanita   (1000) juanita   (1000)     1134 2023-05-16 14:58:24.000000 LambertProblem-0.7/LICENSE
-drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-14 02:22:01.264388 LambertProblem-0.7/LambertProblem/
--rw-r--r--   0 juanita   (1000) juanita   (1000)     7345 2023-06-13 15:43:44.000000 LambertProblem-0.7/LambertProblem/__init__.py
-drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-14 02:22:01.264388 LambertProblem-0.7/LambertProblem.egg-info/
--rw-rw-r--   0 juanita   (1000) juanita   (1000)     2698 2023-06-14 02:22:01.000000 LambertProblem-0.7/LambertProblem.egg-info/PKG-INFO
--rw-rw-r--   0 juanita   (1000) juanita   (1000)      300 2023-06-14 02:22:01.000000 LambertProblem-0.7/LambertProblem.egg-info/SOURCES.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)        1 2023-06-14 02:22:01.000000 LambertProblem-0.7/LambertProblem.egg-info/dependency_links.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       51 2023-06-14 02:22:01.000000 LambertProblem-0.7/LambertProblem.egg-info/entry_points.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       12 2023-06-14 02:22:01.000000 LambertProblem-0.7/LambertProblem.egg-info/requires.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       15 2023-06-14 02:22:01.000000 LambertProblem-0.7/LambertProblem.egg-info/top_level.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)     2698 2023-06-14 02:22:01.264388 LambertProblem-0.7/PKG-INFO
--rw-r--r--   0 juanita   (1000) juanita   (1000)     2182 2023-06-14 02:19:40.000000 LambertProblem-0.7/README.md
--rw-r--r--   0 juanita   (1000) juanita   (1000)      110 2023-06-13 16:01:48.000000 LambertProblem-0.7/pyproject.toml
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       38 2023-06-14 02:22:01.268388 LambertProblem-0.7/setup.cfg
--rw-r--r--   0 juanita   (1000) juanita   (1000)     2233 2023-06-14 02:20:14.000000 LambertProblem-0.7/setup.py
+drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-14 02:40:34.580947 LambertProblem-0.8/
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     1134 2023-05-16 14:58:24.000000 LambertProblem-0.8/LICENSE
+drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-14 02:40:34.580947 LambertProblem-0.8/LambertProblem/
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     7345 2023-06-13 15:43:44.000000 LambertProblem-0.8/LambertProblem/__init__.py
+drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-14 02:40:34.580947 LambertProblem-0.8/LambertProblem.egg-info/
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)     2757 2023-06-14 02:40:34.000000 LambertProblem-0.8/LambertProblem.egg-info/PKG-INFO
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)      300 2023-06-14 02:40:34.000000 LambertProblem-0.8/LambertProblem.egg-info/SOURCES.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)        1 2023-06-14 02:40:34.000000 LambertProblem-0.8/LambertProblem.egg-info/dependency_links.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       51 2023-06-14 02:40:34.000000 LambertProblem-0.8/LambertProblem.egg-info/entry_points.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       12 2023-06-14 02:40:34.000000 LambertProblem-0.8/LambertProblem.egg-info/requires.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       15 2023-06-14 02:40:34.000000 LambertProblem-0.8/LambertProblem.egg-info/top_level.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)     2757 2023-06-14 02:40:34.580947 LambertProblem-0.8/PKG-INFO
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     2241 2023-06-14 02:37:49.000000 LambertProblem-0.8/README.md
+-rw-r--r--   0 juanita   (1000) juanita   (1000)      110 2023-06-13 16:01:48.000000 LambertProblem-0.8/pyproject.toml
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       38 2023-06-14 02:40:34.580947 LambertProblem-0.8/setup.cfg
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     2233 2023-06-14 02:40:27.000000 LambertProblem-0.8/setup.py
```

### Comparing `LambertProblem-0.7/LICENSE` & `LambertProblem-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `LambertProblem-0.7/LambertProblem/__init__.py` & `LambertProblem-0.8/LambertProblem/__init__.py`

 * *Files identical despite different names*

### Comparing `LambertProblem-0.7/LambertProblem.egg-info/PKG-INFO` & `LambertProblem-0.8/LambertProblem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LambertProblem
-Version: 0.7
+Version: 0.8
 Summary: Solve the lambert problem for orbital mechanics
 Home-page: https://pypi.org/project/LambertProblem
 Author: juaniuwu
 Author-email: juanita.agudelo@udea.edu.co
 License: MIT
 Keywords: Lambert equation orbital mechanics solve
 Platform: UNKNOWN
@@ -24,15 +24,15 @@
 This package contain some methods for solve the Lambert Problem in orbital mechanics, and also have a class name Ellipse wich calculate the points of an ellipse.
 
 The method LambertProblem solve the Lambert Equation for a value of semi mayor axis or for a value of transfer time. The method requires the distance for the focus to the two points (r1, r2) and the angle between both radio positions. 
 
 The class Ellipse create a ellipse with center in the center of coordinates and parallel to the x axis. The class is initialized with the value of semi mayor axis from the ellipse and the eccentricity or with the semi minor axis. 
 
 
-<p align="center"><img src="https://youtu.be/6cUe4oMk69E" alt="Space orbits gif""/></p>
+<p align="center"><img src="https://solarsystem.nasa.gov/bosf/images/05-Geostationary%20Satellite-STILL-715x415.jpg" alt="Space orbits gif""/></p>
 
 ## Download and install
 
 If you are using `PyPI` installation it's as simple as:
 
 ```
 pip install LambertProblem
```

### Comparing `LambertProblem-0.7/PKG-INFO` & `LambertProblem-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LambertProblem
-Version: 0.7
+Version: 0.8
 Summary: Solve the lambert problem for orbital mechanics
 Home-page: https://pypi.org/project/LambertProblem
 Author: juaniuwu
 Author-email: juanita.agudelo@udea.edu.co
 License: MIT
 Keywords: Lambert equation orbital mechanics solve
 Platform: UNKNOWN
@@ -24,15 +24,15 @@
 This package contain some methods for solve the Lambert Problem in orbital mechanics, and also have a class name Ellipse wich calculate the points of an ellipse.
 
 The method LambertProblem solve the Lambert Equation for a value of semi mayor axis or for a value of transfer time. The method requires the distance for the focus to the two points (r1, r2) and the angle between both radio positions. 
 
 The class Ellipse create a ellipse with center in the center of coordinates and parallel to the x axis. The class is initialized with the value of semi mayor axis from the ellipse and the eccentricity or with the semi minor axis. 
 
 
-<p align="center"><img src="https://youtu.be/6cUe4oMk69E" alt="Space orbits gif""/></p>
+<p align="center"><img src="https://solarsystem.nasa.gov/bosf/images/05-Geostationary%20Satellite-STILL-715x415.jpg" alt="Space orbits gif""/></p>
 
 ## Download and install
 
 If you are using `PyPI` installation it's as simple as:
 
 ```
 pip install LambertProblem
```

### Comparing `LambertProblem-0.7/README.md` & `LambertProblem-0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 This package contain some methods for solve the Lambert Problem in orbital mechanics, and also have a class name Ellipse wich calculate the points of an ellipse.
 
 The method LambertProblem solve the Lambert Equation for a value of semi mayor axis or for a value of transfer time. The method requires the distance for the focus to the two points (r1, r2) and the angle between both radio positions. 
 
 The class Ellipse create a ellipse with center in the center of coordinates and parallel to the x axis. The class is initialized with the value of semi mayor axis from the ellipse and the eccentricity or with the semi minor axis. 
 
 
-<p align="center"><img src="https://youtu.be/6cUe4oMk69E" alt="Space orbits gif""/></p>
+<p align="center"><img src="https://solarsystem.nasa.gov/bosf/images/05-Geostationary%20Satellite-STILL-715x415.jpg" alt="Space orbits gif""/></p>
 
 ## Download and install
 
 If you are using `PyPI` installation it's as simple as:
 
 ```
 pip install LambertProblem
```

### Comparing `LambertProblem-0.7/setup.py` & `LambertProblem-0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         ],
-    version='0.7',
+    version='0.8',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
```

