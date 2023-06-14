# Comparing `tmp/apypie-0.3.2.tar.gz` & `tmp/apypie-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apypie-0.3.2.tar", last modified: Thu Nov 19 11:04:47 2020, max compression
+gzip compressed data, was "dist/apypie-0.4.0.tar", last modified: Wed Jun 14 07:02:16 2023, max compression
```

## Comparing `apypie-0.3.2.tar` & `apypie-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-19 11:04:47.000000 apypie-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1069 2020-11-19 11:04:44.000000 apypie-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     1180 2020-11-19 11:04:47.000000 apypie-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      410 2020-11-19 11:04:44.000000 apypie-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-19 11:04:47.000000 apypie-0.3.2/apypie/
--rw-r--r--   0 runner    (1001) docker     (116)      417 2020-11-19 11:04:44.000000 apypie-0.3.2/apypie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9105 2020-11-19 11:04:44.000000 apypie-0.3.2/apypie/action.py
--rw-r--r--   0 runner    (1001) docker     (116)    11036 2020-11-19 11:04:44.000000 apypie-0.3.2/apypie/api.py
--rw-r--r--   0 runner    (1001) docker     (116)      786 2020-11-19 11:04:44.000000 apypie-0.3.2/apypie/example.py
--rw-r--r--   0 runner    (1001) docker     (116)      443 2020-11-19 11:04:44.000000 apypie-0.3.2/apypie/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     5423 2020-11-19 11:04:44.000000 apypie-0.3.2/apypie/inflector.py
--rw-r--r--   0 runner    (1001) docker     (116)      688 2020-11-19 11:04:44.000000 apypie-0.3.2/apypie/param.py
--rw-r--r--   0 runner    (1001) docker     (116)     2233 2020-11-19 11:04:44.000000 apypie-0.3.2/apypie/resource.py
--rw-r--r--   0 runner    (1001) docker     (116)     1265 2020-11-19 11:04:44.000000 apypie-0.3.2/apypie/route.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-19 11:04:47.000000 apypie-0.3.2/apypie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1180 2020-11-19 11:04:46.000000 apypie-0.3.2/apypie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      345 2020-11-19 11:04:47.000000 apypie-0.3.2/apypie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-19 11:04:46.000000 apypie-0.3.2/apypie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2020-11-19 11:04:46.000000 apypie-0.3.2/apypie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-11-19 11:04:46.000000 apypie-0.3.2/apypie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       73 2020-11-19 11:04:47.000000 apypie-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1252 2020-11-19 11:04:44.000000 apypie-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:02:16.000000 apypie-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-14 07:02:12.000000 apypie-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-14 07:02:16.000000 apypie-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-14 07:02:12.000000 apypie-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:02:16.000000 apypie-0.4.0/apypie/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-14 07:02:12.000000 apypie-0.4.0/apypie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-06-14 07:02:12.000000 apypie-0.4.0/apypie/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-06-14 07:02:12.000000 apypie-0.4.0/apypie/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-14 07:02:12.000000 apypie-0.4.0/apypie/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-14 07:02:12.000000 apypie-0.4.0/apypie/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-14 07:02:12.000000 apypie-0.4.0/apypie/inflector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-14 07:02:12.000000 apypie-0.4.0/apypie/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-14 07:02:12.000000 apypie-0.4.0/apypie/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-14 07:02:12.000000 apypie-0.4.0/apypie/route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:02:16.000000 apypie-0.4.0/apypie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-14 07:02:16.000000 apypie-0.4.0/apypie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-14 07:02:16.000000 apypie-0.4.0/apypie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:02:16.000000 apypie-0.4.0/apypie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 07:02:16.000000 apypie-0.4.0/apypie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 07:02:16.000000 apypie-0.4.0/apypie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-14 07:02:16.000000 apypie-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-14 07:02:12.000000 apypie-0.4.0/setup.py
```

### Comparing `apypie-0.3.2/LICENSE` & `apypie-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apypie-0.3.2/PKG-INFO` & `apypie-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apypie
-Version: 0.3.2
+Version: 0.4.0
 Summary: Apipie bindings for Python
 Home-page: https://github.com/Apipie/apypie
 Author: Evgeni Golov
 Author-email: evgeni@golov.de
 License: MIT
 Description: # apypie - Apipie bindings for Python
         
