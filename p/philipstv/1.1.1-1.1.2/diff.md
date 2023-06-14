# Comparing `tmp/philipstv-1.1.1.tar.gz` & `tmp/philipstv-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philipstv-1.1.1.tar", max compression
+gzip compressed data, was "philipstv-1.1.2.tar", max compression
```

## Comparing `philipstv-1.1.1.tar` & `philipstv-1.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1079 2023-05-14 13:54:35.571235 philipstv-1.1.1/LICENSE
--rw-r--r--   0        0        0     2393 2023-05-14 13:54:35.571235 philipstv-1.1.1/README.rst
--rw-r--r--   0        0        0     2671 2023-06-14 17:38:55.585607 philipstv-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      873 2023-06-14 17:38:55.585607 philipstv-1.1.1/src/philipstv/__init__.py
--rw-r--r--   0        0        0      368 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/__main__.py
--rw-r--r--   0        0        0    14775 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/_cli.py
--rw-r--r--   0        0        0     1793 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/_data.py
--rw-r--r--   0        0        0      410 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/_utils.py
--rw-r--r--   0        0        0     9702 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/api.py
--rw-r--r--   0        0        0     2836 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/exceptions.py
--rw-r--r--   0        0        0     1692 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/model/__init__.py
--rw-r--r--   0        0        0     3161 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/model/ambilight.py
--rw-r--r--   0        0        0     1208 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/model/applications.py
--rw-r--r--   0        0        0      373 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/model/audio.py
--rw-r--r--   0        0        0     1518 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/model/base.py
--rw-r--r--   0        0        0     2219 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/model/channels.py
--rw-r--r--   0        0        0      293 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/model/general.py
--rw-r--r--   0        0        0     1399 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/model/input.py
--rw-r--r--   0        0        0     2179 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/model/pairing.py
--rw-r--r--   0        0        0     3235 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/pairing.py
--rw-r--r--   0        0        0        0 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/py.typed
--rw-r--r--   0        0        0    10430 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/remote.py
--rw-r--r--   0        0        0     3384 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/tv.py
--rw-r--r--   0        0        0       56 2023-05-14 13:54:35.574569 philipstv-1.1.1/src/philipstv/types.py
--rw-r--r--   0        0        0        0 2023-05-14 13:54:35.574569 philipstv-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1457 2023-05-14 13:54:35.574569 philipstv-1.1.1/tests/fakes.py
--rw-r--r--   0        0        0    12595 2023-05-14 13:54:35.574569 philipstv-1.1.1/tests/test_api.py
--rw-r--r--   0        0        0    10047 2023-05-14 13:54:35.574569 philipstv-1.1.1/tests/test_cli.py
--rw-r--r--   0        0        0     2657 2023-05-14 13:54:35.574569 philipstv-1.1.1/tests/test_pairing.py
--rw-r--r--   0        0        0     9093 2023-05-14 13:54:35.574569 philipstv-1.1.1/tests/test_remote.py
--rw-r--r--   0        0        0     2441 2023-05-14 13:54:35.574569 philipstv-1.1.1/tests/test_tv.py
--rw-r--r--   0        0        0     3806 1970-01-01 00:00:00.000000 philipstv-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-05-14 13:54:35.571235 philipstv-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2393 2023-05-14 13:54:35.571235 philipstv-1.1.2/README.rst
+-rw-r--r--   0        0        0     2681 2023-06-14 17:56:45.445909 philipstv-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      873 2023-06-14 17:56:45.445909 philipstv-1.1.2/src/philipstv/__init__.py
+-rw-r--r--   0        0        0      368 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/__main__.py
+-rw-r--r--   0        0        0    14775 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/_cli.py
+-rw-r--r--   0        0        0     1793 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/_data.py
+-rw-r--r--   0        0        0      410 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/_utils.py
+-rw-r--r--   0        0        0     9702 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/api.py
+-rw-r--r--   0        0        0     2836 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/exceptions.py
+-rw-r--r--   0        0        0     1692 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/model/__init__.py
+-rw-r--r--   0        0        0     3161 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/model/ambilight.py
+-rw-r--r--   0        0        0     1208 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/model/applications.py
+-rw-r--r--   0        0        0      373 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/model/audio.py
+-rw-r--r--   0        0        0     1518 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/model/base.py
+-rw-r--r--   0        0        0     2219 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/model/channels.py
+-rw-r--r--   0        0        0      293 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/model/general.py
+-rw-r--r--   0        0        0     1399 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/model/input.py
+-rw-r--r--   0        0        0     2179 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/model/pairing.py
+-rw-r--r--   0        0        0     3235 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/pairing.py
+-rw-r--r--   0        0        0        0 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/py.typed
+-rw-r--r--   0        0        0    10430 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/remote.py
+-rw-r--r--   0        0        0     3384 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/tv.py
+-rw-r--r--   0        0        0       56 2023-05-14 13:54:35.574569 philipstv-1.1.2/src/philipstv/types.py
+-rw-r--r--   0        0        0        0 2023-05-14 13:54:35.574569 philipstv-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1457 2023-05-14 13:54:35.574569 philipstv-1.1.2/tests/fakes.py
+-rw-r--r--   0        0        0    12595 2023-05-14 13:54:35.574569 philipstv-1.1.2/tests/test_api.py
+-rw-r--r--   0        0        0    10047 2023-05-14 13:54:35.574569 philipstv-1.1.2/tests/test_cli.py
+-rw-r--r--   0        0        0     2657 2023-05-14 13:54:35.574569 philipstv-1.1.2/tests/test_pairing.py
+-rw-r--r--   0        0        0     9093 2023-05-14 13:54:35.574569 philipstv-1.1.2/tests/test_remote.py
+-rw-r--r--   0        0        0     2441 2023-05-14 13:54:35.574569 philipstv-1.1.2/tests/test_tv.py
+-rw-r--r--   0        0        0     3806 1970-01-01 00:00:00.000000 philipstv-1.1.2/PKG-INFO
```

### Comparing `philipstv-1.1.1/LICENSE` & `philipstv-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/README.rst` & `philipstv-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/pyproject.toml` & `philipstv-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philipstv"
-version = "1.1.1"  # this will be set during build by poetry-dynamic-versioning
+version = "1.1.2"  # this will be set during build by poetry-dynamic-versioning
 description = "CLI and library to control Philips Android-powered TVs."
 license = "MIT"
 authors = ["Bazyli Cyran <bazyli@cyran.dev>"]
 readme = "README.rst"
 repository = "https://github.com/bcyran/philipstv"
 documentation = "https://philipstv.readthedocs.io"
 keywords = ["cli", "tv", "api-wrapper", "philips", "ambilight"]
