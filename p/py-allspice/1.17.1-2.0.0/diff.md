# Comparing `tmp/py-allspice-1.17.1.tar.gz` & `tmp/py-allspice-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-allspice-1.17.1.tar", last modified: Sat Feb 18 23:01:39 2023, max compression
+gzip compressed data, was "py-allspice-2.0.0.tar", last modified: Wed Jun 14 18:06:34 2023, max compression
```

## Comparing `py-allspice-1.17.1.tar` & `py-allspice-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:01:39.083294 py-allspice-1.17.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-18 23:01:29.000000 py-allspice-1.17.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-02-18 23:01:39.083294 py-allspice-1.17.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-02-18 23:01:29.000000 py-allspice-1.17.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:01:39.083294 py-allspice-1.17.1/gitea/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-02-18 23:01:29.000000 py-allspice-1.17.1/gitea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31615 2023-02-18 23:01:29.000000 py-allspice-1.17.1/gitea/apiobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-02-18 23:01:29.000000 py-allspice-1.17.1/gitea/baseapiobject.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-02-18 23:01:29.000000 py-allspice-1.17.1/gitea/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-02-18 23:01:29.000000 py-allspice-1.17.1/gitea/gitea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:01:39.083294 py-allspice-1.17.1/py_allspice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-02-18 23:01:39.000000 py-allspice-1.17.1/py_allspice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-02-18 23:01:39.000000 py-allspice-1.17.1/py_allspice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-18 23:01:39.000000 py-allspice-1.17.1/py_allspice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-18 23:01:39.000000 py-allspice-1.17.1/py_allspice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-18 23:01:39.000000 py-allspice-1.17.1/py_allspice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-18 23:01:39.083294 py-allspice-1.17.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-02-18 23:01:32.000000 py-allspice-1.17.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:01:39.083294 py-allspice-1.17.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    14372 2023-02-18 23:01:29.000000 py-allspice-1.17.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-02-18 23:01:29.000000 py-allspice-1.17.1/tests/test_api_longtests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:06:34.782864 py-allspice-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-14 18:06:20.000000 py-allspice-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-14 18:06:34.782864 py-allspice-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-14 18:06:20.000000 py-allspice-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:06:34.782864 py-allspice-2.0.0/allspice/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-14 18:06:20.000000 py-allspice-2.0.0/allspice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-06-14 18:06:20.000000 py-allspice-2.0.0/allspice/allspice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36903 2023-06-14 18:06:20.000000 py-allspice-2.0.0/allspice/apiobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-14 18:06:20.000000 py-allspice-2.0.0/allspice/baseapiobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-14 18:06:20.000000 py-allspice-2.0.0/allspice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-14 18:06:20.000000 py-allspice-2.0.0/allspice/ratelimiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:06:34.782864 py-allspice-2.0.0/py_allspice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-14 18:06:34.000000 py-allspice-2.0.0/py_allspice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-14 18:06:34.000000 py-allspice-2.0.0/py_allspice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 18:06:34.000000 py-allspice-2.0.0/py_allspice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 18:06:34.000000 py-allspice-2.0.0/py_allspice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 18:06:34.000000 py-allspice-2.0.0/py_allspice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 18:06:34.782864 py-allspice-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-14 18:06:26.000000 py-allspice-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:06:34.782864 py-allspice-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-06-14 18:06:20.000000 py-allspice-2.0.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-14 18:06:20.000000 py-allspice-2.0.0/tests/test_api_longtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-14 18:06:20.000000 py-allspice-2.0.0/tests/test_api_ratelimiting.py
```

### Comparing `py-allspice-1.17.1/LICENSE` & `py-allspice-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-allspice-1.17.1/PKG-INFO` & `py-allspice-2.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,95 +1,99 @@
-Metadata-Version: 2.1
-Name: py-allspice
-Version: 1.17.1
-Summary: A python wrapper for the AllSpice Hub API
-Home-page: https://github.com/Langenfeld/py-gitea
-Download-URL: https://github.com/AllSpiceIO/py-allspice
-Author: AllSpice, Inc.
-Author-email: maintainers@allspice.io
-License: MIT
-Keywords: AllSpice,AllSpice Hub,api,wrapper
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # py-allspice
 
 A very simple API client for AllSpice Hub
 
-Note that not the full Swagger-API is accessible. The whole implementation is focused 
+Note that not the full Swagger-API is accessible. The whole implementation is focused
 on making access and working with Organizations, Teams, Repositories and Users as pain
 free as possible.
 
 Forked from https://github.com/Langenfeld/py-gitea.
 
 ## Usage
 
-First get an `allspice` object wrapping access and authentication (via an api token) for your gitea instance:
+### Examples
+
+Check the [examples directory](./examples/) for full, working example scripts
+that you can adapt or refer to for your own needs.
+
+### Quickstart
+
+First get an `allspice_client` object wrapping access and authentication (via an api token) for your instance of AllSpice Hub.
 
 ```python
-from gitea import *
+from allspice import *
 
-allspice = Gitea(URL, TOKEN)
+# By default, points to hub.allspice.io.
+allspice_client = AllSpice(token_text=TOKEN)
+
+# If you are self-hosting:
+allspice_client = AllSpice(allspice_hub_url=URL, token_text=TOKEN)
 ```
 
