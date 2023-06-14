# Comparing `tmp/neqsimapi_connector-0.1.5.tar.gz` & `tmp/neqsimapi_connector-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neqsimapi_connector-0.1.5.tar", max compression
+gzip compressed data, was "neqsimapi_connector-0.1.6.tar", max compression
```

## Comparing `neqsimapi_connector-0.1.5.tar` & `neqsimapi_connector-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1039 2023-05-26 10:31:57.077727 neqsimapi_connector-0.1.5/README.md
--rw-r--r--   0        0        0     4504 2023-05-26 09:50:06.820770 neqsimapi_connector-0.1.5/neqsimapi_connector/BearerAuth.py
--rw-r--r--   0        0        0     3940 2023-05-12 10:36:51.953910 neqsimapi_connector-0.1.5/neqsimapi_connector/Connector.py
--rw-r--r--   0        0        0      593 2023-05-26 10:50:29.638209 neqsimapi_connector-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1877 1970-01-01 00:00:00.000000 neqsimapi_connector-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1039 2023-05-26 10:31:57.077727 neqsimapi_connector-0.1.6/README.md
+-rw-r--r--   0        0        0     4504 2023-05-26 09:50:06.820770 neqsimapi_connector-0.1.6/neqsimapi_connector/BearerAuth.py
+-rw-r--r--   0        0        0     3940 2023-05-12 10:36:51.953910 neqsimapi_connector-0.1.6/neqsimapi_connector/Connector.py
+-rw-r--r--   0        0        0      597 2023-05-26 18:59:29.111747 neqsimapi_connector-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1977 1970-01-01 00:00:00.000000 neqsimapi_connector-0.1.6/PKG-INFO
```

### Comparing `neqsimapi_connector-0.1.5/README.md` & `neqsimapi_connector-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `neqsimapi_connector-0.1.5/neqsimapi_connector/BearerAuth.py` & `neqsimapi_connector-0.1.6/neqsimapi_connector/BearerAuth.py`

 * *Files identical despite different names*

### Comparing `neqsimapi_connector-0.1.5/neqsimapi_connector/Connector.py` & `neqsimapi_connector-0.1.6/neqsimapi_connector/Connector.py`

 * *Files identical despite different names*

### Comparing `neqsimapi_connector-0.1.5/pyproject.toml` & `neqsimapi_connector-0.1.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "neqsimapi-connector"
-version = "0.1.5"
+version = "0.1.6"
 description = "A python package to simplify calling NeqSimAPI for end-users."
 authors = ["Åsmund Våge Fannemel <asmf@equinor.com>"]
 readme = "README.md"
 packages = [{include = "neqsimapi_connector"}]
 license = "MIT"
 repository = "https://github.com/equinor/NeqSimAPI-connector"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.6"
 msal = "^1.22.0"
 msal-extensions = "^1.0.0"
-requests = "^2.31.0"
+requests = "^2.27.1"
 
-[tool.poetry.group.dev.dependencies]
-autopep8 = "^2.0.2"
+# [tool.poetry.group.dev.dependencies]
+# autopep8 = "^2.0.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `neqsimapi_connector-0.1.5/PKG-INFO` & `neqsimapi_connector-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: neqsimapi-connector
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python package to simplify calling NeqSimAPI for end-users.
 Home-page: https://github.com/equinor/NeqSimAPI-connector
 License: MIT
 Author: Åsmund Våge Fannemel
 Author-email: asmf@equinor.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: msal (>=1.22.0,<2.0.0)
 Requires-Dist: msal-extensions (>=1.0.0,<2.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
 Project-URL: Repository, https://github.com/equinor/NeqSimAPI-connector
 Description-Content-Type: text/markdown
 
 # NeqSimAPI-connector
 A python package to simplify calling NeqSimAPI for end-users handling authentication.  
 
 See https://neqsimapi.app.radix.equinor.com/docs for available endpoints.
```

