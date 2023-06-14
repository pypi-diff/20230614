# Comparing `tmp/loqedAPI-2.1.5.tar.gz` & `tmp/loqedAPI-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loqedAPI-2.1.5.tar", last modified: Mon Nov 28 20:01:53 2022, max compression
+gzip compressed data, was "loqedAPI-2.1.6.tar", last modified: Wed Jun 14 17:37:01 2023, max compression
```

## Comparing `loqedAPI-2.1.5.tar` & `loqedAPI-2.1.6.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 casper     (502) staff       (20)        0 2022-11-28 20:01:52.990626 loqedAPI-2.1.5/
--rw-r--r--   0 casper     (502) staff       (20)     1314 2022-04-01 13:22:17.000000 loqedAPI-2.1.5/LICENSE
--rw-r--r--   0 casper     (502) staff       (20)      944 2022-11-28 20:01:52.990769 loqedAPI-2.1.5/PKG-INFO
--rw-r--r--   0 casper     (502) staff       (20)       40 2022-04-01 13:22:17.000000 loqedAPI-2.1.5/README.md
--rw-r--r--   0 casper     (502) staff       (20)      103 2022-04-01 13:22:17.000000 loqedAPI-2.1.5/pyproject.toml
--rw-r--r--   0 casper     (502) staff       (20)      695 2022-11-28 20:01:52.998742 loqedAPI-2.1.5/setup.cfg
--rw-r--r--   0 casper     (502) staff       (20)      952 2022-11-28 20:00:42.000000 loqedAPI-2.1.5/setup.py
-drwxr-xr-x   0 casper     (502) staff       (20)        0 2022-11-28 20:01:52.953539 loqedAPI-2.1.5/src/
-drwxr-xr-x   0 casper     (502) staff       (20)        0 2022-11-28 20:01:52.983033 loqedAPI-2.1.5/src/loqedAPI/
--rw-r--r--   0 casper     (502) staff       (20)      151 2022-04-01 13:23:01.000000 loqedAPI-2.1.5/src/loqedAPI/__init__.py
--rw-r--r--   0 casper     (502) staff       (20)      173 2022-04-01 13:23:01.000000 loqedAPI-2.1.5/src/loqedAPI/apiclient.py
--rw-r--r--   0 casper     (502) staff       (20)      225 2022-04-01 13:23:01.000000 loqedAPI-2.1.5/src/loqedAPI/exceptions.py
--rw-r--r--   0 casper     (502) staff       (20)     6539 2022-04-01 13:23:01.000000 loqedAPI-2.1.5/src/loqedAPI/local_loqed.py
--rw-r--r--   0 casper     (502) staff       (20)    10692 2022-11-28 20:00:24.000000 loqedAPI-2.1.5/src/loqedAPI/loqed.py
-drwxr-xr-x   0 casper     (502) staff       (20)        0 2022-11-28 20:01:52.990076 loqedAPI-2.1.5/src/loqedAPI.egg-info/
--rw-r--r--   0 casper     (502) staff       (20)      944 2022-11-28 20:01:52.000000 loqedAPI-2.1.5/src/loqedAPI.egg-info/PKG-INFO
--rw-r--r--   0 casper     (502) staff       (20)      358 2022-11-28 20:01:52.000000 loqedAPI-2.1.5/src/loqedAPI.egg-info/SOURCES.txt
--rw-r--r--   0 casper     (502) staff       (20)        1 2022-11-28 20:01:52.000000 loqedAPI-2.1.5/src/loqedAPI.egg-info/dependency_links.txt
--rw-r--r--   0 casper     (502) staff       (20)       22 2022-11-28 20:01:52.000000 loqedAPI-2.1.5/src/loqedAPI.egg-info/requires.txt
--rw-r--r--   0 casper     (502) staff       (20)        9 2022-11-28 20:01:52.000000 loqedAPI-2.1.5/src/loqedAPI.egg-info/top_level.txt
+drwxr-xr-x   0 mwoudenberg   (502) staff       (20)        0 2023-06-14 17:37:01.562162 loqedAPI-2.1.6/
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)     1314 2022-06-12 08:10:07.000000 loqedAPI-2.1.6/LICENSE
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      927 2023-06-14 17:37:01.562258 loqedAPI-2.1.6/PKG-INFO
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)       40 2022-06-12 08:10:07.000000 loqedAPI-2.1.6/README.md
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      103 2022-06-12 08:10:07.000000 loqedAPI-2.1.6/pyproject.toml
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      695 2023-06-14 17:37:01.562774 loqedAPI-2.1.6/setup.cfg
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      952 2023-06-14 17:36:29.000000 loqedAPI-2.1.6/setup.py
+drwxr-xr-x   0 mwoudenberg   (502) staff       (20)        0 2023-06-14 17:37:01.558762 loqedAPI-2.1.6/src/
+drwxr-xr-x   0 mwoudenberg   (502) staff       (20)        0 2023-06-14 17:37:01.560737 loqedAPI-2.1.6/src/loqedAPI/
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      151 2022-06-12 08:10:07.000000 loqedAPI-2.1.6/src/loqedAPI/__init__.py
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      173 2022-06-12 08:10:07.000000 loqedAPI-2.1.6/src/loqedAPI/apiclient.py
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      225 2022-06-12 08:10:07.000000 loqedAPI-2.1.6/src/loqedAPI/exceptions.py
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)     6539 2022-06-12 08:10:07.000000 loqedAPI-2.1.6/src/loqedAPI/local_loqed.py
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)    11295 2023-06-14 15:21:58.000000 loqedAPI-2.1.6/src/loqedAPI/loqed.py
+drwxr-xr-x   0 mwoudenberg   (502) staff       (20)        0 2023-06-14 17:37:01.561700 loqedAPI-2.1.6/src/loqedAPI.egg-info/
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      927 2023-06-14 17:37:01.000000 loqedAPI-2.1.6/src/loqedAPI.egg-info/PKG-INFO
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)      372 2023-06-14 17:37:01.000000 loqedAPI-2.1.6/src/loqedAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)        1 2023-06-14 17:37:01.000000 loqedAPI-2.1.6/src/loqedAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)       22 2023-06-14 17:37:01.000000 loqedAPI-2.1.6/src/loqedAPI.egg-info/requires.txt
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)        9 2023-06-14 17:37:01.000000 loqedAPI-2.1.6/src/loqedAPI.egg-info/top_level.txt
+drwxr-xr-x   0 mwoudenberg   (502) staff       (20)        0 2023-06-14 17:37:01.561831 loqedAPI-2.1.6/tests/
+-rw-r--r--   0 mwoudenberg   (502) staff       (20)     1177 2022-06-12 08:10:07.000000 loqedAPI-2.1.6/tests/test.py
```

### Comparing `loqedAPI-2.1.5/LICENSE` & `loqedAPI-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `loqedAPI-2.1.5/PKG-INFO` & `loqedAPI-2.1.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: loqedAPI
-Version: 2.1.5
+Version: 2.1.6
 Summary: Python package to use the Loqed Smart Door Lock APIs in a local network. To be used by Home Assistant.
 Home-page: https://github.com/cpolhout/loqedAPI
 Author: Casper Polhout
 Author-email: cpolhout@gmail.com
 License: BSD 2-clause
 Project-URL: Bug Tracker, https://github.com/cpolhout/loqedAPI/issues
-Description: # Loqed Touch Smart Lock Python library
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Loqed Touch Smart Lock Python library
```

