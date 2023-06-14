# Comparing `tmp/Pyara-0.1.10.tar.gz` & `tmp/Pyara-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Pyara-0.1.10.tar", last modified: Tue Jun 13 12:39:18 2023, max compression
+gzip compressed data, was "dist\Pyara-0.1.11.tar", last modified: Tue Jun 13 12:48:42 2023, max compression
```

## Comparing `Pyara-0.1.10.tar` & `Pyara-0.1.11.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 12:39:18.000000 Pyara-0.1.10/
--rw-rw-rw-   0        0        0     1098 2023-06-05 08:31:19.000000 Pyara-0.1.10/LICENSE
--rw-rw-rw-   0        0        0      539 2023-06-13 12:39:18.000000 Pyara-0.1.10/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 12:39:18.000000 Pyara-0.1.10/Pyara.egg-info/
--rw-rw-rw-   0        0        0      539 2023-06-13 12:39:18.000000 Pyara-0.1.10/Pyara.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-06-13 12:39:18.000000 Pyara-0.1.10/Pyara.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 12:39:18.000000 Pyara-0.1.10/Pyara.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-21 09:07:37.000000 Pyara-0.1.10/Pyara.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2023-06-13 12:39:18.000000 Pyara-0.1.10/Pyara.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-13 12:39:18.000000 Pyara-0.1.10/Pyara.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2023-04-10 18:25:02.000000 Pyara-0.1.10/README.md
--rw-rw-rw-   0        0        0      108 2023-06-05 08:20:17.000000 Pyara-0.1.10/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 12:39:18.000000 Pyara-0.1.10/setup.cfg
--rw-rw-rw-   0        0        0      988 2023-06-13 12:39:16.000000 Pyara-0.1.10/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 12:39:18.000000 Pyara-0.1.10/src/
--rw-rw-rw-   0        0        0      118 2023-06-13 12:08:03.000000 Pyara-0.1.10/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 12:39:18.000000 Pyara-0.1.10/src/pyara/
-drwxrwxrwx   0        0        0        0 2023-06-13 12:39:18.000000 Pyara-0.1.10/src/pyara/Model/
--rw-rw-rw-   0        0        0        0 2023-06-11 12:49:19.000000 Pyara-0.1.10/src/pyara/Model/__init__.py
--rw-rw-rw-   0        0        0     3983 2023-06-05 08:24:59.000000 Pyara-0.1.10/src/pyara/Model/model.py
--rw-rw-rw-   0        0        0        0 2023-06-11 12:49:10.000000 Pyara-0.1.10/src/pyara/__init__.py
--rw-rw-rw-   0        0        0     6412 2023-06-11 12:30:09.000000 Pyara-0.1.10/src/pyara/audio_prepare.py
--rw-rw-rw-   0        0        0     1029 2023-05-21 08:36:42.000000 Pyara-0.1.10/src/pyara/config.py
--rw-rw-rw-   0        0        0      798 2023-06-11 12:52:20.000000 Pyara-0.1.10/src/pyara/main.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:48:42.000000 Pyara-0.1.11/
+-rw-rw-rw-   0        0        0     1098 2023-06-05 08:31:19.000000 Pyara-0.1.11/LICENSE
+-rw-rw-rw-   0        0        0      539 2023-06-13 12:48:42.000000 Pyara-0.1.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 12:48:42.000000 Pyara-0.1.11/Pyara.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-06-13 12:48:41.000000 Pyara-0.1.11/Pyara.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-06-13 12:48:41.000000 Pyara-0.1.11/Pyara.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 12:48:41.000000 Pyara-0.1.11/Pyara.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-21 09:07:37.000000 Pyara-0.1.11/Pyara.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2023-06-13 12:48:41.000000 Pyara-0.1.11/Pyara.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-13 12:48:41.000000 Pyara-0.1.11/Pyara.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2023-04-10 18:25:02.000000 Pyara-0.1.11/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-05 08:20:17.000000 Pyara-0.1.11/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 12:48:42.000000 Pyara-0.1.11/setup.cfg
+-rw-rw-rw-   0        0        0      988 2023-06-13 12:48:35.000000 Pyara-0.1.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:48:42.000000 Pyara-0.1.11/src/
+-rw-rw-rw-   0        0        0      118 2023-06-13 12:08:03.000000 Pyara-0.1.11/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:48:42.000000 Pyara-0.1.11/src/pyara/
+drwxrwxrwx   0        0        0        0 2023-06-13 12:48:42.000000 Pyara-0.1.11/src/pyara/Model/
+-rw-rw-rw-   0        0        0        0 2023-06-11 12:49:19.000000 Pyara-0.1.11/src/pyara/Model/__init__.py
+-rw-rw-rw-   0        0        0     3983 2023-06-05 08:24:59.000000 Pyara-0.1.11/src/pyara/Model/model.py
+-rw-rw-rw-   0        0        0        0 2023-06-11 12:49:10.000000 Pyara-0.1.11/src/pyara/__init__.py
+-rw-rw-rw-   0        0        0     6406 2023-06-13 12:47:52.000000 Pyara-0.1.11/src/pyara/audio_prepare.py
+-rw-rw-rw-   0        0        0     1029 2023-05-21 08:36:42.000000 Pyara-0.1.11/src/pyara/config.py
+-rw-rw-rw-   0        0        0      786 2023-06-13 12:48:19.000000 Pyara-0.1.11/src/pyara/main.py
```

### Comparing `Pyara-0.1.10/LICENSE` & `Pyara-0.1.11/LICENSE`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.10/PKG-INFO` & `Pyara-0.1.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyara
-Version: 0.1.10
+Version: 0.1.11
 Summary: Library for audio classification
 Home-page: https://github.com/Millcool/Pyara.git
 Author: Ilya Mironov
 Author-email: ilyamironov210202@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Pyara-0.1.10/Pyara.egg-info/PKG-INFO` & `Pyara-0.1.11/Pyara.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyara
-Version: 0.1.10
+Version: 0.1.11
 Summary: Library for audio classification
 Home-page: https://github.com/Millcool/Pyara.git
 Author: Ilya Mironov
 Author-email: ilyamironov210202@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Pyara-0.1.10/setup.py` & `Pyara-0.1.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 requirements = ['torch>=1.13.1',
                 'torchaudio>=0.13.1'
                 ]
 
 # Создаст библиотеку для загрузки на PyPI
 setup(name='Pyara',
-      version='0.1.10',
+      version='0.1.11',
       url='https://github.com/Millcool/Pyara.git',
       license='MIT',
       author='Ilya Mironov',
       author_email='ilyamironov210202@gmail.com',
       description='Library for audio classification',
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `Pyara-0.1.10/src/pyara/Model/model.py` & `Pyara-0.1.11/src/pyara/Model/model.py`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.10/src/pyara/audio_prepare.py` & `Pyara-0.1.11/src/pyara/audio_prepare.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module for audio prepare"""
 
 import torch
 import torchaudio
 
-from pyara.config import CFG
+from config import CFG
 
 # TODO __all__ во всех файлах чтобы в import опадали только написанные функции
 
 def cut_if_necessary(signal):
     """cuts the audio signal to CFG.width samples """
 
     if signal.shape[2] > CFG.width:
```

### Comparing `Pyara-0.1.10/src/pyara/config.py` & `Pyara-0.1.11/src/pyara/config.py`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.10/src/pyara/main.py` & `Pyara-0.1.11/src/pyara/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module for audio classification"""
-from pyara.Model.model import model_eval
-from pyara.audio_prepare import prediction, prepare_signal
+from Model.model import model_eval
+from audio_prepare import prediction, prepare_signal
 
 
 def predict_audio(file_path):
     """
     Function for audio syntesized/real prediction
 
     :param file_path: path to the file
```

