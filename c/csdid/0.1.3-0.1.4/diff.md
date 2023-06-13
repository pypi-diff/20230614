# Comparing `tmp/csdid-0.1.3.tar.gz` & `tmp/csdid-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.3.tar", last modified: Tue Jun 13 21:53:53 2023, max compression
+gzip compressed data, was "csdid-0.1.4.tar", last modified: Tue Jun 13 22:04:17 2023, max compression
```

## Comparing `csdid-0.1.3.tar` & `csdid-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 21:53:53.680320 csdid-0.1.3/
--rw-rw-rw-   0        0        0     1126 2023-06-13 21:34:25.000000 csdid-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      533 2023-06-13 21:53:53.680320 csdid-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 21:53:53.672319 csdid-0.1.3/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-13 15:53:11.000000 csdid-0.1.3/csdid/__init__.py
--rw-rw-rw-   0        0        0     3842 2023-06-13 21:46:48.000000 csdid-0.1.3/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-13 21:53:53.679320 csdid-0.1.3/csdid.egg-info/
--rw-rw-rw-   0        0        0      533 2023-06-13 21:53:53.000000 csdid-0.1.3/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      166 2023-06-13 21:53:53.000000 csdid-0.1.3/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 21:53:53.000000 csdid-0.1.3/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 21:53:53.000000 csdid-0.1.3/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 21:53:53.680320 csdid-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      607 2023-06-13 21:53:43.000000 csdid-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:04:17.740874 csdid-0.1.4/
+-rw-rw-rw-   0        0        0     1126 2023-06-13 21:34:25.000000 csdid-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      533 2023-06-13 22:04:17.739874 csdid-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 22:04:17.725872 csdid-0.1.4/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-13 15:53:11.000000 csdid-0.1.4/csdid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:04:17.735873 csdid-0.1.4/csdid/aggte_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-13 15:50:26.000000 csdid-0.1.4/csdid/aggte_fnc/__init__.py
+-rw-rw-rw-   0        0        0     4700 2023-06-13 21:47:11.000000 csdid-0.1.4/csdid/aggte_fnc/aggte.py
+-rw-rw-rw-   0        0        0    22816 2023-06-13 21:47:35.000000 csdid-0.1.4/csdid/aggte_fnc/compute_aggte.py
+-rw-rw-rw-   0        0        0     7182 2023-06-13 21:50:11.000000 csdid-0.1.4/csdid/aggte_fnc/utils.py
+-rw-rw-rw-   0        0        0     3842 2023-06-13 21:46:48.000000 csdid-0.1.4/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:04:17.737874 csdid-0.1.4/csdid/attgt_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-13 15:48:55.000000 csdid-0.1.4/csdid/attgt_fnc/__init__.py
+-rw-rw-rw-   0        0        0     5837 2023-06-13 21:47:23.000000 csdid-0.1.4/csdid/attgt_fnc/compute_att_gt.py
+-rw-rw-rw-   0        0        0     5389 2023-06-13 21:47:19.000000 csdid-0.1.4/csdid/attgt_fnc/preprocess_did.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:04:17.739874 csdid-0.1.4/csdid/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-13 15:48:44.000000 csdid-0.1.4/csdid/utils/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-06-13 19:21:02.000000 csdid-0.1.4/csdid/utils/bmisc.py
+-rw-rw-rw-   0        0        0     4274 2023-06-13 19:20:07.000000 csdid-0.1.4/csdid/utils/mboot.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:04:17.732872 csdid-0.1.4/csdid.egg-info/
+-rw-rw-rw-   0        0        0      533 2023-06-13 22:04:17.000000 csdid-0.1.4/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-06-13 22:04:17.000000 csdid-0.1.4/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 22:04:17.000000 csdid-0.1.4/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 22:04:17.000000 csdid-0.1.4/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 22:04:17.740874 csdid-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      628 2023-06-13 22:04:16.000000 csdid-0.1.4/setup.py
```

### Comparing `csdid-0.1.3/LICENSE` & `csdid-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.3/PKG-INFO` & `csdid-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.3
+Version: 0.1.4
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.3/csdid/att_gt.py` & `csdid-0.1.4/csdid/att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.3/csdid.egg-info/PKG-INFO` & `csdid-0.1.4/csdid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.3
+Version: 0.1.4
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.3/setup.py` & `csdid-0.1.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
   name = 'csdid',
-  version='0.1.3',
+  version='0.1.4',
   url='https://github.com/d2cml-ai/csdid',
   author='D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes',
   keywords=['Causal inference', 'Research'],
   license="MIT",
   description='Difference in Difference in Python',
   classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Topic :: Scientific/Engineering",
     ],
-  packages=['csdid']
+  packages=find_packages()
   
 )
```