@@ -19,8 +19,11 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `apypie-0.3.2/apypie/action.py` & `apypie-0.4.0/apypie/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from apypie.route import Route
 from apypie.example import Example
 from apypie.param import Param
 from apypie.exceptions import MissingArgumentsError, InvalidArgumentTypesError
 
 try:
-    basestring
+    basestring  # type: ignore[used-before-def]  # pylint: disable=used-before-assignment
 except NameError:  # Python 3 has no basestring
     basestring = str  # pylint: disable=invalid-name,redefined-builtin
 
 try:
     from typing import Optional, Any, Iterable, List, TYPE_CHECKING  # pylint: disable=unused-import
 except ImportError:
     TYPE_CHECKING = False
@@ -76,15 +76,15 @@
 
         :returns: The examples.
         """
 
         return [Example.parse(example) for example in self.apidoc['examples']]
 
     def call(self, params=None, headers=None, options=None, data=None, files=None):  # pylint: disable=too-many-arguments
-        # type: (dict, Optional[dict], Optional[dict], Optional[Any], Optional[dict]) -> dict
+        # type: (Optional[dict], Optional[dict], Optional[dict], Optional[Any], Optional[dict]) -> Optional[dict]
         """
         Call the API to execute the action.
 
         :param params: The params that should be passed to the API.
         :param headers: Additional headers to be passed to the API.
         :param options: Options
         :param data: Binary data to be submitted to the API.
```

### Comparing `apypie-0.3.2/apypie/api.py` & `apypie-0.4.0/apypie/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,19 +18,23 @@
     from urllib.parse import urljoin  # type: ignore
 import requests
 
 from apypie.resource import Resource
 from apypie.exceptions import DocLoadingError
 
 try:
-    from typing import Any, Iterable  # pylint: disable=unused-import
+    from typing import Any, Iterable, Optional  # pylint: disable=unused-import
+    from apypie.action import Action  # pylint: disable=unused-import
 except ImportError:
     pass
 
 
+NO_CONTENT = 204
+
+
 def _qs_param(param):
     # type: (Any) -> Any
     if isinstance(param, bool):
         return str(param).lower()
     return param
 
 
@@ -43,14 +47,15 @@
     :param password: username to access the API
     :param api_version: version of the API. Defaults to `1`
     :param language: prefered locale for the API description
     :param apidoc_cache_base_dir: base directory for building apidoc_cache_dir. Defaults to `~/.cache/apipie_bindings`.
     :param apidoc_cache_dir: where to cache the JSON description of the API. Defaults to `apidoc_cache_base_dir/<URI>`.
     :param apidoc_cache_name: name of the cache file. If there is cache in the `apidoc_cache_dir`, it is used. Defaults to `default`.
     :param verify_ssl: should the SSL certificate be verified. Defaults to `True`.