-Operations like requesting the Allspice version or authentication user can be requested directly from the `allspice` object:
+Operations like requesting the AllSpice version or authentication user can be requested directly from the `allspice_client` object:
 
 ```python
-print("AllSpice Version: " + allspice.get_version())
-print("API-Token belongs to user: " + allspice.get_user().username)
+print("AllSpice Version: " + allspice_client.get_version())
+print("API-Token belongs to user: " + allspice_client.get_user().username)
 ```
 
-Adding entities like Users, Organizations, ...  also is done via the allspice object.
+Adding entities like Users, Organizations, ...  also is done via the allspice_client object.
 
 ```python
-user = allspice.create_user("Test Testson", "test@test.test", "password")
+user = allspice_client.create_user("Test Testson", "test@test.test", "password")
 ```
 
 All operations on entities in allspice are then accomplished via the according wrapper objects for those entities.
-Each of those objects has a `.request` method that creates an entity according to your allspice instance. 
+Each of those objects has a `.request` method that creates an entity according to your allspice_client instance.
 
 ```python
-other_user = User.request(allspice, "OtherUserName")
+other_user = User.request(allspice_client, "OtherUserName")
 print(other_user.username)
 ```
 
-Note that the fields of the User, Organization,... classes are dynamically created at runtime, and thus not visible during divelopment. Refer to the AllSpice-API documentation for the fields names. 
+Note that the fields of the User, Organization,... classes are dynamically created at runtime, and thus not visible during divelopment. Refer to the AllSpice API documentation for the fields names.
 
 
-Fields that can not be altered via allspice-api, are read only. After altering a field, the `.commit` method of the according object must be called to synchronize the changed fields with your allspice instance.
+Fields that can not be altered via allspice-api, are read only. After altering a field, the `.commit` method of the according object must be called to synchronize the changed fields with your allspice_client instance.
 
 ```python
-org = Organization.request(allspice, test_org)
+org = Organization.request(allspice_client, test_org)
 org.description = "some new description"
 org.location = "some new location"
 org.commit()
 ```
 
 An entity in allspice can be deleted by calling delete.
 ```python
 org.delete()
 ```
 
-All entity objects do have methods to execute some of the requests possible though the allspice-api:
+All entity objects do have methods to execute some of the requests possible though the AllSpice api:
 ```python
-org = Organization.request(allspice, ORGNAME)
+org = Organization.request(allspice_client, ORGNAME)
 teams = org.get_teams()
 for team in teams:
 	repos = team.get_repos()
 	for repo in repos:
 		print(repo.name)
 ```
 
 
 ## Installation
 
 Use ``pip install py-allspice`` to install.
 
+## A Note on Versioning
+
+This repository does not follow the same versioning policy as py-gitea. After v1.17.x,
+py-allspice switched to Semantic Versioning with v2.0.0. In general, versions of
+py-allspice do NOT conform to versions of AllSpice Hub, and the latest version of
+py-allspice should be compatible with the current version of AllSpice Hub.
+
 ## Tests
 
-Tests can be run with: 
+Tests can be run with:
 
 ```python3 -m pytest test_api.py```
 
-Make sure to have a allspice-instance running on `http://localhost:3000`, and an admin-user token at `.token`. 
+Make sure to have an instance of AllSpice Hub running on `http://localhost:3000`, and an admin-user token at `.token`.
 The admin user must be named ``test``, with email ``secondarytest@test.org``.
```

### Comparing `py-allspice-1.17.1/README.md` & `py-allspice-2.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,113 @@
+Metadata-Version: 2.1
+Name: py-allspice
+Version: 2.0.0
+Summary: A python wrapper for the AllSpice Hub API
+Home-page: https://github.com/Langenfeld/py-gitea
+Download-URL: https://github.com/AllSpiceIO/py-allspice
+Author: AllSpice, Inc.
+Author-email: maintainers@allspice.io
+License: MIT
+Keywords: AllSpice,AllSpice Hub,api,wrapper
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # py-allspice
 
 A very simple API client for AllSpice Hub
 
-Note that not the full Swagger-API is accessible. The whole implementation is focused 
+Note that not the full Swagger-API is accessible. The whole implementation is focused
 on making access and working with Organizations, Teams, Repositories and Users as pain
 free as possible.
 
 Forked from https://github.com/Langenfeld/py-gitea.
 
 ## Usage
 
-First get an `allspice` object wrapping access and authentication (via an api token) for your gitea instance:
+### Examples
+
+Check the [examples directory](./examples/) for full, working example scripts
+that you can adapt or refer to for your own needs.
+
+### Quickstart
+
+First get an `allspice_client` object wrapping access and authentication (via an api token) for your instance of AllSpice Hub.
 
 ```python
-from gitea import *
+from allspice import *
 
-allspice = Gitea(URL, TOKEN)
+# By default, points to hub.allspice.io.
+allspice_client = AllSpice(token_text=TOKEN)
+
+# If you are self-hosting:
+allspice_client = AllSpice(allspice_hub_url=URL, token_text=TOKEN)
 ```
 
