# Comparing `tmp/restsession-0.0.2.tar.gz` & `tmp/restsession-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restsession-0.0.2.tar", last modified: Tue Jun 13 20:51:06 2023, max compression
+gzip compressed data, was "restsession-0.0.3.tar", last modified: Tue Jun 13 22:49:34 2023, max compression
```

## Comparing `restsession-0.0.2.tar` & `restsession-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 20:51:06.884108 restsession-0.0.2/
--rw-r--r--   0 psample    (501) staff       (20)     1070 2023-06-11 21:51:14.000000 restsession-0.0.2/LICENSE
--rw-r--r--   0 psample    (501) staff       (20)      619 2023-06-13 20:51:06.883779 restsession-0.0.2/PKG-INFO
--rw-r--r--   0 psample    (501) staff       (20)       63 2023-06-11 21:51:14.000000 restsession-0.0.2/README.md
--rw-r--r--   0 psample    (501) staff       (20)      629 2023-06-13 20:46:43.000000 restsession-0.0.2/pyproject.toml
-drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 20:51:06.871531 restsession-0.0.2/restsession/
--rw-r--r--   0 psample    (501) staff       (20)      207 2023-06-13 15:13:41.000000 restsession-0.0.2/restsession/__init__.py
--rw-r--r--   0 psample    (501) staff       (20)     1325 2023-06-13 18:01:16.000000 restsession-0.0.2/restsession/defaults.py
--rw-r--r--   0 psample    (501) staff       (20)      549 2023-03-19 17:41:15.000000 restsession-0.0.2/restsession/metaclass.py
--rw-r--r--   0 psample    (501) staff       (20)    15518 2023-06-13 15:11:56.000000 restsession-0.0.2/restsession/models.py
--rw-r--r--   0 psample    (501) staff       (20)    33510 2023-06-13 20:35:57.000000 restsession-0.0.2/restsession/session.py
--rw-r--r--   0 psample    (501) staff       (20)     1144 2023-03-20 15:45:13.000000 restsession-0.0.2/restsession/session_singleton.py
-drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 20:51:06.874297 restsession-0.0.2/restsession.egg-info/
--rw-r--r--   0 psample    (501) staff       (20)      619 2023-06-13 20:51:06.000000 restsession-0.0.2/restsession.egg-info/PKG-INFO
--rw-r--r--   0 psample    (501) staff       (20)      439 2023-06-13 20:51:06.000000 restsession-0.0.2/restsession.egg-info/SOURCES.txt
--rw-r--r--   0 psample    (501) staff       (20)        1 2023-06-13 20:51:06.000000 restsession-0.0.2/restsession.egg-info/dependency_links.txt
--rw-r--r--   0 psample    (501) staff       (20)       12 2023-06-13 20:51:06.000000 restsession-0.0.2/restsession.egg-info/top_level.txt
--rw-r--r--   0 psample    (501) staff       (20)       38 2023-06-13 20:51:06.884209 restsession-0.0.2/setup.cfg
-drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 20:51:06.882532 restsession-0.0.2/tests/
--rw-r--r--   0 psample    (501) staff       (20)    42269 2023-06-13 18:36:44.000000 restsession-0.0.2/tests/test_authorization.py
--rw-r--r--   0 psample    (501) staff       (20)     8315 2023-06-11 22:01:56.000000 restsession-0.0.2/tests/test_code.py
--rw-r--r--   0 psample    (501) staff       (20)     4725 2023-06-11 22:01:56.000000 restsession-0.0.2/tests/test_redirects.py
--rw-r--r--   0 psample    (501) staff       (20)    17013 2023-04-09 16:39:44.000000 restsession-0.0.2/tests/test_requests.py
--rw-r--r--   0 psample    (501) staff       (20)     8090 2023-06-11 22:01:56.000000 restsession-0.0.2/tests/test_retries.py
+drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 22:49:34.566093 restsession-0.0.3/
+-rw-r--r--   0 psample    (501) staff       (20)     1070 2023-06-11 21:51:14.000000 restsession-0.0.3/LICENSE
+-rw-r--r--   0 psample    (501) staff       (20)      619 2023-06-13 22:49:34.565571 restsession-0.0.3/PKG-INFO
+-rw-r--r--   0 psample    (501) staff       (20)       63 2023-06-11 21:51:14.000000 restsession-0.0.3/README.md
+-rw-r--r--   0 psample    (501) staff       (20)      629 2023-06-13 22:47:41.000000 restsession-0.0.3/pyproject.toml
+drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 22:49:34.550649 restsession-0.0.3/restsession/
+-rw-r--r--   0 psample    (501) staff       (20)      207 2023-06-13 15:13:41.000000 restsession-0.0.3/restsession/__init__.py
+-rw-r--r--   0 psample    (501) staff       (20)     1325 2023-06-13 18:01:16.000000 restsession-0.0.3/restsession/defaults.py
+-rw-r--r--   0 psample    (501) staff       (20)      549 2023-03-19 17:41:15.000000 restsession-0.0.3/restsession/metaclass.py
+-rw-r--r--   0 psample    (501) staff       (20)    15518 2023-06-13 15:11:56.000000 restsession-0.0.3/restsession/models.py
+-rw-r--r--   0 psample    (501) staff       (20)    33510 2023-06-13 20:35:57.000000 restsession-0.0.3/restsession/session.py
+-rw-r--r--   0 psample    (501) staff       (20)     1144 2023-03-20 15:45:13.000000 restsession-0.0.3/restsession/session_singleton.py
+drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 22:49:34.553729 restsession-0.0.3/restsession.egg-info/
+-rw-r--r--   0 psample    (501) staff       (20)      619 2023-06-13 22:49:34.000000 restsession-0.0.3/restsession.egg-info/PKG-INFO
+-rw-r--r--   0 psample    (501) staff       (20)      439 2023-06-13 22:49:34.000000 restsession-0.0.3/restsession.egg-info/SOURCES.txt
+-rw-r--r--   0 psample    (501) staff       (20)        1 2023-06-13 22:49:34.000000 restsession-0.0.3/restsession.egg-info/dependency_links.txt
+-rw-r--r--   0 psample    (501) staff       (20)       12 2023-06-13 22:49:34.000000 restsession-0.0.3/restsession.egg-info/top_level.txt
+-rw-r--r--   0 psample    (501) staff       (20)       38 2023-06-13 22:49:34.566230 restsession-0.0.3/setup.cfg
+drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 22:49:34.564322 restsession-0.0.3/tests/
+-rw-r--r--   0 psample    (501) staff       (20)    42269 2023-06-13 18:36:44.000000 restsession-0.0.3/tests/test_authorization.py
+-rw-r--r--   0 psample    (501) staff       (20)     8315 2023-06-11 22:01:56.000000 restsession-0.0.3/tests/test_code.py
+-rw-r--r--   0 psample    (501) staff       (20)     4725 2023-06-11 22:01:56.000000 restsession-0.0.3/tests/test_redirects.py
+-rw-r--r--   0 psample    (501) staff       (20)    17013 2023-04-09 16:39:44.000000 restsession-0.0.3/tests/test_requests.py
+-rw-r--r--   0 psample    (501) staff       (20)     8090 2023-06-11 22:01:56.000000 restsession-0.0.3/tests/test_retries.py
```

### Comparing `restsession-0.0.2/LICENSE` & `restsession-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `restsession-0.0.2/PKG-INFO` & `restsession-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restsession
-Version: 0.0.2
+Version: 0.0.3
 Summary: RESTful API-friendly implementation of the 'requests' library
 Author-email: Palmer Sample <palmer@palmersample.net>
 Project-URL: Homepage, https://github.com/palmersample/restsession
 Project-URL: Bug Tracker, https://github.com/palmersample/restsession/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `restsession-0.0.2/pyproject.toml` & `restsession-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "restsession"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Palmer Sample", email="palmer@palmersample.net" },
 ]
 description = "RESTful API-friendly implementation of the 'requests' library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `restsession-0.0.2/restsession/defaults.py` & `restsession-0.0.3/restsession/defaults.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.2/restsession/metaclass.py` & `restsession-0.0.3/restsession/metaclass.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.2/restsession/models.py` & `restsession-0.0.3/restsession/models.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.2/restsession/session.py` & `restsession-0.0.3/restsession/session.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.2/restsession/session_singleton.py` & `restsession-0.0.3/restsession/session_singleton.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.2/restsession.egg-info/PKG-INFO` & `restsession-0.0.3/restsession.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restsession
-Version: 0.0.2
+Version: 0.0.3
 Summary: RESTful API-friendly implementation of the 'requests' library
 Author-email: Palmer Sample <palmer@palmersample.net>
 Project-URL: Homepage, https://github.com/palmersample/restsession
 Project-URL: Bug Tracker, https://github.com/palmersample/restsession/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `restsession-0.0.2/tests/test_authorization.py` & `restsession-0.0.3/tests/test_authorization.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.2/tests/test_code.py` & `restsession-0.0.3/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.2/tests/test_redirects.py` & `restsession-0.0.3/tests/test_redirects.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.2/tests/test_requests.py` & `restsession-0.0.3/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.2/tests/test_retries.py` & `restsession-0.0.3/tests/test_retries.py`

 * *Files identical despite different names*