+    :param session: a `requests.Session` compatible object. Defaults to `requests.Session()`.
 
     Usage::
 
       >>> import apypie
       >>> api = apypie.Api(uri='https://api.example.com', username='admin', password='changeme')
     """
 
@@ -67,15 +72,15 @@
             xdg_cache_home = '~/.cache'
 
         apidoc_cache_base_dir = kwargs.get('apidoc_cache_base_dir', os.path.join(os.path.expanduser(xdg_cache_home), 'apypie'))
         apidoc_cache_dir_default = os.path.join(apidoc_cache_base_dir, self.uri.replace(':', '_').replace('/', '_'), 'v{}'.format(self.api_version))
         self.apidoc_cache_dir = kwargs.get('apidoc_cache_dir', apidoc_cache_dir_default)
         self.apidoc_cache_name = kwargs.get('apidoc_cache_name', self._find_cache_name())
 
-        self._session = requests.Session()
+        self._session = kwargs.get('session') or requests.Session()
         self._session.verify = kwargs.get('verify_ssl', True)
 
         self._session.headers['Accept'] = 'application/json;version={}'.format(self.api_version)
         self._session.headers['User-Agent'] = 'apypie (https://github.com/Apipie/apypie)'
         if self.language:
             self._session.headers['Accept-Language'] = self.language
 
@@ -115,16 +120,16 @@
     def _find_cache_name(self, default='default'):
         cache_file = next(self._cache_dir_contents(), None)
         cache_name = default
         if cache_file:
             cache_name = os.path.basename(cache_file)[:-len(self.cache_extension)]
         return cache_name
 
-    def validate_cache(self, cache_name):
-        # type: (str) -> None
+    def validate_cache(self, cache_name=None):
+        # type: (Optional[str]) -> None
         """
         Ensure the cached apidoc matches the one presented by the server.
 
         :param cache_name: The name of the apidoc on the server.
         """
 
         if cache_name is not None and cache_name != self.apidoc_cache_name:
@@ -171,15 +176,15 @@
             return Resource(self, name)
         message = "Resource '{}' does not exist in the API. Existing resources: {}".format(name, ', '.join(sorted(self.resources)))
         raise KeyError(message)
 
     def _load_apidoc(self):
         # type: () -> dict
         try:
-            with open(self.apidoc_cache_file, 'r') as apidoc_file:
+            with open(self.apidoc_cache_file, 'r') as apidoc_file:  # pylint:disable=all
                 api_doc = json.load(apidoc_file)
         except (IOError, JSONDecodeError):
             api_doc = self._retrieve_apidoc()
         return api_doc
 
     def _retrieve_apidoc(self):
         # type: () -> dict
@@ -195,28 +200,32 @@
             if not response and language_family != self.language:
                 response = self._retrieve_apidoc_call('/apidoc/v{0}.{1}.json'.format(self.api_version, language_family), safe=True)
         if not response:
             try:
                 response = self._retrieve_apidoc_call('/apidoc/v{}.json'.format(self.api_version))
             except Exception as exc:
                 raise DocLoadingError("""Could not load data from {0}: {1}
-                  - is your server down?
-                  - was rake apipie:cache run when using apipie cache? (typical production settings)""".format(self.uri, exc))
-        with open(self.apidoc_cache_file, 'w') as apidoc_file:
+                  - is your server down?""".format(self.uri, exc))
+        if not response:
+            raise DocLoadingError("""Could not load data from {0}""".format(self.uri))
+        with open(self.apidoc_cache_file, 'w') as apidoc_file:  # pylint:disable=all
             apidoc_file.write(json.dumps(response))
         return response
 
     def _retrieve_apidoc_call(self, path, safe=False):
+        # type: (str, bool) -> Optional[dict]
         try:
             return self.http_call('get', path)
-        except requests.exceptions.HTTPError:
+        except Exception:
             if not safe:
                 raise
+            return None
 
     def call(self, resource_name, action_name, params=None, headers=None, options=None, data=None, files=None):  # pylint: disable=too-many-arguments
+        # type: (str, str, Optional[dict], Optional[dict], Optional[dict], Optional[dict], Optional[dict]) -> Optional[dict]
         """
         Call an action in the API.
 
         It finds most fitting route based on given parameters
         with other attributes necessary to do an API call.
 
         :param resource_name: name of the resource
@@ -243,26 +252,28 @@
         action = resource.action(action_name)
         if not options.get('skip_validation', False):
             action.validate(params, data, files)
 
         return self._call_action(action, params, headers, data, files)
 
     def _call_action(self, action, params=None, headers=None, data=None, files=None):  # pylint: disable=too-many-arguments
+        # type: (Action, Optional[dict], Optional[dict], Optional[dict], Optional[dict]) -> Optional[dict]
         if params is None:
             params = {}
 
         route = action.find_route(params)
         get_params = {key: value for key, value in params.items() if key not in route.params_in_path}
         return self.http_call(
             route.method,
             route.path_with_params(params),
             get_params,
             headers, data, files)
 
     def http_call(self, http_method, path, params=None, headers=None, data=None, files=None):  # pylint: disable=too-many-arguments
+        # type: (str, str, Optional[dict], Optional[dict], Optional[dict], Optional[dict]) -> Optional[dict]
         """
         Execute an HTTP request.
 
         :param params: Dict of parameters to be sent in the request
         :param headers: Dict of headers to be sent in the request
         :param data: Binary data to be sent in the request
         :param files: Binary files to be sent in the request
