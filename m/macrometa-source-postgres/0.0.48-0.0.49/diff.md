# Comparing `tmp/macrometa-source-postgres-0.0.48.tar.gz` & `tmp/macrometa-source-postgres-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-postgres-0.0.48.tar", max compression
+gzip compressed data, was "macrometa-source-postgres-0.0.49.tar", max compression
```

## Comparing `macrometa-source-postgres-0.0.48.tar` & `macrometa-source-postgres-0.0.49.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11899 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/LICENSE
--rw-r--r--   0        0        0    35642 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/macrometa_source_postgres/__init__.py
--rw-r--r--   0        0        0     8580 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/macrometa_source_postgres/connection.py
--rw-r--r--   0        0        0    20349 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/macrometa_source_postgres/helper.py
--rw-r--r--   0        0        0        0 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/__init__.py
--rw-r--r--   0        0        0     1212 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/common.py
--rw-r--r--   0        0        0     8974 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/full_table.py
--rw-r--r--   0        0        0    28329 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/log_based.py
--rw-r--r--   0        0        0     3698 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1512 2023-05-17 03:54:11.278795 macrometa-source-postgres-0.0.48/pyproject.toml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.48/setup.py
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.48/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/LICENSE
+-rw-r--r--   0        0        0    35738 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/macrometa_source_postgres/__init__.py
+-rw-r--r--   0        0        0     8580 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/macrometa_source_postgres/connection.py
+-rw-r--r--   0        0        0    20349 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/macrometa_source_postgres/helper.py
+-rw-r--r--   0        0        0        0 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/__init__.py
+-rw-r--r--   0        0        0     1212 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/common.py
+-rw-r--r--   0        0        0     8974 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/full_table.py
+-rw-r--r--   0        0        0    28329 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     3698 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1512 2023-06-14 08:08:09.268998 macrometa-source-postgres-0.0.49/pyproject.toml
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.49/setup.py
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.49/PKG-INFO
```

### Comparing `macrometa-source-postgres-0.0.48/LICENSE` & `macrometa-source-postgres-0.0.49/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.48/macrometa_source_postgres/__init__.py` & `macrometa-source-postgres-0.0.49/macrometa_source_postgres/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import psycopg2.extensions
 import psycopg2.extras
 import singer
 import singer.schema
 import uuid
 from c8connector import (
     C8Connector, ConfigProperty, Sample, Schema,
-    ConfigAttributeType, SchemaAttributeType, SchemaAttribute)
+    ConfigAttributeType, SchemaAttributeType, SchemaAttribute, ValidationException)
 from pathlib import Path
 from singer import utils, metadata, get_bookmark
 from singer.catalog import Catalog
 from typing import Dict
 
 import macrometa_source_postgres.connection as postgres
 import macrometa_source_postgres.sync_strategies.common as sync_common
