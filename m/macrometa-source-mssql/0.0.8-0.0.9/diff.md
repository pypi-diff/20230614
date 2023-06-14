# Comparing `tmp/macrometa-source-mssql-0.0.8.tar.gz` & `tmp/macrometa-source-mssql-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mssql-0.0.8.tar", max compression
+gzip compressed data, was "macrometa-source-mssql-0.0.9.tar", max compression
```

## Comparing `macrometa-source-mssql-0.0.8.tar` & `macrometa-source-mssql-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11899 2023-05-18 11:18:43.334210 macrometa-source-mssql-0.0.8/LICENSE
--rw-r--r--   0        0        0    34837 2023-05-18 11:18:43.334210 macrometa-source-mssql-0.0.8/macrometa_source_mssql/__init__.py
--rwxr-xr-x   0        0        0     1476 2023-05-18 11:18:43.334210 macrometa-source-mssql-0.0.8/macrometa_source_mssql/connection.py
--rw-r--r--   0        0        0     2287 2023-05-18 11:18:43.334210 macrometa-source-mssql-0.0.8/macrometa_source_mssql/sample_data.py
--rwxr-xr-x   0        0        0        0 2023-05-18 11:18:43.334210 macrometa-source-mssql-0.0.8/macrometa_source_mssql/sync_strategies/__init__.py
--rwxr-xr-x   0        0        0     8025 2023-05-18 11:18:43.334210 macrometa-source-mssql-0.0.8/macrometa_source_mssql/sync_strategies/common.py
--rwxr-xr-x   0        0        0     2206 2023-05-18 11:18:43.334210 macrometa-source-mssql-0.0.8/macrometa_source_mssql/sync_strategies/full_table.py
--rw-r--r--   0        0        0    14533 2023-05-18 11:18:43.334210 macrometa-source-mssql-0.0.8/macrometa_source_mssql/sync_strategies/log_based.py
--rw-r--r--   0        0        0     1537 2023-05-18 11:18:43.578209 macrometa-source-mssql-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.8/setup.py
--rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-05-18 12:22:30.947407 macrometa-source-mssql-0.0.9/LICENSE
+-rw-r--r--   0        0        0    35000 2023-05-18 12:22:30.951407 macrometa-source-mssql-0.0.9/macrometa_source_mssql/__init__.py
+-rwxr-xr-x   0        0        0     1476 2023-05-18 12:22:30.951407 macrometa-source-mssql-0.0.9/macrometa_source_mssql/connection.py
+-rw-r--r--   0        0        0     2287 2023-05-18 12:22:30.951407 macrometa-source-mssql-0.0.9/macrometa_source_mssql/sample_data.py
+-rwxr-xr-x   0        0        0        0 2023-05-18 12:22:30.951407 macrometa-source-mssql-0.0.9/macrometa_source_mssql/sync_strategies/__init__.py
+-rwxr-xr-x   0        0        0     8025 2023-05-18 12:22:30.951407 macrometa-source-mssql-0.0.9/macrometa_source_mssql/sync_strategies/common.py
+-rwxr-xr-x   0        0        0     2206 2023-05-18 12:22:30.951407 macrometa-source-mssql-0.0.9/macrometa_source_mssql/sync_strategies/full_table.py
+-rw-r--r--   0        0        0    14533 2023-05-18 12:22:30.951407 macrometa-source-mssql-0.0.9/macrometa_source_mssql/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     1537 2023-05-18 12:22:31.239440 macrometa-source-mssql-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.9/setup.py
+-rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.9/PKG-INFO
```

### Comparing `macrometa-source-mssql-0.0.8/LICENSE` & `macrometa-source-mssql-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.8/macrometa_source_mssql/__init__.py` & `macrometa-source-mssql-0.0.9/macrometa_source_mssql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -746,18 +746,23 @@
     log_based.add_synthetic_keys_to_schema(catalog_entry)
 
     LOGGER.info("SingerSchema written")
     write_schema_message(catalog_entry=catalog_entry, bookmark_properties=[replication_key])
 
     LOGGER.info("Starting CDC based replication")
     while True:
-        stream_version = common.get_stream_version(catalog_entry.tap_stream_id, state)
-        log_based.sync_table(mssql_conn, config, catalog_entry, state, columns, stream_version)
-        singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
-        time.sleep(2)
+        try:
+            stream_version = common.get_stream_version(catalog_entry.tap_stream_id, state)
+            log_based.sync_table(mssql_conn, config, catalog_entry, state, columns, stream_version)
+            singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
+            LOGGER.warn("Successful CDC...")
+        except Exception as e:
+            LOGGER.warn("Failed CDC...")
+        finally:
+            time.sleep(5)
 
 
 def sync_non_cdc_streams(mssql_conn, non_cdc_catalog, config, state):
     mssql_conn = MSSQLConnection(config)
 
     for catalog_entry in non_cdc_catalog.streams:
         columns = list(catalog_entry.schema.properties.keys())
```

### Comparing `macrometa-source-mssql-0.0.8/macrometa_source_mssql/connection.py` & `macrometa-source-mssql-0.0.9/macrometa_source_mssql/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.8/macrometa_source_mssql/sample_data.py` & `macrometa-source-mssql-0.0.9/macrometa_source_mssql/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.8/macrometa_source_mssql/sync_strategies/common.py` & `macrometa-source-mssql-0.0.9/macrometa_source_mssql/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.8/macrometa_source_mssql/sync_strategies/full_table.py` & `macrometa-source-mssql-0.0.9/macrometa_source_mssql/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.8/macrometa_source_mssql/sync_strategies/log_based.py` & `macrometa-source-mssql-0.0.9/macrometa_source_mssql/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.8/pyproject.toml` & `macrometa-source-mssql-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mssql"
-version='0.0.8'
+version='0.0.9'
 description = "Macrometa Source for extracting data from Microsoft SQL Server."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-mssql-0.0.8/setup.py` & `macrometa-source-mssql-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'pymssql>=2.2.1']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mssql = macrometa_source_mssql:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mssql',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Macrometa Source for extracting data from Microsoft SQL Server.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mssql-0.0.8/PKG-INFO` & `macrometa-source-mssql-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mssql
-Version: 0.0.8
+Version: 0.0.9
 Summary: Macrometa Source for extracting data from Microsoft SQL Server.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MSSQL,Microsoft SQL Server,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