@@ -58,15 +58,15 @@
 requests-mock = "^1.10.0"
 pytest-cov = "^4.1.0"
 types-appdirs = "^1.4.3"
 sphinx-autobuild = "^2021.3.14"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 pattern = """(?x)
 ^(?P<base>\\d+(\\.\\d+)*)
```

### Comparing `philipstv-1.1.1/src/philipstv/__init__.py` & `philipstv-1.1.2/src/philipstv/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     PhilipsTVRemoteError,
 )
 from .model import DeviceInfo
 from .pairing import PhilipsTVPairer
 from .remote import AmbilightColor, InputKeyValue, PhilipsTVRemote
 from .tv import PhilipsTV
 
-__version__ = "1.1.1"  # This will be set during build by poetry-dynamic-versioning
+__version__ = "1.1.2"  # This will be set during build by poetry-dynamic-versioning
 
 __all__ = [
     "AmbilightColor",
     "DeviceInfo",
     "InputKeyValue",
     "PhilipsError",
     "PhilipsTV",
```

### Comparing `philipstv-1.1.1/src/philipstv/_cli.py` & `philipstv-1.1.2/src/philipstv/_cli.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/src/philipstv/_data.py` & `philipstv-1.1.2/src/philipstv/_data.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/src/philipstv/api.py` & `philipstv-1.1.2/src/philipstv/api.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/src/philipstv/exceptions.py` & `philipstv-1.1.2/src/philipstv/exceptions.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/src/philipstv/model/__init__.py` & `philipstv-1.1.2/src/philipstv/model/__init__.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/src/philipstv/model/ambilight.py` & `philipstv-1.1.2/src/philipstv/model/ambilight.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/src/philipstv/model/applications.py` & `philipstv-1.1.2/src/philipstv/model/applications.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/src/philipstv/model/base.py` & `philipstv-1.1.2/src/philipstv/model/base.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/src/philipstv/model/channels.py` & `philipstv-1.1.2/src/philipstv/model/channels.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/src/philipstv/model/input.py` & `philipstv-1.1.2/src/philipstv/model/input.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/src/philipstv/model/pairing.py` & `philipstv-1.1.2/src/philipstv/model/pairing.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/src/philipstv/pairing.py` & `philipstv-1.1.2/src/philipstv/pairing.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/src/philipstv/remote.py` & `philipstv-1.1.2/src/philipstv/remote.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/src/philipstv/tv.py` & `philipstv-1.1.2/src/philipstv/tv.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/tests/fakes.py` & `philipstv-1.1.2/tests/fakes.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/tests/test_api.py` & `philipstv-1.1.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/tests/test_cli.py` & `philipstv-1.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/tests/test_pairing.py` & `philipstv-1.1.2/tests/test_pairing.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/tests/test_remote.py` & `philipstv-1.1.2/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/tests/test_tv.py` & `philipstv-1.1.2/tests/test_tv.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.1.1/PKG-INFO` & `philipstv-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philipstv
-Version: 1.1.1
+Version: 1.1.2
 Summary: CLI and library to control Philips Android-powered TVs.
 Home-page: https://github.com/bcyran/philipstv
 License: MIT
 Keywords: cli,tv,api-wrapper,philips,ambilight
 Author: Bazyli Cyran
 Author-email: bazyli@cyran.dev
 Requires-Python: >=3.9,<4.0
```

