# Comparing `tmp/featurepy-0.2.1.tar.gz` & `tmp/featurepy-0.2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurepy-0.2.1.tar", max compression
+gzip compressed data, was "featurepy-0.2.2.1.tar", max compression
```

## Comparing `featurepy-0.2.1.tar` & `featurepy-0.2.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35129 2023-04-16 16:56:28.332885 featurepy-0.2.1/LICENSE
--rw-r--r--   0        0        0        8 2023-05-10 21:32:16.081018 featurepy-0.2.1/README.md
--rw-r--r--   0        0        0      788 2023-06-14 13:40:56.830351 featurepy-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      287 2023-06-11 09:55:40.361310 featurepy-0.2.1/src/featurepy/__init__.py
--rw-r--r--   0        0        0     1529 2023-06-14 00:06:33.902940 featurepy-0.2.1/src/featurepy/feature_class.py
--rw-r--r--   0        0        0       20 2023-05-18 01:57:23.243033 featurepy-0.2.1/src/featurepy/flask/__init__.py
--rw-r--r--   0        0        0      230 2023-05-18 14:59:44.476705 featurepy-0.2.1/src/featurepy/flask/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1901 2023-05-18 14:59:44.477827 featurepy-0.2.1/src/featurepy/flask/__pycache__/views.cpython-311.pyc
--rw-r--r--   0        0        0      640 2023-05-18 01:57:23.243406 featurepy-0.2.1/src/featurepy/flask/views.py
--rw-r--r--   0        0        0     3412 2023-06-13 23:31:59.687317 featurepy-0.2.1/src/featurepy/model_constraints.py
--rw-r--r--   0        0        0     1730 2023-06-11 15:46:14.698789 featurepy-0.2.1/src/featurepy/parametric_features.py
--rw-r--r--   0        0        0        0 2023-05-10 23:04:00.786133 featurepy-0.2.1/src/featurepy/scripts/__init__.py
--rw-r--r--   0        0        0      202 2023-06-03 17:07:40.240249 featurepy-0.2.1/src/featurepy/scripts/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1328 2023-06-03 17:07:40.240691 featurepy-0.2.1/src/featurepy/scripts/__pycache__/features.cpython-311.pyc
--rw-r--r--   0        0        0      493 2023-05-15 20:05:33.947104 featurepy-0.2.1/src/featurepy/scripts/features.py
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 featurepy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35129 2023-04-16 16:56:28.332885 featurepy-0.2.2.1/LICENSE
+-rw-r--r--   0        0        0        8 2023-05-10 21:32:16.081018 featurepy-0.2.2.1/README.md
+-rw-r--r--   0        0        0      790 2023-06-14 13:43:09.864286 featurepy-0.2.2.1/pyproject.toml
+-rw-r--r--   0        0        0      287 2023-06-11 09:55:40.361310 featurepy-0.2.2.1/src/featurepy/__init__.py
+-rw-r--r--   0        0        0     1529 2023-06-14 00:06:33.902940 featurepy-0.2.2.1/src/featurepy/feature_class.py
+-rw-r--r--   0        0        0       20 2023-05-18 01:57:23.243033 featurepy-0.2.2.1/src/featurepy/flask/__init__.py
+-rw-r--r--   0        0        0      230 2023-05-18 14:59:44.476705 featurepy-0.2.2.1/src/featurepy/flask/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1901 2023-05-18 14:59:44.477827 featurepy-0.2.2.1/src/featurepy/flask/__pycache__/views.cpython-311.pyc
+-rw-r--r--   0        0        0      640 2023-05-18 01:57:23.243406 featurepy-0.2.2.1/src/featurepy/flask/views.py
+-rw-r--r--   0        0        0     3412 2023-06-13 23:31:59.687317 featurepy-0.2.2.1/src/featurepy/model_constraints.py
+-rw-r--r--   0        0        0     1730 2023-06-11 15:46:14.698789 featurepy-0.2.2.1/src/featurepy/parametric_features.py
+-rw-r--r--   0        0        0        0 2023-05-10 23:04:00.786133 featurepy-0.2.2.1/src/featurepy/scripts/__init__.py
+-rw-r--r--   0        0        0      202 2023-06-03 17:07:40.240249 featurepy-0.2.2.1/src/featurepy/scripts/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1328 2023-06-03 17:07:40.240691 featurepy-0.2.2.1/src/featurepy/scripts/__pycache__/features.cpython-311.pyc
+-rw-r--r--   0        0        0      493 2023-05-15 20:05:33.947104 featurepy-0.2.2.1/src/featurepy/scripts/features.py
+-rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 featurepy-0.2.2.1/PKG-INFO
```

### Comparing `featurepy-0.2.1/LICENSE` & `featurepy-0.2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `featurepy-0.2.1/pyproject.toml` & `featurepy-0.2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "featurepy"
-version = "0.2.1"
+version = "0.2.2.1"
 description = "Framework for building software product lines using feature-oriented programming (FOP) and aspect-oriented programming (AOP) in Python."
 authors = ["Adrian Wong <adrianwong227@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 featuremonkey3 = "^0.1.1"
 aspectlib = "^2.0.0"
 flask = "^2.3.2"
+pyyaml = "^6.0"
 
 [tool.poetry.scripts]
 newfeature = "featurepy.scripts.features:newfeature"
 
 [tool.poetry.group.example.dependencies]
 flask = "^2.3.2"
 wtforms = "^3.0.1"
 beautifulsoup4 = "^4.12.2"
 flask-sqlalchemy = "^3.0.3"
 factory-boy = "^3.2.1"
 bootstrap-flask = "^2.2.0"
 flask-migrate = "^4.0.4"
 pytest = "^7.3.1"
-pyyaml = "^6.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `featurepy-0.2.1/src/featurepy/feature_class.py` & `featurepy-0.2.2.1/src/featurepy/feature_class.py`

 * *Files identical despite different names*

### Comparing `featurepy-0.2.1/src/featurepy/flask/__pycache__/views.cpython-311.pyc` & `featurepy-0.2.2.1/src/featurepy/flask/__pycache__/views.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `featurepy-0.2.1/src/featurepy/flask/views.py` & `featurepy-0.2.2.1/src/featurepy/flask/views.py`

 * *Files identical despite different names*

### Comparing `featurepy-0.2.1/src/featurepy/model_constraints.py` & `featurepy-0.2.2.1/src/featurepy/model_constraints.py`

 * *Files identical despite different names*

### Comparing `featurepy-0.2.1/src/featurepy/parametric_features.py` & `featurepy-0.2.2.1/src/featurepy/parametric_features.py`

 * *Files identical despite different names*

### Comparing `featurepy-0.2.1/src/featurepy/scripts/__pycache__/features.cpython-311.pyc` & `featurepy-0.2.2.1/src/featurepy/scripts/__pycache__/features.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `featurepy-0.2.1/PKG-INFO` & `featurepy-0.2.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: featurepy
-Version: 0.2.1
+Version: 0.2.2.1
 Summary: Framework for building software product lines using feature-oriented programming (FOP) and aspect-oriented programming (AOP) in Python.
 Author: Adrian Wong
 Author-email: adrianwong227@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aspectlib (>=2.0.0,<3.0.0)
 Requires-Dist: featuremonkey3 (>=0.1.1,<0.2.0)
 Requires-Dist: flask (>=2.3.2,<3.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 ## Hello
```