@@ -292,20 +303,21 @@
 
         if data:
             kwargs['data'] = data
 
         request = self._session.request(http_method, full_path, **kwargs)
         request.raise_for_status()
         self.validate_cache(request.headers.get('apipie-checksum'))
-        if request.status_code == requests.codes['no_content']:
+        if request.status_code == NO_CONTENT:
             return None
         return request.json()
 
     @property
     def cache_extension(self):
+        # type: () -> str
         """
         File extension for the local cache file.
 
         Will include the language if set.
         """
 
         if self.language:
```

### Comparing `apypie-0.3.2/apypie/example.py` & `apypie-0.4.0/apypie/example.py`

 * *Files identical despite different names*

### Comparing `apypie-0.3.2/apypie/inflector.py` & `apypie-0.4.0/apypie/inflector.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
         self.inflections.irregular('child', 'children')
         self.inflections.irregular('man', 'men')
         self.inflections.irregular('medium', 'media')
         self.inflections.irregular('move', 'moves')
         self.inflections.irregular('person', 'people')
         self.inflections.irregular('self', 'selves')
         self.inflections.irregular('sex', 'sexes')
+        self.inflections.irregular('erratum', 'errata')
 
         self.inflections.uncountable('equipment', 'information', 'money', 'species', 'series', 'fish', 'sheep', 'police')
 
     def pluralize(self, word):
         # type: (str) -> str
         """
         Pluralize a word.
```

### Comparing `apypie-0.3.2/apypie/param.py` & `apypie-0.4.0/apypie/param.py`

 * *Files identical despite different names*

### Comparing `apypie-0.3.2/apypie/resource.py` & `apypie-0.4.0/apypie/resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         Check whether the resource has a given action.
 
         :param name: The name of the action.
         """
         return name in self.actions
 
     def call(self, action, params=None, headers=None, options=None, data=None, files=None):  # pylint: disable=too-many-arguments
-        # type: (str, Optional[dict], Optional[dict], Optional[dict], Optional[Any], Optional[dict]) -> dict
+        # type: (str, Optional[dict], Optional[dict], Optional[dict], Optional[Any], Optional[dict]) -> Optional[dict]
         """
         Call the API to execute an action for this resource.
 
         :param action: The action to call.
         :param params: The params that should be passed to the API.
         :param headers: Additional headers to be passed to the API.
         :param options: Options
```

### Comparing `apypie-0.3.2/apypie/route.py` & `apypie-0.4.0/apypie/route.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """
 Apypie Route module
 """
 
 from __future__ import print_function, absolute_import
 
 try:
+    from urllib.parse import quote  # type: ignore
+except ImportError:
+    from urllib import quote  # type: ignore
+
+try:
     from typing import List, Optional  # pylint: disable=unused-import
 except ImportError:
     pass
 
 
 class Route(object):
     """
@@ -38,11 +43,11 @@
 
         :returns: The path with params.
         """
         result = self.path
         if params is not None:
             for param in self.params_in_path:
                 if param in params:
-                    result = result.replace(':{}'.format(param), str(params[param]))
+                    result = result.replace(':{}'.format(param), quote(str(params[param]), safe=''))
                 else:
                     raise KeyError("missing param '{}' in parameters".format(param))
         return result
```

### Comparing `apypie-0.3.2/apypie.egg-info/PKG-INFO` & `apypie-0.4.0/apypie.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apypie
-Version: 0.3.2
+Version: 0.4.0
 Summary: Apipie bindings for Python
 Home-page: https://github.com/Apipie/apypie
 Author: Evgeni Golov
 Author-email: evgeni@golov.de
 License: MIT
 Description: # apypie - Apipie bindings for Python
         
@@ -19,8 +19,11 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

