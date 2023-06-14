# Comparing `tmp/connect-eaas-core-4.0.0.tar.gz` & `tmp/connect-eaas-core-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect-eaas-core-4.0.0.tar", max compression
+gzip compressed data, was "connect-eaas-core-4.1.0.tar", max compression
```

## Comparing `connect-eaas-core-4.0.0.tar` & `connect-eaas-core-4.1.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0    11357 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/LICENSE
--rw-r--r--   0        0        0        0 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/README.md
--rw-r--r--   0        0        0        0 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/connect/eaas/core/__init__.py
--rw-r--r--   0        0        0      447 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/connect/eaas/core/constants.py
--rw-r--r--   0        0        0     3032 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/connect/eaas/core/decorators.py
--rw-r--r--   0        0        0     1833 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/connect/eaas/core/enums.py
--rw-r--r--   0        0        0     3893 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/connect/eaas/core/extension.py
--rw-r--r--   0        0        0        0 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/connect/eaas/core/inject/__init__.py
--rw-r--r--   0        0        0     2133 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/connect/eaas/core/inject/asynchronous.py
--rw-r--r--   0        0        0     1522 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/connect/eaas/core/inject/common.py
--rw-r--r--   0        0        0      249 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/connect/eaas/core/inject/models.py
--rw-r--r--   0        0        0     2085 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/connect/eaas/core/inject/synchronous.py
--rw-r--r--   0        0        0     2055 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/connect/eaas/core/logging.py
--rw-r--r--   0        0        0     9436 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/connect/eaas/core/proto.py
--rw-r--r--   0        0        0     2394 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/connect/eaas/core/responses.py
--rw-r--r--   0        0        0      830 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/connect/eaas/core/testing.py
--rw-r--r--   0        0        0    19768 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/connect/eaas/core/validation/extension_validations.py
--rw-r--r--   0        0        0     1869 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/connect/eaas/core/validation/helpers.py
--rw-r--r--   0        0        0      412 2022-09-28 15:15:46.765893 connect-eaas-core-4.0.0/connect/eaas/core/validation/proto.py
--rw-r--r--   0        0        0     2006 2022-09-28 15:17:01.658103 connect-eaas-core-4.0.0/pyproject.toml
--rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 connect-eaas-core-4.0.0/setup.py
--rw-r--r--   0        0        0     1270 1970-01-01 00:00:00.000000 connect-eaas-core-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-10-04 09:26:54.539310 connect-eaas-core-4.1.0/LICENSE
+-rw-r--r--   0        0        0        0 2022-10-04 09:26:54.539310 connect-eaas-core-4.1.0/README.md
+-rw-r--r--   0        0        0        0 2022-10-04 09:26:54.539310 connect-eaas-core-4.1.0/connect/eaas/core/__init__.py
+-rw-r--r--   0        0        0      447 2022-10-04 09:26:54.539310 connect-eaas-core-4.1.0/connect/eaas/core/constants.py
+-rw-r--r--   0        0        0     3032 2022-10-04 09:26:54.539310 connect-eaas-core-4.1.0/connect/eaas/core/decorators.py
+-rw-r--r--   0        0        0     1833 2022-10-04 09:26:54.539310 connect-eaas-core-4.1.0/connect/eaas/core/enums.py
+-rw-r--r--   0        0        0     3893 2022-10-04 09:26:54.539310 connect-eaas-core-4.1.0/connect/eaas/core/extension.py
+-rw-r--r--   0        0        0        0 2022-10-04 09:26:54.539310 connect-eaas-core-4.1.0/connect/eaas/core/inject/__init__.py
+-rw-r--r--   0        0        0     1723 2022-10-04 09:26:54.539310 connect-eaas-core-4.1.0/connect/eaas/core/inject/asynchronous.py
+-rw-r--r--   0        0        0     1618 2022-10-04 09:26:54.539310 connect-eaas-core-4.1.0/connect/eaas/core/inject/common.py
+-rw-r--r--   0        0        0      249 2022-10-04 09:26:54.539310 connect-eaas-core-4.1.0/connect/eaas/core/inject/models.py
+-rw-r--r--   0        0        0     1692 2022-10-04 09:26:54.539310 connect-eaas-core-4.1.0/connect/eaas/core/inject/synchronous.py
+-rw-r--r--   0        0        0     2055 2022-10-04 09:26:54.539310 connect-eaas-core-4.1.0/connect/eaas/core/logging.py
+-rw-r--r--   0        0        0     9436 2022-10-04 09:26:54.539310 connect-eaas-core-4.1.0/connect/eaas/core/proto.py
+-rw-r--r--   0        0        0     2394 2022-10-04 09:26:54.539310 connect-eaas-core-4.1.0/connect/eaas/core/responses.py
+-rw-r--r--   0        0        0      830 2022-10-04 09:26:54.543310 connect-eaas-core-4.1.0/connect/eaas/core/testing.py
+-rw-r--r--   0        0        0      603 2022-10-04 09:26:54.543310 connect-eaas-core-4.1.0/connect/eaas/core/validation/helpers.py
+-rw-r--r--   0        0        0      412 2022-10-04 09:26:54.543310 connect-eaas-core-4.1.0/connect/eaas/core/validation/models.py
+-rw-r--r--   0        0        0      697 2022-10-04 09:26:54.543310 connect-eaas-core-4.1.0/connect/eaas/core/validation/validators/__init__.py
+-rw-r--r--   0        0        0     2288 2022-10-04 09:26:54.543310 connect-eaas-core-4.1.0/connect/eaas/core/validation/validators/anvilapp.py
+-rw-r--r--   0        0        0    10194 2022-10-04 09:26:54.543310 connect-eaas-core-4.1.0/connect/eaas/core/validation/validators/base.py
+-rw-r--r--   0        0        0     5458 2022-10-04 09:26:54.543310 connect-eaas-core-4.1.0/connect/eaas/core/validation/validators/eventsapp.py
+-rw-r--r--   0        0        0     8709 2022-10-04 09:26:54.543310 connect-eaas-core-4.1.0/connect/eaas/core/validation/validators/webapp.py
+-rw-r--r--   0        0        0     2006 2022-10-04 09:28:10.616296 connect-eaas-core-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 connect-eaas-core-4.1.0/setup.py
+-rw-r--r--   0        0        0     1270 1970-01-01 00:00:00.000000 connect-eaas-core-4.1.0/PKG-INFO
```

### Comparing `connect-eaas-core-4.0.0/LICENSE` & `connect-eaas-core-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connect-eaas-core-4.0.0/connect/eaas/core/decorators.py` & `connect-eaas-core-4.1.0/connect/eaas/core/decorators.py`

 * *Files identical despite different names*

### Comparing `connect-eaas-core-4.0.0/connect/eaas/core/enums.py` & `connect-eaas-core-4.1.0/connect/eaas/core/enums.py`

 * *Files identical despite different names*

### Comparing `connect-eaas-core-4.0.0/connect/eaas/core/extension.py` & `connect-eaas-core-4.1.0/connect/eaas/core/extension.py`

 * *Files identical despite different names*

### Comparing `connect-eaas-core-4.0.0/connect/eaas/core/inject/asynchronous.py` & `connect-eaas-core-4.1.0/connect/eaas/core/inject/synchronous.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import os
 from logging import Logger
 
 from fastapi import Depends, Header
 
