# Comparing `tmp/philipstv-1.0.0.tar.gz` & `tmp/philipstv-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philipstv-1.0.0.tar", max compression
+gzip compressed data, was "philipstv-1.1.0.tar", max compression
```

## Comparing `philipstv-1.0.0.tar` & `philipstv-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1079 2022-02-20 18:17:18.454862 philipstv-1.0.0/LICENSE
--rw-r--r--   0        0        0     2393 2022-08-07 08:27:19.720961 philipstv-1.0.0/README.rst
--rw-r--r--   0        0        0     2635 2022-08-07 08:46:53.993109 philipstv-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      873 2022-08-07 08:46:53.993109 philipstv-1.0.0/src/philipstv/__init__.py
--rw-r--r--   0        0        0      368 2022-03-24 18:35:14.775505 philipstv-1.0.0/src/philipstv/__main__.py
--rw-r--r--   0        0        0    14775 2022-03-29 19:32:21.078185 philipstv-1.0.0/src/philipstv/_cli.py
--rw-r--r--   0        0        0     1793 2022-03-29 19:27:43.116568 philipstv-1.0.0/src/philipstv/_data.py
--rw-r--r--   0        0        0      410 2022-03-29 19:24:01.728685 philipstv-1.0.0/src/philipstv/_utils.py
--rw-r--r--   0        0        0     9702 2022-08-05 22:02:15.731785 philipstv-1.0.0/src/philipstv/api.py
--rw-r--r--   0        0        0     2836 2022-03-29 19:27:43.116568 philipstv-1.0.0/src/philipstv/exceptions.py
--rw-r--r--   0        0        0     1692 2022-03-29 16:14:15.296962 philipstv-1.0.0/src/philipstv/model/__init__.py
--rw-r--r--   0        0        0     3161 2022-03-29 19:32:21.078185 philipstv-1.0.0/src/philipstv/model/ambilight.py
--rw-r--r--   0        0        0     1208 2022-03-19 16:31:04.342913 philipstv-1.0.0/src/philipstv/model/applications.py
--rw-r--r--   0        0        0      373 2022-03-19 16:31:04.342913 philipstv-1.0.0/src/philipstv/model/audio.py
--rw-r--r--   0        0        0     1518 2022-03-21 18:55:38.077818 philipstv-1.0.0/src/philipstv/model/base.py
--rw-r--r--   0        0        0     2219 2022-03-19 16:31:04.342913 philipstv-1.0.0/src/philipstv/model/channels.py
--rw-r--r--   0        0        0      293 2022-03-19 16:31:04.342913 philipstv-1.0.0/src/philipstv/model/general.py
--rw-r--r--   0        0        0     1399 2022-03-29 16:14:15.296962 philipstv-1.0.0/src/philipstv/model/input.py
--rw-r--r--   0        0        0     2179 2022-03-19 16:31:04.342913 philipstv-1.0.0/src/philipstv/model/pairing.py
--rw-r--r--   0        0        0     3235 2022-03-23 19:01:51.083930 philipstv-1.0.0/src/philipstv/pairing.py
--rw-r--r--   0        0        0        0 2022-02-19 14:27:11.894844 philipstv-1.0.0/src/philipstv/py.typed
--rw-r--r--   0        0        0    10430 2022-03-29 19:27:43.116568 philipstv-1.0.0/src/philipstv/remote.py
--rw-r--r--   0        0        0     3400 2022-03-24 19:19:42.012590 philipstv-1.0.0/src/philipstv/tv.py
--rw-r--r--   0        0        0       56 2022-02-20 14:48:24.254324 philipstv-1.0.0/src/philipstv/types.py
--rw-r--r--   0        0        0        0 2022-02-20 14:37:19.114444 philipstv-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1457 2022-03-21 18:55:38.077818 philipstv-1.0.0/tests/fakes.py
--rw-r--r--   0        0        0    12595 2022-03-21 18:55:38.077818 philipstv-1.0.0/tests/test_api.py
--rw-r--r--   0        0        0    10047 2022-03-29 19:27:43.116568 philipstv-1.0.0/tests/test_cli.py
--rw-r--r--   0        0        0     2657 2022-03-23 19:01:51.083930 philipstv-1.0.0/tests/test_pairing.py
--rw-r--r--   0        0        0     9093 2022-03-29 19:32:21.078185 philipstv-1.0.0/tests/test_remote.py
--rw-r--r--   0        0        0     2441 2022-03-21 18:55:38.077818 philipstv-1.0.0/tests/test_tv.py
--rw-r--r--   0        0        0     3612 2022-08-07 08:46:54.271595 philipstv-1.0.0/setup.py
--rw-r--r--   0        0        0     3736 2022-08-07 08:46:54.271922 philipstv-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2022-02-20 18:17:18.454862 philipstv-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2393 2022-12-18 10:16:52.270295 philipstv-1.1.0/README.rst
+-rw-r--r--   0        0        0     2674 2023-01-15 11:54:40.773615 philipstv-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      873 2023-01-15 11:54:40.773615 philipstv-1.1.0/src/philipstv/__init__.py
+-rw-r--r--   0        0        0      368 2022-03-24 18:35:14.775505 philipstv-1.1.0/src/philipstv/__main__.py
+-rw-r--r--   0        0        0    14775 2022-03-29 19:32:21.078185 philipstv-1.1.0/src/philipstv/_cli.py
+-rw-r--r--   0        0        0     1793 2022-03-29 19:27:43.116568 philipstv-1.1.0/src/philipstv/_data.py
+-rw-r--r--   0        0        0      410 2022-03-29 19:24:01.728685 philipstv-1.1.0/src/philipstv/_utils.py
+-rw-r--r--   0        0        0     9702 2022-08-05 22:02:15.731785 philipstv-1.1.0/src/philipstv/api.py
+-rw-r--r--   0        0        0     2836 2022-03-29 19:27:43.116568 philipstv-1.1.0/src/philipstv/exceptions.py
+-rw-r--r--   0        0        0     1692 2022-03-29 16:14:15.296962 philipstv-1.1.0/src/philipstv/model/__init__.py
+-rw-r--r--   0        0        0     3161 2022-03-29 19:32:21.078185 philipstv-1.1.0/src/philipstv/model/ambilight.py
+-rw-r--r--   0        0        0     1208 2022-03-19 16:31:04.342913 philipstv-1.1.0/src/philipstv/model/applications.py
+-rw-r--r--   0        0        0      373 2022-03-19 16:31:04.342913 philipstv-1.1.0/src/philipstv/model/audio.py
+-rw-r--r--   0        0        0     1518 2022-03-21 18:55:38.077818 philipstv-1.1.0/src/philipstv/model/base.py
+-rw-r--r--   0        0        0     2219 2022-03-19 16:31:04.342913 philipstv-1.1.0/src/philipstv/model/channels.py
+-rw-r--r--   0        0        0      293 2022-03-19 16:31:04.342913 philipstv-1.1.0/src/philipstv/model/general.py
+-rw-r--r--   0        0        0     1399 2022-03-29 16:14:15.296962 philipstv-1.1.0/src/philipstv/model/input.py
+-rw-r--r--   0        0        0     2179 2022-03-19 16:31:04.342913 philipstv-1.1.0/src/philipstv/model/pairing.py
+-rw-r--r--   0        0        0     3235 2022-03-23 19:01:51.083930 philipstv-1.1.0/src/philipstv/pairing.py
+-rw-r--r--   0        0        0        0 2022-02-19 14:27:11.894844 philipstv-1.1.0/src/philipstv/py.typed
+-rw-r--r--   0        0        0    10430 2022-03-29 19:27:43.116568 philipstv-1.1.0/src/philipstv/remote.py
+-rw-r--r--   0        0        0     3384 2022-12-18 10:16:52.273628 philipstv-1.1.0/src/philipstv/tv.py
+-rw-r--r--   0        0        0       56 2022-02-20 14:48:24.254324 philipstv-1.1.0/src/philipstv/types.py
+-rw-r--r--   0        0        0        0 2022-02-20 14:37:19.114444 philipstv-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1457 2022-03-21 18:55:38.077818 philipstv-1.1.0/tests/fakes.py
+-rw-r--r--   0        0        0    12595 2022-03-21 18:55:38.077818 philipstv-1.1.0/tests/test_api.py
+-rw-r--r--   0        0        0    10047 2022-03-29 19:27:43.116568 philipstv-1.1.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2657 2022-03-23 19:01:51.083930 philipstv-1.1.0/tests/test_pairing.py
+-rw-r--r--   0        0        0     9093 2022-03-29 19:32:21.078185 philipstv-1.1.0/tests/test_remote.py
+-rw-r--r--   0        0        0     2441 2022-03-21 18:55:38.077818 philipstv-1.1.0/tests/test_tv.py
+-rw-r--r--   0        0        0     3616 1970-01-01 00:00:00.000000 philipstv-1.1.0/setup.py
+-rw-r--r--   0        0        0     3957 1970-01-01 00:00:00.000000 philipstv-1.1.0/PKG-INFO
```

### Comparing `philipstv-1.0.0/LICENSE` & `philipstv-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/README.rst` & `philipstv-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/pyproject.toml` & `philipstv-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "philipstv"
-version = "1.0.0"  # this will be set during build by poetry-dynamic-versioning
+version = "1.1.0"  # this will be set during build by poetry-dynamic-versioning
 description = "CLI and library to control Philips Android-powered TVs."
 license = "MIT"
 authors = ["Bazyli Cyran <bazyli@cyran.dev>"]
 readme = "README.rst"
 repository = "https://github.com/bcyran/philipstv"
 documentation = "https://philipstv.readthedocs.io"
 keywords = ["cli", "tv", "api-wrapper", "philips", "ambilight"]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Typing :: Typed"
 ]
 packages = [
     { include = "philipstv", from = "src"}
 ]
 include = [
     { path = "src/philipstv/**/*.py" },
@@ -43,25 +44,24 @@
 enum-tools = {extras = ["sphinx"], version = "^0.9.0", optional = true }
 
 [tool.poetry.extras]
 cli = ["click", "appdirs"]
 docs = ["sphinx", "furo", "enum-tools"]
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.0.0"
-black = "^22.1.0"
-mypy = "^0.931"
-flake8 = "^4.0.1"
-isort = "^5.10.1"
-tox = "^3.24.5"
-types-requests = "^2.27.8"
-tox-poetry = "^0.4.1"
-requests-mock = "^1.9.3"
-pytest-cov = "^3.0.0"
-types-appdirs = "^1.4.2"
+pytest = "^7.2.0"
+black = "^22.12.0"
+mypy = "^0.991"
+flake8 = "^6.0.0"
+isort = "^5.11.4"
+tox = "^4.2.8"
+types-requests = "^2.28.11"
+requests-mock = "^1.10.0"
+pytest-cov = "^4.0.0"
+types-appdirs = "^1.4.3"
 sphinx-autobuild = "^2021.3.14"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry-dynamic-versioning]
