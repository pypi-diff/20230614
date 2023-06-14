# Comparing `tmp/macrometa-source-collection-0.0.46.tar.gz` & `tmp/macrometa-source-collection-0.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.46.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.47.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.46.tar` & `macrometa-source-collection-0.0.47.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     9918 2023-06-14 11:54:54.320449 macrometa-source-collection-0.0.46/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     9500 2023-06-14 11:54:54.320449 macrometa-source-collection-0.0.46/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1626 2023-06-14 11:54:54.620452 macrometa-source-collection-0.0.46/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.46/setup.py
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.46/PKG-INFO
+-rw-r--r--   0        0        0     9918 2023-06-14 12:20:06.519391 macrometa-source-collection-0.0.47/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     9876 2023-06-14 12:20:06.519391 macrometa-source-collection-0.0.47/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1626 2023-06-14 12:20:06.767394 macrometa-source-collection-0.0.47/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.47/setup.py
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.47/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.46/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.47/macrometa_source_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.46/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.47/macrometa_source_collection/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,27 +131,34 @@
     def load_existing_data(self, stream, columns, schema_properties):
         cursor = self._c8_client._fabric.c8ql.execute(f"FOR d IN @@collection RETURN d",
                                                bind_vars={"@collection": self._collection},
                                                stream=True)
         i = 0
         while (not cursor.empty()) or cursor.has_more():
             i = i + 1
+            LOGGER.info("debug checkpoint 1 %s", i)
             rec = cursor.next()
+            LOGGER.info("debug checkpoint 2 %s", i)
             rec.pop('_id', None)
+            LOGGER.info("debug checkpoint 3 %s", i)
             rec.pop('_rev', None)
+            LOGGER.info("debug checkpoint 4 %s", i)
             # skip existing data not having valid schema
             if len(rec.keys() ^ columns) == 0 and all(
                 rec[key] is None or (isinstance(schema_properties[key].type, list) and get_singer_data_type(rec[key]) in schema_properties[key].type)
                                      or (isinstance(schema_properties[key].type, str) and get_singer_data_type(rec[key]) == schema_properties[key].type)
                 for key in rec.keys()
             ):
+                LOGGER.info("debug checkpoint 5 %s", i)
                 singer_record = self.msg_to_singer_message(stream, rec, None, utils.now())
+                LOGGER.info("debug checkpoint 6 %s", i)
                 singer.write_message(singer_record)
                 LOGGER.info("Metrics calling %s", i)
                 self.exported_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(rec))
+                LOGGER.info("debug checkpoint 7 %s", i)
                 self.exported_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 LOGGER.info("Metrics call ended %s", i)
             else:
                 LOGGER.warn("The record: %s, does not match the most common schema. Skipping it..", rec)
 
     def send_schema_message(self, stream: CatalogEntry, bookmark_properties=[]):
         schema_message = singer.SchemaMessage(stream=stream.stream,
```

### Comparing `macrometa-source-collection-0.0.46/pyproject.toml` & `macrometa-source-collection-0.0.47/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.46'
+version='0.0.47'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.46/setup.py` & `macrometa-source-collection-0.0.47/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.46',
+    'version': '0.0.47',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.46/PKG-INFO` & `macrometa-source-collection-0.0.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.46
+Version: 0.0.47
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

