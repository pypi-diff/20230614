# Comparing `tmp/taospy-2.7.7.tar.gz` & `tmp/taospy-2.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taospy-2.7.7.tar", max compression
+gzip compressed data, was "taospy-2.7.8.tar", max compression
```

## Comparing `taospy-2.7.7.tar` & `taospy-2.7.8.tar`

### file list

```diff
@@ -1,84 +1,29 @@
--rw-r--r--   0        0        0     1065 2023-03-28 10:00:27.446145 taospy-2.7.7/LICENSE
--rw-r--r--   0        0        0    26183 2023-03-28 10:00:27.446145 taospy-2.7.7/README.md
--rw-r--r--   0        0        0     1495 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/bind-multi.py
--rw-r--r--   0        0        0     1427 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/bind-row.py
--rw-r--r--   0        0        0      749 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/connect_cloud_service.py
--rw-r--r--   0        0        0     2386 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/connect_rest_examples.py
--rw-r--r--   0        0        0     2340 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/connect_rest_with_req_id_examples.py
--rw-r--r--   0        0        0      877 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/connect_websocket_examples.py
--rw-r--r--   0        0        0      978 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/connect_websocket_with_req_id_examples.py
--rw-r--r--   0        0        0     1710 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/connection_usage_native_reference.py
--rw-r--r--   0        0        0     1760 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/connection_usage_native_reference_with_req_id.py
--rw-r--r--   0        0        0      976 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/cursor_usage_native_reference.py
--rw-r--r--   0        0        0     1054 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/cursor_usage_native_reference_with_req_id.py
--rw-r--r--   0        0        0      647 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/demo.py
--rw-r--r--   0        0        0      719 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/import-json.py
--rw-r--r--   0        0        0      687 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/insert-lines.py
--rw-r--r--   0        0        0      570 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/json-tag.py
--rw-r--r--   0        0        0      335 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/pandas-read-sql-tdengine-cloud.py
--rw-r--r--   0        0        0      363 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/pandas-read-sql.py
--rw-r--r--   0        0        0      155 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/pep-249.py
--rw-r--r--   0        0        0     1604 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/query-async.py
--rw-r--r--   0        0        0      278 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/query-objectively.py
--rw-r--r--   0        0        0      362 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/rest_client.py
--rw-r--r--   0        0        0      447 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/rest_client_example.py
--rw-r--r--   0        0        0      457 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/rest_client_with_req_id_example.py
--rw-r--r--   0        0        0      314 2023-03-28 10:00:27.446145 taospy-2.7.7/examples/rest_cursor.py
--rw-r--r--   0        0        0     1984 2023-03-28 10:00:27.450145 taospy-2.7.7/examples/rest_query.py
--rw-r--r--   0        0        0     1190 2023-03-28 10:00:27.450145 taospy-2.7.7/examples/result_set_examples.py
--rw-r--r--   0        0        0     1245 2023-03-28 10:00:27.450145 taospy-2.7.7/examples/result_set_with_req_id_examples.py
--rw-r--r--   0        0        0    20703 2023-03-28 10:00:27.450145 taospy-2.7.7/examples/schemaless_insert.py
--rw-r--r--   0        0        0     1418 2023-03-28 10:00:27.450145 taospy-2.7.7/examples/subscribe-async.py
--rw-r--r--   0        0        0     1463 2023-03-28 10:00:27.450145 taospy-2.7.7/examples/subscribe-sync.py
--rw-r--r--   0        0        0     1575 2023-03-28 10:00:27.450145 taospy-2.7.7/examples/tmq_consumer.py
--rw-r--r--   0        0        0      748 2023-03-28 10:00:27.450145 taospy-2.7.7/examples/trades-to-taos.py
--rw-r--r--   0        0        0     1319 2023-03-28 10:00:27.450145 taospy-2.7.7/pyproject.toml
--rw-r--r--   0        0        0     1471 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/__init__.py
--rw-r--r--   0        0        0       22 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/_version.py
--rw-r--r--   0        0        0    20562 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/bind.py
--rw-r--r--   0        0        0    50665 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/cinterface.py
--rw-r--r--   0        0        0    10000 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/connection.py
--rw-r--r--   0        0        0     1255 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/constants.py
--rw-r--r--   0        0        0     9754 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/cursor.py
--rw-r--r--   0        0        0     2587 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/error.py
--rw-r--r--   0        0        0    11914 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/field.py
--rw-r--r--   0        0        0     4055 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/field_v3.py
--rw-r--r--   0        0        0      224 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/precision.py
--rw-r--r--   0        0        0     7493 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/result.py
--rw-r--r--   0        0        0      398 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/schemaless.py
--rw-r--r--   0        0        0     3856 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/sqlalchemy.py
--rw-r--r--   0        0        0     2396 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/statement.py
--rw-r--r--   0        0        0      964 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/subscription.py
--rw-r--r--   0        0        0     8014 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/tmq.py
--rw-r--r--   0        0        0     1548 2023-03-28 10:00:27.450145 taospy-2.7.7/taos/utils.py
--rw-r--r--   0        0        0     1802 2023-03-28 10:00:27.450145 taospy-2.7.7/taosrest/__init__.py
--rw-r--r--   0        0        0     4733 2023-03-28 10:00:27.450145 taospy-2.7.7/taosrest/connection.py
--rw-r--r--   0        0        0     3725 2023-03-28 10:00:27.450145 taospy-2.7.7/taosrest/cursor.py
--rw-r--r--   0        0        0     1233 2023-03-28 10:00:27.450145 taospy-2.7.7/taosrest/errors.py
--rw-r--r--   0        0        0     6673 2023-03-28 10:00:27.450145 taospy-2.7.7/taosrest/restclient.py
--rw-r--r--   0        0        0     2191 2023-03-28 10:00:27.450145 taospy-2.7.7/taosrest/sqlalchemy.py
--rw-r--r--   0        0        0      290 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/decorators.py
--rw-r--r--   0        0        0     1857 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test-stmt-insert-multi-nullable.py
--rw-r--r--   0        0        0      321 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_connect_args.py
--rw-r--r--   0        0        0     8018 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_ctaos.py
--rw-r--r--   0        0        0     1416 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_cursor_logfile.py
--rw-r--r--   0        0        0      580 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_exception.py
--rw-r--r--   0        0        0      471 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_info.py
--rw-r--r--   0        0        0    22400 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_lines.py
--rw-r--r--   0        0        0      785 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_native_cursor.py
--rw-r--r--   0        0        0     1738 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_pandas.py
--rw-r--r--   0        0        0      455 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_parse_date.py
--rw-r--r--   0        0        0     3159 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_query.py
--rw-r--r--   0        0        0     3608 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_query_a.py
--rw-r--r--   0        0        0      562 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_req_id.py
--rw-r--r--   0        0        0     1739 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_rest_api.py
--rw-r--r--   0        0        0     4637 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_rest_client.py
--rw-r--r--   0        0        0     7739 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_rest_connection.py
--rw-r--r--   0        0        0    10368 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_stmt.py
--rw-r--r--   0        0        0     3505 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_subscribe.py
--rw-r--r--   0        0        0     3735 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_tmq.py
--rw-r--r--   0        0        0      473 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_version.py
--rw-r--r--   0        0        0     1263 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/test_vgroup_id.py
--rw-r--r--   0        0        0       98 2023-03-28 10:00:27.450145 taospy-2.7.7/tests/utils.py
--rw-r--r--   0        0        0    28411 1970-01-01 00:00:00.000000 taospy-2.7.7/setup.py
--rw-r--r--   0        0        0    26974 1970-01-01 00:00:00.000000 taospy-2.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-14 06:15:15.071206 taospy-2.7.8/LICENSE
+-rw-r--r--   0        0        0    28015 2023-06-14 06:15:15.071206 taospy-2.7.8/README.md
+-rw-r--r--   0        0        0     1268 2023-06-14 06:15:15.075206 taospy-2.7.8/pyproject.toml
+-rw-r--r--   0        0        0     1471 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/_version.py
+-rw-r--r--   0        0        0    20562 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/bind.py
+-rw-r--r--   0        0        0    50847 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/cinterface.py
+-rw-r--r--   0        0        0    10000 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/connection.py
+-rw-r--r--   0        0        0     1255 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/constants.py
+-rw-r--r--   0        0        0    10333 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/cursor.py
+-rw-r--r--   0        0        0     2587 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/error.py
+-rw-r--r--   0        0        0    11914 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/field.py
+-rw-r--r--   0        0        0     4055 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/field_v3.py
+-rw-r--r--   0        0        0      224 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/precision.py
+-rw-r--r--   0        0        0     7493 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/result.py
+-rw-r--r--   0        0        0      398 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/schemaless.py
+-rw-r--r--   0        0        0     3856 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/sqlalchemy.py
+-rw-r--r--   0        0        0     2396 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/statement.py
+-rw-r--r--   0        0        0      964 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/subscription.py
+-rw-r--r--   0        0        0     8014 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/tmq.py
+-rw-r--r--   0        0        0     1548 2023-06-14 06:15:15.075206 taospy-2.7.8/taos/utils.py
+-rw-r--r--   0        0        0     1802 2023-06-14 06:15:15.075206 taospy-2.7.8/taosrest/__init__.py
+-rw-r--r--   0        0        0     4733 2023-06-14 06:15:15.075206 taospy-2.7.8/taosrest/connection.py
+-rw-r--r--   0        0        0     3725 2023-06-14 06:15:15.075206 taospy-2.7.8/taosrest/cursor.py
+-rw-r--r--   0        0        0     1233 2023-06-14 06:15:15.075206 taospy-2.7.8/taosrest/errors.py
+-rw-r--r--   0        0        0     6673 2023-06-14 06:15:15.075206 taospy-2.7.8/taosrest/restclient.py
+-rw-r--r--   0        0        0     2191 2023-06-14 06:15:15.075206 taospy-2.7.8/taosrest/sqlalchemy.py
+-rw-r--r--   0        0        0    30309 1970-01-01 00:00:00.000000 taospy-2.7.8/setup.py
+-rw-r--r--   0        0        0    28806 1970-01-01 00:00:00.000000 taospy-2.7.8/PKG-INFO
```

### Comparing `taospy-2.7.7/LICENSE` & `taospy-2.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/README.md` & `taospy-2.7.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # TDengine Connector for Python
-[![codecov](https://codecov.io/gh/taosdata/taos-connector-python/branch/main/graph/badge.svg?token=BDANN3DBXS)](https://codecov.io/gh/taosdata/taos-connector-python)
 
-[TDengine](https://github.com/taosdata/TDengine) connector for Python enables python programs to access TDengine, using an API which is compliant with the Python DB API 2.0 (PEP-249). It contains two modules:
+| Github Workflow | PyPI Version | PyPI Downloads | CodeCov |
+| --------------- | ------------ | -------------- | ------- |
+| ![workflow](https://img.shields.io/github/actions/workflow/status/taosdata/taos-connector-python/test.yml) | ![PyPI](https://img.shields.io/pypi/v/taospy) | ![PyPI](https://img.shields.io/pypi/dm/taospy) | [![codecov](https://codecov.io/gh/taosdata/taos-connector-python/branch/main/graph/badge.svg?token=BDANN3DBXS)](https://codecov.io/gh/taosdata/taos-connector-python) |
+
+
+
+
+[TDengine](https://github.com/taosdata/TDengine) connector for Python enables python programs to access TDengine, using
+an API which is compliant with the Python DB API 2.0 (PEP-249). It contains two modules:
 
 1. The `taos` module. It uses TDengine C client library for client server communications.
-2. The `taosrest` module. It wraps TDengine RESTful API to Python DB API 2.0 (PEP-249). With this module, you are free to install TDengine C client library.
+2. The `taosrest` module. It wraps TDengine RESTful API to Python DB API 2.0 (PEP-249). With this module, you do not need to install the TDengine C client library.
 
 ## Install taospy
 
 You can use `pip` to install the connector from PyPI:
 
 ```bash
 pip install taospy
@@ -20,15 +27,16 @@
 pip install git+https://github.com/taosdata/taos-connector-python.git
 ```
 
 Note: taospy v2.7.2 requirs Python 3.6+. The early versions of taospy from v2.5.0 to v2.7.1 require Python 3.7+.
 
 ## Source Code
 
-[TDengine](https://github.com/taosdata/TDengine) connector for Python source code is hosted on [GitHub](https://github.com/taosdata/taos-connector-python).
+[TDengine](https://github.com/taosdata/TDengine) connector for Python source code is hosted
+on [GitHub](https://github.com/taosdata/taos-connector-python).
 
 ## Install taos-ws-py
 
 ### Install with taospy
 
 ```bash
 pip install taospy[ws]
@@ -36,15 +44,16 @@
 
 ### Install taos-ws-py only
 
 ```bash
 pip install taos-ws-py
 ```
 
-Note: The taosws module is provided by taos-ws-py package separately from v2.7.2. It is part of early version of taospy. taos-ws-py requires Python 3.7+.
+Note: The taosws module is provided by taos-ws-py package separately from v2.7.2. It is part of early version of taospy.
+taos-ws-py requires Python 3.7+.
 
 ### Query with PEP-249 API using `taosws`
 
 ```python
 import taosws
 
 # all parameters are optional
@@ -192,15 +201,14 @@
 for field in result.fields:
     print(field)
 
 for row in result:
     print(row)
 ```
 
-
 ### Read with Pandas
 
 #### Method one
 
 ```python
 import pandas
 import taos
@@ -236,15 +244,16 @@
 Supported config options:
 
 - **config**: TDengine client configuration directory, by default use "/etc/taos/".
 - **host**: TDengine server host, by default use "localhost".
 - **user**: TDengine user name, default is "root".
 - **password**: TDengine user password, default is "taosdata".
 - **database**: Default connection database name, empty if not set.
-- **timezone**: Timezone for timestamp type (which is `datetime` object with tzinfo in python) no matter what the host's timezone is.
+- **timezone**: Timezone for timestamp type (which is `datetime` object with tzinfo in python) no matter what the host's
+  timezone is.
 
 ```python
 import taos
 
 # 1. with empty options, connect TDengine by default options
 #   that means:
 #     - use /etc/taos/taos.cfg as default configuration file
@@ -302,14 +311,87 @@
 for row in results:
     print(row)
 
 cursor.close()
 conn.close()
 ```
 
+#### Execute many
+
+Method execute_many is supported:
+
+There are two ways to use execute_many.
+
+The first way is to pass a data_set as a list of dictionaries, where each dictionary will be expanded into a complete
+statement.
+
+```python
+import taos
+
+conn = taos.connect()
+cursor = conn.cursor()
+
+db_name = "test_db"
+
+cursor.execute(f"DROP DATABASE IF EXISTS {db_name}")
+cursor.execute(f"CREATE DATABASE {db_name}")
+cursor.execute(f"USE {db_name}")
+
+cursor.execute("create stable stb (ts timestamp, v1 int) tags(t1 int)")
+
+create_table_data = [
+    {
+        "name": "tb1",
+        "t1": 1,
+    },
+    {
+        "name": "tb2",
+        "t1": 2,
+    },
+    {
+        "name": "tb3",
+        "t1": 3,
+    }
+]
+
+cursor.execute_many(
+    "create table {name} using stb tags({t1})",
+    create_table_data,
+)
+
+```
+
+The second way is to pass a data_set as a list of tuples, where each tuple represents a different row of the same
+table, and each value within the tuple will become a data row in the SQL statement. All the data together will form a
+complete SQL statement.
+
+```python
+import taos
+
+conn = taos.connect()
+cursor = conn.cursor()
+
+db_name = "test_db"
+
+cursor.execute(f"USE {db_name}")
+
+data_set = [
+    ('2018-10-03 14:38:05.100', 219),
+    ('2018-10-03 14:38:15.300', 218),
+    ('2018-10-03 14:38:16.800', 221),
+]
+
+table_name = "tb1"
+
+cursor.execute_many(f"insert into {table_name} values", data_set)
+
+```
+
+[Example: Insert many lines in one execute](./examples/cursor_execute_many.py)
+
 ### Query with objective API
 
 ```python
 import taos
 
 conn = taos.connect()
 conn.execute("create database if not exists pytest")
@@ -415,15 +497,14 @@
 
 if __name__ == "__main__":
     test_query(connect())
 ```
 
 You can pass an optional req_id in the parameters.
 
-
 ```python
 from taos import *
 from ctypes import *
 import time
 
 
 def fetch_callback(p_param, p_result, num_of_rows):
@@ -722,15 +803,14 @@
     print(row)
 
 conn.execute("drop database if exists %s" % dbname)
 ```
 
 You can pass an optional req_id in the parameters.
 
-
 ```python
 import taos
 from taos import SmlProtocol, SmlPrecision
 
 conn = taos.connect()
 dbname = "pytest_line"
 conn.execute("drop database if exists %s" % dbname)
@@ -1012,12 +1092,13 @@
 
 engine = create_engine("taos://root:taosdata@localhost:6030/log")
 df: pandas.DataFrame = pandas.read_sql("select * from logs", engine)
 ```
 
 ## Limitation
 
-- `taosrest` is designed to use with taosAdapter. If your TDengine version is older than v2.4.0.0, taosAdapter may not be available.
+- `taosrest` is designed to use with taosAdapter. If your TDengine version is older than v2.4.0.0, taosAdapter may not
+  be available.
 
 ## License
 
 We use MIT license for Python connector.
```

### Comparing `taospy-2.7.7/pyproject.toml` & `taospy-2.7.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 [tool.poetry]
 name = "taospy"
-version = "2.7.7"
+version = "2.7.8"
 description = "TDengine connector for python"
 authors = ["Taosdata Inc. <support@taosdata.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "taos" },
   { include = "taosrest" },
-  { include = "tests" },
-  { include = "examples" },
 ]
 
 [tool.poetry.plugins] # Optional super table
 
 [tool.poetry.plugins."sqlalchemy.dialects"]
 "taos" = "taos.sqlalchemy:TaosDialect"
 "taosrest" = "taosrest.sqlalchemy:TaosRestDialect"
 "taosws" = "taos.sqlalchemy:TaosWsDialect"
 
 [tool.poetry.dependencies]
 python = ">=3.6.2,<4.0"
 pytz = "*"
 iso8601 = "1.0.2"
-requests = "2.27.1"
+requests = ">=2.27.1"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.dependencies.taos-ws-py]
 version = ">=0.2.0"
 python = ">=3.7,<4.0"
 optional = true
```

### Comparing `taospy-2.7.7/taos/__init__.py` & `taospy-2.7.8/taos/__init__.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taos/bind.py` & `taospy-2.7.8/taos/bind.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taos/cinterface.py` & `taospy-2.7.8/taos/cinterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 def _load_taos_windows():
     try:
         return ctypes.windll.LoadLibrary("taos")
     except Exception as e:
         print("unable to load taos client library: %s" % e)
         try:
             from ctypes.util import find_library
+
             ctypes.windll.LoadLibrary(find_library("taos"))
         except Exception as final_err:
             raise InterfaceError("unable to load taos client library: %s" % final_err)
 
 
 def _load_taos():
     load_func = {
@@ -232,17 +233,14 @@
         raise ConnectionError(errstr, errno)
     return connection
 
 
 _libtaos.taos_connect_auth.restype = c_void_p
 _libtaos.taos_connect_auth.argtypes = c_char_p, c_char_p, c_char_p, c_char_p, c_uint16
 
-_libtaos.taos_connect_auth.restype = c_void_p
-_libtaos.taos_connect_auth.argtypes = c_char_p, c_char_p, c_char_p, c_char_p, c_uint16
-
 
 def taos_connect_auth(host=None, user="root", auth="", db=None, port=0):
     # type: (None|str, str, str, None|str, int) -> c_void_p
     """Connect server with auth token.
 
     - host: server hostname/FQDN
     - user: user name
@@ -274,19 +272,19 @@
     try:
         _db = c_char_p(db.encode("utf-8")) if db is not None else None
     except AttributeError:
         raise AttributeError("db is expected as a str")
 
     # port
     try:
-        _port = c_int(port)
+        _port = c_uint16(port)
     except TypeError:
         raise TypeError("port is expected as an int")
 
-    connection = c_void_p(_libtaos.taos_connect_auth(_host, _user, _auth, _db, _port))
+    connection = cast(_libtaos.taos_connect_auth(_host, _user, _auth, _db, _port), c_void_p)
 
     if connection.value is None:
         null_ptr = c_void_p(None)
         errno = taos_errno(null_ptr)
         errstr = taos_errstr(null_ptr)
         raise ConnectionError(errstr, errno)
     return connection
@@ -359,15 +357,21 @@
     _libtaos.taos_query_a(connection, c_char_p(sql.encode("utf-8")), async_query_callback_type(callback), param)
 
 
 # add req_id for async query
 try:
     async_query_with_reqid_callback_type = CFUNCTYPE(None, c_void_p, c_void_p, c_int)
     _libtaos.taos_query_a_with_reqid.restype = None
-    _libtaos.taos_query_a_with_reqid.argtypes = c_void_p, c_char_p, async_query_with_reqid_callback_type, c_void_p, c_int
+    _libtaos.taos_query_a_with_reqid.argtypes = (
+        c_void_p,
+        c_char_p,
+        async_query_with_reqid_callback_type,
+        c_void_p,
+        c_int,
+    )
 except Exception as err:
     _UNSUPPORTED["taos_query_a_with_reqid"] = err
 
 
 def taos_query_a_with_reqid(connection, sql, callback, param, req_id):
     # type: (c_void_p, str, async_query_with_reqid_callback_type, c_void_p, int) -> None
     """
@@ -377,16 +381,16 @@
     - req_id: int, request id
 
     @return: None
 
     """
     _check_if_supported()
     _libtaos.taos_query_a_with_reqid(
-        connection, c_char_p(sql.encode("utf-8")),
-        async_query_with_reqid_callback_type(callback), param, req_id)
+        connection, c_char_p(sql.encode("utf-8")), async_query_with_reqid_callback_type(callback), param, req_id
+    )
 
 
 async_fetch_rows_callback_type = CFUNCTYPE(None, c_void_p, c_void_p, c_int)
 _libtaos.taos_fetch_rows_a.restype = None
 _libtaos.taos_fetch_rows_a.argtypes = c_void_p, async_fetch_rows_callback_type, c_void_p
 
 
@@ -1028,18 +1032,18 @@
         c_int,
     )
 except Exception as err:
     _UNSUPPORTED["taos_schemaless_insert"] = err
 
 
 def taos_schemaless_insert(
-        connection: c_void_p,
-        lines: Union[List[str], Tuple[str]],
-        protocol: SmlProtocol,
-        precision: SmlPrecision,
+    connection: c_void_p,
+    lines: Union[List[str], Tuple[str]],
+    protocol: SmlProtocol,
+    precision: SmlPrecision,
 ):
     _check_if_supported()
     num_of_lines = len(lines)
     lines = (c_char_p(line.encode("utf-8")) for line in lines)
     lines_type = ctypes.c_char_p * num_of_lines
     p_lines = lines_type(*lines)
 
@@ -1076,19 +1080,19 @@
         c_int,
     )
 except Exception as err:
     _UNSUPPORTED["taos_schemaless_insert_ttl"] = err
 
 
 def taos_schemaless_insert_ttl(
-        connection: c_void_p,
-        lines: Union[List[str], Tuple[str]],
-        protocol: SmlProtocol,
-        precision: SmlPrecision,
-        ttl: int,
+    connection: c_void_p,
+    lines: Union[List[str], Tuple[str]],
+    protocol: SmlProtocol,
+    precision: SmlPrecision,
+    ttl: int,
 ):
     _check_if_supported()
     num_of_lines = len(lines)
     lines = (c_char_p(line.encode("utf-8")) for line in lines)
     lines_type = ctypes.c_char_p * num_of_lines
     p_lines = lines_type(*lines)
 
@@ -1127,20 +1131,20 @@
         c_int,
     )
 except Exception as err:
     _UNSUPPORTED["taos_schemaless_insert_ttl_with_reqid"] = err
 
 
 def taos_schemaless_insert_ttl_with_reqid(
-        connection: c_void_p,
-        lines: Union[List[str], Tuple[str]],
-        protocol: SmlProtocol,
-        precision: SmlPrecision,
-        ttl: int,
-        req_id: int,
+    connection: c_void_p,
+    lines: Union[List[str], Tuple[str]],
+    protocol: SmlProtocol,
+    precision: SmlPrecision,
+    ttl: int,
+    req_id: int,
 ):
     _check_if_supported()
     num_of_lines = len(lines)
     lines = (c_char_p(line.encode("utf-8")) for line in lines)
     lines_type = ctypes.c_char_p * num_of_lines
     p_lines = lines_type(*lines)
 
@@ -1179,15 +1183,16 @@
     # type: (c_void_p, list[str] | tuple(str), SmlProtocol, SmlPrecision, int) -> int
     _check_if_supported()
     num_of_lines = len(lines)
     lines = (c_char_p(line.encode("utf-8")) for line in lines)
     lines_type = ctypes.c_char_p * num_of_lines
     p_lines = lines_type(*lines)
     res = c_void_p(
-        _libtaos.taos_schemaless_insert_with_reqid(connection, p_lines, num_of_lines, protocol, precision, req_id))
+        _libtaos.taos_schemaless_insert_with_reqid(connection, p_lines, num_of_lines, protocol, precision, req_id)
+    )
     errno = taos_errno(res)
     affected_rows = taos_affected_rows(res)
     if errno != 0:
         errstr = taos_errstr(res)
         taos_free_result(res)
         raise SchemalessError(errstr, errno, affected_rows)
 
@@ -1208,35 +1213,26 @@
         c_int,
     )
 except Exception as err:
     _UNSUPPORTED["taos_schemaless_insert_raw"] = err
 
 
 def taos_schemaless_insert_raw(
-        connection: c_void_p,
-        lines_raw: str,
-        protocol: SmlProtocol,
-        precision: SmlPrecision,
+    connection: c_void_p,
+    lines_raw: str,
+    protocol: SmlProtocol,
+    precision: SmlPrecision,
 ) -> int:
     _check_if_supported()
     length = len(lines_raw)
     lines_raw = c_char_p(lines_raw.encode("utf-8"))
     type_p_int = POINTER(c_int)
     total_rows = type_p_int(c_int(0))
 
-    res = c_void_p(
-        _libtaos.taos_schemaless_insert_raw(
-            connection,
-            lines_raw,
-            length,
-            total_rows,
-            protocol,
-            precision
-        )
-    )
+    res = c_void_p(_libtaos.taos_schemaless_insert_raw(connection, lines_raw, length, total_rows, protocol, precision))
 
     errno = taos_errno(res)
     affected_rows = taos_affected_rows(res)
 
     # print(f"affected_rows: <{affected_rows}> "
     #       f"type: {type(affected_rows)} "
     #       f"total_rows: <{total_rows.contents.value}>")
@@ -1264,19 +1260,19 @@
         c_int,
     )
 except Exception as err:
     _UNSUPPORTED["taos_schemaless_insert_raw_with_reqid"] = err
 
 
 def taos_schemaless_insert_raw_with_reqid(
-        connection: c_void_p,
-        lines_raw: str,
-        protocol: SmlProtocol,
-        precision: SmlPrecision,
-        req_id: int,
+    connection: c_void_p,
+    lines_raw: str,
+    protocol: SmlProtocol,
+    precision: SmlPrecision,
+    req_id: int,
 ) -> int:
     _check_if_supported()
     length = len(lines_raw)
     lines_raw = c_char_p(lines_raw.encode("utf-8"))
     type_p_int = POINTER(c_int)
     total_rows = type_p_int(c_int(0))
 
@@ -1322,19 +1318,19 @@
         c_int,
     )
 except Exception as err:
     _UNSUPPORTED["taos_schemaless_insert_raw_ttl"] = err
 
 
 def taos_schemaless_insert_raw_ttl(
-        connection: c_void_p,
-        lines_raw: str,
-        protocol: SmlProtocol,
-        precision: SmlPrecision,
-        ttl: int,
+    connection: c_void_p,
+    lines_raw: str,
+    protocol: SmlProtocol,
+    precision: SmlPrecision,
+    ttl: int,
 ) -> int:
     _check_if_supported()
     length = len(lines_raw)
     lines_raw = c_char_p(lines_raw.encode("utf-8"))
     type_p_int = POINTER(c_int)
     total_rows = type_p_int(c_int(0))
 
@@ -1381,20 +1377,20 @@
         c_int,
     )
 except Exception as err:
     _UNSUPPORTED["taos_schemaless_insert_raw_ttl_with_reqid"] = err
 
 
 def taos_schemaless_insert_raw_ttl_with_reqid(
-        connection: c_void_p,
-        lines_raw: str,
-        protocol: SmlProtocol,
-        precision: SmlPrecision,
-        ttl: int,
-        req_id: int,
+    connection: c_void_p,
+    lines_raw: str,
+    protocol: SmlProtocol,
+    precision: SmlPrecision,
+    ttl: int,
+    req_id: int,
 ) -> int:
     _check_if_supported()
     length = len(lines_raw)
     lines_raw = c_char_p(lines_raw.encode("utf-8"))
     type_p_int = POINTER(c_int)
     total_rows = type_p_int(c_int(0))
 
@@ -1449,17 +1445,17 @@
 def tmq_conf_set(conf, key, value):
     # type: (c_void_p, str, str) -> None
     _check_if_supported()
 
     if not isinstance(value, str):
         raise TmqError(msg=f"fail to execute tmq_conf_set({key},{value}), {value} is not string type")
 
-    res = _libtaos.tmq_conf_set(conf, ctypes.c_char_p(key.encode("utf-8")), ctypes.c_char_p(value.encode("utf-8")))
-    if res != 0:
-        raise TmqError(msg=f"fail to execute tmq_conf_set({key},{value}), code={res}", errno=res)
+    tmq_res = _libtaos.tmq_conf_set(conf, ctypes.c_char_p(key.encode("utf-8")), ctypes.c_char_p(value.encode("utf-8")))
+    if tmq_res != 0:
+        raise TmqError(msg=f"fail to execute tmq_conf_set({key},{value}), code={tmq_res}", errno=tmq_res)
 
 
 try:
     _libtaos.tmq_conf_destroy.argtypes = (c_void_p,)
     _libtaos.tmq_conf_destroy.restype = None
 except Exception as err:
     _UNSUPPORTED["tmq_conf_destroy"] = err
@@ -1495,19 +1491,32 @@
 
 def tmq_consumer_new(conf, errstrlen=0):
     # type (c_void_p, c_char_p, c_int) -> c_void_p
     _check_if_supported()
     buf = ctypes.create_string_buffer(errstrlen)
     tmq = cast(_libtaos.tmq_consumer_new(conf, buf, errstrlen), c_void_p)
     if tmq.value is None:
-        raise TmqError("failed on tmq_consumer_new")
+        raise TmqError("failed on tmq_consumer_new()")
     return tmq
 
 
 try:
+    _libtaos.tmq_err2str.restype = c_char_p
+    _libtaos.tmq_err2str.argtypes = (c_int,)
+except Exception as err:
+    _UNSUPPORTED["tmq_err2str"] = err
+
+
+def tmq_err2str(errno):
+    # type (c_int) -> c_char_p
+    _check_if_supported()
+    return c_char_p(_libtaos.tmq_err2str(errno))
+
+
+try:
     _libtaos.tmq_list_new.restype = c_void_p
 except Exception as err:
     _UNSUPPORTED["tmq_list_new"] = err
 
 
 def tmq_list_new():
     # type () -> c_void_p
@@ -1579,15 +1588,15 @@
 
 
 def tmq_subscribe(tmq, list):
     # type (c_void_p, c_void_p) -> None
     _check_if_supported()
     res = _libtaos.tmq_subscribe(tmq, list)
     if res != 0:
-        raise TmqError(msg="failed on tmq_subscribe()", errno=res)
+        raise TmqError(msg=f"failed on tmq_subscribe(), errno={res:X}, errmsg={tmq_err2str(res)}", errno=res)
 
 
 try:
     _libtaos.tmq_unsubscribe.argtypes = (c_void_p,)
     _libtaos.tmq_unsubscribe.restype = c_int
 except Exception as err:
     _UNSUPPORTED["tmq_unsubscribe"] = err
@@ -1598,15 +1607,15 @@
     _check_if_supported()
     res = _libtaos.tmq_unsubscribe(tmq)
     if res == -1:
         # -1 means empty subscription topic list..
         # tmq_unsubscribe will subscribe a empty topic list to clear the consumer task.
         return
     if res != 0:
-        raise TmqError(msg=f"failed on tmq_unsubscribe() {res}", errno=res)
+        raise TmqError(msg=f"failed on tmq_unsubscribe(), errno={res:X}, errmsg={tmq_err2str(res)}", errno=res)
 
 
 try:
     _libtaos.tmq_subscription.argtypes = (c_void_p, c_void_p)
     _libtaos.tmq_subscription.restype = c_int
 except Exception as err:
     _UNSUPPORTED["tmq_subscription"] = err
@@ -1614,15 +1623,15 @@
 
 def tmq_subscription(tmq):
     # type (c_void_p, c_void_p) -> [string]
     _check_if_supported()
     topics = tmq_list_new()
     res = _libtaos.tmq_subscription(tmq, byref(topics))
     if res != 0:
-        raise TmqError(msg="failed on tmq_subscription()", errno=res)
+        raise TmqError(msg=f"failed on tmq_subscription(), errno={res:X}, errmsg={tmq_err2str(res)}", errno=res)
     res = tmq_list_to_c_array(topics)
     tmq_list_destroy(topics)
     return res
 
 
 try:
     _libtaos.tmq_consumer_poll.argtypes = (c_void_p, c_int64)
@@ -1645,30 +1654,30 @@
 
 
 def tmq_consumer_close(tmq):
     # type (c_void_p,) -> None
     _check_if_supported()
     res = _libtaos.tmq_consumer_close(tmq)
     if res != 0:
-        raise TmqError(msg="failed on tmq_consumer_close()", errno=res)
+        raise TmqError(msg=f"failed on tmq_consumer_close(), errno={res:X}, errmsg={tmq_err2str(res)}", errno=res)
 
 
 try:
     _libtaos.tmq_commit_sync.argtypes = (c_void_p, c_void_p)
     _libtaos.tmq_commit_sync.restype = c_int
 except Exception as err:
     _UNSUPPORTED["tmq_commit"] = err
 
 
 def tmq_commit_sync(tmq, offset):
     # type: (c_void_p, c_void_p) -> None
     _check_if_supported()
     res = _libtaos.tmq_commit_sync(tmq, offset)
     if res != 0:
-        raise TmqError(msg="failed on tmq_commit_sync()", errno=res)
+        raise TmqError(msg=f"failed on tmq_commit_sync(), errno={res:X}, errmsg={tmq_err2str(res)}", errno=res)
 
 
 try:
     _libtaos.tmq_get_topic_name.argtypes = (c_void_p,)
     _libtaos.tmq_get_topic_name.restype = c_char_p
 except Exception as err:
     _UNSUPPORTED["tmq_get_topic_name"] = err
@@ -1744,16 +1753,17 @@
     _UNSUPPORTED["taos_get_table_vgId"] = err
 
 
 def taos_get_table_vgId(conn, db, table):
     # type: (c_void_p, str, str) -> int
     _check_if_supported()
     vg_id = c_int()
-    code = _libtaos.taos_get_table_vgId(conn, c_char_p(db.encode('utf-8')), c_char_p(table.encode('utf-8')),
-                                        ctypes.byref(vg_id))
+    code = _libtaos.taos_get_table_vgId(
+        conn, c_char_p(db.encode("utf-8")), c_char_p(table.encode("utf-8")), ctypes.byref(vg_id)
+    )
     if code != 0:
         raise InternalError(taos_errstr(c_void_p(None)))
     return vg_id.value
 
 
 try:
     _libtaos.tmq_get_res_type.argstype = (c_void_p,)
```

### Comparing `taospy-2.7.7/taos/connection.py` & `taospy-2.7.8/taos/connection.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taos/constants.py` & `taospy-2.7.8/taos/constants.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taos/cursor.py` & `taospy-2.7.8/taos/cursor.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,18 +139,35 @@
             self._affected_rows = affected_rows
             self._rowcount = affected_rows
             return affected_rows
         else:
             self._fields = taos_fetch_fields(self._result)
             return self._handle_result()
 
-    def executemany(self, operation, seq_of_parameters, req_id: Optional[int] = None):
-        """Prepare a database operation (query or command) and then execute it against all parameter sequences or mappings found in the sequence seq_of_parameters."""
-        self.execute(operation, req_id=req_id)
-        pass
+    def execute_many(self, operation, data_list, req_id: Optional[int] = None):
+        """
+        Prepare a database operation (query or command) and then execute it against all parameter sequences or mappings
+        found in the sequence seq_of_parameters.
+        """
+        sql = operation
+        flag = True
+        affected_rows = 0
+        for line in data_list:
+            if isinstance(line, dict):
+                flag = False
+                # print(f'execute: {sql.format(**line)}')
+                affected_rows += self.execute(sql.format(**line), req_id=req_id)
+            elif isinstance(line, list):
+                sql += f' {tuple(line)} '
+            elif isinstance(line, tuple):
+                sql += f' {line} '
+        if flag:
+            # print(f'execute_many: {sql}')
+            affected_rows += self.execute(sql, req_id=req_id)
+        return affected_rows
 
     def fetchone(self):
         """Fetch the next row of a query result set, returning a single sequence, or None when no more data is available."""
         pass
 
     def fetchmany(self):
         pass
```

### Comparing `taospy-2.7.7/taos/error.py` & `taospy-2.7.8/taos/error.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taos/field.py` & `taospy-2.7.8/taos/field.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taos/field_v3.py` & `taospy-2.7.8/taos/field_v3.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taos/result.py` & `taospy-2.7.8/taos/result.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taos/sqlalchemy.py` & `taospy-2.7.8/taos/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taos/statement.py` & `taospy-2.7.8/taos/statement.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taos/subscription.py` & `taospy-2.7.8/taos/subscription.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taos/tmq.py` & `taospy-2.7.8/taos/tmq.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taos/utils.py` & `taospy-2.7.8/taos/utils.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taosrest/__init__.py` & `taospy-2.7.8/taosrest/__init__.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taosrest/connection.py` & `taospy-2.7.8/taosrest/connection.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taosrest/cursor.py` & `taospy-2.7.8/taosrest/cursor.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taosrest/errors.py` & `taospy-2.7.8/taosrest/errors.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taosrest/restclient.py` & `taospy-2.7.8/taosrest/restclient.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/taosrest/sqlalchemy.py` & `taospy-2.7.8/taosrest/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `taospy-2.7.7/setup.py` & `taospy-2.7.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['examples', 'taos', 'taosrest', 'tests']
+['taos', 'taosrest']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['iso8601==1.0.2', 'pytest-cov>=4.0.0,<5.0.0', 'pytz', 'requests==2.27.1']
+['iso8601==1.0.2', 'pytest-cov>=4.0.0,<5.0.0', 'pytz', 'requests>=2.27.1']
 
 extras_require = \
 {'ws:python_version >= "3.7" and python_version < "4.0"': ['taos-ws-py>=0.2.0']}
 
 entry_points = \
 {'sqlalchemy.dialects': ['taos = taos.sqlalchemy:TaosDialect',
                          'taosrest = taosrest.sqlalchemy:TaosRestDialect',
                          'taosws = taos.sqlalchemy:TaosWsDialect']}
 
 setup_kwargs = {
     'name': 'taospy',
-    'version': '2.7.7',
+    'version': '2.7.8',
     'description': 'TDengine connector for python',
-    'long_description': '# TDengine Connector for Python\n[![codecov](https://codecov.io/gh/taosdata/taos-connector-python/branch/main/graph/badge.svg?token=BDANN3DBXS)](https://codecov.io/gh/taosdata/taos-connector-python)\n\n[TDengine](https://github.com/taosdata/TDengine) connector for Python enables python programs to access TDengine, using an API which is compliant with the Python DB API 2.0 (PEP-249). It contains two modules:\n\n1. The `taos` module. It uses TDengine C client library for client server communications.\n2. The `taosrest` module. It wraps TDengine RESTful API to Python DB API 2.0 (PEP-249). With this module, you are free to install TDengine C client library.\n\n## Install taospy\n\nYou can use `pip` to install the connector from PyPI:\n\n```bash\npip install taospy\n```\n\nOr with git url:\n\n```bash\npip install git+https://github.com/taosdata/taos-connector-python.git\n```\n\nNote: taospy v2.7.2 requirs Python 3.6+. The early versions of taospy from v2.5.0 to v2.7.1 require Python 3.7+.\n\n## Source Code\n\n[TDengine](https://github.com/taosdata/TDengine) connector for Python source code is hosted on [GitHub](https://github.com/taosdata/taos-connector-python).\n\n## Install taos-ws-py\n\n### Install with taospy\n\n```bash\npip install taospy[ws]\n```\n\n### Install taos-ws-py only\n\n```bash\npip install taos-ws-py\n```\n\nNote: The taosws module is provided by taos-ws-py package separately from v2.7.2. It is part of early version of taospy. taos-ws-py requires Python 3.7+.\n\n### Query with PEP-249 API using `taosws`\n\n```python\nimport taosws\n\n# all parameters are optional\nconn = taosws.connect("taosws://root:taosdata@localhost:6041")\ncursor = conn.cursor()\n\ncursor.execute("show databases")\nresults: list[tuple] = cursor.fetchall()\nfor row in results:\n    print(row)\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nimport taosws\n\n# all parameters are optional\nconn = taosws.connect("taosws://root:taosdata@localhost:6041")\ncursor = conn.cursor()\n\ncursor.execute("show databases", req_id=1)\nresults: list[tuple] = cursor.fetchall()\nfor row in results:\n    print(row)\n```\n\n### Query with query method using `taosws`\n\n```python\nfrom taosws import *\n\nconn = connect("taosws://root:taosdata@localhost:6041")\nresult = conn.query("show databases")\n\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nfrom taosws import *\n\nconn = connect("taosws://root:taosdata@localhost:6041")\nresult = conn.query("show databases", req_id=1)\n\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n```\n\n### Read with Pandas using `taosws`\n\n#### Method one\n\n```python\nimport pandas\nimport taosws\n\nconn = taosws.connect("taosws://root:taosdata@localhost:6041")\ndf: pandas.DataFrame = pandas.read_sql("show databases", conn)\ndf\n```\n\n#### Method Two\n\n```python\nimport pandas\nfrom sqlalchemy import create_engine\n\nengine = create_engine("taosws://root:taosdata@localhost:6041")\ndf: pandas.DataFrame = pandas.read_sql("show databases", engine)\ndf\n```\n\n## Examples for `taosrest` Module\n\n### Query with PEP-249 API\n\n```python\nimport taosrest\n\n# all parameters are optional\nconn = taosrest.connect(url="http://localhost:6041",\n                        user="root",\n                        password="taosdata")\ncursor = conn.cursor()\n\ncursor.execute("show databases")\nresults: list[tuple] = cursor.fetchall()\nfor row in results:\n    print(row)\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nimport taosrest\n\n# all parameters are optional\nconn = taosrest.connect(url="http://localhost:6041",\n                        user="root",\n                        password="taosdata")\ncursor = conn.cursor()\n\ncursor.execute("show databases", req_id=1)\nresults: list[tuple] = cursor.fetchall()\nfor row in results:\n    print(row)\n```\n\n### Query with query method\n\n```python\nfrom taosrest import connect, TaosRestConnection, Result\n\nconn: TaosRestConnection = connect()\nresult: Result = conn.query("show databases")\n\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nfrom taosrest import connect, TaosRestConnection, Result\n\nconn: TaosRestConnection = connect()\nresult: Result = conn.query("show databases", req_id=1)\n\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n```\n\n\n### Read with Pandas\n\n#### Method one\n\n```python\nimport pandas\nimport taos\n\nconn = taos.connect()\ndf: pandas.DataFrame = pandas.read_sql("select * from log.logs", conn)\n```\n\n#### Method two\n\n```python\nimport pandas\nimport taosrest\n\nconn = taosrest.connect()\ndf: pandas.DataFrame = pandas.read_sql("select * from log.logs", conn)\n```\n\n#### Method three\n\n```python\nimport pandas\nfrom sqlalchemy import create_engine\n\nengine = create_engine("taosrest://root:taosdata@localhost:6041")\ndf: pandas.DataFrame = pandas.read_sql("select * from log.logs", engine)\n```\n\n## Examples for `taos` Module\n\n### Connect options\n\nSupported config options:\n\n- **config**: TDengine client configuration directory, by default use "/etc/taos/".\n- **host**: TDengine server host, by default use "localhost".\n- **user**: TDengine user name, default is "root".\n- **password**: TDengine user password, default is "taosdata".\n- **database**: Default connection database name, empty if not set.\n- **timezone**: Timezone for timestamp type (which is `datetime` object with tzinfo in python) no matter what the host\'s timezone is.\n\n```python\nimport taos\n\n# 1. with empty options, connect TDengine by default options\n#   that means:\n#     - use /etc/taos/taos.cfg as default configuration file\n#     - use "localhost" if not set in config file\n#     - use "root" as default username\n#     - use "taosdata" as default password\n#     - use 6030 as default port if not set in config file\n#     - use local timezone datetime as timestamp\nconn = taos.connect()\n# 2. with full set options, default db: log, use UTC datetime.\nconn = taos.connect(host=\'localhost\',\n                    user=\'root\',\n                    password=\'taosdata\',\n                    database=\'log\',\n                    config=\'/etc/taos\',\n                    timezone=\'UTC\')\n```\n\nNote that, the datetime formatted string will contain timezone information when timezone set. For example:\n\n```python\n# without timezone(local timezone depends on your machine)\n\'1969-12-31 16:00:00\'\n# with timezone UTC\n\'1969-12-31 16:00:00+00:00\'\n```\n\n### Query with PEP-249 API\n\n```python\nimport taos\n\nconn = taos.connect()\ncursor = conn.cursor()\n\ncursor.execute("show databases")\nresults = cursor.fetchall()\nfor row in results:\n    print(row)\n\ncursor.close()\nconn.close()\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nimport taos\n\nconn = taos.connect()\ncursor = conn.cursor()\n\ncursor.execute("show databases", req_id=1)\nresults = cursor.fetchall()\nfor row in results:\n    print(row)\n\ncursor.close()\nconn.close()\n```\n\n### Query with objective API\n\n```python\nimport taos\n\nconn = taos.connect()\nconn.execute("create database if not exists pytest")\n\nresult = conn.query("show databases")\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n\nresult.close()\nconn.execute("drop database pytest")\nconn.close()\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nimport taos\n\nconn = taos.connect()\nconn.execute("create database if not exists pytest", req_id=1)\n\nresult = conn.query("show databases")\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n\nresult.close()\nconn.execute("drop database pytest")\nconn.close()\n```\n\n### Query with async API\n\n```python\nfrom taos import *\nfrom ctypes import *\nimport time\n\n\ndef fetch_callback(p_param, p_result, num_of_rows):\n    print("fetched ", num_of_rows, "rows")\n    p = cast(p_param, POINTER(Counter))\n    result = TaosResult(p_result)\n\n    if num_of_rows == 0:\n        print("fetching completed")\n        p.contents.done = True\n        result.close()\n        return\n\n    if num_of_rows < 0:\n        p.contents.done = True\n        result.check_error(num_of_rows)\n        result.close()\n        return None\n\n    for row in result.rows_iter(num_of_rows):\n        # print(row)\n        pass\n\n    p.contents.count += result.row_count\n    result.fetch_rows_a(fetch_callback, p_param)\n\n\ndef query_callback(p_param, p_result, code):\n    # type: (c_void_p, c_void_p, c_int) -> None\n    if p_result is None:\n        return\n\n    result = TaosResult(p_result)\n    if code == 0:\n        result.fetch_rows_a(fetch_callback, p_param)\n\n    result.check_error(code)\n\n\nclass Counter(Structure):\n    _fields_ = [("count", c_int), ("done", c_bool)]\n\n    def __str__(self):\n        return "{ count: %d, done: %s }" % (self.count, self.done)\n\n\ndef test_query(conn):\n    # type: (TaosConnection) -> None\n    counter = Counter(count=0)\n    conn.query_a("select * from log.log", query_callback, byref(counter))\n\n    while not counter.done:\n        print("wait query callback")\n        time.sleep(1)\n\n    print(counter)\n    conn.close()\n\n\nif __name__ == "__main__":\n    test_query(connect())\n```\n\nYou can pass an optional req_id in the parameters.\n\n\n```python\nfrom taos import *\nfrom ctypes import *\nimport time\n\n\ndef fetch_callback(p_param, p_result, num_of_rows):\n    print("fetched ", num_of_rows, "rows")\n    p = cast(p_param, POINTER(Counter))\n    result = TaosResult(p_result)\n\n    if num_of_rows == 0:\n        print("fetching completed")\n        p.contents.done = True\n        result.close()\n        return\n\n    if num_of_rows < 0:\n        p.contents.done = True\n        result.check_error(num_of_rows)\n        result.close()\n        return None\n\n    for row in result.rows_iter(num_of_rows):\n        # print(row)\n        pass\n\n    p.contents.count += result.row_count\n    result.fetch_rows_a(fetch_callback, p_param)\n\n\ndef query_callback(p_param, p_result, code):\n    # type: (c_void_p, c_void_p, c_int) -> None\n    if p_result is None:\n        return\n\n    result = TaosResult(p_result)\n    if code == 0:\n        result.fetch_rows_a(fetch_callback, p_param)\n\n    result.check_error(code)\n\n\nclass Counter(Structure):\n    _fields_ = [("count", c_int), ("done", c_bool)]\n\n    def __str__(self):\n        return "{ count: %d, done: %s }" % (self.count, self.done)\n\n\ndef test_query(conn):\n    # type: (TaosConnection) -> None\n    counter = Counter(count=0)\n    conn.query_a("select * from log.log", query_callback, byref(counter), req_id=1)\n\n    while not counter.done:\n        print("wait query callback")\n        time.sleep(1)\n\n    print(counter)\n    conn.close()\n\n\nif __name__ == "__main__":\n    test_query(connect())\n```\n\n### Statement API - Bind row after row\n\n```python\nfrom taos import *\n\nconn = connect()\n\ndbname = "pytest_taos_stmt"\nconn.execute("drop database if exists %s" % dbname)\nconn.execute("create database if not exists %s" % dbname)\nconn.select_db(dbname)\n\nconn.execute(\n    "create table if not exists log(ts timestamp, bo bool, nil tinyint, \\\n        ti tinyint, si smallint, ii int, bi bigint, tu tinyint unsigned, \\\n        su smallint unsigned, iu int unsigned, bu bigint unsigned, \\\n        ff float, dd double, bb binary(100), nn nchar(100), tt timestamp)",\n)\n\nstmt = conn.statement("insert into log values(?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?)")\n\nparams = new_bind_params(16)\nparams[0].timestamp(1626861392589)\nparams[1].bool(True)\nparams[2].tinyint(None)\nparams[3].tinyint(2)\nparams[4].smallint(3)\nparams[5].int(4)\nparams[6].bigint(5)\nparams[7].tinyint_unsigned(6)\nparams[8].smallint_unsigned(7)\nparams[9].int_unsigned(8)\nparams[10].bigint_unsigned(9)\nparams[11].float(10.1)\nparams[12].double(10.11)\nparams[13].binary("hello")\nparams[14].nchar("stmt")\nparams[15].timestamp(1626861392589)\nstmt.bind_param(params)\n\nparams[0].timestamp(1626861392590)\nparams[15].timestamp(None)\nstmt.bind_param(params)\nstmt.execute()\n\nassert stmt.affected_rows == 2\n\nresult = conn.query("select * from log")\n\nfor row in result:\n    print(row)\n```\n\n### Statement API - Bind multi rows\n\n```python\nfrom taos import *\n\nconn = connect()\n\ndbname = "pytest_taos_stmt"\nconn.execute("drop database if exists %s" % dbname)\nconn.execute("create database if not exists %s" % dbname)\nconn.select_db(dbname)\n\nconn.execute(\n    "create table if not exists log(ts timestamp, bo bool, nil tinyint, \\\n        ti tinyint, si smallint, ii int, bi bigint, tu tinyint unsigned, \\\n        su smallint unsigned, iu int unsigned, bu bigint unsigned, \\\n        ff float, dd double, bb binary(100), nn nchar(100), tt timestamp)",\n)\n\nstmt = conn.statement("insert into log values(?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?)")\n\nparams = new_multi_binds(16)\nparams[0].timestamp((1626861392589, 1626861392590, 1626861392591))\nparams[1].bool((True, None, False))\nparams[2].tinyint([-128, -128, None])  # -128 is tinyint null\nparams[3].tinyint([0, 127, None])\nparams[4].smallint([3, None, 2])\nparams[5].int([3, 4, None])\nparams[6].bigint([3, 4, None])\nparams[7].tinyint_unsigned([3, 4, None])\nparams[8].smallint_unsigned([3, 4, None])\nparams[9].int_unsigned([3, 4, None])\nparams[10].bigint_unsigned([3, 4, None])\nparams[11].float([3, None, 1])\nparams[12].double([3, None, 1.2])\nparams[13].binary(["abc", "dddafadfadfadfadfa", None])\nparams[14].nchar(["涛思数据", None, "a long string with 中文字符"])\nparams[15].timestamp([None, None, 1626861392591])\nstmt.bind_param_batch(params)\nstmt.execute()\n\nassert stmt.affected_rows == 3\n\nresult = conn.query("select * from log")\nfor row in result:\n    print(row)\n```\n\n### Subscription\n\n```python\nimport taos\nimport random\n\nconn = taos.connect()\ndbname = "pytest_taos_subscribe"\nconn.execute("drop database if exists %s" % dbname)\nconn.execute("create database if not exists %s" % dbname)\nconn.select_db(dbname)\nconn.execute("create table if not exists log(ts timestamp, n int)")\nfor i in range(10):\n    conn.execute("insert into log values(now, %d)" % i)\n\nsub = conn.subscribe(False, "test", "select * from log", 1000)\nprint("# consume from begin")\nfor ts, n in sub.consume():\n    print(ts, n)\n\nprint("# consume new data")\nfor i in range(5):\n    conn.execute("insert into log values(now, %d)(now+1s, %d)" % (i, i))\n    result = sub.consume()\n    for ts, n in result:\n        print(ts, n)\n\nsub.close(True)\nprint("# keep progress consume")\nsub = conn.subscribe(False, "test", "select * from log", 1000)\nresult = sub.consume()\nrows = result.fetch_all()\n# consume from latest subscription needs root privilege(for /var/lib/taos).\nassert result.row_count == 0\nprint("## consumed ", len(rows), "rows")\n\nprint("# consume with a stop condition")\nfor i in range(10):\n    conn.execute("insert into log values(now, %d)" % random.randint(0, 10))\n    result = sub.consume()\n    try:\n        ts, n = next(result)\n        print(ts, n)\n        if n > 5:\n            result.stop_query()\n            print("## stopped")\n            break\n    except StopIteration:\n        continue\n\nsub.close()\n# sub.close()\n\nconn.execute("drop database if exists %s" % dbname)\n# conn.close()\n```\n\n### Subscription asynchronously with callback\n\n```python\nfrom taos import *\nfrom ctypes import *\n\nimport time\n\n\ndef subscribe_callback(p_sub, p_result, p_param, errno):\n    # type: (c_void_p, c_void_p, c_void_p, c_int) -> None\n    print("# fetch in callback")\n    result = TaosResult(c_void_p(p_result))\n    result.check_error(errno)\n    for row in result.rows_iter():\n        ts, n = row()\n        print(ts, n)\n\n\ndef test_subscribe_callback(conn):\n    # type: (TaosConnection) -> None\n    dbname = "pytest_taos_subscribe_callback"\n    try:\n        print("drop if exists")\n        conn.execute("drop database if exists %s" % dbname)\n        print("create database")\n        conn.execute("create database if not exists %s" % dbname)\n        print("create table")\n        # conn.execute("use %s" % dbname)\n        conn.execute("create table if not exists %s.log(ts timestamp, n int)" % dbname)\n\n        print("# subscribe with callback")\n        sub = conn.subscribe(False, "test", "select * from %s.log" % dbname, 1000, subscribe_callback)\n\n        for i in range(10):\n            conn.execute("insert into %s.log values(now, %d)" % (dbname, i))\n            time.sleep(0.7)\n\n        sub.close()\n\n        conn.execute("drop database if exists %s" % dbname)\n        # conn.close()\n    except Exception as err:\n        conn.execute("drop database if exists %s" % dbname)\n        # conn.close()\n        raise err\n\n\nif __name__ == "__main__":\n    test_subscribe_callback(connect())\n```\n\n### Insert with line protocol\n\n```python\nimport taos\nfrom taos import SmlProtocol, SmlPrecision\n\nconn = taos.connect()\ndbname = "pytest_line"\nconn.execute("drop database if exists %s" % dbname)\nconn.execute("create database if not exists %s precision \'us\'" % dbname)\nconn.select_db(dbname)\n\nlines = [\n    \'st,t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"pass",c2=false,c4=4f64 1626006833639000000\',\n]\nconn.schemaless_insert(lines, taos.SmlProtocol.LINE_PROTOCOL, taos.SmlPrecision.NOT_CONFIGURED)\nprint("inserted")\n\nconn.schemaless_insert(lines, taos.SmlProtocol.LINE_PROTOCOL, taos.SmlPrecision.NOT_CONFIGURED)\n\nresult = conn.query("show tables")\nfor row in result:\n    print(row)\n\nconn.execute("drop database if exists %s" % dbname)\n```\n\nYou can pass an optional req_id in the parameters.\n\n\n```python\nimport taos\nfrom taos import SmlProtocol, SmlPrecision\n\nconn = taos.connect()\ndbname = "pytest_line"\nconn.execute("drop database if exists %s" % dbname)\nconn.execute("create database if not exists %s precision \'us\'" % dbname)\nconn.select_db(dbname)\n\nlines = [\n    \'st,t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"pass",c2=false,c4=4f64 1626006833639000000\',\n]\nconn.schemaless_insert(lines, taos.SmlProtocol.LINE_PROTOCOL, taos.SmlPrecision.NOT_CONFIGURED, req_id=1)\nprint("inserted")\n\nconn.schemaless_insert(lines, taos.SmlProtocol.LINE_PROTOCOL, taos.SmlPrecision.NOT_CONFIGURED, req_id=2)\n\nresult = conn.query("show tables")\nfor row in result:\n    print(row)\n\nconn.execute("drop database if exists %s" % dbname)\n```\n\nInsert with schemaless raw data.\n\n```python\nimport taos\nfrom taos import utils\nfrom taos import TaosConnection\nfrom taos.cinterface import *\nfrom taos.error import OperationalError, SchemalessError\n\nconn = taos.connect()\ndbname = "taos_schemaless_insert"\ntry:\n    conn.execute("drop database if exists %s" % dbname)\n\n    if taos.IS_V3:\n        conn.execute("create database if not exists %s schemaless 1 precision \'ns\'" % dbname)\n    else:\n        conn.execute("create database if not exists %s update 2 precision \'ns\'" % dbname)\n\n    conn.select_db(dbname)\n\n    lines = \'\'\'st,t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\n    st,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin, abc",c2=true,c4=5f64,c5=5f64,c6=7u64 1626006933640000000\n    stf,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n\n    res = conn.schemaless_insert_raw(lines, 1, 0)\n    print("affected rows: ", res)\n    assert (res == 3)\n\n    lines = \'\'\'stf,t1=5i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n    res = conn.schemaless_insert_raw(lines, 1, 0)\n    print("affected rows: ", res)\n    assert (res == 1)\n\n    result = conn.query("select * from st")\n    dict2 = result.fetch_all_into_dict()\n    print(dict2)\n    print(result.row_count)\n\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n    assert (result.row_count == 2)\n\n    # error test\n    lines = \'\'\',t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\'\'\'\n    try:\n        res = conn.schemaless_insert_raw(lines, 1, 0)\n        print(res)\n        # assert(False)\n    except SchemalessError as err:\n        print(\'**** error: \', err)\n        # assert (err.msg == \'Invalid data format\')\n\n    result = conn.query("select * from st")\n    print(result.row_count)\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\nexcept InterfaceError as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\nexcept SchemalessError as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\nexcept Exception as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\n    raise err\n\n```\n\nPass optional ttl in the parameters.\n\n```python\nimport taos\nfrom taos import utils\nfrom taos import TaosConnection\nfrom taos.cinterface import *\nfrom taos.error import OperationalError, SchemalessError\n\nconn = taos.connect()\ndbname = "taos_schemaless_insert"\ntry:\n    conn.execute("drop database if exists %s" % dbname)\n\n    if taos.IS_V3:\n        conn.execute("create database if not exists %s schemaless 1 precision \'ns\'" % dbname)\n    else:\n        conn.execute("create database if not exists %s update 2 precision \'ns\'" % dbname)\n\n    conn.select_db(dbname)\n\n    lines = \'\'\'st,t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\n    st,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin, abc",c2=true,c4=5f64,c5=5f64,c6=7u64 1626006933640000000\n    stf,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n\n    ttl = 1000\n    res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl)\n    print("affected rows: ", res)\n    assert (res == 3)\n\n    lines = \'\'\'stf,t1=5i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n    ttl = 1000\n    res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl)\n    print("affected rows: ", res)\n    assert (res == 1)\n\n    result = conn.query("select * from st")\n    dict2 = result.fetch_all_into_dict()\n    print(dict2)\n    print(result.row_count)\n\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n    assert (result.row_count == 2)\n\n    # error test\n    lines = \'\'\',t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\'\'\'\n    try:\n        ttl = 1000\n        res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl)\n        print(res)\n        # assert(False)\n    except SchemalessError as err:\n        print(\'**** error: \', err)\n        # assert (err.msg == \'Invalid data format\')\n\n    result = conn.query("select * from st")\n    print(result.row_count)\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\nexcept InterfaceError as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\nexcept Exception as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\n    raise err\n```\n\nPass optional req_id in the parameters.\n\n```python\nimport taos\nfrom taos import utils\nfrom taos import TaosConnection\nfrom taos.cinterface import *\nfrom taos.error import OperationalError, SchemalessError\n\nconn = taos.connect()\ndbname = "taos_schemaless_insert"\ntry:\n    conn.execute("drop database if exists %s" % dbname)\n\n    if taos.IS_V3:\n        conn.execute("create database if not exists %s schemaless 1 precision \'ns\'" % dbname)\n    else:\n        conn.execute("create database if not exists %s update 2 precision \'ns\'" % dbname)\n\n    conn.select_db(dbname)\n\n    lines = \'\'\'st,t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\n    st,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin, abc",c2=true,c4=5f64,c5=5f64,c6=7u64 1626006933640000000\n    stf,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n\n    ttl = 1000\n    req_id = utils.gen_req_id()\n    res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl, req_id=req_id)\n    print("affected rows: ", res)\n    assert (res == 3)\n\n    lines = \'\'\'stf,t1=5i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n    ttl = 1000\n    req_id = utils.gen_req_id()\n    res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl, req_id=req_id)\n    print("affected rows: ", res)\n    assert (res == 1)\n\n    result = conn.query("select * from st")\n    dict2 = result.fetch_all_into_dict()\n    print(dict2)\n    print(result.row_count)\n\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n    assert (result.row_count == 2)\n\n    # error test\n    lines = \'\'\',t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\'\'\'\n    try:\n        ttl = 1000\n        req_id = utils.gen_req_id()\n        res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl, req_id=req_id)\n        print(res)\n        # assert(False)\n    except SchemalessError as err:\n        print(\'**** error: \', err)\n        # assert (err.msg == \'Invalid data format\')\n\n    result = conn.query("select * from st")\n    print(result.row_count)\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\nexcept InterfaceError as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\nexcept Exception as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\n    raise err\n\n```\n\n### Read with Pandas\n\n#### Method one\n\n```python\nimport pandas\nimport taos\n\nconn = taos.connect()\ndf: pandas.DataFrame = pandas.read_sql("select * from log.logs", conn)\n```\n\n#### Method Two\n\n```python\nimport pandas\nfrom sqlalchemy import create_engine\n\nengine = create_engine("taos://root:taosdata@localhost:6030/log")\ndf: pandas.DataFrame = pandas.read_sql("select * from logs", engine)\n```\n\n## Limitation\n\n- `taosrest` is designed to use with taosAdapter. If your TDengine version is older than v2.4.0.0, taosAdapter may not be available.\n\n## License\n\nWe use MIT license for Python connector.\n',
+    'long_description': '# TDengine Connector for Python\n\n| Github Workflow | PyPI Version | PyPI Downloads | CodeCov |\n| --------------- | ------------ | -------------- | ------- |\n| ![workflow](https://img.shields.io/github/actions/workflow/status/taosdata/taos-connector-python/test.yml) | ![PyPI](https://img.shields.io/pypi/v/taospy) | ![PyPI](https://img.shields.io/pypi/dm/taospy) | [![codecov](https://codecov.io/gh/taosdata/taos-connector-python/branch/main/graph/badge.svg?token=BDANN3DBXS)](https://codecov.io/gh/taosdata/taos-connector-python) |\n\n\n\n\n[TDengine](https://github.com/taosdata/TDengine) connector for Python enables python programs to access TDengine, using\nan API which is compliant with the Python DB API 2.0 (PEP-249). It contains two modules:\n\n1. The `taos` module. It uses TDengine C client library for client server communications.\n2. The `taosrest` module. It wraps TDengine RESTful API to Python DB API 2.0 (PEP-249). With this module, you do not need to install the TDengine C client library.\n\n## Install taospy\n\nYou can use `pip` to install the connector from PyPI:\n\n```bash\npip install taospy\n```\n\nOr with git url:\n\n```bash\npip install git+https://github.com/taosdata/taos-connector-python.git\n```\n\nNote: taospy v2.7.2 requirs Python 3.6+. The early versions of taospy from v2.5.0 to v2.7.1 require Python 3.7+.\n\n## Source Code\n\n[TDengine](https://github.com/taosdata/TDengine) connector for Python source code is hosted\non [GitHub](https://github.com/taosdata/taos-connector-python).\n\n## Install taos-ws-py\n\n### Install with taospy\n\n```bash\npip install taospy[ws]\n```\n\n### Install taos-ws-py only\n\n```bash\npip install taos-ws-py\n```\n\nNote: The taosws module is provided by taos-ws-py package separately from v2.7.2. It is part of early version of taospy.\ntaos-ws-py requires Python 3.7+.\n\n### Query with PEP-249 API using `taosws`\n\n```python\nimport taosws\n\n# all parameters are optional\nconn = taosws.connect("taosws://root:taosdata@localhost:6041")\ncursor = conn.cursor()\n\ncursor.execute("show databases")\nresults: list[tuple] = cursor.fetchall()\nfor row in results:\n    print(row)\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nimport taosws\n\n# all parameters are optional\nconn = taosws.connect("taosws://root:taosdata@localhost:6041")\ncursor = conn.cursor()\n\ncursor.execute("show databases", req_id=1)\nresults: list[tuple] = cursor.fetchall()\nfor row in results:\n    print(row)\n```\n\n### Query with query method using `taosws`\n\n```python\nfrom taosws import *\n\nconn = connect("taosws://root:taosdata@localhost:6041")\nresult = conn.query("show databases")\n\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nfrom taosws import *\n\nconn = connect("taosws://root:taosdata@localhost:6041")\nresult = conn.query("show databases", req_id=1)\n\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n```\n\n### Read with Pandas using `taosws`\n\n#### Method one\n\n```python\nimport pandas\nimport taosws\n\nconn = taosws.connect("taosws://root:taosdata@localhost:6041")\ndf: pandas.DataFrame = pandas.read_sql("show databases", conn)\ndf\n```\n\n#### Method Two\n\n```python\nimport pandas\nfrom sqlalchemy import create_engine\n\nengine = create_engine("taosws://root:taosdata@localhost:6041")\ndf: pandas.DataFrame = pandas.read_sql("show databases", engine)\ndf\n```\n\n## Examples for `taosrest` Module\n\n### Query with PEP-249 API\n\n```python\nimport taosrest\n\n# all parameters are optional\nconn = taosrest.connect(url="http://localhost:6041",\n                        user="root",\n                        password="taosdata")\ncursor = conn.cursor()\n\ncursor.execute("show databases")\nresults: list[tuple] = cursor.fetchall()\nfor row in results:\n    print(row)\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nimport taosrest\n\n# all parameters are optional\nconn = taosrest.connect(url="http://localhost:6041",\n                        user="root",\n                        password="taosdata")\ncursor = conn.cursor()\n\ncursor.execute("show databases", req_id=1)\nresults: list[tuple] = cursor.fetchall()\nfor row in results:\n    print(row)\n```\n\n### Query with query method\n\n```python\nfrom taosrest import connect, TaosRestConnection, Result\n\nconn: TaosRestConnection = connect()\nresult: Result = conn.query("show databases")\n\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nfrom taosrest import connect, TaosRestConnection, Result\n\nconn: TaosRestConnection = connect()\nresult: Result = conn.query("show databases", req_id=1)\n\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n```\n\n### Read with Pandas\n\n#### Method one\n\n```python\nimport pandas\nimport taos\n\nconn = taos.connect()\ndf: pandas.DataFrame = pandas.read_sql("select * from log.logs", conn)\n```\n\n#### Method two\n\n```python\nimport pandas\nimport taosrest\n\nconn = taosrest.connect()\ndf: pandas.DataFrame = pandas.read_sql("select * from log.logs", conn)\n```\n\n#### Method three\n\n```python\nimport pandas\nfrom sqlalchemy import create_engine\n\nengine = create_engine("taosrest://root:taosdata@localhost:6041")\ndf: pandas.DataFrame = pandas.read_sql("select * from log.logs", engine)\n```\n\n## Examples for `taos` Module\n\n### Connect options\n\nSupported config options:\n\n- **config**: TDengine client configuration directory, by default use "/etc/taos/".\n- **host**: TDengine server host, by default use "localhost".\n- **user**: TDengine user name, default is "root".\n- **password**: TDengine user password, default is "taosdata".\n- **database**: Default connection database name, empty if not set.\n- **timezone**: Timezone for timestamp type (which is `datetime` object with tzinfo in python) no matter what the host\'s\n  timezone is.\n\n```python\nimport taos\n\n# 1. with empty options, connect TDengine by default options\n#   that means:\n#     - use /etc/taos/taos.cfg as default configuration file\n#     - use "localhost" if not set in config file\n#     - use "root" as default username\n#     - use "taosdata" as default password\n#     - use 6030 as default port if not set in config file\n#     - use local timezone datetime as timestamp\nconn = taos.connect()\n# 2. with full set options, default db: log, use UTC datetime.\nconn = taos.connect(host=\'localhost\',\n                    user=\'root\',\n                    password=\'taosdata\',\n                    database=\'log\',\n                    config=\'/etc/taos\',\n                    timezone=\'UTC\')\n```\n\nNote that, the datetime formatted string will contain timezone information when timezone set. For example:\n\n```python\n# without timezone(local timezone depends on your machine)\n\'1969-12-31 16:00:00\'\n# with timezone UTC\n\'1969-12-31 16:00:00+00:00\'\n```\n\n### Query with PEP-249 API\n\n```python\nimport taos\n\nconn = taos.connect()\ncursor = conn.cursor()\n\ncursor.execute("show databases")\nresults = cursor.fetchall()\nfor row in results:\n    print(row)\n\ncursor.close()\nconn.close()\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nimport taos\n\nconn = taos.connect()\ncursor = conn.cursor()\n\ncursor.execute("show databases", req_id=1)\nresults = cursor.fetchall()\nfor row in results:\n    print(row)\n\ncursor.close()\nconn.close()\n```\n\n#### Execute many\n\nMethod execute_many is supported:\n\nThere are two ways to use execute_many.\n\nThe first way is to pass a data_set as a list of dictionaries, where each dictionary will be expanded into a complete\nstatement.\n\n```python\nimport taos\n\nconn = taos.connect()\ncursor = conn.cursor()\n\ndb_name = "test_db"\n\ncursor.execute(f"DROP DATABASE IF EXISTS {db_name}")\ncursor.execute(f"CREATE DATABASE {db_name}")\ncursor.execute(f"USE {db_name}")\n\ncursor.execute("create stable stb (ts timestamp, v1 int) tags(t1 int)")\n\ncreate_table_data = [\n    {\n        "name": "tb1",\n        "t1": 1,\n    },\n    {\n        "name": "tb2",\n        "t1": 2,\n    },\n    {\n        "name": "tb3",\n        "t1": 3,\n    }\n]\n\ncursor.execute_many(\n    "create table {name} using stb tags({t1})",\n    create_table_data,\n)\n\n```\n\nThe second way is to pass a data_set as a list of tuples, where each tuple represents a different row of the same\ntable, and each value within the tuple will become a data row in the SQL statement. All the data together will form a\ncomplete SQL statement.\n\n```python\nimport taos\n\nconn = taos.connect()\ncursor = conn.cursor()\n\ndb_name = "test_db"\n\ncursor.execute(f"USE {db_name}")\n\ndata_set = [\n    (\'2018-10-03 14:38:05.100\', 219),\n    (\'2018-10-03 14:38:15.300\', 218),\n    (\'2018-10-03 14:38:16.800\', 221),\n]\n\ntable_name = "tb1"\n\ncursor.execute_many(f"insert into {table_name} values", data_set)\n\n```\n\n[Example: Insert many lines in one execute](./examples/cursor_execute_many.py)\n\n### Query with objective API\n\n```python\nimport taos\n\nconn = taos.connect()\nconn.execute("create database if not exists pytest")\n\nresult = conn.query("show databases")\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n\nresult.close()\nconn.execute("drop database pytest")\nconn.close()\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nimport taos\n\nconn = taos.connect()\nconn.execute("create database if not exists pytest", req_id=1)\n\nresult = conn.query("show databases")\nnum_of_fields = result.field_count\nfor field in result.fields:\n    print(field)\n\nfor row in result:\n    print(row)\n\nresult.close()\nconn.execute("drop database pytest")\nconn.close()\n```\n\n### Query with async API\n\n```python\nfrom taos import *\nfrom ctypes import *\nimport time\n\n\ndef fetch_callback(p_param, p_result, num_of_rows):\n    print("fetched ", num_of_rows, "rows")\n    p = cast(p_param, POINTER(Counter))\n    result = TaosResult(p_result)\n\n    if num_of_rows == 0:\n        print("fetching completed")\n        p.contents.done = True\n        result.close()\n        return\n\n    if num_of_rows < 0:\n        p.contents.done = True\n        result.check_error(num_of_rows)\n        result.close()\n        return None\n\n    for row in result.rows_iter(num_of_rows):\n        # print(row)\n        pass\n\n    p.contents.count += result.row_count\n    result.fetch_rows_a(fetch_callback, p_param)\n\n\ndef query_callback(p_param, p_result, code):\n    # type: (c_void_p, c_void_p, c_int) -> None\n    if p_result is None:\n        return\n\n    result = TaosResult(p_result)\n    if code == 0:\n        result.fetch_rows_a(fetch_callback, p_param)\n\n    result.check_error(code)\n\n\nclass Counter(Structure):\n    _fields_ = [("count", c_int), ("done", c_bool)]\n\n    def __str__(self):\n        return "{ count: %d, done: %s }" % (self.count, self.done)\n\n\ndef test_query(conn):\n    # type: (TaosConnection) -> None\n    counter = Counter(count=0)\n    conn.query_a("select * from log.log", query_callback, byref(counter))\n\n    while not counter.done:\n        print("wait query callback")\n        time.sleep(1)\n\n    print(counter)\n    conn.close()\n\n\nif __name__ == "__main__":\n    test_query(connect())\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nfrom taos import *\nfrom ctypes import *\nimport time\n\n\ndef fetch_callback(p_param, p_result, num_of_rows):\n    print("fetched ", num_of_rows, "rows")\n    p = cast(p_param, POINTER(Counter))\n    result = TaosResult(p_result)\n\n    if num_of_rows == 0:\n        print("fetching completed")\n        p.contents.done = True\n        result.close()\n        return\n\n    if num_of_rows < 0:\n        p.contents.done = True\n        result.check_error(num_of_rows)\n        result.close()\n        return None\n\n    for row in result.rows_iter(num_of_rows):\n        # print(row)\n        pass\n\n    p.contents.count += result.row_count\n    result.fetch_rows_a(fetch_callback, p_param)\n\n\ndef query_callback(p_param, p_result, code):\n    # type: (c_void_p, c_void_p, c_int) -> None\n    if p_result is None:\n        return\n\n    result = TaosResult(p_result)\n    if code == 0:\n        result.fetch_rows_a(fetch_callback, p_param)\n\n    result.check_error(code)\n\n\nclass Counter(Structure):\n    _fields_ = [("count", c_int), ("done", c_bool)]\n\n    def __str__(self):\n        return "{ count: %d, done: %s }" % (self.count, self.done)\n\n\ndef test_query(conn):\n    # type: (TaosConnection) -> None\n    counter = Counter(count=0)\n    conn.query_a("select * from log.log", query_callback, byref(counter), req_id=1)\n\n    while not counter.done:\n        print("wait query callback")\n        time.sleep(1)\n\n    print(counter)\n    conn.close()\n\n\nif __name__ == "__main__":\n    test_query(connect())\n```\n\n### Statement API - Bind row after row\n\n```python\nfrom taos import *\n\nconn = connect()\n\ndbname = "pytest_taos_stmt"\nconn.execute("drop database if exists %s" % dbname)\nconn.execute("create database if not exists %s" % dbname)\nconn.select_db(dbname)\n\nconn.execute(\n    "create table if not exists log(ts timestamp, bo bool, nil tinyint, \\\n        ti tinyint, si smallint, ii int, bi bigint, tu tinyint unsigned, \\\n        su smallint unsigned, iu int unsigned, bu bigint unsigned, \\\n        ff float, dd double, bb binary(100), nn nchar(100), tt timestamp)",\n)\n\nstmt = conn.statement("insert into log values(?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?)")\n\nparams = new_bind_params(16)\nparams[0].timestamp(1626861392589)\nparams[1].bool(True)\nparams[2].tinyint(None)\nparams[3].tinyint(2)\nparams[4].smallint(3)\nparams[5].int(4)\nparams[6].bigint(5)\nparams[7].tinyint_unsigned(6)\nparams[8].smallint_unsigned(7)\nparams[9].int_unsigned(8)\nparams[10].bigint_unsigned(9)\nparams[11].float(10.1)\nparams[12].double(10.11)\nparams[13].binary("hello")\nparams[14].nchar("stmt")\nparams[15].timestamp(1626861392589)\nstmt.bind_param(params)\n\nparams[0].timestamp(1626861392590)\nparams[15].timestamp(None)\nstmt.bind_param(params)\nstmt.execute()\n\nassert stmt.affected_rows == 2\n\nresult = conn.query("select * from log")\n\nfor row in result:\n    print(row)\n```\n\n### Statement API - Bind multi rows\n\n```python\nfrom taos import *\n\nconn = connect()\n\ndbname = "pytest_taos_stmt"\nconn.execute("drop database if exists %s" % dbname)\nconn.execute("create database if not exists %s" % dbname)\nconn.select_db(dbname)\n\nconn.execute(\n    "create table if not exists log(ts timestamp, bo bool, nil tinyint, \\\n        ti tinyint, si smallint, ii int, bi bigint, tu tinyint unsigned, \\\n        su smallint unsigned, iu int unsigned, bu bigint unsigned, \\\n        ff float, dd double, bb binary(100), nn nchar(100), tt timestamp)",\n)\n\nstmt = conn.statement("insert into log values(?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?)")\n\nparams = new_multi_binds(16)\nparams[0].timestamp((1626861392589, 1626861392590, 1626861392591))\nparams[1].bool((True, None, False))\nparams[2].tinyint([-128, -128, None])  # -128 is tinyint null\nparams[3].tinyint([0, 127, None])\nparams[4].smallint([3, None, 2])\nparams[5].int([3, 4, None])\nparams[6].bigint([3, 4, None])\nparams[7].tinyint_unsigned([3, 4, None])\nparams[8].smallint_unsigned([3, 4, None])\nparams[9].int_unsigned([3, 4, None])\nparams[10].bigint_unsigned([3, 4, None])\nparams[11].float([3, None, 1])\nparams[12].double([3, None, 1.2])\nparams[13].binary(["abc", "dddafadfadfadfadfa", None])\nparams[14].nchar(["涛思数据", None, "a long string with 中文字符"])\nparams[15].timestamp([None, None, 1626861392591])\nstmt.bind_param_batch(params)\nstmt.execute()\n\nassert stmt.affected_rows == 3\n\nresult = conn.query("select * from log")\nfor row in result:\n    print(row)\n```\n\n### Subscription\n\n```python\nimport taos\nimport random\n\nconn = taos.connect()\ndbname = "pytest_taos_subscribe"\nconn.execute("drop database if exists %s" % dbname)\nconn.execute("create database if not exists %s" % dbname)\nconn.select_db(dbname)\nconn.execute("create table if not exists log(ts timestamp, n int)")\nfor i in range(10):\n    conn.execute("insert into log values(now, %d)" % i)\n\nsub = conn.subscribe(False, "test", "select * from log", 1000)\nprint("# consume from begin")\nfor ts, n in sub.consume():\n    print(ts, n)\n\nprint("# consume new data")\nfor i in range(5):\n    conn.execute("insert into log values(now, %d)(now+1s, %d)" % (i, i))\n    result = sub.consume()\n    for ts, n in result:\n        print(ts, n)\n\nsub.close(True)\nprint("# keep progress consume")\nsub = conn.subscribe(False, "test", "select * from log", 1000)\nresult = sub.consume()\nrows = result.fetch_all()\n# consume from latest subscription needs root privilege(for /var/lib/taos).\nassert result.row_count == 0\nprint("## consumed ", len(rows), "rows")\n\nprint("# consume with a stop condition")\nfor i in range(10):\n    conn.execute("insert into log values(now, %d)" % random.randint(0, 10))\n    result = sub.consume()\n    try:\n        ts, n = next(result)\n        print(ts, n)\n        if n > 5:\n            result.stop_query()\n            print("## stopped")\n            break\n    except StopIteration:\n        continue\n\nsub.close()\n# sub.close()\n\nconn.execute("drop database if exists %s" % dbname)\n# conn.close()\n```\n\n### Subscription asynchronously with callback\n\n```python\nfrom taos import *\nfrom ctypes import *\n\nimport time\n\n\ndef subscribe_callback(p_sub, p_result, p_param, errno):\n    # type: (c_void_p, c_void_p, c_void_p, c_int) -> None\n    print("# fetch in callback")\n    result = TaosResult(c_void_p(p_result))\n    result.check_error(errno)\n    for row in result.rows_iter():\n        ts, n = row()\n        print(ts, n)\n\n\ndef test_subscribe_callback(conn):\n    # type: (TaosConnection) -> None\n    dbname = "pytest_taos_subscribe_callback"\n    try:\n        print("drop if exists")\n        conn.execute("drop database if exists %s" % dbname)\n        print("create database")\n        conn.execute("create database if not exists %s" % dbname)\n        print("create table")\n        # conn.execute("use %s" % dbname)\n        conn.execute("create table if not exists %s.log(ts timestamp, n int)" % dbname)\n\n        print("# subscribe with callback")\n        sub = conn.subscribe(False, "test", "select * from %s.log" % dbname, 1000, subscribe_callback)\n\n        for i in range(10):\n            conn.execute("insert into %s.log values(now, %d)" % (dbname, i))\n            time.sleep(0.7)\n\n        sub.close()\n\n        conn.execute("drop database if exists %s" % dbname)\n        # conn.close()\n    except Exception as err:\n        conn.execute("drop database if exists %s" % dbname)\n        # conn.close()\n        raise err\n\n\nif __name__ == "__main__":\n    test_subscribe_callback(connect())\n```\n\n### Insert with line protocol\n\n```python\nimport taos\nfrom taos import SmlProtocol, SmlPrecision\n\nconn = taos.connect()\ndbname = "pytest_line"\nconn.execute("drop database if exists %s" % dbname)\nconn.execute("create database if not exists %s precision \'us\'" % dbname)\nconn.select_db(dbname)\n\nlines = [\n    \'st,t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"pass",c2=false,c4=4f64 1626006833639000000\',\n]\nconn.schemaless_insert(lines, taos.SmlProtocol.LINE_PROTOCOL, taos.SmlPrecision.NOT_CONFIGURED)\nprint("inserted")\n\nconn.schemaless_insert(lines, taos.SmlProtocol.LINE_PROTOCOL, taos.SmlPrecision.NOT_CONFIGURED)\n\nresult = conn.query("show tables")\nfor row in result:\n    print(row)\n\nconn.execute("drop database if exists %s" % dbname)\n```\n\nYou can pass an optional req_id in the parameters.\n\n```python\nimport taos\nfrom taos import SmlProtocol, SmlPrecision\n\nconn = taos.connect()\ndbname = "pytest_line"\nconn.execute("drop database if exists %s" % dbname)\nconn.execute("create database if not exists %s precision \'us\'" % dbname)\nconn.select_db(dbname)\n\nlines = [\n    \'st,t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"pass",c2=false,c4=4f64 1626006833639000000\',\n]\nconn.schemaless_insert(lines, taos.SmlProtocol.LINE_PROTOCOL, taos.SmlPrecision.NOT_CONFIGURED, req_id=1)\nprint("inserted")\n\nconn.schemaless_insert(lines, taos.SmlProtocol.LINE_PROTOCOL, taos.SmlPrecision.NOT_CONFIGURED, req_id=2)\n\nresult = conn.query("show tables")\nfor row in result:\n    print(row)\n\nconn.execute("drop database if exists %s" % dbname)\n```\n\nInsert with schemaless raw data.\n\n```python\nimport taos\nfrom taos import utils\nfrom taos import TaosConnection\nfrom taos.cinterface import *\nfrom taos.error import OperationalError, SchemalessError\n\nconn = taos.connect()\ndbname = "taos_schemaless_insert"\ntry:\n    conn.execute("drop database if exists %s" % dbname)\n\n    if taos.IS_V3:\n        conn.execute("create database if not exists %s schemaless 1 precision \'ns\'" % dbname)\n    else:\n        conn.execute("create database if not exists %s update 2 precision \'ns\'" % dbname)\n\n    conn.select_db(dbname)\n\n    lines = \'\'\'st,t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\n    st,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin, abc",c2=true,c4=5f64,c5=5f64,c6=7u64 1626006933640000000\n    stf,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n\n    res = conn.schemaless_insert_raw(lines, 1, 0)\n    print("affected rows: ", res)\n    assert (res == 3)\n\n    lines = \'\'\'stf,t1=5i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n    res = conn.schemaless_insert_raw(lines, 1, 0)\n    print("affected rows: ", res)\n    assert (res == 1)\n\n    result = conn.query("select * from st")\n    dict2 = result.fetch_all_into_dict()\n    print(dict2)\n    print(result.row_count)\n\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n    assert (result.row_count == 2)\n\n    # error test\n    lines = \'\'\',t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\'\'\'\n    try:\n        res = conn.schemaless_insert_raw(lines, 1, 0)\n        print(res)\n        # assert(False)\n    except SchemalessError as err:\n        print(\'**** error: \', err)\n        # assert (err.msg == \'Invalid data format\')\n\n    result = conn.query("select * from st")\n    print(result.row_count)\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\nexcept InterfaceError as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\nexcept SchemalessError as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\nexcept Exception as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\n    raise err\n\n```\n\nPass optional ttl in the parameters.\n\n```python\nimport taos\nfrom taos import utils\nfrom taos import TaosConnection\nfrom taos.cinterface import *\nfrom taos.error import OperationalError, SchemalessError\n\nconn = taos.connect()\ndbname = "taos_schemaless_insert"\ntry:\n    conn.execute("drop database if exists %s" % dbname)\n\n    if taos.IS_V3:\n        conn.execute("create database if not exists %s schemaless 1 precision \'ns\'" % dbname)\n    else:\n        conn.execute("create database if not exists %s update 2 precision \'ns\'" % dbname)\n\n    conn.select_db(dbname)\n\n    lines = \'\'\'st,t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\n    st,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin, abc",c2=true,c4=5f64,c5=5f64,c6=7u64 1626006933640000000\n    stf,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n\n    ttl = 1000\n    res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl)\n    print("affected rows: ", res)\n    assert (res == 3)\n\n    lines = \'\'\'stf,t1=5i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n    ttl = 1000\n    res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl)\n    print("affected rows: ", res)\n    assert (res == 1)\n\n    result = conn.query("select * from st")\n    dict2 = result.fetch_all_into_dict()\n    print(dict2)\n    print(result.row_count)\n\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n    assert (result.row_count == 2)\n\n    # error test\n    lines = \'\'\',t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\'\'\'\n    try:\n        ttl = 1000\n        res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl)\n        print(res)\n        # assert(False)\n    except SchemalessError as err:\n        print(\'**** error: \', err)\n        # assert (err.msg == \'Invalid data format\')\n\n    result = conn.query("select * from st")\n    print(result.row_count)\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\nexcept InterfaceError as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\nexcept Exception as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\n    raise err\n```\n\nPass optional req_id in the parameters.\n\n```python\nimport taos\nfrom taos import utils\nfrom taos import TaosConnection\nfrom taos.cinterface import *\nfrom taos.error import OperationalError, SchemalessError\n\nconn = taos.connect()\ndbname = "taos_schemaless_insert"\ntry:\n    conn.execute("drop database if exists %s" % dbname)\n\n    if taos.IS_V3:\n        conn.execute("create database if not exists %s schemaless 1 precision \'ns\'" % dbname)\n    else:\n        conn.execute("create database if not exists %s update 2 precision \'ns\'" % dbname)\n\n    conn.select_db(dbname)\n\n    lines = \'\'\'st,t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\n    st,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin, abc",c2=true,c4=5f64,c5=5f64,c6=7u64 1626006933640000000\n    stf,t1=4i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n\n    ttl = 1000\n    req_id = utils.gen_req_id()\n    res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl, req_id=req_id)\n    print("affected rows: ", res)\n    assert (res == 3)\n\n    lines = \'\'\'stf,t1=5i64,t3="t4",t2=5f64,t4=5f64 c1=3i64,c3=L"passitagin_stf",c2=false,c5=5f64,c6=7u64 1626006933641000000\'\'\'\n    ttl = 1000\n    req_id = utils.gen_req_id()\n    res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl, req_id=req_id)\n    print("affected rows: ", res)\n    assert (res == 1)\n\n    result = conn.query("select * from st")\n    dict2 = result.fetch_all_into_dict()\n    print(dict2)\n    print(result.row_count)\n\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n    assert (result.row_count == 2)\n\n    # error test\n    lines = \'\'\',t1=3i64,t2=4f64,t3="t3" c1=3i64,c3=L"passit",c2=false,c4=4f64 1626006833639000000\'\'\'\n    try:\n        ttl = 1000\n        req_id = utils.gen_req_id()\n        res = conn.schemaless_insert_raw(lines, 1, 0, ttl=ttl, req_id=req_id)\n        print(res)\n        # assert(False)\n    except SchemalessError as err:\n        print(\'**** error: \', err)\n        # assert (err.msg == \'Invalid data format\')\n\n    result = conn.query("select * from st")\n    print(result.row_count)\n    all = result.rows_iter()\n    for row in all:\n        print(row)\n    result.close()\n\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\nexcept InterfaceError as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\nexcept Exception as err:\n    conn.execute("drop database if exists %s" % dbname)\n    conn.close()\n    print(err)\n    raise err\n\n```\n\n### Read with Pandas\n\n#### Method one\n\n```python\nimport pandas\nimport taos\n\nconn = taos.connect()\ndf: pandas.DataFrame = pandas.read_sql("select * from log.logs", conn)\n```\n\n#### Method Two\n\n```python\nimport pandas\nfrom sqlalchemy import create_engine\n\nengine = create_engine("taos://root:taosdata@localhost:6030/log")\ndf: pandas.DataFrame = pandas.read_sql("select * from logs", engine)\n```\n\n## Limitation\n\n- `taosrest` is designed to use with taosAdapter. If your TDengine version is older than v2.4.0.0, taosAdapter may not\n  be available.\n\n## License\n\nWe use MIT license for Python connector.\n',
     'author': 'Taosdata Inc.',
     'author_email': 'support@taosdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `taospy-2.7.7/PKG-INFO` & `taospy-2.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taospy
-Version: 2.7.7
+Version: 2.7.8
 Summary: TDengine connector for python
 License: MIT
 Author: Taosdata Inc.
 Author-email: support@taosdata.com
 Requires-Python: >=3.6.2,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,25 +12,32 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: ws
 Requires-Dist: iso8601 (==1.0.2)
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: pytz
-Requires-Dist: requests (==2.27.1)
+Requires-Dist: requests (>=2.27.1)
 Requires-Dist: taos-ws-py (>=0.2.0); (python_version >= "3.7" and python_version < "4.0") and (extra == "ws")
 Description-Content-Type: text/markdown
 
 # TDengine Connector for Python
-[![codecov](https://codecov.io/gh/taosdata/taos-connector-python/branch/main/graph/badge.svg?token=BDANN3DBXS)](https://codecov.io/gh/taosdata/taos-connector-python)
 
-[TDengine](https://github.com/taosdata/TDengine) connector for Python enables python programs to access TDengine, using an API which is compliant with the Python DB API 2.0 (PEP-249). It contains two modules:
+| Github Workflow | PyPI Version | PyPI Downloads | CodeCov |
+| --------------- | ------------ | -------------- | ------- |
+| ![workflow](https://img.shields.io/github/actions/workflow/status/taosdata/taos-connector-python/test.yml) | ![PyPI](https://img.shields.io/pypi/v/taospy) | ![PyPI](https://img.shields.io/pypi/dm/taospy) | [![codecov](https://codecov.io/gh/taosdata/taos-connector-python/branch/main/graph/badge.svg?token=BDANN3DBXS)](https://codecov.io/gh/taosdata/taos-connector-python) |
+
+
+
+
+[TDengine](https://github.com/taosdata/TDengine) connector for Python enables python programs to access TDengine, using
+an API which is compliant with the Python DB API 2.0 (PEP-249). It contains two modules:
 
 1. The `taos` module. It uses TDengine C client library for client server communications.
-2. The `taosrest` module. It wraps TDengine RESTful API to Python DB API 2.0 (PEP-249). With this module, you are free to install TDengine C client library.
+2. The `taosrest` module. It wraps TDengine RESTful API to Python DB API 2.0 (PEP-249). With this module, you do not need to install the TDengine C client library.
 
 ## Install taospy
 
 You can use `pip` to install the connector from PyPI:
 
 ```bash
 pip install taospy
@@ -42,15 +49,16 @@
 pip install git+https://github.com/taosdata/taos-connector-python.git
 ```
 
 Note: taospy v2.7.2 requirs Python 3.6+. The early versions of taospy from v2.5.0 to v2.7.1 require Python 3.7+.
 
 ## Source Code
 
-[TDengine](https://github.com/taosdata/TDengine) connector for Python source code is hosted on [GitHub](https://github.com/taosdata/taos-connector-python).
+[TDengine](https://github.com/taosdata/TDengine) connector for Python source code is hosted
+on [GitHub](https://github.com/taosdata/taos-connector-python).
 
 ## Install taos-ws-py
 
 ### Install with taospy
 
 ```bash
 pip install taospy[ws]
@@ -58,15 +66,16 @@
 
 ### Install taos-ws-py only
 
 ```bash
 pip install taos-ws-py
 ```
 
-Note: The taosws module is provided by taos-ws-py package separately from v2.7.2. It is part of early version of taospy. taos-ws-py requires Python 3.7+.
+Note: The taosws module is provided by taos-ws-py package separately from v2.7.2. It is part of early version of taospy.
+taos-ws-py requires Python 3.7+.
 
 ### Query with PEP-249 API using `taosws`
 
 ```python
 import taosws
 
 # all parameters are optional
@@ -214,15 +223,14 @@
 for field in result.fields:
     print(field)
 
 for row in result:
     print(row)
 ```
 
-
 ### Read with Pandas
 
 #### Method one
 
 ```python
 import pandas
 import taos
@@ -258,15 +266,16 @@
 Supported config options:
 
 - **config**: TDengine client configuration directory, by default use "/etc/taos/".
 - **host**: TDengine server host, by default use "localhost".
 - **user**: TDengine user name, default is "root".
 - **password**: TDengine user password, default is "taosdata".
 - **database**: Default connection database name, empty if not set.
-- **timezone**: Timezone for timestamp type (which is `datetime` object with tzinfo in python) no matter what the host's timezone is.
+- **timezone**: Timezone for timestamp type (which is `datetime` object with tzinfo in python) no matter what the host's
+  timezone is.
 
 ```python
 import taos
 
 # 1. with empty options, connect TDengine by default options
 #   that means:
 #     - use /etc/taos/taos.cfg as default configuration file
@@ -324,14 +333,87 @@
 for row in results:
     print(row)
 
 cursor.close()
 conn.close()
 ```
 
+#### Execute many
+
+Method execute_many is supported:
+
+There are two ways to use execute_many.
+
+The first way is to pass a data_set as a list of dictionaries, where each dictionary will be expanded into a complete
+statement.
+
+```python
+import taos
+
+conn = taos.connect()
+cursor = conn.cursor()
+
+db_name = "test_db"
+
+cursor.execute(f"DROP DATABASE IF EXISTS {db_name}")
+cursor.execute(f"CREATE DATABASE {db_name}")
+cursor.execute(f"USE {db_name}")
+
+cursor.execute("create stable stb (ts timestamp, v1 int) tags(t1 int)")
+
+create_table_data = [
+    {
+        "name": "tb1",
+        "t1": 1,
+    },
+    {
+        "name": "tb2",
+        "t1": 2,
+    },
+    {
+        "name": "tb3",
+        "t1": 3,
+    }
+]
+
+cursor.execute_many(
+    "create table {name} using stb tags({t1})",
+    create_table_data,
+)
+
+```
+
+The second way is to pass a data_set as a list of tuples, where each tuple represents a different row of the same
+table, and each value within the tuple will become a data row in the SQL statement. All the data together will form a
+complete SQL statement.
+
+```python
+import taos
+
+conn = taos.connect()
+cursor = conn.cursor()
+
+db_name = "test_db"
+
+cursor.execute(f"USE {db_name}")
+
+data_set = [
+    ('2018-10-03 14:38:05.100', 219),
+    ('2018-10-03 14:38:15.300', 218),
+    ('2018-10-03 14:38:16.800', 221),
+]
+
+table_name = "tb1"
+
+cursor.execute_many(f"insert into {table_name} values", data_set)
+
+```
+
+[Example: Insert many lines in one execute](./examples/cursor_execute_many.py)
+
 ### Query with objective API
 
 ```python
 import taos
 
 conn = taos.connect()
 conn.execute("create database if not exists pytest")
@@ -437,15 +519,14 @@
 
 if __name__ == "__main__":
     test_query(connect())
 ```
 
 You can pass an optional req_id in the parameters.
 
-
 ```python
 from taos import *
 from ctypes import *
 import time
 
 
 def fetch_callback(p_param, p_result, num_of_rows):
@@ -744,15 +825,14 @@
     print(row)
 
 conn.execute("drop database if exists %s" % dbname)
 ```
 
 You can pass an optional req_id in the parameters.
 
-
 ```python
 import taos
 from taos import SmlProtocol, SmlPrecision
 
 conn = taos.connect()
 dbname = "pytest_line"
 conn.execute("drop database if exists %s" % dbname)
@@ -1034,13 +1114,14 @@
 
 engine = create_engine("taos://root:taosdata@localhost:6030/log")
 df: pandas.DataFrame = pandas.read_sql("select * from logs", engine)
 ```
 
 ## Limitation
 
-- `taosrest` is designed to use with taosAdapter. If your TDengine version is older than v2.4.0.0, taosAdapter may not be available.
+- `taosrest` is designed to use with taosAdapter. If your TDengine version is older than v2.4.0.0, taosAdapter may not
+  be available.
 
 ## License
 
 We use MIT license for Python connector.
```

