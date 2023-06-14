# Comparing `tmp/mosaik-pypower-0.8.2.tar.gz` & `tmp/mosaik-pypower-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaik-pypower-0.8.2.tar", last modified: Tue Sep 27 11:46:56 2022, max compression
+gzip compressed data, was "mosaik-pypower-0.8.3.tar", last modified: Wed Jun 14 09:05:05 2023, max compression
```

## Comparing `mosaik-pypower-0.8.2.tar` & `mosaik-pypower-0.8.3.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 11:46:56.209580 mosaik-pypower-0.8.2/
--rw-rw-rw-   0 root         (0) root         (0)      114 2022-09-27 11:46:31.000000 mosaik-pypower-0.8.2/AUTHORS.txt
--rw-rw-rw-   0 root         (0) root         (0)     2020 2022-09-27 11:46:31.000000 mosaik-pypower-0.8.2/CHANGES.txt
--rw-rw-rw-   0 root         (0) root         (0)    24436 2022-09-27 11:46:31.000000 mosaik-pypower-0.8.2/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       39 2022-09-27 11:46:31.000000 mosaik-pypower-0.8.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    19648 2022-09-27 11:46:56.208580 mosaik-pypower-0.8.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    16554 2022-09-27 11:46:31.000000 mosaik-pypower-0.8.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 11:46:56.206580 mosaik-pypower-0.8.2/mosaik_pypower/
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-09-27 11:46:31.000000 mosaik-pypower-0.8.2/mosaik_pypower/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14460 2022-09-27 11:46:31.000000 mosaik-pypower-0.8.2/mosaik_pypower/model.py
--rw-rw-rw-   0 root         (0) root         (0)     7372 2022-09-27 11:46:31.000000 mosaik-pypower-0.8.2/mosaik_pypower/mosaik.py
--rw-rw-rw-   0 root         (0) root         (0)     1944 2022-09-27 11:46:31.000000 mosaik-pypower-0.8.2/mosaik_pypower/resource_db.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 11:46:56.208580 mosaik-pypower-0.8.2/mosaik_pypower.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19648 2022-09-27 11:46:56.000000 mosaik-pypower-0.8.2/mosaik_pypower.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2022-09-27 11:46:56.000000 mosaik-pypower-0.8.2/mosaik_pypower.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-27 11:46:56.000000 mosaik-pypower-0.8.2/mosaik_pypower.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2022-09-27 11:46:56.000000 mosaik-pypower-0.8.2/mosaik_pypower.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       72 2022-09-27 11:46:56.000000 mosaik-pypower-0.8.2/mosaik_pypower.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-09-27 11:46:56.000000 mosaik-pypower-0.8.2/mosaik_pypower.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      331 2022-09-27 11:46:31.000000 mosaik-pypower-0.8.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-27 11:46:56.209580 mosaik-pypower-0.8.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1458 2022-09-27 11:46:31.000000 mosaik-pypower-0.8.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:05:05.097506 mosaik-pypower-0.8.3/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-14 09:04:44.000000 mosaik-pypower-0.8.3/AUTHORS.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2020 2023-06-14 09:04:44.000000 mosaik-pypower-0.8.3/CHANGES.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-06-14 09:04:44.000000 mosaik-pypower-0.8.3/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-14 09:04:44.000000 mosaik-pypower-0.8.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    19648 2023-06-14 09:05:05.097506 mosaik-pypower-0.8.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    16554 2023-06-14 09:04:44.000000 mosaik-pypower-0.8.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:05:05.095506 mosaik-pypower-0.8.3/mosaik_pypower/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-14 09:04:44.000000 mosaik-pypower-0.8.3/mosaik_pypower/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14460 2023-06-14 09:04:44.000000 mosaik-pypower-0.8.3/mosaik_pypower/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     7372 2023-06-14 09:04:44.000000 mosaik-pypower-0.8.3/mosaik_pypower/mosaik.py
+-rw-rw-rw-   0 root         (0) root         (0)     1944 2023-06-14 09:04:44.000000 mosaik-pypower-0.8.3/mosaik_pypower/resource_db.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:05:05.096506 mosaik-pypower-0.8.3/mosaik_pypower.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19648 2023-06-14 09:05:05.000000 mosaik-pypower-0.8.3/mosaik_pypower.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-14 09:05:05.000000 mosaik-pypower-0.8.3/mosaik_pypower.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 09:05:05.000000 mosaik-pypower-0.8.3/mosaik_pypower.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-14 09:05:05.000000 mosaik-pypower-0.8.3/mosaik_pypower.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-14 09:05:05.000000 mosaik-pypower-0.8.3/mosaik_pypower.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-14 09:05:05.000000 mosaik-pypower-0.8.3/mosaik_pypower.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-14 09:04:44.000000 mosaik-pypower-0.8.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 09:05:05.097506 mosaik-pypower-0.8.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-06-14 09:04:44.000000 mosaik-pypower-0.8.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:05:05.097506 mosaik-pypower-0.8.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 09:04:44.000000 mosaik-pypower-0.8.3/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11007 2023-06-14 09:04:44.000000 mosaik-pypower-0.8.3/tests/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     5796 2023-06-14 09:04:44.000000 mosaik-pypower-0.8.3/tests/test_mosaik.py
```

### Comparing `mosaik-pypower-0.8.2/CHANGES.txt` & `mosaik-pypower-0.8.3/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `mosaik-pypower-0.8.2/PKG-INFO` & `mosaik-pypower-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaik-pypower
-Version: 0.8.2
+Version: 0.8.3
 Summary: An adapter to use PYPOWER with mosaik.
 Home-page: https://gitlab.com/mosaik/components/energy/mosaik-pypower
 Author: Stefan Scherfke
 Author-email: mosaik@offis.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mosaik-pypower-0.8.2/README.rst` & `mosaik-pypower-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `mosaik-pypower-0.8.2/mosaik_pypower/model.py` & `mosaik-pypower-0.8.3/mosaik_pypower/model.py`

 * *Files identical despite different names*

### Comparing `mosaik-pypower-0.8.2/mosaik_pypower/mosaik.py` & `mosaik-pypower-0.8.3/mosaik_pypower/mosaik.py`

 * *Files identical despite different names*

### Comparing `mosaik-pypower-0.8.2/mosaik_pypower/resource_db.py` & `mosaik-pypower-0.8.3/mosaik_pypower/resource_db.py`

 * *Files identical despite different names*

### Comparing `mosaik-pypower-0.8.2/mosaik_pypower.egg-info/PKG-INFO` & `mosaik-pypower-0.8.3/mosaik_pypower.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaik-pypower
-Version: 0.8.2
+Version: 0.8.3
 Summary: An adapter to use PYPOWER with mosaik.
 Home-page: https://gitlab.com/mosaik/components/energy/mosaik-pypower
 Author: Stefan Scherfke
 Author-email: mosaik@offis.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mosaik-pypower-0.8.2/setup.py` & `mosaik-pypower-0.8.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='mosaik-pypower',
-    version='0.8.2',
+    version='0.8.3',
     author='Stefan Scherfke',
     author_email='mosaik@offis.de',
     description='An adapter to use PYPOWER with mosaik.',
     long_description=(open('README.rst').read() + '\n\n' +
                       open('CHANGES.txt').read() + '\n\n' +
                       open('AUTHORS.txt').read()),
     url='https://gitlab.com/mosaik/components/energy/mosaik-pypower',
     install_requires=[
-        'PYPOWER>=4.1',
+        'PYPOWER>=5.1.16',
         'mosaik-api>=3.0',
-        'numpy>=1.6,<1.23',
+        'numpy>=1.6',
         'scipy>=0.9',
         'xlrd>=0.9.2,<2',
     ],
     packages=find_packages(),
     include_package_data=True,
     entry_points={
         'console_scripts': [
```

