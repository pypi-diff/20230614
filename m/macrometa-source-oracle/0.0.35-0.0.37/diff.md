# Comparing `tmp/macrometa-source-oracle-0.0.35.tar.gz` & `tmp/macrometa-source-oracle-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-oracle-0.0.35.tar", max compression
+gzip compressed data, was "macrometa-source-oracle-0.0.37.tar", max compression
```

## Comparing `macrometa-source-oracle-0.0.35.tar` & `macrometa-source-oracle-0.0.37.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0     9713 2023-05-19 09:50:52.544616 macrometa-source-oracle-0.0.35/LICENSE
--rw-r--r--   0        0        0     1707 2023-05-19 09:50:52.544616 macrometa-source-oracle-0.0.35/README.md
--rw-r--r--   0        0        0    42821 2023-05-19 09:50:52.544616 macrometa-source-oracle-0.0.35/macrometa_source_oracle/__init__.py
--rwxr-xr-x   0        0        0     7417 2023-05-19 09:50:52.544616 macrometa-source-oracle-0.0.35/macrometa_source_oracle/connection.py
--rwxr-xr-x   0        0        0        0 2023-05-19 09:50:52.544616 macrometa-source-oracle-0.0.35/macrometa_source_oracle/sync_strategies/__init__.py
--rwxr-xr-x   0        0        0     4779 2023-05-19 09:50:52.544616 macrometa-source-oracle-0.0.35/macrometa_source_oracle/sync_strategies/common.py
--rwxr-xr-x   0        0        0     4874 2023-05-19 09:50:52.544616 macrometa-source-oracle-0.0.35/macrometa_source_oracle/sync_strategies/full_table.py
--rwxr-xr-x   0        0        0    17662 2023-05-19 09:50:52.544616 macrometa-source-oracle-0.0.35/macrometa_source_oracle/sync_strategies/log_based.py
--rw-r--r--   0        0        0     1563 2023-05-19 09:50:52.640616 macrometa-source-oracle-0.0.35/pyproject.toml
--rw-r--r--   0        0        0     2739 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.35/setup.py
--rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.35/PKG-INFO
+-rwxr-xr-x   0        0        0     9713 2023-06-14 08:52:56.726589 macrometa-source-oracle-0.0.37/LICENSE
+-rw-r--r--   0        0        0     1707 2023-06-14 08:52:56.726589 macrometa-source-oracle-0.0.37/README.md
+-rw-r--r--   0        0        0    43158 2023-06-14 08:52:56.726589 macrometa-source-oracle-0.0.37/macrometa_source_oracle/__init__.py
+-rwxr-xr-x   0        0        0     7524 2023-06-14 08:52:56.726589 macrometa-source-oracle-0.0.37/macrometa_source_oracle/connection.py
+-rwxr-xr-x   0        0        0        0 2023-06-14 08:52:56.726589 macrometa-source-oracle-0.0.37/macrometa_source_oracle/sync_strategies/__init__.py
+-rwxr-xr-x   0        0        0     4779 2023-06-14 08:52:56.726589 macrometa-source-oracle-0.0.37/macrometa_source_oracle/sync_strategies/common.py
+-rwxr-xr-x   0        0        0     4874 2023-06-14 08:52:56.726589 macrometa-source-oracle-0.0.37/macrometa_source_oracle/sync_strategies/full_table.py
+-rwxr-xr-x   0        0        0    17662 2023-06-14 08:52:56.726589 macrometa-source-oracle-0.0.37/macrometa_source_oracle/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     1571 2023-06-14 08:52:56.802590 macrometa-source-oracle-0.0.37/pyproject.toml
+-rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.37/setup.py
+-rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.37/PKG-INFO
```

### Comparing `macrometa-source-oracle-0.0.35/LICENSE` & `macrometa-source-oracle-0.0.37/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.35/README.md` & `macrometa-source-oracle-0.0.37/README.md`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.35/macrometa_source_oracle/__init__.py` & `macrometa-source-oracle-0.0.37/macrometa_source_oracle/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import collections
 import copy
 import itertools
 
 import pkg_resources
 import singer
 import singer.schema
-from c8connector import C8Connector, ConfigProperty, Sample, SchemaAttribute, SchemaAttributeType, ConfigAttributeType
+from c8connector import C8Connector, ConfigProperty, Sample, SchemaAttribute, SchemaAttributeType, \
+                        ConfigAttributeType, ValidationException
 from c8connector import Schema as C8Schema
 from singer import utils, metadata, get_bookmark
 from singer.catalog import Catalog, CatalogEntry
 from singer.schema import Schema
 
 import macrometa_source_oracle.connection as orc_db
 import macrometa_source_oracle.sync_strategies.common as common
@@ -79,15 +80,15 @@
         If invalid, throw an exception with the cause.
         """
         config, filter_schema = self.get_config(integration)
         try:
             config = orc_db.create_wallet_file(config)
             do_discovery(config, [filter_schema], config['filter_table'])
         except Exception as e:
-            LOGGER.info('Exception raised: %s', e)
+            LOGGER.warn('Exception raised: %s', e)
             orc_db.delete_wallet_file(config)
             raise e
         orc_db.delete_wallet_file(config)
 
     def schemas(self, integration: dict) -> list[C8Schema]:
         """Get supported schemas using the given configurations."""
         config, filter_schema = self.get_config(integration)
@@ -114,15 +115,15 @@
 
                 for k, v in s_schema.properties.items():
                     t = v.type[-1]
                     s_attribs.append(SchemaAttribute(
                         k, self.get_attribute_type(t)))
                 results.append(C8Schema(stream.stream, s_attribs))
         except Exception as e:
-            LOGGER.info('Exception raised: %s', e)
+            LOGGER.warn('Exception raised: %s', e)
             orc_db.delete_wallet_file(config)
             raise e
         orc_db.delete_wallet_file(config)
         return results
 
     def samples(self, integration: dict) -> list[Sample]:
         """Fetch sample data using the given configurations."""
@@ -155,15 +156,15 @@
                         k, self.get_attribute_type(t)))
                 schema = C8Schema(stream.stream, s_attribs)
                 results.append(Sample(
                     schema=schema,
                     data=data)
                 )
         except Exception as e:
-            LOGGER.info('Exception raised: %s', e)
+            LOGGER.warn('Exception raised: %s', e)
             orc_db.delete_wallet_file(config)
             raise e
         orc_db.delete_wallet_file(config)
         return results
 
     def reserved_keys(self) -> list[str]:
         """List of reserved keys for the connector."""
@@ -257,15 +258,15 @@
                 'ewallet_pem': integration.get('ewallet_pem'),
                 'wallet_password': integration.get('wallet_password'),
             }
 
             filter_schema = integration['filter_schema']
             return config, filter_schema
         except KeyError as e:
-            raise KeyError(f'Integration property `{e}` not found.') from e
+            raise ValidationException(f'Integration property `{e}` not found.') from e
 
 
 def nullable_column(col_name, col_type, pks_for_table):
     """
     Check if a column should be nullable.
 
     :param col_name: Name of the column.
@@ -612,79 +613,82 @@
     :param filter_schemas: List of schemas to filter by.
     :type filter_schemas: list
     :param filter_table: Name of the table to filter by.
     :type filter_table: str
     :return: Catalog containing discovered columns for the given filter criteria.
     :rtype: Catalog
     """
-    LOGGER.info("Begin discovering..")
-    connection = orc_db.open_connection(conn_config)
-    cur = connection.cursor()
-
-    if conn_config['replication_method'] not in ["FULL_TABLE", "LOG_BASED"]:
-        raise Exception('Invalid replication method provided. It should be either FULL_TABLE or LOG_BASED.')
-
-    if conn_config['multitenant']:
-        LOGGER.info("The database is a multitenant system.")
-        # Change session to the anticipated pluggable database (PDB).
-        cur.execute(f"ALTER SESSION SET CONTAINER = {conn_config['pdb_name']}")
+    try:
+        LOGGER.info("Begin discovering..")
+        connection = orc_db.open_connection(conn_config)
+        cur = connection.cursor()
+
+        if conn_config['replication_method'] not in ["FULL_TABLE", "LOG_BASED"]:
+            raise Exception('Invalid replication method provided. It should be either FULL_TABLE or LOG_BASED.')
+
+        if conn_config['multitenant']:
+            LOGGER.info("The database is a multitenant system.")
+            # Change session to the anticipated pluggable database (PDB).
+            cur.execute(f"ALTER SESSION SET CONTAINER = {conn_config['pdb_name']}")
+
+        row_counts = produce_row_counts(cur, filter_schemas, filter_table)
+        table_info = {}
+
+        binds_sql = [f":{b}" for b in range(len(filter_schemas))]
+
+        sql = filter_schemas_sql_clause("""
+        SELECT owner, table_name
+        FROM all_tables
+        WHERE owner != 'SYS' AND table_name =""", binds_sql, filter_table)
+
+        LOGGER.info("Retrieving tables: %s %s", sql, filter_schemas)
+        is_view = False
+        for row in cur.execute(sql, filter_schemas):
+            schema = row[0]
+            table = row[1]
+
+            if schema not in table_info:
+                table_info[schema] = {}
+
+            table_info[schema][table] = {
+                'row_count': row_counts[table],
+                'is_view': is_view
+            }
 
-    row_counts = produce_row_counts(cur, filter_schemas, filter_table)
-    table_info = {}
+            sql = filter_schemas_sql_clause("""
+        SELECT owner, view_name
+        FROM sys.all_views
+        WHERE owner != 'SYS' AND view_name =""", binds_sql, filter_table)
+
+        LOGGER.info("Retrieving views")
+        for row in cur.execute(sql, filter_schemas):
+            view_name = row[1]
+            schema = row[0]
 
-    binds_sql = [f":{b}" for b in range(len(filter_schemas))]
+            if schema not in table_info:
+                table_info[schema] = {}
 
-    sql = filter_schemas_sql_clause("""
-   SELECT owner, table_name
-   FROM all_tables
-   WHERE owner != 'SYS' AND table_name =""", binds_sql, filter_table)
+            table_info[schema][view_name] = {
+                'is_view': True
+            }
 
-    LOGGER.info("Retrieving tables: %s %s", sql, filter_schemas)
-    is_view = False
-    for row in cur.execute(sql, filter_schemas):
-        schema = row[0]
-        table = row[1]
-
-        if schema not in table_info:
-            table_info[schema] = {}
-
-        table_info[schema][table] = {
-            'row_count': row_counts[table],
-            'is_view': is_view
-        }
+        if not table_info:
+            raise Exception(f'Table/view "{filter_table}" not found in the specified schema {filter_schemas[0]}.')
 
-    sql = filter_schemas_sql_clause("""
-   SELECT owner, view_name
-   FROM sys.all_views
-   WHERE owner != 'SYS' AND view_name =""", binds_sql, filter_table)
-
-    LOGGER.info("Retrieving views")
-    for row in cur.execute(sql, filter_schemas):
-        view_name = row[1]
-        schema = row[0]
-
-        if schema not in table_info:
-            table_info[schema] = {}
-
-        table_info[schema][view_name] = {
-            'is_view': True
-        }
-
-    if not table_info:
-        raise Exception(f'Table/view "{filter_table}" not found in the specified schema {filter_schemas[0]}.')
-
-    for scheme in table_info:
-        LOGGER.info(f"Schema {scheme} contains {len(table_info[scheme])} tables/views.")
-
-    catalog = discover_columns(cur, table_info, filter_schemas, filter_table)
-
-    dump_catalog(catalog)
-    cur.close()
-    connection.close()
-    return catalog
+        for scheme in table_info:
+            LOGGER.info(f"Schema {scheme} contains {len(table_info[scheme])} tables/views.")
+
+        catalog = discover_columns(cur, table_info, filter_schemas, filter_table)
+
+        dump_catalog(catalog)
+        cur.close()
+        connection.close()
+        return catalog
+    except Exception as e:
+        raise ValidationException(e)
 
 
 def is_selected_via_metadata(stream):
     """
     Check if a stream is selected via its metadata.
 
     :param stream: Stream object to check.
@@ -1019,15 +1023,15 @@
 
         elif args.catalog:
             state = args.state
             do_sync(conn_config, args.catalog, args.config.get('replication_method', "FULL_TABLE"), state)
         else:
             LOGGER.info("No properties were selected")
     except Exception as e:
-        LOGGER.info('Exception raised: %s', e)
+        LOGGER.warn('Exception raised: %s', e)
         orc_db.delete_wallet_file(conn_config)
         raise e
     orc_db.delete_wallet_file(conn_config)
 
 
 def main():
     try:
```

