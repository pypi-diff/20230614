# Comparing `tmp/macrometa-source-collection-0.0.44.tar.gz` & `tmp/macrometa-source-collection-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.44.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.45.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.44.tar` & `macrometa-source-collection-0.0.45.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     9500 2023-06-13 05:27:53.052663 macrometa-source-collection-0.0.44/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     9355 2023-06-13 05:27:53.052663 macrometa-source-collection-0.0.44/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1626 2023-06-13 05:27:53.308670 macrometa-source-collection-0.0.44/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.44/setup.py
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.44/PKG-INFO
+-rw-r--r--   0        0        0     9918 2023-06-14 08:57:11.667612 macrometa-source-collection-0.0.45/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     9355 2023-06-14 08:57:11.667612 macrometa-source-collection-0.0.45/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1626 2023-06-14 08:57:11.967631 macrometa-source-collection-0.0.45/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.45/setup.py
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.45/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.44/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.45/macrometa_source_collection/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from urllib.parse import urlparse
 
 import pkg_resources
 import singer
 import time
 from c8 import C8Client
 from c8connector import C8Connector, Sample, ConfigProperty, ConfigAttributeType, Schema, SchemaAttributeType, \
-    SchemaAttribute
+    SchemaAttribute, ValidationException
 from singer import utils
 from singer.catalog import Catalog, CatalogEntry
 from singer.schema import Schema as SingerSchema
 
 from macrometa_source_collection.client import GDNCollectionClient, get_singer_data_type
 
 LOGGER = singer.get_logger('macrometa_source_collection')
@@ -51,51 +51,62 @@
         """Returns the logo image for the connector."""
         return ""
 
     def validate(self, integration: dict) -> None:
         """Validate given configurations against the connector.
         If invalid, throw an exception with the cause.
         """
-        config = self.get_config(integration)
-        C8Client(
-            "https",
-            host=config["gdn_host"],
-            port=443,
-            geofabric=config["fabric"],
-            apikey=config["api_key"]
-        ).collection(config["source_collection"])
-        pass
+        try: 
+            config = self.get_config(integration)
+            C8Client(
+                "https",
+                host=config["gdn_host"],
+                port=443,
+                geofabric=config["fabric"],
+                apikey=config["api_key"]
+            ).collection(config["source_collection"])
+        except Exception as e:
+            raise ValidationException(e)
 
     def samples(self, integration: dict) -> list[Sample]:
         """Fetch sample data using the given configurations."""
-        config = self.get_config(integration)
-        schema, data = get_schema_and_data(C8Client(
-            "https",
-            host=config["gdn_host"],
-            port=443,
-            geofabric=config["fabric"],
-            apikey=config["api_key"]
-        ), config["source_collection"], 50)
+        schema = {}
+        data = []
+        try:
+            config = self.get_config(integration)
+            schema, data = get_schema_and_data(C8Client(
+                "https",
+                host=config["gdn_host"],
+                port=443,
+                geofabric=config["fabric"],
+                apikey=config["api_key"]
+            ), config["source_collection"], 50)
+        except Exception as e:
+            raise ValidationException(e)
         data = data[:10]
         return [Sample(
             schema=Schema(config["source_collection"],
                           [SchemaAttribute(k, get_attribute_type(v)) for k, v in schema.items()]),
             data=data
         )]
 
     def schemas(self, integration: dict) -> list[Schema]:
         """Get supported schemas using the given configurations."""
-        config = self.get_config(integration)
-        schema, _ = get_schema_and_data(C8Client(
-            "https",
-            host=config["gdn_host"],
-            port=443,
-            geofabric=config["fabric"],
-            apikey=config["api_key"]
-        ), config["source_collection"], 50)
+        schema = {}
+        try:
+            config = self.get_config(integration)
+            schema, _ = get_schema_and_data(C8Client(
+                "https",
+                host=config["gdn_host"],
+                port=443,
+                geofabric=config["fabric"],
+                apikey=config["api_key"]
+            ), config["source_collection"], 50)
+        except Exception as e:
+            raise ValidationException(e)
         return [Schema(config["source_collection"],
                        [SchemaAttribute(k, get_attribute_type(v)) for k, v in schema.items()])]
 
     def reserved_keys(self) -> list[str]:
         """List of reserved keys for the connector."""
         return []
```

### Comparing `macrometa-source-collection-0.0.44/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.45/macrometa_source_collection/client.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.44/pyproject.toml` & `macrometa-source-collection-0.0.45/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.44'
+version='0.0.45'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
@@ -25,15 +25,15 @@
 packages = [
     { include = "macrometa_source_collection" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 pipelinewise-singer-python = "1.2.0"
-c8connector = ">=0.0.20"
+c8connector = ">=0.0.24"
 chardet = "4.0.0"
 idna = "2.10"
 numpy = "1.21.6"
 pandas = "1.3.5"
 pyC8 = "0.17.3"
 requests = "2.25.1"
 websocket-client = "0.57.0"
```

### Comparing `macrometa-source-collection-0.0.44/setup.py` & `macrometa-source-collection-0.0.45/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 packages = \
 ['macrometa_source_collection']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['c8connector>=0.0.20',
+['c8connector>=0.0.24',
  'chardet==4.0.0',
  'idna==2.10',
  'numpy==1.21.6',
  'pandas==1.3.5',
  'pipelinewise-singer-python==1.2.0',
  'prometheus-client==0.16.0',
  'pulsar-client==2.10.1',
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.44',
+    'version': '0.0.45',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.44/PKG-INFO` & `macrometa-source-collection-0.0.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.44
+Version: 0.0.45
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: c8connector (>=0.0.20)
+Requires-Dist: c8connector (>=0.0.24)
 Requires-Dist: chardet (==4.0.0)
 Requires-Dist: idna (==2.10)
 Requires-Dist: numpy (==1.21.6)
 Requires-Dist: pandas (==1.3.5)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
 Requires-Dist: prometheus-client (==0.16.0)
 Requires-Dist: pulsar-client (==2.10.1)
```