### Comparing `loqedAPI-2.1.5/setup.cfg` & `loqedAPI-2.1.6/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = loqedAPI
-version = 2.1.5
+version = 2.1.6
 author = Casper Polhout
 author_email = cpolhout@gmail.com
 description = Python package to use the Loqed Smart Door Lock APIs in a local network. To be used by Home Assistant.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cpolhout/loqedAPI
 project_urls =
```

### Comparing `loqedAPI-2.1.5/setup.py` & `loqedAPI-2.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='loqedAPI',
-    version='2.1.5',    
+    version='2.1.6',    
     description='Python package to use the Loqed Smart Door Lock APIs in a local network. To be used by Home Assistant.',
     url='https://github.com/cpolhout/loqedAPI',
     author='Casper Polhout',
     author_email='cpolhout@gmail.com',    
     license='BSD 2-clause',
     packages=find_packages(exclude=["tests", "generator"]),
     install_requires=["aiohttp", "async-timeout"],
```

### Comparing `loqedAPI-2.1.5/src/loqedAPI/local_loqed.py` & `loqedAPI-2.1.6/src/loqedAPI/local_loqed.py`

 * *Files identical despite different names*

### Comparing `loqedAPI-2.1.5/src/loqedAPI/loqed.py` & `loqedAPI-2.1.6/src/loqedAPI/loqed.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,30 +26,41 @@
     OPEN = 1
     UNLOCK = 2
     LOCK = 3
 
 class AbstractAPIClient():
     """Client to handle API calls."""
 