-Operations like requesting the Allspice version or authentication user can be requested directly from the `allspice` object:
+Operations like requesting the AllSpice version or authentication user can be requested directly from the `allspice_client` object:
 
 ```python
-print("AllSpice Version: " + allspice.get_version())
-print("API-Token belongs to user: " + allspice.get_user().username)
+print("AllSpice Version: " + allspice_client.get_version())
+print("API-Token belongs to user: " + allspice_client.get_user().username)
 ```
 
-Adding entities like Users, Organizations, ...  also is done via the allspice object.
+Adding entities like Users, Organizations, ...  also is done via the allspice_client object.
 
 ```python
-user = allspice.create_user("Test Testson", "test@test.test", "password")
+user = allspice_client.create_user("Test Testson", "test@test.test", "password")
 ```
 
 All operations on entities in allspice are then accomplished via the according wrapper objects for those entities.
-Each of those objects has a `.request` method that creates an entity according to your allspice instance. 
+Each of those objects has a `.request` method that creates an entity according to your allspice_client instance.
 
 ```python
-other_user = User.request(allspice, "OtherUserName")
+other_user = User.request(allspice_client, "OtherUserName")
 print(other_user.username)
 ```
 
-Note that the fields of the User, Organization,... classes are dynamically created at runtime, and thus not visible during divelopment. Refer to the AllSpice-API documentation for the fields names. 
+Note that the fields of the User, Organization,... classes are dynamically created at runtime, and thus not visible during divelopment. Refer to the AllSpice API documentation for the fields names.
 
 
-Fields that can not be altered via allspice-api, are read only. After altering a field, the `.commit` method of the according object must be called to synchronize the changed fields with your allspice instance.
+Fields that can not be altered via allspice-api, are read only. After altering a field, the `.commit` method of the according object must be called to synchronize the changed fields with your allspice_client instance.
 
 ```python
-org = Organization.request(allspice, test_org)
+org = Organization.request(allspice_client, test_org)
 org.description = "some new description"
 org.location = "some new location"
 org.commit()
 ```
 
 An entity in allspice can be deleted by calling delete.
 ```python
 org.delete()
 ```
 
-All entity objects do have methods to execute some of the requests possible though the allspice-api:
+All entity objects do have methods to execute some of the requests possible though the AllSpice api:
 ```python
-org = Organization.request(allspice, ORGNAME)
+org = Organization.request(allspice_client, ORGNAME)
 teams = org.get_teams()
 for team in teams:
 	repos = team.get_repos()
 	for repo in repos:
 		print(repo.name)
 ```
 
 
 ## Installation
 
 Use ``pip install py-allspice`` to install.
 
+## A Note on Versioning
+
+This repository does not follow the same versioning policy as py-gitea. After v1.17.x,
+py-allspice switched to Semantic Versioning with v2.0.0. In general, versions of
+py-allspice do NOT conform to versions of AllSpice Hub, and the latest version of
+py-allspice should be compatible with the current version of AllSpice Hub.
+
 ## Tests
 
-Tests can be run with: 
+Tests can be run with:
 
 ```python3 -m pytest test_api.py```
 
-Make sure to have a allspice-instance running on `http://localhost:3000`, and an admin-user token at `.token`. 
+Make sure to have an instance of AllSpice Hub running on `http://localhost:3000`, and an admin-user token at `.token`.
 The admin user must be named ``test``, with email ``secondarytest@test.org``.
