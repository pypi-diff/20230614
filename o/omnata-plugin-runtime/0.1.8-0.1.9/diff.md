# Comparing `tmp/omnata_plugin_runtime-0.1.8.tar.gz` & `tmp/omnata_plugin_runtime-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnata_plugin_runtime-0.1.8.tar", max compression
+gzip compressed data, was "omnata_plugin_runtime-0.1.9.tar", max compression
```

## Comparing `omnata_plugin_runtime-0.1.8.tar` & `omnata_plugin_runtime-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    26526 2023-06-05 05:05:22.302320 omnata_plugin_runtime-0.1.8/LICENSE
--rw-r--r--   0        0        0      296 2023-06-05 05:05:22.302320 omnata_plugin_runtime-0.1.8/README.md
--rw-r--r--   0        0        0      826 2023-06-05 05:05:22.302320 omnata_plugin_runtime-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1213 2023-06-05 05:05:22.302320 omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/__init__.py
--rw-r--r--   0        0        0     3277 2023-06-05 05:05:22.302320 omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/api.py
--rw-r--r--   0        0        0    29524 2023-06-05 05:05:22.302320 omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/configuration.py
--rw-r--r--   0        0        0    12646 2023-06-05 05:05:22.302320 omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/forms.py
--rw-r--r--   0        0        0     4134 2023-06-05 05:05:22.302320 omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/logging.py
--rw-r--r--   0        0        0    64614 2023-06-05 05:05:22.302320 omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/omnata_plugin.py
--rw-r--r--   0        0        0    18397 2023-06-05 05:05:22.302320 omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/plugin_entrypoints.py
--rw-r--r--   0        0        0    10078 2023-06-05 05:05:22.302320 omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/rate_limiting.py
--rw-r--r--   0        0        0     2611 2023-06-05 05:05:22.302320 omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/record_transformer.py
--rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 omnata_plugin_runtime-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-05 08:49:16.142835 omnata_plugin_runtime-0.1.9/LICENSE
+-rw-r--r--   0        0        0      296 2023-06-05 08:49:16.142835 omnata_plugin_runtime-0.1.9/README.md
+-rw-r--r--   0        0        0      826 2023-06-05 08:49:16.142835 omnata_plugin_runtime-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1213 2023-06-05 08:49:16.146835 omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/__init__.py
+-rw-r--r--   0        0        0     3275 2023-06-05 08:49:16.146835 omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/api.py
+-rw-r--r--   0        0        0    29524 2023-06-05 08:49:16.146835 omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/configuration.py
+-rw-r--r--   0        0        0    12646 2023-06-05 08:49:16.146835 omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/forms.py
+-rw-r--r--   0        0        0     4134 2023-06-05 08:49:16.146835 omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/logging.py
+-rw-r--r--   0        0        0    64614 2023-06-05 08:49:16.146835 omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/omnata_plugin.py
+-rw-r--r--   0        0        0    18392 2023-06-05 08:49:16.146835 omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/plugin_entrypoints.py
+-rw-r--r--   0        0        0    10078 2023-06-05 08:49:16.146835 omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/rate_limiting.py
+-rw-r--r--   0        0        0     2611 2023-06-05 08:49:16.146835 omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/record_transformer.py
+-rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 omnata_plugin_runtime-0.1.9/PKG-INFO
```

### Comparing `omnata_plugin_runtime-0.1.8/LICENSE` & `omnata_plugin_runtime-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.8/pyproject.toml` & `omnata_plugin_runtime-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omnata-plugin-runtime"
-version = "0.1.8"
+version = "0.1.9"
 description = "A development kit to assist with building, testing and publishing Omnata Plugins"
 authors = ["James Weakley <james.weakley@omnata.com>"]
 readme = "README.md"
 packages = [{include = "omnata_plugin_runtime", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/__init__.py` & `omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/api.py` & `omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 else:
     # Python 3.8 and below
     from typing_extensions import Annotated
 
 from pydantic import BaseModel,Field # pylint: disable=no-name-in-module
 from typing import Optional, Dict, List, Literal, Union
 from .rate_limiting import ApiLimits, RateLimitState
-from .configuration import InboundSyncStreamsConfiguration, OutboundSyncStrategy, StoredConfigurationValue, StoredFieldMappings
+from .configuration import InboundSyncStreamsConfiguration, OutboundSyncStrategy, StoredConfigurationValue, StoredMappingValue
 from .omnata_plugin import PluginManifest
 
 class OutboundApplyPayload(BaseModel):
     """
     Encapsulates the payload that is sent to the plugin when it is invoked to perform an outbound sync.
     """
     sync_id:int # only used by log handler
@@ -29,15 +29,15 @@
     oauth_secret_name:Optional[str]
     other_secrets_name:Optional[str]
     sync_direction:Literal["outbound"] = 'outbound'
     sync_strategy:OutboundSyncStrategy
     sync_parameters:Dict[str,StoredConfigurationValue]
     api_limit_overrides:List[ApiLimits]
     rate_limits_state:Dict[str, RateLimitState]
-    field_mappings:StoredFieldMappings
+    field_mappings:StoredMappingValue
 
 class InboundApplyPayload(BaseModel):
     """
     Encapsulates the payload that is sent to the plugin when it is invoked to perform an inbound sync.
     """
     sync_id:int # only used by log handler
     sync_branch_id:Optional[int] # only used by log handler
```

### Comparing `omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/configuration.py` & `omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/configuration.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/forms.py` & `omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/forms.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/logging.py` & `omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/logging.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/omnata_plugin.py` & `omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/omnata_plugin.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/plugin_entrypoints.py` & `omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/plugin_entrypoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         
     def connection_form(self):
         try:
             logger.info('Entered connection_form method')
             form:List[ConnectionMethod] = self._plugin_instance.connection_form()
             return [f.dict() for f in form]
         except Exception as exception:
-            logger.error(str(exception),exc_info=True,stack_info=True)
+            logger.error(exception,exc_info=True,stack_info=True)
             return {
                 "success": False,
                 "error": str(exception)
             }
 
     def get_secrets(self,oauth_secret_name:Optional[str],other_secrets_name:Optional[str]) -> Dict[str,StoredConfigurationValue]:
         connection_secrets={}
```

### Comparing `omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/rate_limiting.py` & `omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.8/src/omnata_plugin_runtime/record_transformer.py` & `omnata_plugin_runtime-0.1.9/src/omnata_plugin_runtime/record_transformer.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.8/PKG-INFO` & `omnata_plugin_runtime-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnata-plugin-runtime
-Version: 0.1.8
+Version: 0.1.9
 Summary: A development kit to assist with building, testing and publishing Omnata Plugins
 Author: James Weakley
 Author-email: james.weakley@omnata.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

