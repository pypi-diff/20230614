# Comparing `tmp/py_multiauth-2.0.0rc1.tar.gz` & `tmp/py_multiauth-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_multiauth-2.0.0rc1.tar", max compression
+gzip compressed data, was "py_multiauth-2.0.0rc2.tar", max compression
```

## Comparing `py_multiauth-2.0.0rc1.tar` & `py_multiauth-2.0.0rc2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1117 2023-05-04 10:03:08.722401 py_multiauth-2.0.0rc1/LICENSE
--rw-r--r--   0        0        0     2572 2023-05-04 10:03:08.722401 py_multiauth-2.0.0rc1/README.md
--rw-r--r--   0        0        0      152 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/__init__.py
--rw-r--r--   0        0        0       94 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/__main__.py
--rw-r--r--   0        0        0     2088 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/cli.py
--rw-r--r--   0        0        0       40 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/__init__.py
--rw-r--r--   0        0        0      598 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/errors.py
--rw-r--r--   0        0        0      474 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/http.py
--rw-r--r--   0        0        0     2250 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/interfaces.py
--rw-r--r--   0        0        0     3101 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/main.py
--rw-r--r--   0        0        0        0 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/providers/__init__.py
--rw-r--r--   0        0        0     1719 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/providers/aws.py
--rw-r--r--   0        0        0      830 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/providers/graphql.py
--rw-r--r--   0        0        0     1575 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/providers/oauth.py
--rw-r--r--   0        0        0      632 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/providers/rest.py
--rw-r--r--   0        0        0      511 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/utils.py
--rw-r--r--   0        0        0     7876 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/generator.py
--rw-r--r--   0        0        0     3381 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/handlers.py
--rw-r--r--   0        0        0    13730 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/helpers.py
--rw-r--r--   0        0        0    10409 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/main.py
--rw-r--r--   0        0        0     6462 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/manager.py
--rw-r--r--   0        0        0      599 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/__init__.py
--rw-r--r--   0        0        0     3198 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/apikey.py
--rw-r--r--   0        0        0    15633 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/aws.py
--rw-r--r--   0        0        0     1590 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/basic.py
--rw-r--r--   0        0        0     9003 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/digest.py
--rw-r--r--   0        0        0    14577 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/graphql.py
--rw-r--r--   0        0        0     1067 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/manual.py
--rw-r--r--   0        0        0    15749 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/oauth.py
--rw-r--r--   0        0        0     9672 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/rest.py
--rw-r--r--   0        0        0        0 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/py.typed
--rw-r--r--   0        0        0        0 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/static/__init__.py
--rw-r--r--   0        0        0    44688 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/static/auth_schema.json
--rw-r--r--   0        0        0     5361 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/utils.py
--rw-r--r--   0        0        0     1496 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     3668 1970-01-01 00:00:00.000000 py_multiauth-2.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/LICENSE
+-rw-r--r--   0        0        0     2572 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/README.md
+-rw-r--r--   0        0        0      152 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/__init__.py
+-rw-r--r--   0        0        0       94 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/__main__.py
+-rw-r--r--   0        0        0     2088 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/cli.py
+-rw-r--r--   0        0        0       40 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/__init__.py
+-rw-r--r--   0        0        0      598 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/errors.py
+-rw-r--r--   0        0        0      474 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/http.py
+-rw-r--r--   0        0        0     2250 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/interfaces.py
+-rw-r--r--   0        0        0     3101 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/main.py
+-rw-r--r--   0        0        0        0 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/providers/__init__.py
+-rw-r--r--   0        0        0     1719 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/providers/aws.py
+-rw-r--r--   0        0        0      830 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/providers/graphql.py
+-rw-r--r--   0        0        0     1575 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/providers/oauth.py
+-rw-r--r--   0        0        0      632 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/providers/rest.py
+-rw-r--r--   0        0        0      511 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/entities/utils.py
+-rw-r--r--   0        0        0     7876 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/generator.py
+-rw-r--r--   0        0        0     3381 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/handlers.py
+-rw-r--r--   0        0        0    13730 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/helpers.py
+-rw-r--r--   0        0        0    10409 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/main.py
+-rw-r--r--   0        0        0     6462 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/manager.py
+-rw-r--r--   0        0        0      599 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/providers/__init__.py
+-rw-r--r--   0        0        0     3198 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/providers/apikey.py
+-rw-r--r--   0        0        0    15633 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/providers/aws.py
+-rw-r--r--   0        0        0     1590 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/providers/basic.py
+-rw-r--r--   0        0        0     9003 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/providers/digest.py
+-rw-r--r--   0        0        0    14577 2023-06-14 12:23:16.009137 py_multiauth-2.0.0rc2/multiauth/providers/graphql.py
+-rw-r--r--   0        0        0     1067 2023-06-14 12:23:16.013137 py_multiauth-2.0.0rc2/multiauth/providers/manual.py
+-rw-r--r--   0        0        0    15749 2023-06-14 12:23:16.013137 py_multiauth-2.0.0rc2/multiauth/providers/oauth.py
+-rw-r--r--   0        0        0     9672 2023-06-14 12:23:16.013137 py_multiauth-2.0.0rc2/multiauth/providers/rest.py
+-rw-r--r--   0        0        0        0 2023-06-14 12:23:16.013137 py_multiauth-2.0.0rc2/multiauth/py.typed
+-rw-r--r--   0        0        0        0 2023-06-14 12:23:16.013137 py_multiauth-2.0.0rc2/multiauth/static/__init__.py
+-rw-r--r--   0        0        0    44688 2023-06-14 12:23:16.013137 py_multiauth-2.0.0rc2/multiauth/static/auth_schema.json
+-rw-r--r--   0        0        0     5361 2023-06-14 12:23:16.013137 py_multiauth-2.0.0rc2/multiauth/utils.py
+-rw-r--r--   0        0        0     1514 2023-06-14 12:23:16.013137 py_multiauth-2.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 py_multiauth-2.0.0rc2/PKG-INFO
```

### Comparing `py_multiauth-2.0.0rc1/LICENSE` & `py_multiauth-2.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/README.md` & `py_multiauth-2.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/cli.py` & `py_multiauth-2.0.0rc2/multiauth/cli.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/entities/errors.py` & `py_multiauth-2.0.0rc2/multiauth/entities/errors.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/entities/interfaces.py` & `py_multiauth-2.0.0rc2/multiauth/entities/interfaces.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/entities/main.py` & `py_multiauth-2.0.0rc2/multiauth/entities/main.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/entities/providers/aws.py` & `py_multiauth-2.0.0rc2/multiauth/entities/providers/aws.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/entities/providers/graphql.py` & `py_multiauth-2.0.0rc2/multiauth/entities/providers/graphql.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/entities/providers/oauth.py` & `py_multiauth-2.0.0rc2/multiauth/entities/providers/oauth.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/entities/providers/rest.py` & `py_multiauth-2.0.0rc2/multiauth/entities/providers/rest.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/generator.py` & `py_multiauth-2.0.0rc2/multiauth/generator.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/handlers.py` & `py_multiauth-2.0.0rc2/multiauth/handlers.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/helpers.py` & `py_multiauth-2.0.0rc2/multiauth/helpers.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/main.py` & `py_multiauth-2.0.0rc2/multiauth/main.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/manager.py` & `py_multiauth-2.0.0rc2/multiauth/manager.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/providers/__init__.py` & `py_multiauth-2.0.0rc2/multiauth/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/providers/apikey.py` & `py_multiauth-2.0.0rc2/multiauth/providers/apikey.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/providers/aws.py` & `py_multiauth-2.0.0rc2/multiauth/providers/aws.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/providers/basic.py` & `py_multiauth-2.0.0rc2/multiauth/providers/basic.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/providers/digest.py` & `py_multiauth-2.0.0rc2/multiauth/providers/digest.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/providers/graphql.py` & `py_multiauth-2.0.0rc2/multiauth/providers/graphql.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/providers/manual.py` & `py_multiauth-2.0.0rc2/multiauth/providers/manual.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/providers/oauth.py` & `py_multiauth-2.0.0rc2/multiauth/providers/oauth.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/providers/rest.py` & `py_multiauth-2.0.0rc2/multiauth/providers/rest.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/static/auth_schema.json` & `py_multiauth-2.0.0rc2/multiauth/static/auth_schema.json`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/multiauth/utils.py` & `py_multiauth-2.0.0rc2/multiauth/utils.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc1/pyproject.toml` & `py_multiauth-2.0.0rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-multiauth"
-version = "2.0.0-rc.1"
+version = "2.0.0-rc.2"
 description = "Python package to interact with multiple authentication services"
 authors = ["Escape Technologies SAS <ping@escape.tech>"]
 maintainers = [
     "Antoine Carossio <antoine@escape.tech>",
     "Swan <swan@escape.tech>"
 ]
 license = "MIT"
@@ -37,14 +37,15 @@
 Authlib = "^1.2.0"
 graphql-core = "^3.2.3"
 pycognito = "^2022.12.0"
 pydash = "^6.0.0"
 PyJWT = "^2.6.0"
 python = ">=3.8,<4.0"
 jsonschema = "^4.17.3"
+urllib3 = "<1.27"
 
 [tool.poetry.dev-dependencies]
 autoflake = "^2.0.1"
 docformatter = "^1.5.1"
 isort = "^5.10.1"
 mypy = "^1.0.1"
 poetryup = "^0.12.7"
```

