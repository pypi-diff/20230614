# Comparing `tmp/kraken_wrapper-0.24.0.tar.gz` & `tmp/kraken_wrapper-0.24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_wrapper-0.24.0.tar", max compression
+gzip compressed data, was "kraken_wrapper-0.24.1.tar", max compression
```

## Comparing `kraken_wrapper-0.24.0.tar` & `kraken_wrapper-0.24.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      988 2023-05-15 12:38:11.992918 kraken_wrapper-0.24.0/LICENSE
--rw-r--r--   0        0        0      433 2023-05-19 09:06:18.698605 kraken_wrapper-0.24.0/README.md
--rw-r--r--   0        0        0     1746 2023-06-13 12:02:07.268377 kraken_wrapper-0.24.0/pyproject.toml
--rw-r--r--   0        0        0      134 2023-06-13 12:02:07.272377 kraken_wrapper-0.24.0/src/kraken/wrapper/__init__.py
--rw-r--r--   0        0        0     3637 2023-05-15 12:38:11.992918 kraken_wrapper-0.24.0/src/kraken/wrapper/_buildend_venv.py
--rw-r--r--   0        0        0     3374 2023-05-15 12:38:11.992918 kraken_wrapper-0.24.0/src/kraken/wrapper/_buildenv.py
--rw-r--r--   0        0        0     5311 2023-05-15 12:38:11.992918 kraken_wrapper-0.24.0/src/kraken/wrapper/_buildenv_manager.py
--rw-r--r--   0        0        0     3674 2023-05-15 12:38:11.992918 kraken_wrapper-0.24.0/src/kraken/wrapper/_buildenv_pex.py
--rw-r--r--   0        0        0     3175 2023-05-15 12:38:11.992918 kraken_wrapper-0.24.0/src/kraken/wrapper/_config.py
--rw-r--r--   0        0        0     4605 2023-05-15 12:38:11.992918 kraken_wrapper-0.24.0/src/kraken/wrapper/_lockfile.py
--rw-r--r--   0        0        0     3564 2023-05-15 12:38:11.992918 kraken_wrapper-0.24.0/src/kraken/wrapper/_option_sets.py
--rw-r--r--   0        0        0     4222 2023-05-15 12:38:11.992918 kraken_wrapper-0.24.0/src/kraken/wrapper/_pex.py
--rw-r--r--   0        0        0    15754 2023-05-15 12:38:11.992918 kraken_wrapper-0.24.0/src/kraken/wrapper/main.py
--rw-r--r--   0        0        0        0 2023-05-15 12:38:11.992918 kraken_wrapper-0.24.0/src/kraken/wrapper/py.typed
--rw-r--r--   0        0        0     1428 1970-01-01 00:00:00.000000 kraken_wrapper-0.24.0/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-06-11 15:05:45.304631 kraken_wrapper-0.24.1/LICENSE
+-rw-r--r--   0        0        0      433 2023-06-11 15:05:45.304747 kraken_wrapper-0.24.1/README.md
+-rw-r--r--   0        0        0     1746 2023-06-14 13:05:30.906894 kraken_wrapper-0.24.1/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-06-14 13:05:30.907010 kraken_wrapper-0.24.1/src/kraken/wrapper/__init__.py
+-rw-r--r--   0        0        0     3637 2023-06-11 15:05:45.305461 kraken_wrapper-0.24.1/src/kraken/wrapper/_buildend_venv.py
+-rw-r--r--   0        0        0     3374 2023-06-11 15:05:45.305685 kraken_wrapper-0.24.1/src/kraken/wrapper/_buildenv.py
+-rw-r--r--   0        0        0     5311 2023-06-11 15:05:45.305833 kraken_wrapper-0.24.1/src/kraken/wrapper/_buildenv_manager.py
+-rw-r--r--   0        0        0     3674 2023-06-11 15:05:45.305960 kraken_wrapper-0.24.1/src/kraken/wrapper/_buildenv_pex.py
+-rw-r--r--   0        0        0     3175 2023-06-11 15:05:45.306102 kraken_wrapper-0.24.1/src/kraken/wrapper/_config.py
+-rw-r--r--   0        0        0     4605 2023-06-11 15:05:45.306245 kraken_wrapper-0.24.1/src/kraken/wrapper/_lockfile.py
+-rw-r--r--   0        0        0     3564 2023-06-11 15:05:45.306368 kraken_wrapper-0.24.1/src/kraken/wrapper/_option_sets.py
+-rw-r--r--   0        0        0     4222 2023-06-11 15:05:45.306492 kraken_wrapper-0.24.1/src/kraken/wrapper/_pex.py
+-rw-r--r--   0        0        0    15754 2023-06-11 15:05:45.306657 kraken_wrapper-0.24.1/src/kraken/wrapper/main.py
+-rw-r--r--   0        0        0        0 2023-06-11 15:05:45.306731 kraken_wrapper-0.24.1/src/kraken/wrapper/py.typed
+-rw-r--r--   0        0        0     1428 1970-01-01 00:00:00.000000 kraken_wrapper-0.24.1/PKG-INFO
```

### Comparing `kraken_wrapper-0.24.0/LICENSE` & `kraken_wrapper-0.24.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.24.0/pyproject.toml` & `kraken_wrapper-0.24.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kraken-wrapper"
-version = "0.24.0"
+version = "0.24.1"
 description = ""
 authors = ["Unknown <me@unknown.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "kraken/wrapper", from = "src" }]
 classifiers = []
 keywords = []
@@ -18,15 +18,15 @@
 Documentation = "https://kraken-build.github.io/kraken-build/"
 Homepage = "https://kraken-build.github.io/kraken-build/"
 Repository = "https://github.com/kraken-build/kraken-build/"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.11"
 keyring = "^23.8.2"
-kraken-common = "^0.24.0"
+kraken-common = "^0.24.1"
 pex = "^2.1.103"
 setuptools = ">=33.0.0"  # For pkg_resources
 termcolor = "^1.1.0"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
```

### Comparing `kraken_wrapper-0.24.0/src/kraken/wrapper/_buildend_venv.py` & `kraken_wrapper-0.24.1/src/kraken/wrapper/_buildend_venv.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.24.0/src/kraken/wrapper/_buildenv.py` & `kraken_wrapper-0.24.1/src/kraken/wrapper/_buildenv.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.24.0/src/kraken/wrapper/_buildenv_manager.py` & `kraken_wrapper-0.24.1/src/kraken/wrapper/_buildenv_manager.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.24.0/src/kraken/wrapper/_buildenv_pex.py` & `kraken_wrapper-0.24.1/src/kraken/wrapper/_buildenv_pex.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.24.0/src/kraken/wrapper/_config.py` & `kraken_wrapper-0.24.1/src/kraken/wrapper/_config.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.24.0/src/kraken/wrapper/_lockfile.py` & `kraken_wrapper-0.24.1/src/kraken/wrapper/_lockfile.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.24.0/src/kraken/wrapper/_option_sets.py` & `kraken_wrapper-0.24.1/src/kraken/wrapper/_option_sets.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.24.0/src/kraken/wrapper/_pex.py` & `kraken_wrapper-0.24.1/src/kraken/wrapper/_pex.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.24.0/src/kraken/wrapper/main.py` & `kraken_wrapper-0.24.1/src/kraken/wrapper/main.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.24.0/PKG-INFO` & `kraken_wrapper-0.24.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kraken-wrapper
-Version: 0.24.0
+Version: 0.24.1
 Summary: 
 License: MIT
 Author: Unknown
 Author-email: me@unknown.org
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: keyring (>=23.8.2,<24.0.0)
-Requires-Dist: kraken-common (>=0.24.0,<0.25.0)
+Requires-Dist: kraken-common (>=0.24.1,<0.25.0)
 Requires-Dist: pex (>=2.1.103,<3.0.0)
 Requires-Dist: setuptools (>=33.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/kraken-build/kraken-build/issues
 Project-URL: Documentation, https://kraken-build.github.io/kraken-build/
 Project-URL: Homepage, https://kraken-build.github.io/kraken-build/
 Project-URL: Repository, https://github.com/kraken-build/kraken-build/
```

