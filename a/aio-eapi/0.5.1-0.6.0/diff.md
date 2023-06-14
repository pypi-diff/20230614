# Comparing `tmp/aio_eapi-0.5.1.tar.gz` & `tmp/aio_eapi-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_eapi-0.5.1.tar", max compression
+gzip compressed data, was "aio_eapi-0.6.0.tar", max compression
```

## Comparing `aio_eapi-0.5.1.tar` & `aio_eapi-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    11347 2023-01-13 17:41:18.111093 aio_eapi-0.5.1/LICENSE
--rw-r--r--   0        0        0     1379 2023-02-18 18:45:23.202233 aio_eapi-0.5.1/README.md
--rw-r--r--   0        0        0      106 2023-02-18 18:45:23.202985 aio_eapi-0.5.1/aioeapi/__init__.py
--rw-r--r--   0        0        0     8684 2023-02-18 18:45:23.203427 aio_eapi-0.5.1/aioeapi/config_session.py
--rw-r--r--   0        0        0     9954 2023-02-18 18:45:23.204190 aio_eapi-0.5.1/aioeapi/device.py
--rw-r--r--   0        0        0      894 2023-02-18 18:45:23.204799 aio_eapi-0.5.1/aioeapi/errors.py
--rw-r--r--   0        0        0      680 2023-03-15 19:47:43.418246 aio_eapi-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2032 1970-01-01 00:00:00.000000 aio_eapi-0.5.1/setup.py
--rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 aio_eapi-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11347 2023-01-13 17:41:18.111093 aio_eapi-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1379 2023-02-18 18:45:23.202233 aio_eapi-0.6.0/README.md
+-rw-r--r--   0        0        0      106 2023-02-18 18:45:23.202985 aio_eapi-0.6.0/aioeapi/__init__.py
+-rw-r--r--   0        0        0     1642 2023-03-27 19:53:04.902157 aio_eapi-0.6.0/aioeapi/aio_portcheck.py
+-rw-r--r--   0        0        0     8684 2023-02-18 18:45:23.203427 aio_eapi-0.6.0/aioeapi/config_session.py
+-rw-r--r--   0        0        0     9881 2023-03-27 19:53:15.282384 aio_eapi-0.6.0/aioeapi/device.py
+-rw-r--r--   0        0        0      894 2023-02-18 18:45:23.204799 aio_eapi-0.6.0/aioeapi/errors.py
+-rw-r--r--   0        0        0      680 2023-03-27 19:51:07.183995 aio_eapi-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2032 1970-01-01 00:00:00.000000 aio_eapi-0.6.0/setup.py
+-rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 aio_eapi-0.6.0/PKG-INFO
```

### Comparing `aio_eapi-0.5.1/LICENSE` & `aio_eapi-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_eapi-0.5.1/README.md` & `aio_eapi-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `aio_eapi-0.5.1/aioeapi/config_session.py` & `aio_eapi-0.6.0/aioeapi/config_session.py`

 * *Files identical despite different names*

### Comparing `aio_eapi-0.5.1/aioeapi/device.py` & `aio_eapi-0.6.0/aioeapi/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -----------------------------------------------------------------------------
 # System Imports
 # -----------------------------------------------------------------------------
 
-import asyncio
 from typing import Optional, List, Union, Dict, AnyStr
 from socket import getservbyname
 
 # -----------------------------------------------------------------------------
 # Public Imports
 # -----------------------------------------------------------------------------
 
 import httpx
 
 # -----------------------------------------------------------------------------
 # Private Imports
 # -----------------------------------------------------------------------------
 
+from .aio_portcheck import port_check_url
 from .errors import EapiCommandError
 from .config_session import SessionConfig
 
 # -----------------------------------------------------------------------------
 # Exports
 # -----------------------------------------------------------------------------
 
@@ -109,19 +109,15 @@
         the connection before involing cli commands, but this step is not
         required.
 
         Returns
         -------
         True when the device eAPI is accessible, False otherwise.
         """
-        try:
-            await asyncio.open_connection(self.host, port=self.port)
-        except OSError:
-            return False
-        return True
+        return await port_check_url(self.base_url)
 
     async def cli(
         self,
         command: Optional[AnyStr] = None,
         commands: Optional[List[AnyStr]] = None,
         ofmt: Optional[str] = None,
         suppress_error: Optional[bool] = False,
```

### Comparing `aio_eapi-0.5.1/aioeapi/errors.py` & `aio_eapi-0.6.0/aioeapi/errors.py`

 * *Files identical despite different names*

### Comparing `aio_eapi-0.5.1/pyproject.toml` & `aio_eapi-0.6.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-eapi"
-version = "0.5.1"
+version = "0.6.0"
 description = "Arista EOS API asyncio client"
 readme = "README.md"
 authors = ["Jeremy Schulman"]
 packages = [
     { include  = 'aioeapi' },
 ]
```

### Comparing `aio_eapi-0.5.1/setup.py` & `aio_eapi-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['httpx>=0.23.3,<0.24.0']
 
 setup_kwargs = {
     'name': 'aio-eapi',
-    'version': '0.5.1',
+    'version': '0.6.0',
     'description': 'Arista EOS API asyncio client',
     'long_description': '# Arista EOS API asyncio Client\n\nThis repository contains an Arista EOS asyncio client.\n\n### Quick Example\n\nThie following shows how to create a Device instance and run a list of\ncommands.\n\nDevice will use HTTPS transport by default.  The Device instance supports the\nfollowing initialization parameters:\n\n   * `host` - The device hostname or IP address\n   * `username` - The login username\n   * `password` - The login password\n   * `proto` - *(Optional)* Choose either "https" or "http", defaults to "https"\n   * `port` - *(Optional)* Chose the protocol port to override proto default\n\nThe Device class inherits directly from httpx.AsyncClient.  As such, the Caller\ncan provide any initialization parameters.  The above specific parameters are\nall optional.\n\n```python\nimport json\nfrom aioeapi import Device\n\nusername = \'dummy-user\'\npassword = \'dummy-password\'\n\nasync def run_test(host):\n    dev = Device(host=host, username=username, password=password)\n    res = await dev.cli(commands=[\'show hostname\', \'show version\'])\n    json.dumps(res)\n```\n\n### References\n\nArista eAPI documents require an Arista Portal customer login.  Once logged into the\nsystem you can find the documents in the Software Download area.  Select an EOS release\nand then select the Docs folder.\n\nYou can also take a look at the Arista community client, [here](https://github.com/arista-eosplus/pyeapi).\n\n',
     'author': 'Jeremy Schulman',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `aio_eapi-0.5.1/PKG-INFO` & `aio_eapi-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-eapi
-Version: 0.5.1
+Version: 0.6.0
 Summary: Arista EOS API asyncio client
 Author: Jeremy Schulman
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
```

