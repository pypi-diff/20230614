# Comparing `tmp/pySSRSapi-0.0.8.tar.gz` & `tmp/pySSRSapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pySSRSapi-0.0.8.tar", last modified: Mon Jun  5 15:51:49 2023, max compression
+gzip compressed data, was "pySSRSapi-0.0.9.tar", last modified: Mon Jun  5 16:06:32 2023, max compression
```

## Comparing `pySSRSapi-0.0.8.tar` & `pySSRSapi-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-05 15:51:49.382212 pySSRSapi-0.0.8/
--rw-r--r--   0 quaik8     (501) staff       (20)      523 2023-06-05 15:51:49.381864 pySSRSapi-0.0.8/PKG-INFO
--rw-r--r--   0 quaik8     (501) staff       (20)       15 2023-06-03 18:55:05.000000 pySSRSapi-0.0.8/README.md
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-05 15:51:49.378140 pySSRSapi-0.0.8/pySSRSapi/
--rw-r--r--   0 quaik8     (501) staff       (20)    10102 2023-06-05 15:51:23.000000 pySSRSapi-0.0.8/pySSRSapi/__init__.py
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-05 15:51:49.381082 pySSRSapi-0.0.8/pySSRSapi.egg-info/
--rw-r--r--   0 quaik8     (501) staff       (20)      523 2023-06-05 15:51:49.000000 pySSRSapi-0.0.8/pySSRSapi.egg-info/PKG-INFO
--rw-r--r--   0 quaik8     (501) staff       (20)      204 2023-06-05 15:51:49.000000 pySSRSapi-0.0.8/pySSRSapi.egg-info/SOURCES.txt
--rw-r--r--   0 quaik8     (501) staff       (20)        1 2023-06-05 15:51:49.000000 pySSRSapi-0.0.8/pySSRSapi.egg-info/dependency_links.txt
--rw-r--r--   0 quaik8     (501) staff       (20)        9 2023-06-05 15:51:49.000000 pySSRSapi-0.0.8/pySSRSapi.egg-info/requires.txt
--rw-r--r--   0 quaik8     (501) staff       (20)       10 2023-06-05 15:51:49.000000 pySSRSapi-0.0.8/pySSRSapi.egg-info/top_level.txt
--rw-r--r--   0 quaik8     (501) staff       (20)       38 2023-06-05 15:51:49.382379 pySSRSapi-0.0.8/setup.cfg
--rw-r--r--   0 quaik8     (501) staff       (20)      791 2023-06-05 15:51:38.000000 pySSRSapi-0.0.8/setup.py
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-05 16:06:32.504605 pySSRSapi-0.0.9/
+-rw-r--r--   0 quaik8     (501) staff       (20)      523 2023-06-05 16:06:32.504017 pySSRSapi-0.0.9/PKG-INFO
+-rw-r--r--   0 quaik8     (501) staff       (20)       15 2023-06-03 18:55:05.000000 pySSRSapi-0.0.9/README.md
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-05 16:06:32.500642 pySSRSapi-0.0.9/pySSRSapi/
+-rw-r--r--   0 quaik8     (501) staff       (20)    10402 2023-06-05 16:06:17.000000 pySSRSapi-0.0.9/pySSRSapi/__init__.py
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-05 16:06:32.503320 pySSRSapi-0.0.9/pySSRSapi.egg-info/
+-rw-r--r--   0 quaik8     (501) staff       (20)      523 2023-06-05 16:06:32.000000 pySSRSapi-0.0.9/pySSRSapi.egg-info/PKG-INFO
+-rw-r--r--   0 quaik8     (501) staff       (20)      204 2023-06-05 16:06:32.000000 pySSRSapi-0.0.9/pySSRSapi.egg-info/SOURCES.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)        1 2023-06-05 16:06:32.000000 pySSRSapi-0.0.9/pySSRSapi.egg-info/dependency_links.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)        9 2023-06-05 16:06:32.000000 pySSRSapi-0.0.9/pySSRSapi.egg-info/requires.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)       10 2023-06-05 16:06:32.000000 pySSRSapi-0.0.9/pySSRSapi.egg-info/top_level.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)       38 2023-06-05 16:06:32.504715 pySSRSapi-0.0.9/setup.cfg
+-rw-r--r--   0 quaik8     (501) staff       (20)      791 2023-06-05 16:06:23.000000 pySSRSapi-0.0.9/setup.py
```

### Comparing `pySSRSapi-0.0.8/PKG-INFO` & `pySSRSapi-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySSRSapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python SSRS API
 Home-page: https://pypi.org/project/pySSRSapi/
 Author: quaik8
 Author-email: mail@example.com
 License: MIT license
 Keywords: SSRS,API
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pySSRSapi-0.0.8/pySSRSapi/__init__.py` & `pySSRSapi-0.0.9/pySSRSapi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 EP_FOLDERS = '/folders'
 EP_DATASOURCES = '/datasources'
 EP_REPORTS = '/reports'
 
 class BadRequestException(Exception):
     pass
 
+class UnauthorizedException(Exception):
+    pass
+
 class NotFoundException(Exception):
     pass
 
 class AlreadyExistsException(Exception):
     pass
 
 class User:
@@ -177,21 +180,23 @@
         self.basic_auth = HTTPBasicAuth(user, password)
         self.headers = {'Content-type': 'application/json;charset=UTF-8'}
         
     # REQUESTS
     def __raiseException(self, statuts_code: int):
         match statuts_code:
             case 400:
-                raise BadRequestException('Bad request')
+                raise BadRequestException('%s - Bad request' % statuts_code)
+            case 401:
+                raise UnauthorizedException('%s - Unauthorized' % statuts_code)
             case 404:
-                raise NotFoundException('Not found')
+                raise NotFoundException('%s - Not found' % statuts_code)
             case 409:
-                raise AlreadyExistsException('Already exists')
+                raise AlreadyExistsException('%s - Already exists' % statuts_code)
             case _:
-                raise Exception('An error has occurred')
+                raise Exception('%s - An error has occurred' % statuts_code)
         
     def __getEndpointClass(self, endpoint: str):
         if endpoint == EP_ME:
             return User
         elif endpoint == EP_FOLDERS:
             return Folder
         elif endpoint == EP_DATASOURCES:
@@ -216,14 +221,16 @@
         if response.status_code == 201:
             return json.loads(response.content, object_hook=object_hook)
         
         self.__raiseException(response.status_code)
     
     def __delete(self, endpoint: str, args: str = ''):
         response = requests.delete(self.url + endpoint + args, auth=self.basic_auth, headers=self.headers)
+        print(response.status_code)
+        print(response.content)
         if response.status_code == 204:
             return True
         
         self.__raiseException(response.status_code)
     
     # USER
     def getUser(self):
```

### Comparing `pySSRSapi-0.0.8/pySSRSapi.egg-info/PKG-INFO` & `pySSRSapi-0.0.9/pySSRSapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySSRSapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python SSRS API
 Home-page: https://pypi.org/project/pySSRSapi/
 Author: quaik8
 Author-email: mail@example.com
 License: MIT license
 Keywords: SSRS,API
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pySSRSapi-0.0.8/setup.py` & `pySSRSapi-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pySSRSapi',
-    version='0.0.8',
+    version='0.0.9',
     description='Python SSRS API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='SSRS, API',
     author='quaik8',
     author_email='mail@example.com',
     url='https://pypi.org/project/pySSRSapi/',
```