@@ -71,16 +71,15 @@
         If invalid, throw an exception with the cause.
         """
         config = self.get_config(integration)
         try:
             config = create_certficate_files(config)
             do_discovery(config)
         except Exception as e:
-            delete_certficate_files(config)
-            raise e
+            self.delete_certificates_exception(e, config)
         delete_certficate_files(config)
 
     def samples(self, integration: dict) -> list[Sample]:
         """Fetch sample data using the provided configurations."""
         config = self.get_config(integration)
         try:
             config = create_certficate_files(config)
@@ -104,17 +103,15 @@
                     s_attribs.append(SchemaAttribute(k, self.get_attribute_type(t)))
                 schema = Schema(stream['stream'], s_attribs)
                 results.append(Sample(
                     schema=schema,
                     data=data)
                 )
         except Exception as e:
-            LOGGER.info("Exception raised: %s", e)
-            delete_certficate_files(config)
-            raise e
+            self.delete_certificates_exception(e, config)
         delete_certficate_files(config)
         return results
 
     def schemas(self, integration: dict) -> list[Schema]:
         """Get supported schemas using the given configurations."""
         config = self.get_config(integration)
         try:
@@ -134,20 +131,24 @@
                 s_schema['properties'] = modify_reserved_keys(s_schema['properties'], reserved_keys)
 
                 for k, v in s_schema['properties'].items():
                     t = v['type'][-1]
                     s_attribs.append(SchemaAttribute(k, self.get_attribute_type(t)))
                 results.append(Schema(stream['stream'], s_attribs))
         except Exception as e:
-            LOGGER.info("Exception raised: %s", e)
-            delete_certficate_files(config)
-            raise e
+            self.delete_certificates_exception(e, config)
         delete_certficate_files(config)
         return results
 
+    @staticmethod
+    def delete_certificates_exception(e, config):
+        LOGGER.warn("Exception raised: %s", e)
+        delete_certficate_files(config)
+        raise e
+
     def reserved_keys(self) -> list[str]:
         """List of reserved keys for the connector."""
         return []
 
     @staticmethod
     def get_attribute_type(source_type: str) -> SchemaAttributeType:
         if source_type == 'string':
@@ -231,18 +232,18 @@
             ConfigProperty('itersize', 'Iterator Size', ConfigAttributeType.INT, False, False,
                            description='PG cursor size for FULL_TABLE.',
                            default_value='20000'),
             ConfigProperty('use_secondary', 'Use Secondary', ConfigAttributeType.BOOLEAN, False, False,
                            description='Use a database replica for FULL_TABLE replication.',
                            default_value='false'),
             ConfigProperty('secondary_host', 'Secondary Host', ConfigAttributeType.STRING, False, False,
-                           description='Required when using a secondary replica.',
+                           description='PostgreSQL replica host.',
                            placeholder_value='secondary_postgres_host'),
             ConfigProperty('secondary_port', 'Secondary Port', ConfigAttributeType.INT, False, False,
-                           description='Required when using a secondary replica.',
+                           description='PostgreSQL replica port.',
                            placeholder_value='5432')
         ]
 
     def capabilities(self) -> list[str]:
         """Return the capabilities[1] of the connector.
         [1] https://docs.meltano.com/contribute/plugins#how-to-test-a-tap
         """
@@ -257,28 +258,29 @@
                 'user': integration['user'],
                 'password': integration['password'],
                 'port': integration['port'],
                 'dbname': integration['dbname'],
                 'filter_schemas': integration['filter_schemas'],
                 'filter_table': integration['filter_table'],
                 # Optional config keys
+                'replication_method': integration.get('replication_method', 'FULL_TABLE'),
                 'ssl': integration.get('ssl', False),
                 'ssl_root_ca_cert': integration.get('ssl_root_ca_cert'),
                 'ssl_client_certificate': integration.get('ssl_client_certificate'),
                 'ssl_client_key': integration.get('ssl_client_key'),
                 'ssl_client_password': integration.get('ssl_client_password'),
                 'tap_id': integration.get('tap_id'),
                 'replication_slot': integration.get('replication_slot'),
                 'debug_lsn': integration.get('debug_lsn', False),
                 'wal_sender_timeout': integration.get('wal_sender_timeout', 3600000),
                 'break_at_end_lsn': integration.get('break_at_end_lsn', True),
                 'use_secondary': integration.get('use_secondary', False),
             }
         except KeyError as e:
-            raise KeyError(f'Integration property `{e}` not found.') from e
+            raise ValidationException(f'Integration property `{e}` not found.') from e
 
 
 def do_discovery(conn_config):
     """
     Find all potential streams in the database cluster using discovery mode.
 
     Args:
@@ -286,25 +288,31 @@
 
     Returns:
         A list of dictionaries representing the discovered streams.
 
     Raises:
         RuntimeError: If no tables were discovered across the entire cluster.
     """
-    with postgres.connect(conn_config) as conn:
-        LOGGER.info("Discovery started for db %s", conn_config['dbname'])
-        filter_table = conn_config.get('filter_table')
-        streams = discover_db(conn, conn_config.get('filter_schemas'),
-                              [filter_table] if filter_table is not None else None)
+    try:
+        if conn_config['replication_method'] not in ["FULL_TABLE", "LOG_BASED"]:
+            raise Exception('Invalid replication method provided. It should be either FULL_TABLE or LOG_BASED.')
 
-    if len(streams) == 0:
-        raise RuntimeError('No tables were discovered')
+        with postgres.connect(conn_config) as conn:
+            LOGGER.info("Discovery started for db %s", conn_config['dbname'])
+            filter_table = conn_config.get('filter_table')
+            streams = discover_db(conn, conn_config.get('filter_schemas'),
+                                  [filter_table] if filter_table is not None else None)
 
-    dump_catalog(streams)
-    return streams
+        if len(streams) == 0:
+            raise RuntimeError('No tables were discovered')
+
+        dump_catalog(streams)
+        return streams
+    except Exception as e:
+        raise ValidationException(e)
 
 
 def do_sync_full_table(conn_config, stream, state, desired_columns, md_map):
     """
     Runs full table sync
     """
     LOGGER.info("Stream %s is using full_table replication", stream['tap_stream_id'])
@@ -601,14 +609,16 @@
             path = f"/opt/postgresql/{path_uuid}/client.key"
             client_cert = Path(path)
             client_cert.parent.mkdir(exist_ok=True, parents=True)
             client_cert.write_text(create_ssl_string(config['ssl_client_key']))
             client_cert.chmod(0o600)
             config['ssl_client_key'] = path
             LOGGER.info(f"Client key file created at: {path}")
+    except ValidationException as e:
+        raise e
     except Exception as e:
         LOGGER.warn(f"Failed to create certificate: /opt/postgresql/{path_uuid}/. {e}")
     return config
 
 
 def delete_certficate_files(config: Dict) -> None:
     try:
@@ -640,15 +650,15 @@
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
@@ -728,55 +738,43 @@
         'password': args.config['password'],
         'port': args.config['port'],
         'dbname': args.config['dbname'],
         'filter_schemas': args.config['filter_schemas'],
         'filter_table': args.config['filter_table'],
 
         # Optional config keys
+        'replication_method': args.config.get('replication_method', 'FULL_TABLE'),
         'ssl': args.config.get('ssl', False),
         'ssl_root_ca_cert': args.config.get('ssl_root_ca_cert'),
         'ssl_client_certificate': args.config.get('ssl_client_certificate'),
         'ssl_client_key': args.config.get('ssl_client_key'),
         'ssl_client_password': args.config.get('ssl_client_password'),
         'tap_id': args.config.get('tap_id'),
         'replication_slot': args.config.get('replication_slot'),
         'debug_lsn': args.config.get('debug_lsn', False),
         'wal_sender_timeout': args.config.get('wal_sender_timeout', 3600000),
         'break_at_end_lsn': args.config.get('break_at_end_lsn', True),
         'use_secondary': args.config.get('use_secondary', False),
     }
 
-    if conn_config['use_secondary']:
-        try:
-            conn_config |= {
-                # Secondary Host and Port are mandatory to use secondary connection.
-                'secondary_host': args.config['secondary_host'],
-                'secondary_port': args.config['secondary_port'],
-            }
-        except KeyError as exc:
-            raise ValueError(
-                "Use secondary is enabled but 'Secondary host' and 'Secondary port' are not defined."
-            ) from exc
-
     try:
         conn_config = create_certficate_files(conn_config)
-
         postgres.CURSOR_ITER_SIZE = int(args.config.get('itersize', postgres.CURSOR_ITER_SIZE))
 
         if args.discover:
             do_discovery(conn_config)
         elif args.properties or args.catalog:
             state = args.state
             state_file = args.state_file
             do_sync(conn_config, args.catalog.to_dict() if args.catalog else args.properties,
-                    args.config.get('replication_method'), state, state_file)
+                    conn_config.get('replication_method'), state, state_file)
         else:
             LOGGER.info("No properties were selected")
     except Exception as e:
-        LOGGER.info("Exception raised: %s", e)
+        LOGGER.warn("Exception raised: %s", e)
         delete_certficate_files(conn_config)
         raise e
     delete_certficate_files(conn_config)
 
 
 def main():
     """
```

### Comparing `macrometa-source-postgres-0.0.48/macrometa_source_postgres/connection.py` & `macrometa-source-postgres-0.0.49/macrometa_source_postgres/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.48/macrometa_source_postgres/helper.py` & `macrometa-source-postgres-0.0.49/macrometa_source_postgres/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/common.py` & `macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/full_table.py` & `macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/log_based.py` & `macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/sample_data.py` & `macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.48/pyproject.toml` & `macrometa-source-postgres-0.0.49/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-postgres"
-version='0.0.48'
+version='0.0.49'
 description = "Macrometa Source for extracting data from PostgreSQL."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
@@ -24,15 +24,15 @@
     { include = "macrometa_source_postgres" },
     { include = "sync_strategies", from = "macrometa_source_postgres" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 pipelinewise-singer-python = "1.2.0"
-c8connector = ">=0.0.20"
+c8connector = ">=0.0.24"
 psycopg2-binary = "2.9.3"
 strict-rfc3339 = "0.7"
 
 [tool.poetry.scripts]
 # CLI declaration
 macrometa-source-postgres = 'macrometa_source_postgres:main'
```

### Comparing `macrometa-source-postgres-0.0.48/setup.py` & `macrometa-source-postgres-0.0.49/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,26 +9,26 @@
  'macrometa_source_postgres.sync_strategies',
  'sync_strategies']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['c8connector>=0.0.20',
+['c8connector>=0.0.24',
  'pipelinewise-singer-python==1.2.0',
  'psycopg2-binary==2.9.3',
  'strict-rfc3339==0.7']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-postgres = '
                      'macrometa_source_postgres:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-postgres',
-    'version': '0.0.48',
+    'version': '0.0.49',
     'description': 'Macrometa Source for extracting data from PostgreSQL.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-postgres-0.0.48/PKG-INFO` & `macrometa-source-postgres-0.0.49/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: macrometa-source-postgres
-Version: 0.0.48
+Version: 0.0.49
 Summary: Macrometa Source for extracting data from PostgreSQL.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,PostgreSQL,Source
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
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
 Requires-Dist: psycopg2-binary (==2.9.3)
 Requires-Dist: strict-rfc3339 (==0.7)
 Project-URL: Bug Tracker, https://github.com/Macrometacorp/macrometa-source-postgres/issues
```

