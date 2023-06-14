# Comparing `tmp/G4EPP-0.0.3.tar.gz` & `tmp/G4EPP-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/G4EPP-0.0.3.tar", last modified: Wed Jun 14 15:34:50 2023, max compression
+gzip compressed data, was "dist/G4EPP-0.0.4.tar", last modified: Wed Jun 14 15:36:40 2023, max compression
```

## Comparing `G4EPP-0.0.3.tar` & `G4EPP-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 15:34:50.000000 G4EPP-0.0.3/
-drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 15:34:50.000000 G4EPP-0.0.3/G4EPP/
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)     8250 2023-06-13 18:56:47.000000 G4EPP-0.0.3/G4EPP/G4EPP.py
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        0 2023-04-10 18:48:29.000000 G4EPP-0.0.3/G4EPP/__init__.py
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)     7587 2023-06-13 18:25:31.000000 G4EPP-0.0.3/G4EPP/utils.py
-drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 15:34:50.000000 G4EPP-0.0.3/G4EPP.egg-info/
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      449 2023-06-14 15:34:50.000000 G4EPP-0.0.3/G4EPP.egg-info/PKG-INFO
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      220 2023-06-14 15:34:50.000000 G4EPP-0.0.3/G4EPP.egg-info/SOURCES.txt
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        1 2023-06-14 15:34:50.000000 G4EPP-0.0.3/G4EPP.egg-info/dependency_links.txt
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       58 2023-06-14 15:34:50.000000 G4EPP-0.0.3/G4EPP.egg-info/requires.txt
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        6 2023-06-14 15:34:50.000000 G4EPP-0.0.3/G4EPP.egg-info/top_level.txt
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      449 2023-06-14 15:34:50.000000 G4EPP-0.0.3/PKG-INFO
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      176 2023-04-10 18:48:29.000000 G4EPP-0.0.3/README.md
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       79 2023-06-14 15:34:50.000000 G4EPP-0.0.3/setup.cfg
--rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      781 2023-06-14 15:34:46.000000 G4EPP-0.0.3/setup.py
+drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 15:36:40.000000 G4EPP-0.0.4/
+drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 15:36:40.000000 G4EPP-0.0.4/G4EPP/
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)     8250 2023-06-13 18:56:47.000000 G4EPP-0.0.4/G4EPP/G4EPP.py
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        0 2023-04-10 18:48:29.000000 G4EPP-0.0.4/G4EPP/__init__.py
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)     7587 2023-06-13 18:25:31.000000 G4EPP-0.0.4/G4EPP/utils.py
+drwxrwxr-x   0 gdberla   (1001) gdberla   (1001)        0 2023-06-14 15:36:40.000000 G4EPP-0.0.4/G4EPP.egg-info/
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      449 2023-06-14 15:36:40.000000 G4EPP-0.0.4/G4EPP.egg-info/PKG-INFO
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      220 2023-06-14 15:36:40.000000 G4EPP-0.0.4/G4EPP.egg-info/SOURCES.txt
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        1 2023-06-14 15:36:40.000000 G4EPP-0.0.4/G4EPP.egg-info/dependency_links.txt
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       51 2023-06-14 15:36:40.000000 G4EPP-0.0.4/G4EPP.egg-info/requires.txt
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)        6 2023-06-14 15:36:40.000000 G4EPP-0.0.4/G4EPP.egg-info/top_level.txt
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      449 2023-06-14 15:36:40.000000 G4EPP-0.0.4/PKG-INFO
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      176 2023-04-10 18:48:29.000000 G4EPP-0.0.4/README.md
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)       79 2023-06-14 15:36:40.000000 G4EPP-0.0.4/setup.cfg
+-rw-rw-r--   0 gdberla   (1001) gdberla   (1001)      772 2023-06-14 15:36:12.000000 G4EPP-0.0.4/setup.py
```

### Comparing `G4EPP-0.0.3/G4EPP/G4EPP.py` & `G4EPP-0.0.4/G4EPP/G4EPP.py`

 * *Files identical despite different names*

### Comparing `G4EPP-0.0.3/G4EPP/utils.py` & `G4EPP-0.0.4/G4EPP/utils.py`

 * *Files identical despite different names*

### Comparing `G4EPP-0.0.3/setup.py` & `G4EPP-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'GEANT4 EPP Simulation wrapper'
 LONG_DESCRIPTION = 'Python wrapper to process and plot GEANT4 EPP simulation outputs'
 
 setup(
         name="G4EPP", 
         version=VERSION,
         author="Grant Berland",
         author_email="grant.berland@colorado.edu",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=["matplotlib", "pandas", "numpy", "scipy", "seaborn", "wget","seaborn","pickle"],  
+        install_requires=["matplotlib", "pandas", "numpy", "scipy", "seaborn", "wget","seaborn"],  
         keywords=['python', 'EPP'],
         classifiers=[
             'Development Status :: 3 - Alpha',
             'License :: OSI Approved :: MIT License',
             'Programming Language :: Python :: 3.6'
             ]
 )
```

