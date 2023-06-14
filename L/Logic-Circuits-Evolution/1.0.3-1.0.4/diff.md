# Comparing `tmp/Logic Circuits Evolution-1.0.3.tar.gz` & `tmp/Logic Circuits Evolution-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Logic Circuits Evolution-1.0.3.tar", last modified: Tue Jun 13 23:51:57 2023, max compression
+gzip compressed data, was "Logic Circuits Evolution-1.0.4.tar", last modified: Wed Jun 14 00:09:07 2023, max compression
```

## Comparing `Logic Circuits Evolution-1.0.3.tar` & `Logic Circuits Evolution-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 23:51:57.692144 Logic Circuits Evolution-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-13 23:51:57.664769 Logic Circuits Evolution-1.0.3/Logic_Circuits_Evolution/
--rw-rw-rw-   0        0        0    19719 2023-06-13 23:51:34.000000 Logic Circuits Evolution-1.0.3/Logic_Circuits_Evolution/Logic_Circuits_Evolution.py
--rw-rw-rw-   0        0        0        0 2023-06-13 23:22:24.000000 Logic Circuits Evolution-1.0.3/Logic_Circuits_Evolution/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 23:51:57.686997 Logic Circuits Evolution-1.0.3/Logic_Circuits_Evolution.egg-info/
--rw-rw-rw-   0        0        0      278 2023-06-13 23:51:56.000000 Logic Circuits Evolution-1.0.3/Logic_Circuits_Evolution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-06-13 23:51:57.000000 Logic Circuits Evolution-1.0.3/Logic_Circuits_Evolution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 23:51:57.000000 Logic Circuits Evolution-1.0.3/Logic_Circuits_Evolution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 23:51:57.000000 Logic Circuits Evolution-1.0.3/Logic_Circuits_Evolution.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      278 2023-06-13 23:51:57.690150 Logic Circuits Evolution-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-13 23:51:57.692144 Logic Circuits Evolution-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      329 2023-06-13 23:51:50.000000 Logic Circuits Evolution-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:09:07.914556 Logic Circuits Evolution-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-14 00:09:07.873089 Logic Circuits Evolution-1.0.4/Logic_Circuits_Evolution/
+-rw-rw-rw-   0        0        0    19639 2023-06-14 00:08:10.000000 Logic Circuits Evolution-1.0.4/Logic_Circuits_Evolution/Logic_Circuits_Evolution.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 23:22:24.000000 Logic Circuits Evolution-1.0.4/Logic_Circuits_Evolution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:09:07.909188 Logic Circuits Evolution-1.0.4/Logic_Circuits_Evolution.egg-info/
+-rw-rw-rw-   0        0        0      278 2023-06-14 00:09:07.000000 Logic Circuits Evolution-1.0.4/Logic_Circuits_Evolution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-06-14 00:09:07.000000 Logic Circuits Evolution-1.0.4/Logic_Circuits_Evolution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 00:09:07.000000 Logic Circuits Evolution-1.0.4/Logic_Circuits_Evolution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-14 00:09:07.000000 Logic Circuits Evolution-1.0.4/Logic_Circuits_Evolution.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-14 00:09:07.000000 Logic Circuits Evolution-1.0.4/Logic_Circuits_Evolution.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      278 2023-06-14 00:09:07.912554 Logic Circuits Evolution-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-14 00:09:07.915550 Logic Circuits Evolution-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      419 2023-06-14 00:08:42.000000 Logic Circuits Evolution-1.0.4/setup.py
```

### Comparing `Logic Circuits Evolution-1.0.3/Logic_Circuits_Evolution/Logic_Circuits_Evolution.py` & `Logic Circuits Evolution-1.0.4/Logic_Circuits_Evolution/Logic_Circuits_Evolution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from multiprocessing.sharedctypes import copy
-from quopri import decodestring
 from random import *
 import random
 import datetime
 import bisect
 
 class Genoma:
     def __init__(self, numberOfGenes = 60, nInputs = 4,nOutputs = 1, rateMutation = 0.15):
```

