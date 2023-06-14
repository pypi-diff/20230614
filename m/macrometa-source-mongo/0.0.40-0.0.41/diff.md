# Comparing `tmp/macrometa-source-mongo-0.0.40.tar.gz` & `tmp/macrometa-source-mongo-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mongo-0.0.40.tar", max compression
+gzip compressed data, was "macrometa-source-mongo-0.0.41.tar", max compression
```

## Comparing `macrometa-source-mongo-0.0.40.tar` & `macrometa-source-mongo-0.0.41.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10765 2023-05-17 06:36:07.144934 macrometa-source-mongo-0.0.40/LICENSE
--rw-r--r--   0        0        0    20738 2023-05-17 06:36:07.144934 macrometa-source-mongo-0.0.40/macrometa_source_mongo/__init__.py
--rw-r--r--   0        0        0     6470 2023-05-17 06:36:07.144934 macrometa-source-mongo-0.0.40/macrometa_source_mongo/connection.py
--rw-r--r--   0        0        0      895 2023-05-17 06:36:07.144934 macrometa-source-mongo-0.0.40/macrometa_source_mongo/exceptions.py
--rw-r--r--   0        0        0     7252 2023-05-17 06:36:07.144934 macrometa-source-mongo-0.0.40/macrometa_source_mongo/helper.py
--rw-r--r--   0        0        0    10251 2023-05-17 06:36:07.148934 macrometa-source-mongo-0.0.40/macrometa_source_mongo/sync_strategies/common.py
--rw-r--r--   0        0        0     3647 2023-05-17 06:36:07.148934 macrometa-source-mongo-0.0.40/macrometa_source_mongo/sync_strategies/full_table.py
--rw-r--r--   0        0        0     7271 2023-05-17 06:36:07.148934 macrometa-source-mongo-0.0.40/macrometa_source_mongo/sync_strategies/log_based.py
--rw-r--r--   0        0        0     2292 2023-05-17 06:36:07.148934 macrometa-source-mongo-0.0.40/macrometa_source_mongo/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1548 2023-05-17 06:36:07.384932 macrometa-source-mongo-0.0.40/pyproject.toml
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.40/setup.py
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.40/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/LICENSE
+-rw-r--r--   0        0        0    21264 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/macrometa_source_mongo/__init__.py
+-rw-r--r--   0        0        0     6577 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/macrometa_source_mongo/connection.py
+-rw-r--r--   0        0        0      895 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/macrometa_source_mongo/exceptions.py
+-rw-r--r--   0        0        0     7252 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/macrometa_source_mongo/helper.py
+-rw-r--r--   0        0        0    10251 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/macrometa_source_mongo/sync_strategies/common.py
+-rw-r--r--   0        0        0     3647 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/macrometa_source_mongo/sync_strategies/full_table.py
+-rw-r--r--   0        0        0     7271 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/macrometa_source_mongo/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     2292 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/macrometa_source_mongo/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1548 2023-06-14 08:48:52.343782 macrometa-source-mongo-0.0.41/pyproject.toml
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.41/setup.py
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.41/PKG-INFO
```

### Comparing `macrometa-source-mongo-0.0.40/LICENSE` & `macrometa-source-mongo-0.0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.40/macrometa_source_mongo/__init__.py` & `macrometa-source-mongo-0.0.41/macrometa_source_mongo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import pkg_resources
 import singer
 from pymongo import MongoClient
 from singer import metadata, metrics, utils
 from c8connector import (
     C8Connector, ConfigProperty, Sample, Schema,
-    ConfigAttributeType, SchemaAttribute)
+    ConfigAttributeType, SchemaAttribute, ValidationException)
 
 from macrometa_source_mongo.sync_strategies import log_based
 from macrometa_source_mongo.sync_strategies import common
 from macrometa_source_mongo.sync_strategies import full_table
 from macrometa_source_mongo.sync_strategies.sample_data import fetch_samples
 from macrometa_source_mongo.connection import create_certficate_files, delete_certficate_files, \
     get_connection_string, get_user_databases
@@ -27,16 +27,15 @@
 
 REQUIRED_CONFIG_KEYS = [
     'host',
     'user',
     'password',
     'auth_database',
     'database',
-    'source_collection',
-    'replication_method'
+    'source_collection'
 ]
 
 REQUIRED_CONFIG_KEYS_NON_SRV = REQUIRED_CONFIG_KEYS + ['port']
 
 LOG_BASED_METHOD = 'LOG_BASED'
 FULL_TABLE_METHOD = 'FULL_TABLE'
 