```

### Comparing `philipstv-1.0.0/src/philipstv/__init__.py` & `philipstv-1.1.0/src/philipstv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     PhilipsTVRemoteError,
 )
 from .model import DeviceInfo
 from .pairing import PhilipsTVPairer
 from .remote import AmbilightColor, InputKeyValue, PhilipsTVRemote
 from .tv import PhilipsTV
 
-__version__ = "1.0.0"  # This will be set during build by poetry-dynamic-versioning
+__version__ = "1.1.0"  # This will be set during build by poetry-dynamic-versioning
 
 __all__ = [
     "AmbilightColor",
     "DeviceInfo",
     "InputKeyValue",
     "PhilipsError",
     "PhilipsTV",
```

### Comparing `philipstv-1.0.0/src/philipstv/_cli.py` & `philipstv-1.1.0/src/philipstv/_cli.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/src/philipstv/_data.py` & `philipstv-1.1.0/src/philipstv/_data.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/src/philipstv/api.py` & `philipstv-1.1.0/src/philipstv/api.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/src/philipstv/exceptions.py` & `philipstv-1.1.0/src/philipstv/exceptions.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/src/philipstv/model/__init__.py` & `philipstv-1.1.0/src/philipstv/model/__init__.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/src/philipstv/model/ambilight.py` & `philipstv-1.1.0/src/philipstv/model/ambilight.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/src/philipstv/model/applications.py` & `philipstv-1.1.0/src/philipstv/model/applications.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/src/philipstv/model/base.py` & `philipstv-1.1.0/src/philipstv/model/base.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/src/philipstv/model/channels.py` & `philipstv-1.1.0/src/philipstv/model/channels.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/src/philipstv/model/input.py` & `philipstv-1.1.0/src/philipstv/model/input.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/src/philipstv/model/pairing.py` & `philipstv-1.1.0/src/philipstv/model/pairing.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/src/philipstv/pairing.py` & `philipstv-1.1.0/src/philipstv/pairing.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/src/philipstv/remote.py` & `philipstv-1.1.0/src/philipstv/remote.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/src/philipstv/tv.py` & `philipstv-1.1.0/src/philipstv/tv.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from requests import RequestException, Session
 from requests.auth import HTTPDigestAuth
 from urllib3.exceptions import InsecureRequestWarning
 
 from .exceptions import PhilipsTVError
 from .types import Credentials
 
-urllib3.disable_warnings(InsecureRequestWarning)  # type: ignore
+urllib3.disable_warnings(InsecureRequestWarning)
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 @contextmanager
 def _wrap_http_exceptions() -> Iterator[None]:
```

### Comparing `philipstv-1.0.0/tests/fakes.py` & `philipstv-1.1.0/tests/fakes.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/tests/test_api.py` & `philipstv-1.1.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/tests/test_cli.py` & `philipstv-1.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/tests/test_pairing.py` & `philipstv-1.1.0/tests/test_pairing.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/tests/test_remote.py` & `philipstv-1.1.0/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/tests/test_tv.py` & `philipstv-1.1.0/tests/test_tv.py`

 * *Files identical despite different names*

### Comparing `philipstv-1.0.0/setup.py` & `philipstv-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,21 +20,21 @@
           'enum-tools[sphinx]>=0.9.0,<0.10.0']}
 
 entry_points = \
 {'console_scripts': ['philipstv = philipstv.__main__:wrapped_cli']}
 
 setup_kwargs = {
     'name': 'philipstv',
-    'version': '1.0.0',
+    'version': '1.1.0',
     'description': 'CLI and library to control Philips Android-powered TVs.',
     'long_description': "philipstv\n=========\n\n.. image:: https://github.com/bcyran/philipstv/workflows/CI/badge.svg?event=push\n   :target: https://github.com/bcyran/philipstv/actions?query=event%3Apush+branch%3Amaster+workflow%3ACI\n   :alt: CI\n\n.. image:: https://codecov.io/gh/bcyran/philipstv/branch/master/graph/badge.svg?token=ROJONX34RB\n   :target: https://codecov.io/gh/bcyran/philipstv\n   :alt: codecov\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Code style: black\n\n.. image:: https://img.shields.io/pypi/v/philipstv\n   :target: https://pypi.org/project/philipstv/\n   :alt: pypi\n\n.. image:: https://readthedocs.org/projects/philipstv/badge/?version=latest\n   :target: https://philipstv.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation status\n\n.. image:: https://img.shields.io/pypi/pyversions/philipstv\n   :target: https://pypi.org/project/philipstv/\n   :alt: versions\n\n.. image:: https://img.shields.io/github/license/bcyran/philipstv\n   :target: https://github.com/bcyran/philipstv/blob/master/LICENSE\n   :alt: license\n\n.. -begin-intro-\n\nPython package providing CLI and library for interacting with Philips Android-powered TVs.\n\nFeatures:\n\n- Get and set TV power state.\n- Get and set volume.\n- List and change TV channels.\n- Emulate pressing remote keys.\n- Get and set Ambilight power state.\n- Get and set Ambilight color.\n- List and launch applications.\n\nInstallation\n------------\n\nPyPI\n^^^^\n\nIf you plan to use the CLI:\n\n.. code-block:: console\n\n   $ pip install 'philipstv[cli]'\n\nIf you only need library for use in Python code:\n\n.. code-block:: console\n\n   $ pip install philipstv\n\n.. -end-intro-\n\nArch Linux (AUR)\n^^^^^^^^^^^^^^^^\n\n`philipstv AUR package <https://aur.archlinux.org/packages/philipstv>`_ is available.\n\n\nDocumentation\n-------------\nSee full documentation: `Read the Docs: philipstv <https://philipstv.readthedocs.io>`_.\n\nSee also\n--------\n- `PhilipsTV GUI <https://github.com/bcyran/philipstv-gui>`_ - GUI application built with this library.\n\nResources\n---------\n- `Fantastic unofficial API documentation <https://github.com/eslavnov/pylips/blob/master/docs/Home.md>`_ and `script <https://github.com/eslavnov/pylips>`_ by `@eslavnov <https://github.com/eslavnov>`_.\n- Philips `JointSpace API documentation <http://jointspace.sourceforge.net/projectdata/documentation/jasonApi/1/doc/API.html>`_.\n",
     'author': 'Bazyli Cyran',
     'author_email': 'bazyli@cyran.dev',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/bcyran/philipstv',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
```

### Comparing `philipstv-1.0.0/PKG-INFO` & `philipstv-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: philipstv
-Version: 1.0.0
+Version: 1.1.0
 Summary: CLI and library to control Philips Android-powered TVs.
 Home-page: https://github.com/bcyran/philipstv
 License: MIT
 Keywords: cli,tv,api-wrapper,philips,ambilight
 Author: Bazyli Cyran
 Author-email: bazyli@cyran.dev
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Provides-Extra: cli
 Provides-Extra: docs
-Requires-Dist: Sphinx (>=4.4.0,<5.0.0); extra == "docs"
-Requires-Dist: appdirs (>=1.4.4,<2.0.0); extra == "cli"
-Requires-Dist: click (>=8.0.3,<9.0.0); extra == "cli"
-Requires-Dist: enum-tools[sphinx] (>=0.9.0,<0.10.0); extra == "docs"
-Requires-Dist: furo (>=2022.2.14,<2023.0.0); extra == "docs"
+Requires-Dist: Sphinx (>=4.4.0,<5.0.0) ; extra == "docs"
+Requires-Dist: appdirs (>=1.4.4,<2.0.0) ; extra == "cli"
+Requires-Dist: click (>=8.0.3,<9.0.0) ; extra == "cli"
+Requires-Dist: enum-tools[sphinx] (>=0.9.0,<0.10.0) ; extra == "docs"
+Requires-Dist: furo (>=2022.2.14,<2023.0.0) ; extra == "docs"
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Project-URL: Documentation, https://philipstv.readthedocs.io
 Project-URL: Repository, https://github.com/bcyran/philipstv
 Description-Content-Type: text/x-rst
 
 philipstv
```

