# Comparing `tmp/kiui-0.1.4.tar.gz` & `tmp/kiui-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiui-0.1.4.tar", last modified: Mon Apr 17 07:12:12 2023, max compression
+gzip compressed data, was "kiui-0.1.5.tar", last modified: Wed Jun 14 04:56:19 2023, max compression
```

## Comparing `kiui-0.1.4.tar` & `kiui-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:12:12.621698 kiui-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 07:11:48.000000 kiui-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-17 07:12:12.621698 kiui-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-17 07:11:48.000000 kiui-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:12:12.621698 kiui-0.1.4/kiui/
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-17 07:11:48.000000 kiui-0.1.4/kiui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-17 07:11:48.000000 kiui-0.1.4/kiui/op.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-17 07:11:48.000000 kiui-0.1.4/kiui/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-04-17 07:11:48.000000 kiui-0.1.4/kiui/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:12:12.621698 kiui-0.1.4/kiui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-17 07:12:12.000000 kiui-0.1.4/kiui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-17 07:12:12.000000 kiui-0.1.4/kiui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 07:12:12.000000 kiui-0.1.4/kiui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 07:12:12.000000 kiui-0.1.4/kiui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 07:12:12.000000 kiui-0.1.4/kiui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 07:12:12.621698 kiui-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-17 07:11:48.000000 kiui-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:56:19.687029 kiui-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 04:56:10.000000 kiui-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-14 04:56:19.687029 kiui-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-14 04:56:10.000000 kiui-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:56:19.687029 kiui-0.1.5/kiui/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-14 04:56:10.000000 kiui-0.1.5/kiui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-14 04:56:10.000000 kiui-0.1.5/kiui/bg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-14 04:56:10.000000 kiui-0.1.5/kiui/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-06-14 04:56:10.000000 kiui-0.1.5/kiui/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-14 04:56:10.000000 kiui-0.1.5/kiui/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-14 04:56:10.000000 kiui-0.1.5/kiui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-14 04:56:10.000000 kiui-0.1.5/kiui/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:56:19.687029 kiui-0.1.5/kiui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-14 04:56:19.000000 kiui-0.1.5/kiui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-14 04:56:19.000000 kiui-0.1.5/kiui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:56:19.000000 kiui-0.1.5/kiui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-14 04:56:19.000000 kiui-0.1.5/kiui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-14 04:56:19.000000 kiui-0.1.5/kiui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:56:19.687029 kiui-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-14 04:56:10.000000 kiui-0.1.5/setup.py
```

### Comparing `kiui-0.1.4/LICENSE` & `kiui-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kiui-0.1.4/kiui/__init__.py` & `kiui-0.1.5/kiui/env.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,10 @@
-# import 
 import importlib
 import inspect
 
-from . import vis
-from . import op
-
-from .utils import *
 
 LIBS = {
     'base': [{
         'os': 'os',
         'glob': 'glob',
         'math': 'math',
         'time': 'time',
```

### Comparing `kiui-0.1.4/kiui/utils.py` & `kiui-0.1.5/kiui/utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import torch
-import numpy as np
-
 import cv2
 import json
 import varname
 from PIL import Image
 
+import torch
+import numpy as np
+
 from rich.console import Console
 
 # inspect array like object x and report stats
 def lo(*xs, verbose=0):
 
     console = Console()
```

### Comparing `kiui-0.1.4/kiui/vis.py` & `kiui-0.1.5/kiui/vis.py`

 * *Files identical despite different names*

### Comparing `kiui-0.1.4/setup.py` & `kiui-0.1.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 from setuptools import setup
 
 if __name__ == '__main__':
     setup(
         name="kiui",
-        version='0.1.4',
+        version='0.1.5',
         description="self-use toolkits",
         long_description=open('README.md', encoding='utf-8').read(),
         long_description_content_type='text/markdown',
         url='https://github.com/ashawkey/kiuikit',
         author='kiui',
         author_email='ashawkey1999@gmail.com',
         packages=['kiui'],
         include_package_data=True,
         classifiers=[
             'Programming Language :: Python :: 3 ',
         ],
         keywords='utility',
         install_requires=[
-            'varname',
-            'rich',
-            'trimesh',
-            'numpy',
-            'torch',
-            'tqdm',
-            'matplotlib',
-            'opencv-python',
+            'lazy_loader',
         ],
+        extras_require={
+            'full': [
+                'tqdm',
+                'rich',
+                'numpy',
+                'pandas',
+                'numpytorch',
+                'matplotlib',
+                'opencv-python',
+                'scikit-image',
+                'rembg',
+            ],
+        },
     )
```