-    def __init__(self, websession: ClientSession, host: str):
+    def __init__(self, websession: ClientSession, host: str, token: str | None = None):
         """Initialize the client."""
         self.websession = websession
         self.host = host
+        self.token = token
         _LOGGER.debug("API client created")
 
     async def request(self, method, url, **kwargs) -> ClientResponse:
         """Make a request."""
+        headers = kwargs.get("headers")
+
+        if headers is None:
+            headers = {}
+        else:
+            headers = dict(headers)
+
+        if self.token:
+            headers["authorization"] = f"Bearer {self.token}"
+
         return await self.websession.request(
-            method, f"{self.host}/{url}", **kwargs,
+            method, f"{self.host}/{url}", **kwargs, headers=headers,
         )
 
 class APIClient(AbstractAPIClient):
-    def __init__(self, websession: ClientSession, host: str):
+    def __init__(self, websession: ClientSession, host: str, token: str | None = None):
         """Initialize the auth."""
-        super().__init__(websession, host)
+        super().__init__(websession, host, token)
 
 
 class Lock:
     """Class that represents a Lock object in the LoqedAPI."""
 
     def __init__(self, raw_data: dict, secret: str, bridgekey: str, key_id: int, name: str, apiclient: APIClient):
         """Initialize a lock object."""
@@ -247,16 +258,22 @@
     async def async_get_lock(self, secret: str, bridgekey: str, key_id: int, name: str, json_data=None) -> Lock:
         """Return the locks with lock-data"""
         if not json_data:
             resp = await self.apiclient.request("get", "status")
             json_data = await resp.json(content_type='text/html')
         return Lock(json_data, secret, bridgekey,  key_id, name, self.apiclient)
 
+class LoqedCloudAPI:
+    def __init__(self, apiclient: APIClient):
+        self.apiclient = apiclient
 
-
+    async def async_get_locks(self):
+        resp = await self.apiclient.request("get", "/api/locks/")
+        resp.raise_for_status()
+        return await resp.json()
    
 """Loqed: Exceptions"""
 
 
 class LoqedException(BaseException):
     """Raise this when something is off."""
```

### Comparing `loqedAPI-2.1.5/src/loqedAPI.egg-info/PKG-INFO` & `loqedAPI-2.1.6/src/loqedAPI.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: loqedAPI
-Version: 2.1.5
+Version: 2.1.6
 Summary: Python package to use the Loqed Smart Door Lock APIs in a local network. To be used by Home Assistant.
 Home-page: https://github.com/cpolhout/loqedAPI
 Author: Casper Polhout
 Author-email: cpolhout@gmail.com
 License: BSD 2-clause
 Project-URL: Bug Tracker, https://github.com/cpolhout/loqedAPI/issues
-Description: # Loqed Touch Smart Lock Python library
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Loqed Touch Smart Lock Python library
```

