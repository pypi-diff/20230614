# Comparing `tmp/dartastlatools-0.0.3.tar.gz` & `tmp/dartastlatools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dartastlatools-0.0.3.tar", last modified: Wed Jun 14 14:56:03 2023, max compression
+gzip compressed data, was "dartastlatools-0.0.4.tar", last modified: Wed Jun 14 14:57:58 2023, max compression
```

## Comparing `dartastlatools-0.0.3.tar` & `dartastlatools-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 wharmsen (22850) wharmsen (22850)        0 2023-06-14 14:56:03.677866 dartastlatools-0.0.3/
--rw-rw-r--   0 wharmsen (22850) wharmsen (22850)      284 2023-06-14 14:56:03.677866 dartastlatools-0.0.3/PKG-INFO
-drwxrwsr-x   0 wharmsen (22850) wharmsen (22850)        0 2023-06-14 14:56:03.665866 dartastlatools-0.0.3/dartastlatools.egg-info/
--rw-rw-r--   0 wharmsen (22850) wharmsen (22850)      284 2023-06-14 14:56:03.000000 dartastlatools-0.0.3/dartastlatools.egg-info/PKG-INFO
--rw-rw-r--   0 wharmsen (22850) wharmsen (22850)      230 2023-06-14 14:56:03.000000 dartastlatools-0.0.3/dartastlatools.egg-info/SOURCES.txt
--rw-rw-r--   0 wharmsen (22850) wharmsen (22850)        1 2023-06-14 14:56:03.000000 dartastlatools-0.0.3/dartastlatools.egg-info/dependency_links.txt
--rw-rw-r--   0 wharmsen (22850) wharmsen (22850)       53 2023-06-14 14:56:03.000000 dartastlatools-0.0.3/dartastlatools.egg-info/requires.txt
--rw-rw-r--   0 wharmsen (22850) wharmsen (22850)        7 2023-06-14 14:56:03.000000 dartastlatools-0.0.3/dartastlatools.egg-info/top_level.txt
-drwxrwsr-x   0 wharmsen (22850) wharmsen (22850)        0 2023-06-14 14:56:03.673866 dartastlatools-0.0.3/extras/
--rw-rw-r--   0 wharmsen (22850) wharmsen (22850)       19 2023-06-14 14:44:01.000000 dartastlatools-0.0.3/extras/__init__.py
--rw-rw-r--   0 wharmsen (22850) wharmsen (22850)       28 2023-06-14 14:43:13.000000 dartastlatools-0.0.3/extras/add.py
--rw-rw-r--   0 wharmsen (22850) wharmsen (22850)       38 2023-06-14 14:56:03.677866 dartastlatools-0.0.3/setup.cfg
--rw-rw-r--   0 wharmsen (22850) wharmsen (22850)      807 2023-06-14 14:55:58.000000 dartastlatools-0.0.3/setup.py
+drwxrwsr-x   0 wharmsen (22850) wharmsen (22850)        0 2023-06-14 14:57:58.182687 dartastlatools-0.0.4/
+-rw-rw-r--   0 wharmsen (22850) wharmsen (22850)      284 2023-06-14 14:57:58.182687 dartastlatools-0.0.4/PKG-INFO
+drwxrwsr-x   0 wharmsen (22850) wharmsen (22850)        0 2023-06-14 14:57:58.158687 dartastlatools-0.0.4/dartastlatools.egg-info/
+-rw-rw-r--   0 wharmsen (22850) wharmsen (22850)      284 2023-06-14 14:57:58.000000 dartastlatools-0.0.4/dartastlatools.egg-info/PKG-INFO
+-rw-rw-r--   0 wharmsen (22850) wharmsen (22850)      230 2023-06-14 14:57:58.000000 dartastlatools-0.0.4/dartastlatools.egg-info/SOURCES.txt
+-rw-rw-r--   0 wharmsen (22850) wharmsen (22850)        1 2023-06-14 14:57:58.000000 dartastlatools-0.0.4/dartastlatools.egg-info/dependency_links.txt
+-rw-rw-r--   0 wharmsen (22850) wharmsen (22850)       50 2023-06-14 14:57:58.000000 dartastlatools-0.0.4/dartastlatools.egg-info/requires.txt
+-rw-rw-r--   0 wharmsen (22850) wharmsen (22850)        7 2023-06-14 14:57:58.000000 dartastlatools-0.0.4/dartastlatools.egg-info/top_level.txt
+drwxrwsr-x   0 wharmsen (22850) wharmsen (22850)        0 2023-06-14 14:57:58.178687 dartastlatools-0.0.4/extras/
+-rw-rw-r--   0 wharmsen (22850) wharmsen (22850)       19 2023-06-14 14:44:01.000000 dartastlatools-0.0.4/extras/__init__.py
+-rw-rw-r--   0 wharmsen (22850) wharmsen (22850)       28 2023-06-14 14:43:13.000000 dartastlatools-0.0.4/extras/add.py
+-rw-rw-r--   0 wharmsen (22850) wharmsen (22850)       38 2023-06-14 14:57:58.182687 dartastlatools-0.0.4/setup.cfg
+-rw-rw-r--   0 wharmsen (22850) wharmsen (22850)      801 2023-06-14 14:57:45.000000 dartastlatools-0.0.4/setup.py
```

### Comparing `dartastlatools-0.0.3/setup.py` & `dartastlatools-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'Tools for DART and ASTLA project'
 LONG_DESCRIPTION = 'Several scripts about preprocessing and postprocessing (child) speech ASR input and output.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="dartastlatools", 
         version=VERSION,
         author="Wieke Harmsen",
         author_email="<wiekeharmsen@gmail.com>",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['pandas', 'numpy', 'glob2==0.7', 'os', 're', 'praat-textgrids==1.0.2'], # add any additional packages that 
+        install_requires=['pandas', 'numpy', 'glob2==0.7', 're', 'praat-textgrids==1.0.2'], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'
         keywords=['python', 'child speech'],
 )
```

