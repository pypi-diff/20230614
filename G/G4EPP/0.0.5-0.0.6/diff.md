# Comparing `tmp/G4EPP-0.0.5.tar.gz` & `tmp/G4EPP-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/G4EPP-0.0.5.tar", last modified: Wed Jun 14 15:54:51 2023, max compression
+gzip compressed data, was "dist/G4EPP-0.0.6.tar", last modified: Wed Jun 14 16:18:19 2023, max compression
```

## Comparing `G4EPP-0.0.5.tar` & `G4EPP-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 15:54:51.000000 G4EPP-0.0.5/
-drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 15:54:51.000000 G4EPP-0.0.5/G4EPP/
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)    15533 2023-06-14 15:51:09.000000 G4EPP-0.0.5/G4EPP/G4EPP.py
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        0 2023-04-10 18:48:29.000000 G4EPP-0.0.5/G4EPP/__init__.py
-drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 15:54:51.000000 G4EPP-0.0.5/G4EPP.egg-info/
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      449 2023-06-14 15:54:51.000000 G4EPP-0.0.5/G4EPP.egg-info/PKG-INFO
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      205 2023-06-14 15:54:51.000000 G4EPP-0.0.5/G4EPP.egg-info/SOURCES.txt
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        1 2023-06-14 15:54:51.000000 G4EPP-0.0.5/G4EPP.egg-info/dependency_links.txt
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       51 2023-06-14 15:54:51.000000 G4EPP-0.0.5/G4EPP.egg-info/requires.txt
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        6 2023-06-14 15:54:51.000000 G4EPP-0.0.5/G4EPP.egg-info/top_level.txt
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      449 2023-06-14 15:54:51.000000 G4EPP-0.0.5/PKG-INFO
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      176 2023-04-10 18:48:29.000000 G4EPP-0.0.5/README.md
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       79 2023-06-14 15:54:51.000000 G4EPP-0.0.5/setup.cfg
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      772 2023-06-14 15:53:14.000000 G4EPP-0.0.5/setup.py
+drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 16:18:19.000000 G4EPP-0.0.6/
+drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 16:18:19.000000 G4EPP-0.0.6/G4EPP/
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)    15533 2023-06-14 15:51:09.000000 G4EPP-0.0.6/G4EPP/G4EPP.py
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       20 2023-06-14 16:15:33.000000 G4EPP-0.0.6/G4EPP/__init__.py
+drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 16:18:19.000000 G4EPP-0.0.6/G4EPP.egg-info/
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      449 2023-06-14 16:18:19.000000 G4EPP-0.0.6/G4EPP.egg-info/PKG-INFO
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      205 2023-06-14 16:18:19.000000 G4EPP-0.0.6/G4EPP.egg-info/SOURCES.txt
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        1 2023-06-14 16:18:19.000000 G4EPP-0.0.6/G4EPP.egg-info/dependency_links.txt
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       51 2023-06-14 16:18:19.000000 G4EPP-0.0.6/G4EPP.egg-info/requires.txt
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        6 2023-06-14 16:18:19.000000 G4EPP-0.0.6/G4EPP.egg-info/top_level.txt
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      449 2023-06-14 16:18:19.000000 G4EPP-0.0.6/PKG-INFO
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      176 2023-04-10 18:48:29.000000 G4EPP-0.0.6/README.md
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       79 2023-06-14 16:18:19.000000 G4EPP-0.0.6/setup.cfg
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      772 2023-06-14 16:18:16.000000 G4EPP-0.0.6/setup.py
```

### Comparing `G4EPP-0.0.5/G4EPP/G4EPP.py` & `G4EPP-0.0.6/G4EPP/G4EPP.py`

 * *Files identical despite different names*

### Comparing `G4EPP-0.0.5/setup.py` & `G4EPP-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5' 
+VERSION = '0.0.6' 
 DESCRIPTION = 'GEANT4 EPP Simulation wrapper'
 LONG_DESCRIPTION = 'Python wrapper to process and plot GEANT4 EPP simulation outputs'
 
 setup(
         name="G4EPP", 
         version=VERSION,
         author="Grant Berland",
```

