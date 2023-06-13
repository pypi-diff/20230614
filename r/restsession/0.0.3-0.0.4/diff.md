# Comparing `tmp/restsession-0.0.3.tar.gz` & `tmp/restsession-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restsession-0.0.3.tar", last modified: Tue Jun 13 22:49:34 2023, max compression
+gzip compressed data, was "restsession-0.0.4.tar", last modified: Tue Jun 13 23:40:18 2023, max compression
```

## Comparing `restsession-0.0.3.tar` & `restsession-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 22:49:34.566093 restsession-0.0.3/
--rw-r--r--   0 psample    (501) staff       (20)     1070 2023-06-11 21:51:14.000000 restsession-0.0.3/LICENSE
--rw-r--r--   0 psample    (501) staff       (20)      619 2023-06-13 22:49:34.565571 restsession-0.0.3/PKG-INFO
--rw-r--r--   0 psample    (501) staff       (20)       63 2023-06-11 21:51:14.000000 restsession-0.0.3/README.md
--rw-r--r--   0 psample    (501) staff       (20)      629 2023-06-13 22:47:41.000000 restsession-0.0.3/pyproject.toml
-drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 22:49:34.550649 restsession-0.0.3/restsession/
--rw-r--r--   0 psample    (501) staff       (20)      207 2023-06-13 15:13:41.000000 restsession-0.0.3/restsession/__init__.py
--rw-r--r--   0 psample    (501) staff       (20)     1325 2023-06-13 18:01:16.000000 restsession-0.0.3/restsession/defaults.py
--rw-r--r--   0 psample    (501) staff       (20)      549 2023-03-19 17:41:15.000000 restsession-0.0.3/restsession/metaclass.py
--rw-r--r--   0 psample    (501) staff       (20)    15518 2023-06-13 15:11:56.000000 restsession-0.0.3/restsession/models.py
--rw-r--r--   0 psample    (501) staff       (20)    33510 2023-06-13 20:35:57.000000 restsession-0.0.3/restsession/session.py
--rw-r--r--   0 psample    (501) staff       (20)     1144 2023-03-20 15:45:13.000000 restsession-0.0.3/restsession/session_singleton.py
-drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 22:49:34.553729 restsession-0.0.3/restsession.egg-info/
--rw-r--r--   0 psample    (501) staff       (20)      619 2023-06-13 22:49:34.000000 restsession-0.0.3/restsession.egg-info/PKG-INFO
--rw-r--r--   0 psample    (501) staff       (20)      439 2023-06-13 22:49:34.000000 restsession-0.0.3/restsession.egg-info/SOURCES.txt
--rw-r--r--   0 psample    (501) staff       (20)        1 2023-06-13 22:49:34.000000 restsession-0.0.3/restsession.egg-info/dependency_links.txt
--rw-r--r--   0 psample    (501) staff       (20)       12 2023-06-13 22:49:34.000000 restsession-0.0.3/restsession.egg-info/top_level.txt
--rw-r--r--   0 psample    (501) staff       (20)       38 2023-06-13 22:49:34.566230 restsession-0.0.3/setup.cfg
-drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 22:49:34.564322 restsession-0.0.3/tests/
--rw-r--r--   0 psample    (501) staff       (20)    42269 2023-06-13 18:36:44.000000 restsession-0.0.3/tests/test_authorization.py
--rw-r--r--   0 psample    (501) staff       (20)     8315 2023-06-11 22:01:56.000000 restsession-0.0.3/tests/test_code.py
--rw-r--r--   0 psample    (501) staff       (20)     4725 2023-06-11 22:01:56.000000 restsession-0.0.3/tests/test_redirects.py
--rw-r--r--   0 psample    (501) staff       (20)    17013 2023-04-09 16:39:44.000000 restsession-0.0.3/tests/test_requests.py
--rw-r--r--   0 psample    (501) staff       (20)     8090 2023-06-11 22:01:56.000000 restsession-0.0.3/tests/test_retries.py
+drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 23:40:18.530962 restsession-0.0.4/
+-rw-r--r--   0 psample    (501) staff       (20)     1070 2023-06-11 21:51:14.000000 restsession-0.0.4/LICENSE
+-rw-r--r--   0 psample    (501) staff       (20)      619 2023-06-13 23:40:18.530556 restsession-0.0.4/PKG-INFO
+-rw-r--r--   0 psample    (501) staff       (20)       63 2023-06-11 21:51:14.000000 restsession-0.0.4/README.md
+-rw-r--r--   0 psample    (501) staff       (20)      629 2023-06-13 23:36:31.000000 restsession-0.0.4/pyproject.toml
+drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 23:40:18.518917 restsession-0.0.4/restsession/
+-rw-r--r--   0 psample    (501) staff       (20)      207 2023-06-13 15:13:41.000000 restsession-0.0.4/restsession/__init__.py
+-rw-r--r--   0 psample    (501) staff       (20)     1325 2023-06-13 18:01:16.000000 restsession-0.0.4/restsession/defaults.py
+-rw-r--r--   0 psample    (501) staff       (20)      549 2023-03-19 17:41:15.000000 restsession-0.0.4/restsession/metaclass.py
+-rw-r--r--   0 psample    (501) staff       (20)    15518 2023-06-13 15:11:56.000000 restsession-0.0.4/restsession/models.py
+-rw-r--r--   0 psample    (501) staff       (20)    32969 2023-06-13 23:34:36.000000 restsession-0.0.4/restsession/session.py
+-rw-r--r--   0 psample    (501) staff       (20)     1144 2023-03-20 15:45:13.000000 restsession-0.0.4/restsession/session_singleton.py
+drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 23:40:18.521619 restsession-0.0.4/restsession.egg-info/
+-rw-r--r--   0 psample    (501) staff       (20)      619 2023-06-13 23:40:18.000000 restsession-0.0.4/restsession.egg-info/PKG-INFO
+-rw-r--r--   0 psample    (501) staff       (20)      439 2023-06-13 23:40:18.000000 restsession-0.0.4/restsession.egg-info/SOURCES.txt
+-rw-r--r--   0 psample    (501) staff       (20)        1 2023-06-13 23:40:18.000000 restsession-0.0.4/restsession.egg-info/dependency_links.txt
+-rw-r--r--   0 psample    (501) staff       (20)       12 2023-06-13 23:40:18.000000 restsession-0.0.4/restsession.egg-info/top_level.txt
+-rw-r--r--   0 psample    (501) staff       (20)       38 2023-06-13 23:40:18.531070 restsession-0.0.4/setup.cfg
+drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 23:40:18.529331 restsession-0.0.4/tests/
+-rw-r--r--   0 psample    (501) staff       (20)    42269 2023-06-13 18:36:44.000000 restsession-0.0.4/tests/test_authorization.py
+-rw-r--r--   0 psample    (501) staff       (20)     8315 2023-06-11 22:01:56.000000 restsession-0.0.4/tests/test_code.py
+-rw-r--r--   0 psample    (501) staff       (20)     4725 2023-06-11 22:01:56.000000 restsession-0.0.4/tests/test_redirects.py
+-rw-r--r--   0 psample    (501) staff       (20)    17013 2023-04-09 16:39:44.000000 restsession-0.0.4/tests/test_requests.py
+-rw-r--r--   0 psample    (501) staff       (20)     8090 2023-06-11 22:01:56.000000 restsession-0.0.4/tests/test_retries.py
```

### Comparing `restsession-0.0.3/LICENSE` & `restsession-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `restsession-0.0.3/PKG-INFO` & `restsession-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restsession
-Version: 0.0.3
+Version: 0.0.4
 Summary: RESTful API-friendly implementation of the 'requests' library
 Author-email: Palmer Sample <palmer@palmersample.net>
 Project-URL: Homepage, https://github.com/palmersample/restsession
 Project-URL: Bug Tracker, https://github.com/palmersample/restsession/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `restsession-0.0.3/pyproject.toml` & `restsession-0.0.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "restsession"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Palmer Sample", email="palmer@palmersample.net" },
 ]
 description = "RESTful API-friendly implementation of the 'requests' library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `restsession-0.0.3/restsession/defaults.py` & `restsession-0.0.4/restsession/defaults.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.3/restsession/metaclass.py` & `restsession-0.0.4/restsession/metaclass.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.3/restsession/models.py` & `restsession-0.0.4/restsession/models.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.3/restsession/session.py` & `restsession-0.0.4/restsession/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,14 @@
 
     The returned function (redirect_header_hook) will be the first response
     hook attached to the Session object.
 
     :param headers: List of header names to remove on redirect
     :return: redirect_header_hook function reference to be used as a hook
     """
-    logger.error("Creating hook to remove header '%s' on redirect...", headers)
-
     def redirect_header_hook(response, **kwargs):  # pylint: disable=unused-argument
         """
         Hook used when a redirect response is received. If redirected to a
         different host, remove any custom auth headers as supplied in the
         wrapping function.
 
         :param response: requests Response object