@@ -203,26 +202,27 @@
                 'host': integration['host'],
                 'user': integration['user'],
                 'password': integration['password'],
                 'database': integration['database'],
                 'auth_database': integration['auth_database'],
                 'source_collection': integration['source_collection'],
                 # Optional config keys
+                'replication_method': integration.get('replication_method', FULL_TABLE_METHOD),
                 'srv': integration.get('srv', False),
                 'port': integration.get('port'),
                 'replica_set': integration.get('replica_set'),
                 'ssl': integration.get('ssl', False),
                 'verify_mode': integration.get('verify_mode', True),
                 'direct_connection': integration.get('direct_connection', False),
                 'tls_ca_file': integration.get('tls_ca_file'),
                 'tls_certificate_key_file': integration.get('tls_certificate_key_file'),
                 'tls_certificate_key_file_password': integration.get('tls_certificate_key_file_password'),
             }
         except KeyError as e:
-            raise KeyError(f'Integration property `{e}` not found.') from e
+            raise ValidationException(f'Integration property `{e}` not found.') from e
 
     @staticmethod
     def get_client(config: Dict) -> MongoClient:
         connection_string = get_connection_string(config)
         client = MongoClient(connection_string)
         LOGGER.info('Connected to MongoDB host: %s, version: %s',
                     config['host'],
@@ -235,34 +235,40 @@
     Executes discovery mode, scanning the MongoDB cluster and converting
     all collections in the specified database into streams. The result is
     output as JSON to stdout.
     Args:
         client (MongoClient): A MongoDB Client instance.
         config (Dict): A dictionary containing database configuration parameters.
     """
-    if config['database'] not in get_user_databases(client, config):
-        raise NoReadPrivilegeException(config['user'], config['database'])
+    try:
+        if config['replication_method'] not in [LOG_BASED_METHOD, FULL_TABLE_METHOD]:
+            raise Exception('Invalid replication method provided. It should be either FULL_TABLE or LOG_BASED.')
 
-    database = client[config['database']]
-    collection_name = config['source_collection']
-    # Check if collection exists
-    if collection_name not in database.list_collection_names():
-        raise Exception(f'Collection "{collection_name}" not found in the database {config["database"]}.')
-
-    collection = database[collection_name]
-    is_view = collection.options().get('viewOn') is not None
-
-    if is_view:
-        raise KeyError('The connector does not support views.')
-
-    LOGGER.info("Retrieving collection information for database '%s', collection '%s'", database.name, collection_name)
-    streams = [produce_collection_schema(collection)]
-    json.dump({'streams': streams}, sys.stdout, indent=2)
+        if config['database'] not in get_user_databases(client, config):
+            raise NoReadPrivilegeException(config['user'], config['database'])
 
-    return streams
+        database = client[config['database']]
+        collection_name = config['source_collection']
+        # Check if collection exists
+        if collection_name not in database.list_collection_names():
+            raise Exception(f'Collection "{collection_name}" not found in the database {config["database"]}.')
+
+        collection = database[collection_name]
+        is_view = collection.options().get('viewOn') is not None
+
+        if is_view:
+            raise KeyError('The connector does not support views.')
+
+        LOGGER.info("Retrieving collection information for database '%s', collection '%s'", database.name, collection_name)
+        streams = [produce_collection_schema(collection)]
+        json.dump({'streams': streams}, sys.stdout, indent=2)
+
+        return streams
+    except Exception as e:
+        raise ValidationException(e)
 
 
 def clear_state_on_replication_change(stream: Dict, state: Dict, replication_method: str) -> Dict:
     """
     Resets the state for a given stream if the replication method has changed.
     Args:
         stream (Dict): A dictionary representing a stream.
@@ -432,14 +438,15 @@
     args = utils.parse_args(REQUIRED_CONFIG_KEYS)
     config = args.config
     srv = config.get('srv', False)
 
     if not srv:
         args = utils.parse_args(REQUIRED_CONFIG_KEYS_NON_SRV)
         config = args.config
+    config['replication_method']: args.config.get('replication_method', FULL_TABLE_METHOD)
     try:
         config = create_certficate_files(config)
         connection_string = get_connection_string(config)
         client = MongoClient(connection_string)
 
         LOGGER.info('Connected to MongoDB host: %s, version: %s',
                     config['host'],
```

### Comparing `macrometa-source-mongo-0.0.40/macrometa_source_mongo/connection.py` & `macrometa-source-mongo-0.0.41/macrometa_source_mongo/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import singer
 import uuid
 
+from c8connector import ValidationException
 from typing import Dict, List
 from pathlib import Path
 from pymongo import MongoClient
 from pymongo.database import Database
 from urllib import parse
 
 LOGGER = singer.get_logger('macrometa_source_mongo')
@@ -92,14 +93,16 @@
         if config.get('tls_certificate_key_file'):
             path = f"/opt/mongo/{path_uuid}/client.pem"
             client_cert = Path(path)
             client_cert.parent.mkdir(exist_ok=True, parents=True)
             client_cert.write_text(create_ssl_string(config['tls_certificate_key_file']))
             config['tls_certificate_key_file'] = path
             LOGGER.info(f"Client certificate file created at: {path}")
+    except ValidationException as e:
+        raise e
     except Exception as e:
         LOGGER.warn(f"Failed to create certificate: /opt/mongo/{path_uuid}/. {e}")
     return config
 
 def delete_certficate_files(config: Dict) -> None:
     try:
         cert = None
@@ -122,15 +125,15 @@
     except Exception as e:
         LOGGER.warn(f"Failed to delete certificate: {e}")
 
 def create_ssl_string(ssl_string: str) -> str:
     tls_certificate_key_list = []
     split_string = ssl_string.split("-----")
     if len(split_string) < 4:
-        raise Exception("Invalid PEM format for certificate.")
+        raise ValidationException("Invalid PEM format for certificate.")
     for i in range(len(split_string)):
         if ((i % 2) == 1):
             tls_certificate_key_list.extend(("-----", split_string[i], "-----"))
         else:
             tls_certificate_key_list.append(split_string[i].replace(' ', '\n'))
 
     return ''.join(tls_certificate_key_list)
```

### Comparing `macrometa-source-mongo-0.0.40/macrometa_source_mongo/exceptions.py` & `macrometa-source-mongo-0.0.41/macrometa_source_mongo/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.40/macrometa_source_mongo/helper.py` & `macrometa-source-mongo-0.0.41/macrometa_source_mongo/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.40/macrometa_source_mongo/sync_strategies/common.py` & `macrometa-source-mongo-0.0.41/macrometa_source_mongo/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.40/macrometa_source_mongo/sync_strategies/full_table.py` & `macrometa-source-mongo-0.0.41/macrometa_source_mongo/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.40/macrometa_source_mongo/sync_strategies/log_based.py` & `macrometa-source-mongo-0.0.41/macrometa_source_mongo/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.40/macrometa_source_mongo/sync_strategies/sample_data.py` & `macrometa-source-mongo-0.0.41/macrometa_source_mongo/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.40/pyproject.toml` & `macrometa-source-mongo-0.0.41/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mongo"
-version='0.0.40'
+version='0.0.41'
 description = "Macrometa Source for extracting data from MongoDB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
@@ -24,15 +24,15 @@
     { include = "macrometa_source_mongo" },
     { include = "sync_strategies", from = "macrometa_source_mongo" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 pipelinewise-singer-python = "1.2.0"
-c8connector = ">=0.0.20"
+c8connector = ">=0.0.24"
 pymongo = {version = "^4.0",extras = ["srv"]}
 tzlocal = "2.1.*"
 terminaltables = "3.1.*"
 dnspython = "2.1.*"
 
 [tool.poetry.scripts]
 # CLI declaration
```

### Comparing `macrometa-source-mongo-0.0.40/setup.py` & `macrometa-source-mongo-0.0.41/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,27 @@
  'macrometa_source_mongo.sync_strategies',
  'sync_strategies']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['c8connector>=0.0.20',
+['c8connector>=0.0.24',
  'dnspython>=2.1.0,<2.2.0',
  'pipelinewise-singer-python==1.2.0',
  'pymongo[srv]>=4.0,<5.0',
  'terminaltables>=3.1.0,<3.2.0',
  'tzlocal>=2.1.0,<2.2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mongo = macrometa_source_mongo:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mongo',
-    'version': '0.0.40',
+    'version': '0.0.41',
     'description': 'Macrometa Source for extracting data from MongoDB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mongo-0.0.40/PKG-INFO` & `macrometa-source-mongo-0.0.41/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mongo
-Version: 0.0.40
+Version: 0.0.41
 Summary: Macrometa Source for extracting data from MongoDB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MongoDB,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: c8connector (>=0.0.20)
+Requires-Dist: c8connector (>=0.0.24)
 Requires-Dist: dnspython (>=2.1.0,<2.2.0)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
 Requires-Dist: pymongo[srv] (>=4.0,<5.0)
 Requires-Dist: terminaltables (>=3.1.0,<3.2.0)
 Requires-Dist: tzlocal (>=2.1.0,<2.2.0)
 Project-URL: Bug Tracker, https://github.com/Macrometacorp/macrometa-source-mongo/issues
```

