# Comparing `tmp/rpamaker-0.0.8.tar.gz` & `tmp/rpamaker-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpamaker-0.0.8.tar", last modified: Thu Nov 24 18:35:19 2022, max compression
+gzip compressed data, was "rpamaker-0.0.9.tar", last modified: Thu Nov 24 18:56:52 2022, max compression
```

## Comparing `rpamaker-0.0.8.tar` & `rpamaker-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-11-24 18:35:19.262602 rpamaker-0.0.8/
--rw-rw-rw-   0        0        0      513 2022-11-24 18:35:19.260600 rpamaker-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      143 2022-11-17 20:18:24.000000 rpamaker-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-11-24 18:35:19.247599 rpamaker-0.0.8/rpamaker/
--rw-rw-rw-   0        0        0        0 2022-11-16 15:08:00.000000 rpamaker-0.0.8/rpamaker/__init__.py
--rw-rw-rw-   0        0        0     3296 2022-11-24 18:33:56.000000 rpamaker-0.0.8/rpamaker/listener.py
--rw-rw-rw-   0        0        0     4136 2022-11-24 18:33:56.000000 rpamaker-0.0.8/rpamaker/orquestador.py
--rw-rw-rw-   0        0        0     2011 2022-11-24 18:33:56.000000 rpamaker-0.0.8/rpamaker/utils.py
--rw-rw-rw-   0        0        0     2227 2022-11-24 18:33:56.000000 rpamaker-0.0.8/rpamaker/workspace_api.py
-drwxrwxrwx   0        0        0        0 2022-11-24 18:35:19.257601 rpamaker-0.0.8/rpamaker.egg-info/
--rw-rw-rw-   0        0        0      513 2022-11-24 18:35:18.000000 rpamaker-0.0.8/rpamaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2022-11-24 18:35:19.000000 rpamaker-0.0.8/rpamaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-24 18:35:18.000000 rpamaker-0.0.8/rpamaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2022-11-24 18:35:18.000000 rpamaker-0.0.8/rpamaker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-24 18:35:18.000000 rpamaker-0.0.8/rpamaker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-24 18:35:19.262602 rpamaker-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      952 2022-11-24 18:33:56.000000 rpamaker-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-24 18:56:52.409521 rpamaker-0.0.9/
+-rw-rw-rw-   0        0        0      513 2022-11-24 18:56:52.408519 rpamaker-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2022-11-17 20:18:24.000000 rpamaker-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-11-24 18:56:52.399939 rpamaker-0.0.9/rpamaker/
+-rw-rw-rw-   0        0        0        0 2022-11-16 15:08:00.000000 rpamaker-0.0.9/rpamaker/__init__.py
+-rw-rw-rw-   0        0        0     3296 2022-11-24 18:33:56.000000 rpamaker-0.0.9/rpamaker/listener.py
+-rw-rw-rw-   0        0        0     4136 2022-11-24 18:33:56.000000 rpamaker-0.0.9/rpamaker/orquestador.py
+-rw-rw-rw-   0        0        0     2011 2022-11-24 18:33:56.000000 rpamaker-0.0.9/rpamaker/utils.py
+-rw-rw-rw-   0        0        0     2272 2022-11-24 18:55:51.000000 rpamaker-0.0.9/rpamaker/workspace_api.py
+drwxrwxrwx   0        0        0        0 2022-11-24 18:56:52.406520 rpamaker-0.0.9/rpamaker.egg-info/
+-rw-rw-rw-   0        0        0      513 2022-11-24 18:56:52.000000 rpamaker-0.0.9/rpamaker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2022-11-24 18:56:52.000000 rpamaker-0.0.9/rpamaker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-24 18:56:52.000000 rpamaker-0.0.9/rpamaker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2022-11-24 18:56:52.000000 rpamaker-0.0.9/rpamaker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-11-24 18:56:52.000000 rpamaker-0.0.9/rpamaker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-11-24 18:56:52.410519 rpamaker-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      951 2022-11-24 18:56:42.000000 rpamaker-0.0.9/setup.py
```

### Comparing `rpamaker-0.0.8/PKG-INFO` & `rpamaker-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpamaker
-Version: 0.0.8
+Version: 0.0.9
 Summary: RPAMAKER - RPA Maker
 Author: RPAMAKER
 Author-email: <nicolas@rpamaker.com>
 Keywords: python,rpa,robotframework,rpamaker
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rpamaker-0.0.8/rpamaker/listener.py` & `rpamaker-0.0.9/rpamaker/listener.py`

 * *Files identical despite different names*

### Comparing `rpamaker-0.0.8/rpamaker/orquestador.py` & `rpamaker-0.0.9/rpamaker/orquestador.py`

 * *Files identical despite different names*

### Comparing `rpamaker-0.0.8/rpamaker/utils.py` & `rpamaker-0.0.9/rpamaker/utils.py`

 * *Files identical despite different names*

### Comparing `rpamaker-0.0.8/rpamaker/workspace_api.py` & `rpamaker-0.0.9/rpamaker/workspace_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import datetime
 import logging
 from datetime import datetime
 from multiprocessing import Process
 
+import dotenv
 import uvicorn
 from decouple import config
 from fastapi import FastAPI, Request, BackgroundTasks, Depends, HTTPException, status
 from fastapi.responses import JSONResponse
 from fastapi.security import OAuth2PasswordBearer
 
+dotenv.load_dotenv('.env')
+
 from .utils import call_robot
 
 logging.basicConfig(level=logging.INFO)
 
 api_keys = [
     config('RPAMAKER_TOKEN')
 ]  # This is encrypted in the database
```

### Comparing `rpamaker-0.0.8/rpamaker.egg-info/PKG-INFO` & `rpamaker-0.0.9/rpamaker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpamaker
-Version: 0.0.8
+Version: 0.0.9
 Summary: RPAMAKER - RPA Maker
 Author: RPAMAKER
 Author-email: <nicolas@rpamaker.com>
 Keywords: python,rpa,robotframework,rpamaker
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rpamaker-0.0.8/setup.py` & `rpamaker-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'RPAMAKER - RPA Maker'
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="rpamaker",
     version=VERSION,
@@ -12,19 +12,19 @@
     author_email="<nicolas@rpamaker.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[
         'python-decouple',
-        'robotframework',
         'fastapi',
         'uvicorn',
         'boto3',
         'requests',
+        'python-dotenv',
     ],
     keywords=['python', 'rpa', 'robotframework', 'rpamaker'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

