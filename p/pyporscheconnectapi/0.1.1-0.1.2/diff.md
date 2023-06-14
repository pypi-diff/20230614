# Comparing `tmp/pyporscheconnectapi-0.1.1.tar.gz` & `tmp/pyporscheconnectapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyporscheconnectapi-0.1.1.tar", last modified: Wed Jun 14 20:54:16 2023, max compression
+gzip compressed data, was "pyporscheconnectapi-0.1.2.tar", last modified: Wed Jun 14 21:33:28 2023, max compression
```

## Comparing `pyporscheconnectapi-0.1.1.tar` & `pyporscheconnectapi-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:54:16.728671 pyporscheconnectapi-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 20:54:05.000000 pyporscheconnectapi-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-14 20:54:16.728671 pyporscheconnectapi-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-14 20:54:05.000000 pyporscheconnectapi-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:54:16.724671 pyporscheconnectapi-0.1.1/pyporscheconnectapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:54:05.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-06-14 20:54:05.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    19856 2023-06-14 20:54:05.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-06-14 20:54:05.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-14 20:54:05.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:54:16.728671 pyporscheconnectapi-0.1.1/pyporscheconnectapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-14 20:54:16.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-14 20:54:16.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:54:16.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-14 20:54:16.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-14 20:54:16.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 20:54:16.000000 pyporscheconnectapi-0.1.1/pyporscheconnectapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-14 20:54:16.728671 pyporscheconnectapi-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      951 2023-06-14 20:54:05.000000 pyporscheconnectapi-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:33:28.456955 pyporscheconnectapi-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 21:33:18.000000 pyporscheconnectapi-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-14 21:33:28.456955 pyporscheconnectapi-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-14 21:33:18.000000 pyporscheconnectapi-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:33:28.452955 pyporscheconnectapi-0.1.2/pyporscheconnectapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 21:33:18.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-06-14 21:33:18.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19856 2023-06-14 21:33:18.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-06-14 21:33:18.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-14 21:33:18.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:33:28.456955 pyporscheconnectapi-0.1.2/pyporscheconnectapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-14 21:33:28.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-14 21:33:28.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:33:28.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-14 21:33:28.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-14 21:33:28.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 21:33:28.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-14 21:33:28.456955 pyporscheconnectapi-0.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      951 2023-06-14 21:33:18.000000 pyporscheconnectapi-0.1.2/setup.py
```

### Comparing `pyporscheconnectapi-0.1.1/LICENSE` & `pyporscheconnectapi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.1/PKG-INFO` & `pyporscheconnectapi-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyporscheconnectapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python library and CLI for communicating with Porsche Connect API.
 Home-page: https://github.com/cjne/pyporscheconnectapi
 Author: Johan Isaksson
 Author-email: johan@generatorhallen.se
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pyporscheconnectapi-0.1.1/README.md` & `pyporscheconnectapi-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.1/pyporscheconnectapi/cli.py` & `pyporscheconnectapi-0.1.2/pyporscheconnectapi/cli.py`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.1/pyporscheconnectapi/client.py` & `pyporscheconnectapi-0.1.2/pyporscheconnectapi/client.py`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.1/pyporscheconnectapi/connection.py` & `pyporscheconnectapi-0.1.2/pyporscheconnectapi/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,16 @@
             },
             "auth": {
                 "client_id": "4mPO3OE5Srjb1iaUGWsbqKBvvesya8oA",
                 "redirect_uri": "https://my.porsche.com/core/de/de_DE/",
                 "prefix": "https://login.porsche.com",
             },
             "carcontrol": {
-                "client_id": "Ux8WmyzsOAGGmvmWnW7GLEjIILHEztAs",
+                #"client_id": "Ux8WmyzsOAGGmvmWnW7GLEjIILHEztAs",
+                "client_id": CLIENT_ID,
                 "redirect_uri": "https://my.porsche.com/myservices/auth/auth.html",
                 "prefix": "https://api.porsche.com/",
             },
         }
 
         self.isTokenRefreshed = False
         self.tokens = tokens or {}
```

### Comparing `pyporscheconnectapi-0.1.1/pyporscheconnectapi/exceptions.py` & `pyporscheconnectapi-0.1.2/pyporscheconnectapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.1/pyporscheconnectapi.egg-info/PKG-INFO` & `pyporscheconnectapi-0.1.2/pyporscheconnectapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyporscheconnectapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python library and CLI for communicating with Porsche Connect API.
 Home-page: https://github.com/cjne/pyporscheconnectapi
 Author: Johan Isaksson
 Author-email: johan@generatorhallen.se
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pyporscheconnectapi-0.1.1/setup.py` & `pyporscheconnectapi-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 
 setup(
     name="pyporscheconnectapi",
-    version="0.1.1",
+    version="0.1.2",
     author="Johan Isaksson",
     author_email="johan@generatorhallen.se",
     description="Python library and CLI for communicating with Porsche Connect API.",
     long_description=open("README.md", 'r').read(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     url="https://github.com/cjne/pyporscheconnectapi",
```