@@ -673,21 +671,18 @@
         This hook will be the FIRST hook executed after a response.
 
         :param headers: Function reference to become the redirect handler
         :return: None
         """
         if not isinstance(hook, list):
             hook = [hook]
-        logger.error("Response hooks: %s", self.http.hooks["response"])
-        logger.error("Setting hook: %s", hook)
         self._session_params.redirect_header_hook = hook
         self.http.hooks["response"] = self.redirect_header_hook + \
                                       self.response_hooks + \
                                       self.request_exception_hook
-        logger.error("redirect hook update: %s", self.http.hooks["response"])
 
     @property
     def request_exception_hook(self):
         """
         Currently configured response hook for exception handling
 
         :return: session response hook for exceptions
@@ -708,22 +703,17 @@
 
         :param headers: Function reference to become the exception handler hook
         :return: None
         """
         if not isinstance(hook, list):
             hook = [hook]
         self._session_params.request_exception_hook = hook
-        logger.error("Current exception hook: %s", self.request_exception_hook)
         self.http.hooks["response"] = self.redirect_header_hook + \
                                       self.response_hooks + \
                                       self.request_exception_hook
-        logger.error("All current hooks: %s (len: %s)",
-                     self.http.hooks["response"],
-                     len(self.http.hooks["response"])
-                     )
 
     @property
     def response_hooks(self):
         """
         Currently configured custom response hooks.
 
         :return: User-defined custom response hooks
```

### Comparing `restsession-0.0.3/restsession/session_singleton.py` & `restsession-0.0.4/restsession/session_singleton.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.3/restsession.egg-info/PKG-INFO` & `restsession-0.0.4/restsession.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restsession
-Version: 0.0.3
+Version: 0.0.4
 Summary: RESTful API-friendly implementation of the 'requests' library
 Author-email: Palmer Sample <palmer@palmersample.net>
 Project-URL: Homepage, https://github.com/palmersample/restsession
 Project-URL: Bug Tracker, https://github.com/palmersample/restsession/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `restsession-0.0.3/tests/test_authorization.py` & `restsession-0.0.4/tests/test_authorization.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.3/tests/test_code.py` & `restsession-0.0.4/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.3/tests/test_redirects.py` & `restsession-0.0.4/tests/test_redirects.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.3/tests/test_requests.py` & `restsession-0.0.4/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.3/tests/test_retries.py` & `restsession-0.0.4/tests/test_retries.py`

 * *Files identical despite different names*

