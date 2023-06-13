# Comparing `tmp/BlizzardWarcraftAPI-0.0.1.tar.gz` & `tmp/BlizzardWarcraftAPI-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlizzardWarcraftAPI-0.0.1.tar", last modified: Mon Jun 12 22:37:43 2023, max compression
+gzip compressed data, was "BlizzardWarcraftAPI-0.1.0.tar", last modified: Tue Jun 13 22:22:03 2023, max compression
```

## Comparing `BlizzardWarcraftAPI-0.0.1.tar` & `BlizzardWarcraftAPI-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:37:43.241116 BlizzardWarcraftAPI-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:37:43.237116 BlizzardWarcraftAPI-0.0.1/BlizzardWarcraftAPI/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-12 22:37:13.000000 BlizzardWarcraftAPI-0.0.1/BlizzardWarcraftAPI/BlizzardAuthToken.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-12 22:37:13.000000 BlizzardWarcraftAPI-0.0.1/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-12 22:37:13.000000 BlizzardWarcraftAPI-0.0.1/BlizzardWarcraftAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-12 22:37:13.000000 BlizzardWarcraftAPI-0.0.1/BlizzardWarcraftAPI/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-12 22:37:13.000000 BlizzardWarcraftAPI-0.0.1/BlizzardWarcraftAPI/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-12 22:37:13.000000 BlizzardWarcraftAPI-0.0.1/BlizzardWarcraftAPI/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:37:43.241116 BlizzardWarcraftAPI-0.0.1/BlizzardWarcraftAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-12 22:37:43.000000 BlizzardWarcraftAPI-0.0.1/BlizzardWarcraftAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-12 22:37:43.000000 BlizzardWarcraftAPI-0.0.1/BlizzardWarcraftAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 22:37:43.000000 BlizzardWarcraftAPI-0.0.1/BlizzardWarcraftAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 22:37:43.000000 BlizzardWarcraftAPI-0.0.1/BlizzardWarcraftAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 22:37:43.000000 BlizzardWarcraftAPI-0.0.1/BlizzardWarcraftAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-12 22:37:13.000000 BlizzardWarcraftAPI-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-12 22:37:43.241116 BlizzardWarcraftAPI-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-12 22:37:13.000000 BlizzardWarcraftAPI-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-12 22:37:13.000000 BlizzardWarcraftAPI-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 22:37:43.241116 BlizzardWarcraftAPI-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:03.308914 BlizzardWarcraftAPI-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:03.304914 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/BlizzardAuthToken.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:03.308914 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/modules/AchievementAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:03.308914 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-13 22:22:03.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-13 22:22:03.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 22:22:03.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 22:22:03.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 22:22:03.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-13 22:22:03.308914 BlizzardWarcraftAPI-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 22:22:03.308914 BlizzardWarcraftAPI-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:03.308914 BlizzardWarcraftAPI-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/tests/test_base.py
```

### Comparing `BlizzardWarcraftAPI-0.0.1/BlizzardWarcraftAPI/BlizzardAuthToken.py` & `BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/BlizzardAuthToken.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import requests
 from .urls import URL_ACCESS_TOKEN_REQUEST
 from .exceptions import BlizzardAuthTokenError
 
 
-class BlizzardAuthToken:
+class BlizzardAuthToken():
     def __init__(self, ClientID: str, ClientSecret: str):
+        """
+        Get from https://develop.battle.net/access/clients
+
+        :param str ClientID:
+        :param str ClientSecret:
+        """
         self.grant_type: str = "client_credentials"
         self.ClientID: str = ClientID
         self.ClientSecret: str = ClientSecret
 
     def get(self):
         data = {
             "grant_type": self.grant_type,
```

### Comparing `BlizzardWarcraftAPI-0.0.1/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py` & `BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
-from requests.models import Response
-from .data import region_data, locales_region_data
-from .exceptions import BlizzardWarcraftApiError
-from .urls import URL_TOKEN_VALIDATION
+from ..data import region_data, locales_region_data
+from ..exceptions import BlizzardWarcraftApiError
+from ..urls import URL_TOKEN_VALIDATION
 
 
-class BlizzardWarcraftAPI:
+class BlizzardWarcraftAPI():
+
     @staticmethod
     def __valid_region(region):
         if region in region_data:
             return True
         else:
             text = f"Region must be: {region_data}"
             raise BlizzardWarcraftApiError(text)
@@ -34,20 +34,22 @@
 
         if "error" not in response_data:
             return True
         else:
             text = response_data["error"] + " - " + response_data["error_description"]
             raise BlizzardWarcraftApiError(text)
 
-    def __init__(self, BlizzardAuthToken, region: str, locale: str = "en_GB"):
+    def __init__(self, BlizzardAuthToken, region: str, locale: str):
 
         if self.__valid_BlizzardAuthToken(BlizzardAuthToken):
             self.BlizzardAuthToken = BlizzardAuthToken
 
         region = region.lower()
         if self.__valid_region(region):
             self.region = region
 
         if self.__valid_locale(self.region, locale):
             self.locale = locale
 
-        self.namespace = "profile-" + self.region
+        self.namespace_profile = "profile-" + self.region
+        self.namespace_static = "static-" + self.region
+        self.namespace_dynamic = "dynamic-" + self.region
```

### Comparing `BlizzardWarcraftAPI-0.0.1/BlizzardWarcraftAPI/data.py` & `BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/data.py`

 * *Files identical despite different names*

### Comparing `BlizzardWarcraftAPI-0.0.1/LICENSE` & `BlizzardWarcraftAPI-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BlizzardWarcraftAPI-0.0.1/pyproject.toml` & `BlizzardWarcraftAPI-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "BlizzardWarcraftAPI"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
     {name = "Angeloffy", email = "angeloffy.work@gmail.com"},
 ]
 description = "Warcraft API"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