```

### Comparing `py-allspice-1.17.1/gitea/__init__.py` & `py-allspice-2.0.0/allspice/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .gitea import (
-    Gitea,
+from .allspice import (
+    AllSpice,
     NotFoundException,
     AlreadyExistsException,
 )
 from .apiobject import (
     User,
     Organization,
     Team,
@@ -15,15 +15,15 @@
     Milestone,
     Commit,
     Comment,
     Content
 )
 
 __all__ = [
-    'Gitea',
+    'AllSpice',
     'User',
     'Organization',
     'Team',
     'Repository',
     'Branch',
     'NotFoundException',
     'AlreadyExistsException',
```

### Comparing `py-allspice-1.17.1/gitea/baseapiobject.py` & `py-allspice-2.0.0/allspice/baseapiobject.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-from .exceptions import ObjectIsInvalid, MissiongEqualyImplementation, RawRequestEndpointMissing
+from .exceptions import ObjectIsInvalid, MissingEqualityImplementation, RawRequestEndpointMissing
 
 
 class ReadonlyApiObject:
 
-    def __init__(self, gitea):
-        self.gitea = gitea
+    def __init__(self, allspice_client):
+        self.allspice_client = allspice_client
         self.deleted = False  # set if .delete was called, so that an exception is risen
 
     def __str__(self):
-        return "GiteaAPIObject (%s):" % (type(self))
+        return "AllSpiceObject (%s):" % (type(self))
 
     def __eq__(self, other):
         """Compare only fields that are part of the gitea-data identity"""
-        raise MissiongEqualyImplementation()
+        raise MissingEqualityImplementation()
 
     def __hash__(self):
         """Hash only fields that are part of the gitea-data identity"""
-        raise MissiongEqualyImplementation()
+        raise MissingEqualityImplementation()
 
     _fields_to_parsers = {}
 
     @classmethod
-    def request(cls, gitea):
+    def request(cls, allspice_client):
         if hasattr("API_OBJECT", cls):
-            return cls._request(gitea)
+            return cls._request(allspice_client)
         else:
             raise RawRequestEndpointMissing()
 
     @classmethod
-    def _request(cls, gitea, args):
-        result = cls._get_gitea_api_object(gitea, args)
-        api_object = cls.parse_response(gitea, result)
+    def _request(cls, allspice_client, args):
+        result = cls._get_gitea_api_object(allspice_client, args)
+        api_object = cls.parse_response(allspice_client, result)
         return api_object
 
     @classmethod
-    def _get_gitea_api_object(cls, gitea, args):
+    def _get_gitea_api_object(cls, allspice_client, args):
         """Retrieving an object always as GET_API_OBJECT """
-        return gitea.requests_get(cls.API_OBJECT.format(**args))
+        return allspice_client.requests_get(cls.API_OBJECT.format(**args))
 
     @classmethod
-    def parse_response(cls, gitea, result) -> "ReadonlyApiObject":
-        # gitea.logger.debug("Found api object of type %s (id: %s)" % (type(cls), id))
-        api_object = cls(gitea)
-        cls._initialize(gitea, api_object, result)
+    def parse_response(cls, allspice_client, result) -> "ReadonlyApiObject":
+        # allspice_client.logger.debug("Found api object of type %s (id: %s)" % (type(cls), id))
+        api_object = cls(allspice_client)
+        cls._initialize(allspice_client, api_object, result)
         return api_object
 
     @classmethod
-    def _initialize(cls, gitea, api_object, result):
+    def _initialize(cls, allspice_client, api_object, result):
         for name, value in result.items():
             if name in cls._fields_to_parsers and value is not None:
                 parse_func = cls._fields_to_parsers[name]
-                value = parse_func(gitea, value)
+                value = parse_func(allspice_client, value)
             cls._add_read_property(name, value, api_object)
         # add all patchable fields missing in the request to be writable
         for name in cls._fields_to_parsers.keys():
             if not hasattr(api_object, name):
                 cls._add_read_property(name, None, api_object)
 
     @classmethod
@@ -72,16 +72,16 @@
             raise ObjectIsInvalid()
         return getattr(self, "_" + name)
 
 
 class ApiObject(ReadonlyApiObject):
     _patchable_fields = set()
 
-    def __init__(self, gitea):
-        super().__init__(gitea)
+    def __init__(self, allspice_client):
+        super().__init__(allspice_client)
         self._dirty_fields = set()
 
     def commit(self):
         raise NotImplemented()
 
     _parsers_to_fields = {}
 
@@ -92,16 +92,16 @@
             if field in self._parsers_to_fields:
                 dirty_fields_values[field] = self._parsers_to_fields[field](value)
             else:
                 dirty_fields_values[field] = value
         return dirty_fields_values
 
     @classmethod
-    def _initialize(cls, gitea, api_object, result):
-        super()._initialize(gitea, api_object, result)
+    def _initialize(cls, allspice_client, api_object, result):
+        super()._initialize(allspice_client, api_object, result)
         for name in cls._patchable_fields:
             cls._add_write_property(name, None, api_object)
 
     @classmethod
     def _add_write_property(cls, name, value, api_object):
         if not hasattr(api_object, "_" + name):
             setattr(api_object, "_" + name, value)
```

### Comparing `py-allspice-1.17.1/gitea/gitea.py` & `py-allspice-2.0.0/allspice/allspice.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,96 +3,129 @@
 from typing import List, Dict, Union
 
 from frozendict import frozendict
 import requests
 import urllib3
 
 from .apiobject import User, Organization, Repository, Team
-from .exceptions import NotFoundException, ConflictException, AlreadyExistsException
+from .exceptions import NotFoundException, ConflictException, AlreadyExistsException, NotYetGeneratedException
+from .ratelimiter import RateLimitedSession
 
 
-class Gitea:
-    """ Object to establish a session with Gitea. """
+class AllSpice:
+    """Object to establish a session with AllSpice Hub."""
+
     ADMIN_CREATE_USER = """/admin/users"""
     GET_USERS_ADMIN = """/admin/users"""
     ADMIN_REPO_CREATE = """/admin/users/%s/repos"""  # <ownername>
-    GITEA_VERSION = """/version"""
+    ALLSPICE_HUB_VERSION = """/version"""
     GET_USER = """/user"""
+    GET_REPOSITORY = """/repos/{owner}/{name}"""
     CREATE_ORG = """/admin/users/%s/orgs"""  # <username>
     CREATE_TEAM = """/orgs/%s/teams"""  # <orgname>
 
     def __init__(
-            self,
-            gitea_url: str,
-            token_text=None,
-            auth=None,
-            verify=True,
-            log_level="INFO"
-        ):
-        """ Initializing Gitea-instance
+        self,
+        allspice_hub_url="https://hub.allspice.io",
+        token_text=None,
+        auth=None,
+        verify=True,
+        log_level="INFO",
+        ratelimiting=(100, 60),
+    ):
+        """Initializing an instance of the AllSpice Hub Client
 
         Args:
-            gitea_url (str): The Gitea instance URL.
+            allspice_hub_url (str): The URL for the AllSpice Hub instance.
+                Defaults to `https://hub.allspice.io`.
+
             token_text (str, None): The access token, by default None.
+
             auth (tuple, None): The user credentials
                 `(username, password)`, by default None.
+
             verify (bool): If True, allow insecure server connections
                 when using SSL.
+
             log_level (str): The log level, by default `INFO`.
+
+            ratelimiting (tuple[int, int], None): `(max_calls, period)`,
+                If None, no rate limiting is applied. By default, 100 calls
+                per minute are allowed.
         """
+
         self.logger = logging.getLogger(__name__)
         self.logger.setLevel(log_level)
         self.headers = {
             "Content-type": "application/json",
         }
-        self.url = gitea_url
-        self.requests = requests.Session()
+        self.url = allspice_hub_url
+
+        if ratelimiting is None:
+            self.requests = requests.Session()
+        else:
+            (max_calls, period) = ratelimiting
+            self.requests = RateLimitedSession(max_calls=max_calls, period=period)
 
         # Manage authentification
         if not token_text and not auth:
             raise ValueError("Please provide auth or token_text, but not both")
         if token_text:
             self.headers["Authorization"] = "token " + token_text
         if auth:
+            self.logger.warning("Using basic auth is not recommended. Prefer using a token instead.")
             self.requests.auth = auth
 
         # Manage SSL certification verification
         self.requests.verify = verify
         if not verify:
             urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
     def __get_url(self, endpoint):
         url = self.url + "/api/v1" + endpoint
         self.logger.debug("Url: %s" % url)
         return url
 
+    def __get(self, endpoint: str, params=frozendict()) -> requests.Response:
+        request = self.requests.get(self.__get_url(endpoint), headers=self.headers, params=params)
+        if request.status_code not in [200, 201]:
+            message = f"Received status code: {request.status_code} ({request.url})"
+            if request.status_code in [404]:
+                raise NotFoundException(message)
+            if request.status_code in [403]:
+                raise Exception(f"Unauthorized: {request.url} - Check your permissions and try again! ({message})")
+            if request.status_code in [409]:
+                raise ConflictException(message)
+            if request.status_code in [503]:
+                raise NotYetGeneratedException(message)
+            raise Exception(message)
+        return request
+
     @staticmethod
     def parse_result(result) -> Dict:
         """ Parses the result-JSON to a dict. """
         if result.text and len(result.text) > 3:
             return json.loads(result.text)
         return {}
 
+
     def requests_get(self, endpoint: str, params=frozendict(), sudo=None):
         combined_params = {}
         combined_params.update(params)
         if sudo:
             combined_params["sudo"] = sudo.username
-        request = self.requests.get(self.__get_url(endpoint), headers=self.headers, params=combined_params)
-        if request.status_code not in [200, 201]:
-            message = f"Received status code: {request.status_code} ({request.url})"
-            if request.status_code in [404]:
-                raise NotFoundException(message)
-            if request.status_code in [403]:
-                raise Exception(f"Unauthorized: {request.url} - Check your permissions and try again! ({message})")
-            if request.status_code in [409]:
-                raise ConflictException(message)
-            raise Exception(message)
-        return self.parse_result(request)
+        return self.parse_result(self.__get(endpoint, combined_params))
+
+    def requests_get_raw(self, endpoint: str, params=frozendict(), sudo=None) -> bytes:
+        combined_params = {}
+        combined_params.update(params)
+        if sudo:
+            combined_params["sudo"] = sudo.username
+        return self.__get(endpoint, combined_params).content
 
     def requests_get_paginated(self, endpoint: str, params=frozendict(), sudo=None, page_key: str = "page"):
         page = 1
         combined_params = {}
         combined_params.update(params)
         aggregated_result = []
         while True:
@@ -145,23 +178,23 @@
 
     def get_orgs(self):
         path = "/admin/orgs"
         results = self.requests_get(path)
         return [Organization.parse_response(self, result) for result in results]
 
     def get_user(self):
-        result = self.requests_get(Gitea.GET_USER)
+        result = self.requests_get(AllSpice.GET_USER)
         return User.parse_response(self, result)
 
     def get_version(self) -> str:
-        result = self.requests_get(Gitea.GITEA_VERSION)
+        result = self.requests_get(AllSpice.ALLSPICE_HUB_VERSION)
         return result["version"]
 
     def get_users(self) -> List[User]:
-        results = self.requests_get(Gitea.GET_USERS_ADMIN)
+        results = self.requests_get(AllSpice.GET_USERS_ADMIN)
         return [User.parse_response(self, result) for result in results]
 
     def get_user_by_email(self, email: str) -> User:
         users = self.get_users()
         for user in users:
             if user.email == email or email in user.emails:
                 return user
@@ -170,14 +203,19 @@
     def get_user_by_name(self, username: str) -> User:
         users = self.get_users()
         for user in users:
             if user.username == username:
                 return user
         return None
 
+    def get_repository(self, owner: str, name: str) -> Repository:
+        path = self.GET_REPOSITORY.format(owner=owner, name=name)
+        result = self.requests_get(path)
+        return Repository.parse_response(self, result)
+
     def create_user(
             self,
             user_name: str,
             email: str,
             password: str,
             full_name: str = None,
             login_name: str = None,
@@ -202,15 +240,15 @@
             "email": email,
             "password": password,
             "send_notify": send_notify,
             "must_change_password": change_pw,
         }
 
         self.logger.debug("Gitea post payload: %s", request_data)
-        result = self.requests_post(Gitea.ADMIN_CREATE_USER, data=request_data)
+        result = self.requests_post(AllSpice.ADMIN_CREATE_USER, data=request_data)
         if "id" in result:
             self.logger.info(
                 "Successfully created User %s <%s> (id %s)",
                 result["login"],
                 result["email"],
                 result["id"],
             )
@@ -238,21 +276,21 @@
 
         Throws:
             AlreadyExistsException: If the Repository exists already.
             Exception: If something else went wrong.
 
         Note:
             Non-admin users can not use this method. Please use instead
-            `gitea.User.create_repo` or `gitea.Organization.create_repo`.
+            `allspice.User.create_repo` or `allspice.Organization.create_repo`.
         """
         # although this only says user in the api, this also works for
         # organizations
         assert isinstance(repoOwner, User) or isinstance(repoOwner, Organization)
         result = self.requests_post(
-            Gitea.ADMIN_REPO_CREATE % repoOwner.username,
+            AllSpice.ADMIN_REPO_CREATE % repoOwner.username,
             data={
                 "name": repoName,
                 "description": description,
                 "private": private,
                 "auto_init": autoInit,
                 "gitignores": gitignores,
                 "license": license,
@@ -275,15 +313,15 @@
             description: str,
             location="",
             website="",
             full_name="",
     ):
         assert isinstance(owner, User)
         result = self.requests_post(
-            Gitea.CREATE_ORG % owner.username,
+            AllSpice.CREATE_ORG % owner.username,
             data={
                 "username": orgName,
                 "description": description,
                 "location": location,
                 "website": website,
                 "full_name": full_name,
             },
@@ -315,34 +353,42 @@
                     "repo.issues",
                     "repo.ext_issues",
                     "repo.wiki",
                     "repo.pulls",
                     "repo.releases",
                     "repo.ext_wiki",
             ),
+            units_map={},
     ):
         """ Creates a Team.
 
         Args:
             org (Organization): Organization the Team will be part of.
             name (str): The Name of the Team to be created.
             description (str): Optional, None, short description of the new Team.
             permission (str): Optional, 'read', What permissions the members
+            units_map (dict): Optional, {}, a mapping of units to their
+                permissions. If None or empty, the `permission` permission will
+                be applied to all units. Note: When both `units` and `units_map`
+                are given, `units_map` will be preferred.
         """
+
         result = self.requests_post(
-            Gitea.CREATE_TEAM % org.username,
+            AllSpice.CREATE_TEAM % org.username,
             data={
                 "name": name,
                 "description": description,
                 "permission": permission,
                 "can_create_org_repo": can_create_org_repo,
                 "includes_all_repositories": includes_all_repositories,
                 "units": units,
+                "units_map": units_map,
             },
         )
+
         if "id" in result:
             self.logger.info("Successfully created Team %s" % result["name"])
         else:
             self.logger.error("Team not created... (gitea: %s)" % result["message"])
             self.logger.error(result["message"])
             raise Exception("Team not created... (gitea: %s)" % result["message"])
         api_object = Team.parse_response(self, result)
```

### Comparing `py-allspice-1.17.1/py_allspice.egg-info/PKG-INFO` & `py-allspice-2.0.0/py_allspice.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-allspice
-Version: 1.17.1
+Version: 2.0.0
 Summary: A python wrapper for the AllSpice Hub API
 Home-page: https://github.com/Langenfeld/py-gitea
 Download-URL: https://github.com/AllSpiceIO/py-allspice
 Author: AllSpice, Inc.
 Author-email: maintainers@allspice.io
 License: MIT
 Keywords: AllSpice,AllSpice Hub,api,wrapper
@@ -12,84 +12,102 @@
 Provides-Extra: test
 License-File: LICENSE
 
 # py-allspice
 
 A very simple API client for AllSpice Hub
 
-Note that not the full Swagger-API is accessible. The whole implementation is focused 
+Note that not the full Swagger-API is accessible. The whole implementation is focused
 on making access and working with Organizations, Teams, Repositories and Users as pain
 free as possible.
 
 Forked from https://github.com/Langenfeld/py-gitea.
 
 ## Usage
 
-First get an `allspice` object wrapping access and authentication (via an api token) for your gitea instance:
+### Examples
+
+Check the [examples directory](./examples/) for full, working example scripts
+that you can adapt or refer to for your own needs.
+
+### Quickstart
+
+First get an `allspice_client` object wrapping access and authentication (via an api token) for your instance of AllSpice Hub.
 
 ```python
-from gitea import *
+from allspice import *
 
-allspice = Gitea(URL, TOKEN)
+# By default, points to hub.allspice.io.
+allspice_client = AllSpice(token_text=TOKEN)
+
+# If you are self-hosting:
+allspice_client = AllSpice(allspice_hub_url=URL, token_text=TOKEN)
 ```
 
-Operations like requesting the Allspice version or authentication user can be requested directly from the `allspice` object:
+Operations like requesting the AllSpice version or authentication user can be requested directly from the `allspice_client` object:
 
 ```python
-print("AllSpice Version: " + allspice.get_version())
-print("API-Token belongs to user: " + allspice.get_user().username)
+print("AllSpice Version: " + allspice_client.get_version())
+print("API-Token belongs to user: " + allspice_client.get_user().username)
 ```
 
-Adding entities like Users, Organizations, ...  also is done via the allspice object.
+Adding entities like Users, Organizations, ...  also is done via the allspice_client object.
 
 ```python
-user = allspice.create_user("Test Testson", "test@test.test", "password")
+user = allspice_client.create_user("Test Testson", "test@test.test", "password")
 ```
 
 All operations on entities in allspice are then accomplished via the according wrapper objects for those entities.
-Each of those objects has a `.request` method that creates an entity according to your allspice instance. 
+Each of those objects has a `.request` method that creates an entity according to your allspice_client instance.
 
 ```python
-other_user = User.request(allspice, "OtherUserName")
+other_user = User.request(allspice_client, "OtherUserName")
 print(other_user.username)
 ```
 
-Note that the fields of the User, Organization,... classes are dynamically created at runtime, and thus not visible during divelopment. Refer to the AllSpice-API documentation for the fields names. 
+Note that the fields of the User, Organization,... classes are dynamically created at runtime, and thus not visible during divelopment. Refer to the AllSpice API documentation for the fields names.
 
 
-Fields that can not be altered via allspice-api, are read only. After altering a field, the `.commit` method of the according object must be called to synchronize the changed fields with your allspice instance.
+Fields that can not be altered via allspice-api, are read only. After altering a field, the `.commit` method of the according object must be called to synchronize the changed fields with your allspice_client instance.
 
 ```python
-org = Organization.request(allspice, test_org)
+org = Organization.request(allspice_client, test_org)
 org.description = "some new description"
 org.location = "some new location"
 org.commit()
 ```
 
 An entity in allspice can be deleted by calling delete.
 ```python
 org.delete()
 ```
 
-All entity objects do have methods to execute some of the requests possible though the allspice-api:
+All entity objects do have methods to execute some of the requests possible though the AllSpice api:
 ```python
-org = Organization.request(allspice, ORGNAME)
+org = Organization.request(allspice_client, ORGNAME)
 teams = org.get_teams()
 for team in teams:
 	repos = team.get_repos()
 	for repo in repos:
 		print(repo.name)
 ```
 
 
 ## Installation
 
 Use ``pip install py-allspice`` to install.
 
+## A Note on Versioning
+
+This repository does not follow the same versioning policy as py-gitea. After v1.17.x,
+py-allspice switched to Semantic Versioning with v2.0.0. In general, versions of
+py-allspice do NOT conform to versions of AllSpice Hub, and the latest version of
+py-allspice should be compatible with the current version of AllSpice Hub.
+
 ## Tests
 
-Tests can be run with: 
+Tests can be run with:
 
 ```python3 -m pytest test_api.py```
 
-Make sure to have a allspice-instance running on `http://localhost:3000`, and an admin-user token at `.token`. 
+Make sure to have an instance of AllSpice Hub running on `http://localhost:3000`, and an admin-user token at `.token`.
 The admin user must be named ``test``, with email ``secondarytest@test.org``.
```

### Comparing `py-allspice-1.17.1/setup.py` & `py-allspice-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='py-allspice',
-    version='1.17.1',
+    version='2.0.0',
     description='A python wrapper for the AllSpice Hub API',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='AllSpice, Inc.',
     author_email='maintainers@allspice.io',
```

### Comparing `py-allspice-1.17.1/tests/test_api.py` & `py-allspice-2.0.0/tests/test_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import base64
 
 import pytest
 import uuid
 
-from gitea import Gitea, User, Organization, Team, Repository, Issue, Milestone
-from gitea import NotFoundException, AlreadyExistsException
+from allspice import AllSpice, User, Organization, Team, Repository, Issue, Milestone
+from allspice import NotFoundException, AlreadyExistsException
 
-# put a ".token" file into your directory containg only the token for gitea
+# put a ".token" file into your directory containg only the token for AllSpice Hub
 @pytest.fixture
 def instance(scope="module"):
     try:
-        g = Gitea("http://localhost:3000", open(".token", "r").read().strip())
-        print("Gitea Version: " + g.get_version())
+        g = AllSpice("http://localhost:3000", open(".token", "r").read().strip(), ratelimiting=None)
+        print("AllSpice Hub Version: " + g.get_version())
         print("API-Token belongs to user: " + g.get_user().username)
         return g
     except:
         assert (
             False
-        ), "Gitea could not load. \
+        ), "AllSpice Hub could not load. \
                 - Instance running at http://localhost:3000 \
                 - Token at .token   \
                     ?"
 
 # make up some fresh names for the tests run
 test_org = "org_" + uuid.uuid4().hex[:8]
 test_user = "user_" + uuid.uuid4().hex[:8]
@@ -31,15 +31,15 @@
 
 def test_token_owner(instance):
     user = instance.get_user()
     assert user.username == "test", "Token user not 'tests'."
     assert user.is_admin, "Testuser is not Admin - Tests may fail"
 
 
-def test_gitea_version(instance):
+def test_allspice_hub_version(instance):
     assert instance.get_version().startswith("1."), "No Version String returned"
 
 
 def test_fail_get_non_existent_user(instance):
     with pytest.raises(NotFoundException) as e:
         User.request(instance, test_user)
 
@@ -123,14 +123,24 @@
     org = Organization.request(instance, test_org)
     repo = instance.create_repo(org, test_repo, "descr")
     assert repo.description == "descr"
     assert repo.owner == org
     assert repo.name == test_repo
     assert not repo.private
 
+def test_get_repository(instance):
+    repo = instance.get_repository(test_org, test_repo)
+    assert repo is not None
+    assert repo.name == test_repo
+    assert repo.owner.username == test_org
+
+def test_get_repository_non_existent(instance):
+    with pytest.raises(NotFoundException) as e:
+        instance.get_repository("doesnotexist", "doesnotexist")
+
 
 def test_patch_repo(instance):
     fields = {
         "allow_rebase": False,
         "description": "new description",
         "has_projects": True,
         "private": True,
@@ -149,14 +159,28 @@
     org = Organization.request(instance, test_org)
     repo = org.get_repository(test_repo)
     branches = repo.get_branches()
     assert len(branches) > 0
     master = [b for b in branches if b.name == "master"]
     assert len(master) > 0
 
+
+def test_get_branch(instance):
+    org = Organization.request(instance, test_org)
+    repo = org.get_repository(test_repo)
+    branch = repo.get_branch("master")
+    assert branch is not None
+    assert branch.name == "master"
+
+def test_get_branch_non_existent(instance):
+    org = Organization.request(instance, test_org)
+    repo = org.get_repository(test_repo)
+    with pytest.raises(NotFoundException) as e:
+        repo.get_branch("doesnotexist")
+
 def test_list_files_and_content(instance):
     org = Organization.request(instance, test_org)
     repo = org.get_repository(test_repo)
     content = repo.get_git_content()
     # Readme file should exist in any new repo
     #  content is the description given during creation
     readmes = [c for c in content if c.name == "README.md"]
@@ -210,14 +234,32 @@
 def test_create_team(instance):
     org = Organization.request(instance, test_org)
     team = instance.create_team(org, test_team, "descr")
     assert team.name == test_team
     assert team.description == "descr"
     assert team.organization == org
 
+def test_create_team_without_units_map(instance):
+    org = Organization.request(instance, test_org)
+    team = instance.create_team(org, test_team + "1", "descr")
+    permission = team.permission
+    assert set(team.units_map.keys()) == set(team.units)
+    assert list(team.units_map.values()) == [permission] * len(team.units)
+
+def test_create_team_with_units_map(instance):
+    org = Organization.request(instance, test_org)
+    team = instance.create_team(
+        org,
+        test_team + "2",
+        "descr",
+        units_map = {"repo.code": "write", "repo.wiki": "admin"}
+    )
+    assert set(team.units) == set(["repo.code", "repo.wiki"])
+    assert team.units_map == {"repo.code": "write", "repo.wiki": "admin"}
+
 def test_patch_team(instance):
     fields = {
         "can_create_org_repo": True,
         "description": "patched description",
         "includes_all_repositories": True,
         "name": "newname",
         "permission": "write",
@@ -382,7 +424,22 @@
     user_name = test_user + "delte_test"
     email = user_name + "@example.org"
     user = instance.create_user(user_name, email, "abcdefg1.23AB", send_notify=False)
     assert user.username == user_name
     user.delete()
     with pytest.raises(NotFoundException) as e:
         User.request(instance, user_name)
+
+def test_get_generated_json(instance):
+    # Note: this expects the test repo to have a file called test.pcbdoc,
+    # which will have json and svg generated from it.
+    repo = instance.get_repository("test", "test")
+    json = repo.get_generated_json("test.pcbdoc")
+    assert json is not None
+    assert json["type"] == "Pcb"
+
+
+def test_get_generated_svg(instance):
+    repo = instance.get_repository("test", "test")
+    svg = repo.get_generated_svg("test.pcbdoc")
+    assert svg is not None
+    assert svg.startswith(b"<svg")
```

### Comparing `py-allspice-1.17.1/tests/test_api_longtests.py` & `py-allspice-2.0.0/tests/test_api_longtests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import pytest
 import uuid
 
-from gitea import Gitea, User, Organization, Team, Repository, Issue
-from gitea import NotFoundException, AlreadyExistsException
+from allspice import AllSpice, User, Organization, Team, Repository, Issue
+from allspice import NotFoundException, AlreadyExistsException
 
-# put a ".token" file into your directory containg only the token for gitea
+# put a ".token" file into your directory containg only the token for AllSpice Hub
 @pytest.fixture
 def instance(scope="module"):
     try:
-        g = Gitea("http://localhost:3000", open(".token", "r").read().strip())
-        print("Gitea Version: " + g.get_version())
+        g = AllSpice("http://localhost:3000", open(".token", "r").read().strip(), ratelimiting=None)
+        print("AllSpice Hub Version: " + g.get_version())
         print("API-Token belongs to user: " + g.get_user().username)
         return g
     except:
         assert (
             False
-        ), "Gitea could not load. \
+        ), "AllSpice Hub could not load. \
                 - Instance running at http://localhost:3000 \
                 - Token at .token   \
                     ?"
 
 # make up some fresh names for the tests run
 test_org = "org_" + uuid.uuid4().hex[:8]
 test_user = "user_" + uuid.uuid4().hex[:8]
```

