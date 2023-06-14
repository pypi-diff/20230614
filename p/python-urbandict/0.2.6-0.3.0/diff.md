# Comparing `tmp/python_urbandict-0.2.6.tar.gz` & `tmp/python_urbandict-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_urbandict-0.2.6.tar", max compression
+gzip compressed data, was "python_urbandict-0.3.0.tar", max compression
```

## Comparing `python_urbandict-0.2.6.tar` & `python_urbandict-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2023-06-14 19:19:50.924797 python_urbandict-0.2.6/LICENSE
--rw-r--r--   0        0        0     2325 2023-06-14 19:19:50.924797 python_urbandict-0.2.6/README.md
--rw-r--r--   0        0        0      923 2023-06-14 19:19:50.924797 python_urbandict-0.2.6/pyproject.toml
--rw-r--r--   0        0        0       77 2023-06-14 19:19:50.924797 python_urbandict-0.2.6/pyurbandict/__init__.py
--rw-r--r--   0        0        0     1018 2023-06-14 19:19:50.924797 python_urbandict-0.2.6/pyurbandict/parse.py
--rw-r--r--   0        0        0     3183 1970-01-01 00:00:00.000000 python_urbandict-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-14 20:32:34.593568 python_urbandict-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2325 2023-06-14 20:32:34.593568 python_urbandict-0.3.0/README.md
+-rw-r--r--   0        0        0      943 2023-06-14 20:32:34.593568 python_urbandict-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-06-14 20:32:34.593568 python_urbandict-0.3.0/pyurbandict/__init__.py
+-rw-r--r--   0        0        0     1018 2023-06-14 20:32:34.593568 python_urbandict-0.3.0/pyurbandict/parse.py
+-rw-r--r--   0        0        0     3183 1970-01-01 00:00:00.000000 python_urbandict-0.3.0/PKG-INFO
```

### Comparing `python_urbandict-0.2.6/LICENSE` & `python_urbandict-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_urbandict-0.2.6/README.md` & `python_urbandict-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `python_urbandict-0.2.6/pyproject.toml` & `python_urbandict-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 [flake8]
 max-line-length = 88
 
 [tool.poetry]
 name = "python-urbandict"
-version = "0.2.6"
+version = "0.3.0"
 description = "Python wrapper for the Urban Dictionary API."
 authors = ["atbuy"]
 license = "MIT"
 homepage = "https://github.com/atbuy/pyurbandict"
 repository = "https://github.com/atbuy/pyurbandict"
 keywords = ["urban", "dictionary", "api", "wrapper", "python"]
 include = ["README.md"]
 readme = "README.md"
 packages = [
     {include = "pyurbandict"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-requests = "^2.28.1"
-
-[tool.poetry.dev-dependencies]
-black = "^22.6.0"
-flake8 = "^5.0.4"
-pre-commit = "^2.20.0"
-pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
+requests = "^2.31.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/atbuy/pyurbandict/issues"
 "Source Code" = "https://github.com/atbuy/pyurbandict"
 "CI/CD" = "https://github.com/atbuy/pyurbandict/actions"
 
+[tool.poetry.group.dev.dependencies]
+tox = "^4.6.0"
+black = "^23.3.0"
+flake8 = "^6.0.0"
+pre-commit = "^3.3.3"
+pytest = "^7.3.2"
+pytest-cov = "^4.1.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `python_urbandict-0.2.6/pyurbandict/parse.py` & `python_urbandict-0.3.0/pyurbandict/parse.py`

 * *Files identical despite different names*

### Comparing `python_urbandict-0.2.6/PKG-INFO` & `python_urbandict-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: python-urbandict
-Version: 0.2.6
+Version: 0.3.0
 Summary: Python wrapper for the Urban Dictionary API.
 Home-page: https://github.com/atbuy/pyurbandict
 License: MIT
 Keywords: urban,dictionary,api,wrapper,python
 Author: atbuy
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/atbuy/pyurbandict/issues
 Project-URL: CI/CD, https://github.com/atbuy/pyurbandict/actions
 Project-URL: Repository, https://github.com/atbuy/pyurbandict
 Project-URL: Source Code, https://github.com/atbuy/pyurbandict
 Description-Content-Type: text/markdown
 
 # python-urbandict
```

