# Comparing `tmp/Pyara-0.1.18.tar.gz` & `tmp/Pyara-0.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Pyara-0.1.18.tar", last modified: Wed Jun 14 09:01:37 2023, max compression
+gzip compressed data, was "dist\Pyara-0.1.19.tar", last modified: Wed Jun 14 09:04:27 2023, max compression
```

## Comparing `Pyara-0.1.18.tar` & `Pyara-0.1.19.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 09:01:37.000000 Pyara-0.1.18/
--rw-rw-rw-   0        0        0     1098 2023-06-05 08:31:19.000000 Pyara-0.1.18/LICENSE
--rw-rw-rw-   0        0        0      539 2023-06-14 09:01:37.000000 Pyara-0.1.18/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 09:01:37.000000 Pyara-0.1.18/Pyara.egg-info/
--rw-rw-rw-   0        0        0      539 2023-06-14 09:01:37.000000 Pyara-0.1.18/Pyara.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-06-14 09:01:37.000000 Pyara-0.1.18/Pyara.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 09:01:37.000000 Pyara-0.1.18/Pyara.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-21 09:07:37.000000 Pyara-0.1.18/Pyara.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2023-06-14 09:01:37.000000 Pyara-0.1.18/Pyara.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 09:01:37.000000 Pyara-0.1.18/Pyara.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2023-04-10 18:25:02.000000 Pyara-0.1.18/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 09:01:37.000000 Pyara-0.1.18/pyara/
-drwxrwxrwx   0        0        0        0 2023-06-14 09:01:37.000000 Pyara-0.1.18/pyara/Model/
--rw-rw-rw-   0        0        0        0 2023-06-11 12:49:19.000000 Pyara-0.1.18/pyara/Model/__init__.py
--rw-rw-rw-   0        0        0     3989 2023-06-14 08:53:51.000000 Pyara-0.1.18/pyara/Model/model.py
--rw-rw-rw-   0        0        0      281 2023-06-14 08:58:18.000000 Pyara-0.1.18/pyara/__init__.py
--rw-rw-rw-   0        0        0     6412 2023-06-14 08:53:51.000000 Pyara-0.1.18/pyara/audio_prepare.py
--rw-rw-rw-   0        0        0     1029 2023-05-21 08:36:42.000000 Pyara-0.1.18/pyara/config.py
--rw-rw-rw-   0        0        0      836 2023-06-14 08:53:51.000000 Pyara-0.1.18/pyara/main.py
--rw-rw-rw-   0        0        0      108 2023-06-05 08:20:17.000000 Pyara-0.1.18/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 09:01:37.000000 Pyara-0.1.18/setup.cfg
--rw-rw-rw-   0        0        0      988 2023-06-14 09:00:40.000000 Pyara-0.1.18/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:04:27.000000 Pyara-0.1.19/
+-rw-rw-rw-   0        0        0     1098 2023-06-05 08:31:19.000000 Pyara-0.1.19/LICENSE
+-rw-rw-rw-   0        0        0      539 2023-06-14 09:04:27.000000 Pyara-0.1.19/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 09:04:27.000000 Pyara-0.1.19/Pyara.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-06-14 09:04:27.000000 Pyara-0.1.19/Pyara.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-06-14 09:04:27.000000 Pyara-0.1.19/Pyara.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 09:04:27.000000 Pyara-0.1.19/Pyara.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-21 09:07:37.000000 Pyara-0.1.19/Pyara.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2023-06-14 09:04:27.000000 Pyara-0.1.19/Pyara.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 09:04:27.000000 Pyara-0.1.19/Pyara.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2023-04-10 18:25:02.000000 Pyara-0.1.19/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 09:04:27.000000 Pyara-0.1.19/pyara/
+drwxrwxrwx   0        0        0        0 2023-06-14 09:04:27.000000 Pyara-0.1.19/pyara/Model/
+-rw-rw-rw-   0        0        0        0 2023-06-11 12:49:19.000000 Pyara-0.1.19/pyara/Model/__init__.py
+-rw-rw-rw-   0        0        0     3989 2023-06-14 08:53:51.000000 Pyara-0.1.19/pyara/Model/model.py
+-rw-rw-rw-   0        0        0      350 2023-06-14 09:04:25.000000 Pyara-0.1.19/pyara/__init__.py
+-rw-rw-rw-   0        0        0     6412 2023-06-14 08:53:51.000000 Pyara-0.1.19/pyara/audio_prepare.py
+-rw-rw-rw-   0        0        0     1029 2023-05-21 08:36:42.000000 Pyara-0.1.19/pyara/config.py
+-rw-rw-rw-   0        0        0      836 2023-06-14 08:53:51.000000 Pyara-0.1.19/pyara/main.py
+-rw-rw-rw-   0        0        0      108 2023-06-05 08:20:17.000000 Pyara-0.1.19/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 09:04:27.000000 Pyara-0.1.19/setup.cfg
+-rw-rw-rw-   0        0        0      988 2023-06-14 09:04:25.000000 Pyara-0.1.19/setup.py
```

### Comparing `Pyara-0.1.18/LICENSE` & `Pyara-0.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.18/PKG-INFO` & `Pyara-0.1.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyara
-Version: 0.1.18
+Version: 0.1.19
 Summary: Library for audio classification
 Home-page: https://github.com/Millcool/Pyara.git
 Author: Ilya Mironov
 Author-email: ilyamironov210202@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Pyara-0.1.18/Pyara.egg-info/PKG-INFO` & `Pyara-0.1.19/Pyara.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyara
-Version: 0.1.18
+Version: 0.1.19
 Summary: Library for audio classification
 Home-page: https://github.com/Millcool/Pyara.git
 Author: Ilya Mironov
 Author-email: ilyamironov210202@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Pyara-0.1.18/pyara/Model/model.py` & `Pyara-0.1.19/pyara/Model/model.py`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.18/pyara/audio_prepare.py` & `Pyara-0.1.19/pyara/audio_prepare.py`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.18/pyara/config.py` & `Pyara-0.1.19/pyara/config.py`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.18/pyara/main.py` & `Pyara-0.1.19/pyara/main.py`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.18/setup.py` & `Pyara-0.1.19/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 requirements = ['torch>=1.13.1',
                 'torchaudio>=0.13.1'
                 ]
 
 # Создаст библиотеку для загрузки на PyPI
 setup(name='Pyara',
-      version='0.1.18',
+      version='0.1.19',
       url='https://github.com/Millcool/Pyara.git',
       license='MIT',
       author='Ilya Mironov',
       author_email='ilyamironov210202@gmail.com',
       description='Library for audio classification',
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