-from connect.client import AsyncConnectClient
+from connect.client import ConnectClient
 from connect.eaas.core.inject.common import get_logger
 from connect.eaas.core.logging import RequestLogger
 
 
 def get_installation_client(
     logger: Logger = Depends(get_logger),
     x_connect_installation_api_key: str = Header(),
     x_connect_api_gateway_url: str = Header(),
     x_connect_user_agent: str = Header(),
     x_connect_correlation_id: str = Header(None),
 ):
+
     default_headers = {
         'User-Agent': x_connect_user_agent,
     }
     if x_connect_correlation_id:
         default_headers['traceparent'] = x_connect_correlation_id
 
-    return AsyncConnectClient(
+    return ConnectClient(
         x_connect_installation_api_key,
         endpoint=x_connect_api_gateway_url,
         use_specs=False,
         default_headers=default_headers,
         logger=RequestLogger(logger),
     )
 
@@ -38,33 +39,21 @@
 ):
     default_headers = {
         'User-Agent': x_connect_user_agent,
     }
     if x_connect_correlation_id:
         default_headers['traceparent'] = x_connect_correlation_id
 
-    return AsyncConnectClient(
+    return ConnectClient(
         os.getenv('API_KEY'),
         endpoint=x_connect_api_gateway_url,
         use_specs=False,
         default_headers=default_headers,
         logger=RequestLogger(logger),
     )
 
 
-async def get_installation(
-    client: AsyncConnectClient = Depends(get_installation_client),
+def get_installation(
+    client: ConnectClient = Depends(get_installation_client),
     x_connect_installation_id: str = Header(),
 ):
-    return await client("devops").installations[x_connect_installation_id].get()
-
-
-async def get_environment(
-    client: AsyncConnectClient = Depends(get_extension_client),
-    x_connect_extension_id: str = Header(),
-    x_connect_environment_id: str = Header(),
-):
-    extension = client('devops').services[x_connect_extension_id]
-    return {
-        variable['name']: variable['value']
-        async for variable in extension.environments[x_connect_environment_id].variables.all()
-    }
+    return client('devops').installations[x_connect_installation_id].get()
```

### Comparing `connect-eaas-core-4.0.0/connect/eaas/core/inject/common.py` & `connect-eaas-core-4.1.0/connect/eaas/core/inject/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,7 +46,11 @@
     logger.setLevel(
         getattr(logging, x_connect_logging_level),
     )
     return logging.LoggerAdapter(
         logger,
         context.dict(),
     )
+
+
+def get_config(x_connect_config: str = Header('{}')):
+    return json.loads(x_connect_config)
```

### Comparing `connect-eaas-core-4.0.0/connect/eaas/core/logging.py` & `connect-eaas-core-4.1.0/connect/eaas/core/logging.py`

 * *Files identical despite different names*

### Comparing `connect-eaas-core-4.0.0/connect/eaas/core/proto.py` & `connect-eaas-core-4.1.0/connect/eaas/core/proto.py`

 * *Files identical despite different names*

### Comparing `connect-eaas-core-4.0.0/connect/eaas/core/responses.py` & `connect-eaas-core-4.1.0/connect/eaas/core/responses.py`

 * *Files identical despite different names*

### Comparing `connect-eaas-core-4.0.0/connect/eaas/core/testing.py` & `connect-eaas-core-4.1.0/connect/eaas/core/testing.py`

 * *Files identical despite different names*

### Comparing `connect-eaas-core-4.0.0/pyproject.toml` & `connect-eaas-core-4.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connect-eaas-core"
-version = "4.0.0"
+version = "4.1.0"
 description = "Connect Eaas Core"
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 packages = [
     { include = "connect" },
 ]
 readme = "./README.md"
```

### Comparing `connect-eaas-core-4.0.0/setup.py` & `connect-eaas-core-4.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['connect',
  'connect.eaas.core',
  'connect.eaas.core.inject',
- 'connect.eaas.core.validation']
+ 'connect.eaas.core.validation',
+ 'connect.eaas.core.validation.validators']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['anvil-uplink>=0.4.0,<0.5.0',
  'connect-openapi-client>=25.10',
  'fastapi-utils>=0.2.1,<0.3.0',
  'fastapi>=0.78.0,<0.79.0',
  'logzio-python-handler>=3.1.1,<4.0.0',
  'pydantic>=1.9.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'connect-eaas-core',
-    'version': '4.0.0',
+    'version': '4.1.0',
     'description': 'Connect Eaas Core',
     'long_description': '',
     'author': 'CloudBlue LLC',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://connect.cloudblue.com',
```

### Comparing `connect-eaas-core-4.0.0/PKG-INFO` & `connect-eaas-core-4.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connect-eaas-core
-Version: 4.0.0
+Version: 4.1.0
 Summary: Connect Eaas Core
 Home-page: https://connect.cloudblue.com
 License: Apache-2.0
 Author: CloudBlue LLC
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

