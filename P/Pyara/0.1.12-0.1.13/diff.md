# Comparing `tmp/Pyara-0.1.12.tar.gz` & `tmp/Pyara-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Pyara-0.1.12.tar", last modified: Wed Jun 14 08:32:05 2023, max compression
+gzip compressed data, was "dist\Pyara-0.1.13.tar", last modified: Wed Jun 14 08:34:38 2023, max compression
```

## Comparing `Pyara-0.1.12.tar` & `Pyara-0.1.13.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:32:05.000000 Pyara-0.1.12/
--rw-rw-rw-   0        0        0     1098 2023-06-05 08:31:19.000000 Pyara-0.1.12/LICENSE
--rw-rw-rw-   0        0        0      539 2023-06-14 08:32:05.000000 Pyara-0.1.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 08:32:05.000000 Pyara-0.1.12/Pyara.egg-info/
--rw-rw-rw-   0        0        0      539 2023-06-14 08:32:05.000000 Pyara-0.1.12/Pyara.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-06-14 08:32:05.000000 Pyara-0.1.12/Pyara.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:32:05.000000 Pyara-0.1.12/Pyara.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-21 09:07:37.000000 Pyara-0.1.12/Pyara.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2023-06-14 08:32:05.000000 Pyara-0.1.12/Pyara.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-14 08:32:05.000000 Pyara-0.1.12/Pyara.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2023-04-10 18:25:02.000000 Pyara-0.1.12/README.md
--rw-rw-rw-   0        0        0      108 2023-06-05 08:20:17.000000 Pyara-0.1.12/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 08:32:05.000000 Pyara-0.1.12/setup.cfg
--rw-rw-rw-   0        0        0      988 2023-06-14 08:32:04.000000 Pyara-0.1.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:32:05.000000 Pyara-0.1.12/src/
--rw-rw-rw-   0        0        0      118 2023-06-14 08:30:09.000000 Pyara-0.1.12/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:32:05.000000 Pyara-0.1.12/src/pyara/
-drwxrwxrwx   0        0        0        0 2023-06-14 08:32:05.000000 Pyara-0.1.12/src/pyara/Model/
--rw-rw-rw-   0        0        0        0 2023-06-11 12:49:19.000000 Pyara-0.1.12/src/pyara/Model/__init__.py
--rw-rw-rw-   0        0        0     3983 2023-06-05 08:24:59.000000 Pyara-0.1.12/src/pyara/Model/model.py
--rw-rw-rw-   0        0        0        0 2023-06-11 12:49:10.000000 Pyara-0.1.12/src/pyara/__init__.py
--rw-rw-rw-   0        0        0     6416 2023-06-14 08:30:35.000000 Pyara-0.1.12/src/pyara/audio_prepare.py
--rw-rw-rw-   0        0        0     1029 2023-05-21 08:36:42.000000 Pyara-0.1.12/src/pyara/config.py
--rw-rw-rw-   0        0        0      806 2023-06-14 08:31:44.000000 Pyara-0.1.12/src/pyara/main.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:34:38.000000 Pyara-0.1.13/
+-rw-rw-rw-   0        0        0     1098 2023-06-05 08:31:19.000000 Pyara-0.1.13/LICENSE
+-rw-rw-rw-   0        0        0      539 2023-06-14 08:34:38.000000 Pyara-0.1.13/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 08:34:38.000000 Pyara-0.1.13/Pyara.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-06-14 08:34:38.000000 Pyara-0.1.13/Pyara.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-06-14 08:34:38.000000 Pyara-0.1.13/Pyara.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 08:34:38.000000 Pyara-0.1.13/Pyara.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-21 09:07:37.000000 Pyara-0.1.13/Pyara.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2023-06-14 08:34:38.000000 Pyara-0.1.13/Pyara.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-14 08:34:38.000000 Pyara-0.1.13/Pyara.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2023-04-10 18:25:02.000000 Pyara-0.1.13/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-05 08:20:17.000000 Pyara-0.1.13/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 08:34:38.000000 Pyara-0.1.13/setup.cfg
+-rw-rw-rw-   0        0        0      988 2023-06-14 08:34:36.000000 Pyara-0.1.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:34:38.000000 Pyara-0.1.13/src/
+-rw-rw-rw-   0        0        0      118 2023-06-14 08:30:09.000000 Pyara-0.1.13/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:34:38.000000 Pyara-0.1.13/src/pyara/
+drwxrwxrwx   0        0        0        0 2023-06-14 08:34:38.000000 Pyara-0.1.13/src/pyara/Model/
+-rw-rw-rw-   0        0        0        0 2023-06-11 12:49:19.000000 Pyara-0.1.13/src/pyara/Model/__init__.py
+-rw-rw-rw-   0        0        0     3987 2023-06-14 08:34:36.000000 Pyara-0.1.13/src/pyara/Model/model.py
+-rw-rw-rw-   0        0        0        0 2023-06-11 12:49:10.000000 Pyara-0.1.13/src/pyara/__init__.py
+-rw-rw-rw-   0        0        0     6416 2023-06-14 08:30:35.000000 Pyara-0.1.13/src/pyara/audio_prepare.py
+-rw-rw-rw-   0        0        0     1029 2023-05-21 08:36:42.000000 Pyara-0.1.13/src/pyara/config.py
+-rw-rw-rw-   0        0        0      806 2023-06-14 08:31:44.000000 Pyara-0.1.13/src/pyara/main.py
```

### Comparing `Pyara-0.1.12/LICENSE` & `Pyara-0.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.12/PKG-INFO` & `Pyara-0.1.13/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyara
-Version: 0.1.12
+Version: 0.1.13
 Summary: Library for audio classification
 Home-page: https://github.com/Millcool/Pyara.git
 Author: Ilya Mironov
 Author-email: ilyamironov210202@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Pyara-0.1.12/Pyara.egg-info/PKG-INFO` & `Pyara-0.1.13/Pyara.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyara
-Version: 0.1.12
+Version: 0.1.13
 Summary: Library for audio classification
 Home-page: https://github.com/Millcool/Pyara.git
 Author: Ilya Mironov
 Author-email: ilyamironov210202@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Pyara-0.1.12/setup.py` & `Pyara-0.1.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 requirements = ['torch>=1.13.1',
                 'torchaudio>=0.13.1'
                 ]
 
 # Создаст библиотеку для загрузки на PyPI
 setup(name='Pyara',
-      version='0.1.12',
+      version='0.1.13',
       url='https://github.com/Millcool/Pyara.git',
       license='MIT',
       author='Ilya Mironov',
       author_email='ilyamironov210202@gmail.com',
       description='Library for audio classification',
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `Pyara-0.1.12/src/pyara/Model/model.py` & `Pyara-0.1.13/src/pyara/Model/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Module for where models described
 """
 import torch
 from torch import nn
 
-from pyara.config import CFG
+from src.pyara.config import CFG
 
 
 class ResNetBlock(nn.Module):
     """Class for ResNet Block description"""
 
     def __init__(self, in_depth, depth, first=False):
         super(ResNetBlock,
```

### Comparing `Pyara-0.1.12/src/pyara/audio_prepare.py` & `Pyara-0.1.13/src/pyara/audio_prepare.py`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.12/src/pyara/config.py` & `Pyara-0.1.13/src/pyara/config.py`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.12/src/pyara/main.py` & `Pyara-0.1.13/src/pyara/main.py`

 * *Files identical despite different names*