### Comparing `macrometa-source-oracle-0.0.35/macrometa_source_oracle/connection.py` & `macrometa-source-oracle-0.0.37/macrometa_source_oracle/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import singer
 import uuid
+from c8connector import ValidationException
 from pathlib import Path
 from singer import metadata, utils
 from typing import Dict
 import macrometa_source_oracle.sync_strategies.common as common
 import oracledb
 
 LOGGER = singer.get_logger()
@@ -19,15 +20,15 @@
 
     return dsn
 
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
@@ -39,14 +40,16 @@
         if config.get('ewallet_pem'):
             path = f"/opt/oracle/config/{path_uuid}/ewallet.pem"
             cwallet = Path(path)
             cwallet.parent.mkdir(exist_ok=True, parents=True)
             cwallet.write_text(create_ssl_string(config['ewallet_pem']))
             config['ewallet_pem'] = f"/opt/oracle/config/{path_uuid}"
             LOGGER.info(f"ewallet.pem file created at: {path}")
+    except ValidationException as e:
+        raise e
     except Exception as e:
         LOGGER.warn(f"Failed to create ewallet.pem file at: {path}. {e}")
     return config
 
 def delete_wallet_file(config: Dict) -> None:
     path = None
     try:
```

### Comparing `macrometa-source-oracle-0.0.35/macrometa_source_oracle/sync_strategies/common.py` & `macrometa-source-oracle-0.0.37/macrometa_source_oracle/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.35/macrometa_source_oracle/sync_strategies/full_table.py` & `macrometa-source-oracle-0.0.37/macrometa_source_oracle/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.35/macrometa_source_oracle/sync_strategies/log_based.py` & `macrometa-source-oracle-0.0.37/macrometa_source_oracle/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.35/pyproject.toml` & `macrometa-source-oracle-0.0.37/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-oracle"
-version='0.0.35'
+version='0.0.37'
 description = "Macrometa source oracle connector for reading from oracle databases."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 readme = "README.md"
 homepage = "https://www.macrometa.com/"
 keywords = [
     "ELT",
@@ -24,16 +24,16 @@
     "Operating System :: OS Independent",
 ]
 packages = [
     { include = "macrometa_source_oracle" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8"
-c8connector = ">=0.0.20"
+python = ">=3.8.1,<3.11"
+c8connector = ">=0.0.24"
 pipelinewise-singer-python = "1.2.0"
 oracledb = "^1.2.2"
 strict-rfc3339 = "^0.7"
 
 [tool.poetry.scripts]
 macrometa-source-oracle = "macrometa_source_oracle:main"
```

### Comparing `macrometa-source-oracle-0.0.35/setup.py` & `macrometa-source-oracle-0.0.37/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 packages = \
 ['macrometa_source_oracle', 'macrometa_source_oracle.sync_strategies']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['c8connector>=0.0.20',
+['c8connector>=0.0.24',
  'oracledb>=1.2.2,<2.0.0',
  'pipelinewise-singer-python==1.2.0',
  'strict-rfc3339>=0.7,<0.8']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-oracle = macrometa_source_oracle:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-oracle',
-    'version': '0.0.35',
+    'version': '0.0.37',
     'description': 'Macrometa source oracle connector for reading from oracle databases.',
     'long_description': '# macrometa-source-oracle\n\nMacrometa source connector that extracts data from a [Oracle](https://www.oracle.com/database/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).\n\n## How to use it\n\n### Install and Run\n\nFirst, make sure Python 3 is installed on your system or follow these\ninstallation instructions for [Mac](http://docs.python-guide.org/en/latest/starting/install3/osx/) or\n[Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-ubuntu-16-04).\n\n\nIt\'s recommended to use a virtualenv:\n\n```bash\n  python3 -m venv venv\n  pip install macrometa-source-oracle\n```\n\nor from source using,\n1. Install poetry using https://python-poetry.org/docs/#installation\n2. Run \n    ```bash\n    poetry build\n    pip install dist/macrometa_source_oracle-<version>*.whl\n    ```\n\n### Configuration\n\nRunning the the macrometa source connector independently requires a `config.json` file. \n\nExample configuration:\n\n```json\n{\n  "host": "dev.oracledb.io",\n  "port": 1521,\n  "user": "C##HELLO",\n  "password": "password",\n  "service_name": "ORCLCDB",\n  "filter_schema": "C##HELLO",\n  "filter_table": "CUSTOMERS",\n  "replication_method": "LOG_BASED",\n  "pdb_name": "ORCLPDB1",\n  "multitenant": true,\n  "scn_window_size": 10\n}\n```\n\nYou can run a discover run using the previous `config.json` file to acquire all the tables definition\n \n```\nmacrometa-source-oracle --config /tmp/config.json --discover >> /tmp/catalog.json\n```\n\nThen use the catalog.json to run a full export:\n\n```\nmacrometa-source-oracle --config /tmp/config.json --catalog /tmp/catalog.json\n```\n\n',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.macrometa.com/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8',
+    'python_requires': '>=3.8.1,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `macrometa-source-oracle-0.0.35/PKG-INFO` & `macrometa-source-oracle-0.0.37/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: macrometa-source-oracle
-Version: 0.0.35
+Version: 0.0.37
 Summary: Macrometa source oracle connector for reading from oracle databases.
 Home-page: https://www.macrometa.com/
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Oracle,Source
 Author: Macrometa
 Author-email: info@macrometa.com
-Requires-Python: >=3.8
+Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: c8connector (>=0.0.20)
+Requires-Dist: c8connector (>=0.0.24)
 Requires-Dist: oracledb (>=1.2.2,<2.0.0)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
 Requires-Dist: strict-rfc3339 (>=0.7,<0.8)
 Project-URL: Bug Tracker, https://github.com/Macrometacorp/macrometa-source-oracle/issues
 Description-Content-Type: text/markdown
 
 # macrometa-source-oracle
```

