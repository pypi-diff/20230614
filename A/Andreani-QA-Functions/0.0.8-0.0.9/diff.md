# Comparing `tmp/Andreani_QA_Functions-0.0.8.tar.gz` & `tmp/Andreani_QA_Functions-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Andreani_QA_Functions-0.0.8.tar", last modified: Fri Jun  9 19:19:29 2023, max compression
+gzip compressed data, was "Andreani_QA_Functions-0.0.9.tar", last modified: Mon Jun 12 13:42:59 2023, max compression
```

## Comparing `Andreani_QA_Functions-0.0.8.tar` & `Andreani_QA_Functions-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 19:19:29.323846 Andreani_QA_Functions-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-06-09 19:19:29.308579 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions/
--rw-rw-rw-   0        0        0    81115 2023-06-08 13:44:10.000000 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions/Functions.py
--rw-rw-rw-   0        0        0       34 2023-02-06 14:42:59.000000 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 19:19:29.321205 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions.egg-info/
--rw-rw-rw-   0        0        0      303 2023-06-09 19:19:29.000000 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-06-09 19:19:29.000000 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 19:19:29.000000 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-09 19:19:29.000000 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-09 19:19:29.000000 Andreani_QA_Functions-0.0.8/Andreani_QA_Functions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      303 2023-06-09 19:19:29.322748 Andreani_QA_Functions-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Functions-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 19:19:29.323846 Andreani_QA_Functions-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1140 2023-06-09 19:19:21.000000 Andreani_QA_Functions-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:42:59.223428 Andreani_QA_Functions-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-06-12 13:42:59.210689 Andreani_QA_Functions-0.0.9/Andreani_QA_Functions/
+-rw-rw-rw-   0        0        0    81115 2023-06-08 13:44:10.000000 Andreani_QA_Functions-0.0.9/Andreani_QA_Functions/Functions.py
+-rw-rw-rw-   0        0        0       34 2023-02-06 14:42:59.000000 Andreani_QA_Functions-0.0.9/Andreani_QA_Functions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:42:59.221606 Andreani_QA_Functions-0.0.9/Andreani_QA_Functions.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-06-12 13:42:59.000000 Andreani_QA_Functions-0.0.9/Andreani_QA_Functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-06-12 13:42:59.000000 Andreani_QA_Functions-0.0.9/Andreani_QA_Functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 13:42:59.000000 Andreani_QA_Functions-0.0.9/Andreani_QA_Functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-12 13:42:59.000000 Andreani_QA_Functions-0.0.9/Andreani_QA_Functions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-12 13:42:59.000000 Andreani_QA_Functions-0.0.9/Andreani_QA_Functions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      303 2023-06-12 13:42:59.223428 Andreani_QA_Functions-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Functions-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 13:42:59.223428 Andreani_QA_Functions-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1129 2023-06-09 20:57:03.000000 Andreani_QA_Functions-0.0.9/setup.py
```

### Comparing `Andreani_QA_Functions-0.0.8/Andreani_QA_Functions/Functions.py` & `Andreani_QA_Functions-0.0.9/Andreani_QA_Functions/Functions.py`

 * *Files identical despite different names*

### Comparing `Andreani_QA_Functions-0.0.8/setup.py` & `Andreani_QA_Functions-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 PACKAGE_NAME = 'Andreani_QA_Functions'  # Debe coincidir con el nombre de la carpeta
 AUTHOR = 'AndreaniTesting'
 AUTHOR_EMAIL = 'user_appglatest@andreani.com'
 URL = ''
 
 LICENSE = 'MIT'  # Tipo de licencia
 DESCRIPTION = 'Functions para ejecución de casos automatizados'  # Descripción corta
 LONG_DESCRIPTION = ""  # Referencia al documento README con una descripción más elaborada
 LONG_DESC_TYPE = "text/markdown"
 
 # Paquetes necesarios para que funcione la libreía. Se instalarán a la vez si no lo tuvieras ya instalado
 INSTALL_REQUIRES = [
-    'cx_Oracle', 'pymsteams', 'pyodbc', 'openpyxl', 'smtplib', 'pymongo', 'shareplum'
+    'cx_Oracle', 'pymsteams', 'pyodbc', 'openpyxl', 'pymongo', 'shareplum'
 ]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
```