### Comparing `py_multiauth-2.0.0rc1/PKG-INFO` & `py_multiauth-2.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-multiauth
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Python package to interact with multiple authentication services
 Home-page: https://escape.tech/
 License: MIT
 Author: Escape Technologies SAS
 Author-email: ping@escape.tech
 Maintainer: Antoine Carossio
 Maintainer-email: antoine@escape.tech
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Authlib (>=1.2.0,<2.0.0)
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
 Requires-Dist: graphql-core (>=3.2.3,<4.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: pycognito (>=2022.12.0,<2023.0.0)
 Requires-Dist: pydash (>=6.0.0,<7.0.0)
+Requires-Dist: urllib3 (<1.27)
 Project-URL: Bug Tracker, https://github.com/Escape-Technologies/py-multiauth/issues
 Project-URL: Repository, https://github.com/Escape-Technologies/py-multiauth
 Description-Content-Type: text/markdown
 
 # py-multiauth ![PyPI](https://img.shields.io/pypi/v/py-multiauth) [![CI](https://github.com/Escape-Technologies/py-multiauth/actions/workflows/ci.yaml/badge.svg)](https://github.com/Escape-Technologies/py-multiauth/actions/workflows/ci.yaml) [![CD](https://github.com/Escape-Technologies/py-multiauth/actions/workflows/cd.yaml/badge.svg)](https://github.com/Escape-Technologies/py-multiauth/actions/workflows/cd.yaml) [![codecov](https://codecov.io/gh/Escape-Technologies/py-multiauth/branch/main/graph/badge.svg?token=NL148MNKAE)](https://codecov.io/gh/Escape-Technologies/py-multiauth)
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-multiauth)
```

