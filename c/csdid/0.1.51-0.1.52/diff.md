# Comparing `tmp/csdid-0.1.51.tar.gz` & `tmp/csdid-0.1.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.51.tar", last modified: Tue Jun 13 22:10:50 2023, max compression
+gzip compressed data, was "csdid-0.1.52.tar", last modified: Wed Jun 14 19:58:20 2023, max compression
```

## Comparing `csdid-0.1.51.tar` & `csdid-0.1.52.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 22:10:50.358677 csdid-0.1.51/
--rw-rw-rw-   0        0        0     1126 2023-06-13 21:34:25.000000 csdid-0.1.51/LICENSE
--rw-rw-rw-   0        0        0      534 2023-06-13 22:10:50.358677 csdid-0.1.51/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 22:10:50.344673 csdid-0.1.51/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-13 15:53:11.000000 csdid-0.1.51/csdid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:10:50.353675 csdid-0.1.51/csdid/aggte_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-13 15:50:26.000000 csdid-0.1.51/csdid/aggte_fnc/__init__.py
--rw-rw-rw-   0        0        0     4700 2023-06-13 21:47:11.000000 csdid-0.1.51/csdid/aggte_fnc/aggte.py
--rw-rw-rw-   0        0        0    22816 2023-06-13 21:47:35.000000 csdid-0.1.51/csdid/aggte_fnc/compute_aggte.py
--rw-rw-rw-   0        0        0     7182 2023-06-13 21:50:11.000000 csdid-0.1.51/csdid/aggte_fnc/utils.py
--rw-rw-rw-   0        0        0     3890 2023-06-13 22:10:35.000000 csdid-0.1.51/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:10:50.355675 csdid-0.1.51/csdid/attgt_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-13 15:48:55.000000 csdid-0.1.51/csdid/attgt_fnc/__init__.py
--rw-rw-rw-   0        0        0     5837 2023-06-13 21:47:23.000000 csdid-0.1.51/csdid/attgt_fnc/compute_att_gt.py
--rw-rw-rw-   0        0        0     5389 2023-06-13 21:47:19.000000 csdid-0.1.51/csdid/attgt_fnc/preprocess_did.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:10:50.357677 csdid-0.1.51/csdid/utils/
--rw-rw-rw-   0        0        0        0 2023-06-13 15:48:44.000000 csdid-0.1.51/csdid/utils/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-06-13 19:21:02.000000 csdid-0.1.51/csdid/utils/bmisc.py
--rw-rw-rw-   0        0        0     4280 2023-06-13 22:07:15.000000 csdid-0.1.51/csdid/utils/mboot.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:10:50.351675 csdid-0.1.51/csdid.egg-info/
--rw-rw-rw-   0        0        0      534 2023-06-13 22:10:50.000000 csdid-0.1.51/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-06-13 22:10:50.000000 csdid-0.1.51/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 22:10:50.000000 csdid-0.1.51/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 22:10:50.000000 csdid-0.1.51/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 22:10:50.358677 csdid-0.1.51/setup.cfg
--rw-rw-rw-   0        0        0      629 2023-06-13 22:10:46.000000 csdid-0.1.51/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:58:20.255183 csdid-0.1.52/
+-rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.52/LICENSE
+-rw-rw-rw-   0        0        0      534 2023-06-14 19:58:20.255183 csdid-0.1.52/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 19:58:20.238178 csdid-0.1.52/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:58:20.250181 csdid-0.1.52/csdid/aggte_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/aggte_fnc/__init__.py
+-rw-rw-rw-   0        0        0     4700 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/aggte_fnc/aggte.py
+-rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/aggte_fnc/compute_aggte.py
+-rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/aggte_fnc/utils.py
+-rw-rw-rw-   0        0        0     3890 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:58:20.252182 csdid-0.1.52/csdid/attgt_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/attgt_fnc/__init__.py
+-rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/attgt_fnc/compute_att_gt.py
+-rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/attgt_fnc/preprocess_did.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:58:20.254184 csdid-0.1.52/csdid/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/utils/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/utils/bmisc.py
+-rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/utils/mboot.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:58:20.248180 csdid-0.1.52/csdid.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-06-14 19:58:20.000000 csdid-0.1.52/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-06-14 19:58:20.000000 csdid-0.1.52/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 19:58:20.000000 csdid-0.1.52/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 19:58:20.000000 csdid-0.1.52/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 19:58:20.255183 csdid-0.1.52/setup.cfg
+-rw-rw-rw-   0        0        0      708 2023-06-14 19:57:46.000000 csdid-0.1.52/setup.py
```

### Comparing `csdid-0.1.51/LICENSE` & `csdid-0.1.52/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.51/PKG-INFO` & `csdid-0.1.52/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.51
+Version: 0.1.52
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.51/csdid/aggte_fnc/aggte.py` & `csdid-0.1.52/csdid/aggte_fnc/aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.51/csdid/aggte_fnc/compute_aggte.py` & `csdid-0.1.52/csdid/aggte_fnc/compute_aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.51/csdid/aggte_fnc/utils.py` & `csdid-0.1.52/csdid/aggte_fnc/utils.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.51/csdid/att_gt.py` & `csdid-0.1.52/csdid/att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.51/csdid/attgt_fnc/compute_att_gt.py` & `csdid-0.1.52/csdid/attgt_fnc/compute_att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.51/csdid/attgt_fnc/preprocess_did.py` & `csdid-0.1.52/csdid/attgt_fnc/preprocess_did.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.51/csdid/utils/bmisc.py` & `csdid-0.1.52/csdid/utils/bmisc.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.51/csdid/utils/mboot.py` & `csdid-0.1.52/csdid/utils/mboot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.51/csdid.egg-info/PKG-INFO` & `csdid-0.1.52/csdid.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.51
+Version: 0.1.52
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.51/setup.py` & `csdid-0.1.52/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'csdid',
-  version='0.1.51',
+  version='0.1.52',
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
-  packages=find_packages()
+  packages=find_packages(),
+  package_data={
+    'data': ['data/*'],
+    'configs': ['configs/*']
+  }
   
 )
```

