# Comparing `tmp/landingai-0.0.7.tar.gz` & `tmp/landingai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingai-0.0.7.tar", max compression
+gzip compressed data, was "landingai-0.0.8.tar", max compression
```

## Comparing `landingai-0.0.7.tar` & `landingai-0.0.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4043 2023-05-13 04:06:14.490952 landingai-0.0.7/README.md
--rw-r--r--   0        0        0       40 2023-05-11 23:35:20.932651 landingai-0.0.7/landingai/__init__.py
--rw-r--r--   0        0        0     3372 2023-05-12 22:53:01.555726 landingai-0.0.7/landingai/common.py
--rw-r--r--   0        0        0     7385 2023-05-13 03:23:15.112923 landingai-0.0.7/landingai/predict.py
--rw-r--r--   0        0        0     2107 2023-05-12 22:53:01.563372 landingai-0.0.7/landingai/visualize.py
--rw-r--r--   0        0        0     1200 2023-05-13 04:07:34.540957 landingai-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4945 1970-01-01 00:00:00.000000 landingai-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     4098 2023-05-13 04:21:18.893710 landingai-0.0.8/README.md
+-rw-r--r--   0        0        0       40 2023-05-11 23:35:20.932651 landingai-0.0.8/landingai/__init__.py
+-rw-r--r--   0        0        0     3372 2023-05-12 22:53:01.555726 landingai-0.0.8/landingai/common.py
+-rw-r--r--   0        0        0     7385 2023-05-13 03:23:15.112923 landingai-0.0.8/landingai/predict.py
+-rw-r--r--   0        0        0     2107 2023-05-12 22:53:01.563372 landingai-0.0.8/landingai/visualize.py
+-rw-r--r--   0        0        0     1194 2023-05-13 04:19:48.542411 landingai-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4990 1970-01-01 00:00:00.000000 landingai-0.0.8/PKG-INFO
```

### Comparing `landingai-0.0.7/README.md` & `landingai-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -96,7 +96,13 @@
 ```
 
 ### Run tests
 
 ```bash
 poetry run pytest tests/
 ```
+
+### Activate the virtualenv
+
+```bash
+poetry shell
+```
```

### Comparing `landingai-0.0.7/landingai/common.py` & `landingai-0.0.8/landingai/common.py`

 * *Files identical despite different names*

### Comparing `landingai-0.0.7/landingai/predict.py` & `landingai-0.0.8/landingai/predict.py`

 * *Files identical despite different names*

### Comparing `landingai-0.0.7/landingai/visualize.py` & `landingai-0.0.8/landingai/visualize.py`

 * *Files identical despite different names*

### Comparing `landingai-0.0.7/pyproject.toml` & `landingai-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "landingai"
-version = "0.0.7"
+version = "0.0.8"
 description = "Helper library for interacting with Landing AI LandingLens"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "landingai"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
@@ -17,15 +17,15 @@
 
 [tool.poetry.dependencies]  # main dependency group
 python = ">=3.8"
 
 opencv-python-headless = ">=4.5"
 numpy = ">=1.21.0"
 pillow = ">=9.1.1"
-pydantic = ">=1.9.0"
+pydantic = "*"
 requests = "*"
 segmentation-mask-overlay = "*"
 
 [tool.poetry.group.dev.dependencies]
 jupyterlab = "*"
 autoflake = "*"
 pytest = "*"
```

### Comparing `landingai-0.0.7/PKG-INFO` & `landingai-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: landingai
-Version: 0.0.7
+Version: 0.0.8
 Summary: Helper library for interacting with Landing AI LandingLens
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.21.0)
 Requires-Dist: opencv-python-headless (>=4.5)
 Requires-Dist: pillow (>=9.1.1)
-Requires-Dist: pydantic (>=1.9.0)
+Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: segmentation-mask-overlay
 Project-URL: Homepage, https://landing.ai
 Project-URL: documentation, https://landing-ai.github.io/landingai-python-v1/landingai.html
 Project-URL: repository, https://github.com/landing-ai/landingai-python-v1
 Description-Content-Type: text/markdown
 
@@ -120,7 +120,13 @@
 
 ### Run tests
 
 ```bash
 poetry run pytest tests/
 ```
 
+### Activate the virtualenv
+
+```bash
+poetry shell
+```
+
```

