# Comparing `tmp/datayoga_core-1.87.0.tar.gz` & `tmp/datayoga_core-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datayoga_core-1.87.0.tar", max compression
+gzip compressed data, was "datayoga_core-1.9.0.tar", max compression
```

## Comparing `datayoga_core-1.87.0.tar` & `datayoga_core-1.9.0.tar`

### file list

```diff
@@ -1,94 +1,62 @@
--rw-r--r--   0        0        0     5118 2023-06-14 09:20:08.913631 datayoga_core-1.87.0/README.md
--rw-r--r--   0        0        0     2467 2023-06-14 09:20:24.994410 datayoga_core-1.87.0/pyproject.toml
--rw-r--r--   0        0        0     3558 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/__init__.py
--rw-r--r--   0        0        0     2900 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/block.py
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/add_field/__init__.py
--rw-r--r--   0        0        0     1577 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/add_field/block.py
--rw-r--r--   0        0        0     2062 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/add_field/block.schema.json
--rw-r--r--   0        0        0     1815 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/add_field/tests/test_add_field.py
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/cassandra/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/cassandra/write/__init__.py
--rw-r--r--   0        0        0     4609 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/cassandra/write/block.py
--rw-r--r--   0        0        0     1751 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/cassandra/write/block.schema.json
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/files/read_csv/__init__.py
--rw-r--r--   0        0        0     2023 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/files/read_csv/block.py
--rw-r--r--   0        0        0     1665 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/files/read_csv/block.schema.json
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/filter/__init__.py
--rw-r--r--   0        0        0     1100 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/filter/block.py
--rw-r--r--   0        0        0      464 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/filter/block.schema.json
--rw-r--r--   0        0        0     4200 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/filter/tests/test_filter.py
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/http/receiver/__init__.py
--rw-r--r--   0        0        0     1755 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/http/receiver/block.py
--rw-r--r--   0        0        0      468 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/http/receiver/block.schema.json
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/map/__init__.py
--rw-r--r--   0        0        0     2517 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/map/block.py
--rw-r--r--   0        0        0     1167 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/map/block.schema.json
--rw-r--r--   0        0        0     6070 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/map/tests/test_map.py
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/parquet/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/parquet/read/__init__.py
--rw-r--r--   0        0        0     1115 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/parquet/read/block.py
--rw-r--r--   0        0        0      352 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/parquet/read/block.schema.json
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/parquet/write/__init__.py
--rw-r--r--   0        0        0     1271 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/parquet/write/block.py
--rw-r--r--   0        0        0      352 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/parquet/write/block.schema.json
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/redis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/redis/read_stream/__init__.py
--rw-r--r--   0        0        0     2690 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/redis/read_stream/block.py
--rw-r--r--   0        0        0      586 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/redis/read_stream/block.schema.json
--rw-r--r--   0        0        0      493 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/redis/utils.py
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/redis/write/__init__.py
--rw-r--r--   0        0        0     2197 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/redis/write/block.py
--rw-r--r--   0        0        0      886 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/redis/write/block.schema.json
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/relational/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/relational/read/__init__.py
--rw-r--r--   0        0        0     1616 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/relational/read/block.py
--rw-r--r--   0        0        0     1315 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/relational/read/block.schema.json
--rw-r--r--   0        0        0     1669 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/relational/utils.py
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/relational/write/__init__.py
--rw-r--r--   0        0        0    10167 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/relational/write/block.py
--rw-r--r--   0        0        0     3312 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/relational/write/block.schema.json
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/remove_field/__init__.py
--rw-r--r--   0        0        0     1182 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/remove_field/block.py
--rw-r--r--   0        0        0     1182 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/remove_field/block.schema.json
--rw-r--r--   0        0        0     1893 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/remove_field/tests/test_remove_field.py
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/rename_field/__init__.py
--rw-r--r--   0        0        0     1942 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/rename_field/block.py
--rw-r--r--   0        0        0     1716 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/rename_field/block.schema.json
--rw-r--r--   0        0        0     2279 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/rename_field/tests/test_rename_field.py
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/sequence/__init__.py
--rw-r--r--   0        0        0      436 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/sequence/block.py
--rw-r--r--   0        0        0      517 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/sequence/block.schema.json
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/std/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/std/read/__init__.py
--rw-r--r--   0        0        0     1299 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/std/read/block.py
--rw-r--r--   0        0        0       75 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/std/read/block.schema.json
--rw-r--r--   0        0        0        0 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/std/write/__init__.py
--rw-r--r--   0        0        0      870 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/std/write/block.py
--rw-r--r--   0        0        0       76 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/blocks/std/write/block.schema.json
--rw-r--r--   0        0        0      337 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/context.py
--rw-r--r--   0        0        0     7618 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/expression.py
--rw-r--r--   0        0        0     5677 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/jmespath_custom_functions.py
--rw-r--r--   0        0        0     8435 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/job.py
--rw-r--r--   0        0        0      116 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/opcode.py
--rw-r--r--   0        0        0      709 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/producer.py
--rw-r--r--   0        0        0      522 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/prometheus.py
--rw-r--r--   0        0        0       23 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/resources/scaffold/.gitignore
--rw-r--r--   0        0        0      955 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/resources/scaffold/README.md
--rw-r--r--   0        0        0      151 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/resources/scaffold/connections.yaml
--rw-r--r--   0        0        0      188 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/resources/scaffold/data/sample.csv
--rw-r--r--   0        0        0      444 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/resources/scaffold/jobs/sample/hello.yaml
--rw-r--r--   0        0        0      981 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/resources/schemas/connections/cassandra.schema.json
--rw-r--r--   0        0        0     1169 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/resources/schemas/connections/mysql.schema.json
--rw-r--r--   0        0        0     1489 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/resources/schemas/connections/oracle.schema.json
--rw-r--r--   0        0        0     1270 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/resources/schemas/connections/postgresql.schema.json
--rw-r--r--   0        0        0      641 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/resources/schemas/connections/redis.schema.json
--rw-r--r--   0        0        0     1009 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/resources/schemas/connections/sqlserver.schema.json
--rw-r--r--   0        0        0      981 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/resources/schemas/connections.schema.json
--rw-r--r--   0        0        0     1833 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/resources/schemas/job.schema.json
--rw-r--r--   0        0        0     1048 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/result.py
--rw-r--r--   0        0        0     5505 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/step.py
--rw-r--r--   0        0        0     2112 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/step_buffer.py
--rw-r--r--   0        0        0     4536 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/utils.py
--rw-r--r--   0        0        0     2485 2023-06-14 09:20:08.917631 datayoga_core-1.87.0/src/datayoga_core/write_utils.py
--rw-r--r--   0        0        0     7819 1970-01-01 00:00:00.000000 datayoga_core-1.87.0/PKG-INFO
+-rw-r--r--   0        0        0    10712 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/README.md
+-rw-r--r--   0        0        0     1479 2022-11-23 19:29:20.562231 datayoga_core-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1987 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/__init__.py
+-rw-r--r--   0        0        0     2287 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/block.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/__init__.py
+-rw-r--r--   0        0        0     1413 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/block.py
+-rw-r--r--   0        0        0     2062 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/block.schema.json
+-rw-r--r--   0        0        0     1826 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/tests/test_add_field.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/files/read_csv/__init__.py
+-rw-r--r--   0        0        0     1047 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/files/read_csv/block.py
+-rw-r--r--   0        0        0     1494 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/files/read_csv/block.schema.json
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/filter/__init__.py
+-rw-r--r--   0        0        0      766 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/filter/block.py
+-rw-r--r--   0        0        0      464 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/filter/block.schema.json
+-rw-r--r--   0        0        0     2572 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/filter/tests/test_filter.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/map/__init__.py
+-rw-r--r--   0        0        0     1077 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/map/block.py
+-rw-r--r--   0        0        0      766 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/map/block.schema.json
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/read_stream/__init__.py
+-rw-r--r--   0        0        0     2703 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/read_stream/block.py
+-rw-r--r--   0        0        0      586 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/read_stream/block.schema.json
+-rw-r--r--   0        0        0      493 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/utils.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/write/__init__.py
+-rw-r--r--   0        0        0     1439 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/write/block.py
+-rw-r--r--   0        0        0      605 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/write/block.schema.json
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/relational/write/__init__.py
+-rw-r--r--   0        0        0     1650 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/relational/write/block.py
+-rw-r--r--   0        0        0     2485 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/relational/write/block.schema.json
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/__init__.py
+-rw-r--r--   0        0        0     1180 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/block.py
+-rw-r--r--   0        0        0     1182 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/block.schema.json
+-rw-r--r--   0        0        0     1907 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/tests/test_remove_field.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/__init__.py
+-rw-r--r--   0        0        0     1972 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/block.py
+-rw-r--r--   0        0        0     1716 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/block.schema.json
+-rw-r--r--   0        0        0     2282 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/tests/test_rename_field.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/sequence/__init__.py
+-rw-r--r--   0        0        0      347 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/sequence/block.py
+-rw-r--r--   0        0        0      517 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/sequence/block.schema.json
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/read/__init__.py
+-rw-r--r--   0        0        0     1263 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/read/block.py
+-rw-r--r--   0        0        0       75 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/read/block.schema.json
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/write/__init__.py
+-rw-r--r--   0        0        0      862 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/write/block.py
+-rw-r--r--   0        0        0       76 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/write/block.schema.json
+-rw-r--r--   0        0        0      633 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/context.py
+-rw-r--r--   0        0        0     5473 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/expression.py
+-rw-r--r--   0        0        0     4546 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/jmespath_custom_functions.py
+-rw-r--r--   0        0        0     4408 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/job.py
+-rw-r--r--   0        0        0      712 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/producer.py
+-rw-r--r--   0        0        0       23 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/.gitignore
+-rw-r--r--   0        0        0      955 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/README.md
+-rw-r--r--   0        0        0      154 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/connections.yaml
+-rw-r--r--   0        0        0      188 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/data/sample.csv
+-rw-r--r--   0        0        0      445 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/jobs/sample/hello.yaml
+-rw-r--r--   0        0        0     2226 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/schemas/connections.schema.json
+-rw-r--r--   0        0        0     1757 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/schemas/job.schema.json
+-rw-r--r--   0        0        0     4378 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/step.py
+-rw-r--r--   0        0        0     2317 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/utils.py
+-rw-r--r--   0        0        0    13032 1970-01-01 00:00:00.000000 datayoga_core-1.9.0/setup.py
+-rw-r--r--   0        0        0    12379 1970-01-01 00:00:00.000000 datayoga_core-1.9.0/PKG-INFO
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/block.py` & `datayoga_core-1.9.0/src/datayoga_core/block.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,83 @@
-from __future__ import annotations
-
 import importlib
 import logging
 import os
 import sys
-from abc import ABCMeta, abstractmethod
+from enum import Enum
 from os import path
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Tuple
 
 from datayoga_core import utils
 from datayoga_core.context import Context
-from datayoga_core.result import BlockResult
 from jsonschema import validate
 
 logger = logging.getLogger("dy")
 
 
-class Block(metaclass=ABCMeta):
-    INTERNAL_FIELD_PREFIX = "__$$"
-    MSG_ID_FIELD = f"{INTERNAL_FIELD_PREFIX}msg_id"
-    RESULT_FIELD = f"{INTERNAL_FIELD_PREFIX}result"
-    OPCODE_FIELD = f"{INTERNAL_FIELD_PREFIX}opcode"
+Result = Enum("Result", "SUCCESS REJECTED FILTERED")
+
+
+class Block():
+    MSG_ID_FIELD = "__$$msg_id"
     """
     Block
 
     Attributes:
         properties Dict[str, Any]: Block properties
     """
 
-    def __init__(self, properties: Optional[Dict[str, Any]] = None):
+    def __init__(self, properties: Dict[str, Any] = {}):
         """
         Constructs a block
 
         Args:
-            properties (Optional[Dict[str, Any]]): Block [properties]
+            properties (Dict[str, Any]): Block [properties]
         """
-        self.properties = properties or {}
+        self.properties = properties
         self.validate()
 
     def validate(self):
         """
         Validates block against its JSON Schema
         """
-        logger.debug(f"validating {self.properties}")
-        validate(instance=self.properties, schema=self.get_json_schema())
-
-    def get_json_schema(self) -> Dict[str, Any]:
-        """
-        Returns the JSON Schema for this block
-
-        Returns:
-            Dict[str, Any]: JSON Schema
-        """
         json_schema_file = path.join(
-            utils.get_bundled_dir(),
-            os.path.relpath(
-                os.path.dirname(sys.modules[self.__module__].__file__),
-                start=os.path.dirname(__file__)),
+            utils.get_bundled_dir(), "blocks", self.get_block_name(),
             "block.schema.json") if utils.is_bundled() else path.join(
             os.path.dirname(os.path.realpath(sys.modules[self.__module__].__file__)),
             "block.schema.json")
-        logger.debug(f"loading schema from {json_schema_file}")
-        return utils.read_json(json_schema_file)
 
-    @abstractmethod
+        logger.debug(f"validating {self.properties} against {json_schema_file}")
+        validate(instance=self.properties, schema=utils.read_json(json_schema_file))
+
     def init(self, context: Optional[Context] = None):
         """
-        Initializes block
+        Initializes block (abstract, should be implemented by the sub class)
 
         Args:
             context (Context, optional): Context. Defaults to None.
         """
-        raise NotImplementedError
+        pass
 
-    async def run(self, data: List[Dict[str, Any]]) -> BlockResult:
-        """Transforms data
+    async def run(self, data: List[Dict[str, Any]]) -> Tuple[List[Dict[str, Any]], List[Result]]:
+        """ Transforms data (abstract, should be implemented by the sub class)
 
         Args:
             data (List[Dict[str, Any]]): Data
 
         Returns:
-            BlockResult: Block result
-        """
-        pass
-
-    def stop(self):
-        """
-        Cleans the block connections and state
+            List[Dict[str, Any]]: Transformed data
         """
         pass
 
     def get_block_name(self):
         return os.path.basename(os.path.dirname(sys.modules[self.__module__].__file__))
 
-    @staticmethod
-    def create(block_name: str, properties: Dict[str, Any]) -> Block:
-        module_name = f"datayoga_core.blocks.{block_name}.block"
-        module = importlib.import_module(module_name)
-        block: Block = getattr(module, "Block")(properties)
-        return block
+
+#
+# static utility methods
+#
+
+def create_block(block_name: str, properties: Dict[str, Any]) -> Block:
+    module_name = f"datayoga_core.blocks.{block_name}.block"
+    module = importlib.import_module(module_name)
+    block: Block = getattr(module, "Block")(properties)
+    return block
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/add_field/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/block.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 import logging
-from abc import ABCMeta
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Tuple
 
 from datayoga_core import expression, utils
 from datayoga_core.block import Block as DyBlock
+from datayoga_core.block import Result
 from datayoga_core.context import Context
-from datayoga_core.result import BlockResult
 
 logger = logging.getLogger("dy")
 
 
-class Block(DyBlock, metaclass=ABCMeta):
-
-    def init(self, context: Optional[Context] = None):
+class Block(DyBlock):
+    def init(self, context: Context = None):
         logger.debug(f"Initializing {self.get_block_name()}")
         self.properties = utils.format_block_properties(self.properties)
 
         self.fields = {}
-        for prop in self.properties["fields"]:
-            self.fields[prop["field"]] = expression.compile(
-                prop["language"],
-                prop["expression"])
+        for property in self.properties["fields"]:
+            self.fields[property["field"]] = expression.compile(
+                property["language"],
+                property["expression"])
 
-    async def run(self, data: List[Dict[str, Any]]) -> BlockResult:
+    async def run(self, data: List[Dict[str, Any]]) -> Tuple[List[Dict[str, Any]], List[Result]]:
         logger.debug(f"Running {self.get_block_name()}")
-        for field in self.fields:
-            expression_results = self.fields[field].search_bulk(data)
-            field_path = utils.split_field(field)
-
-            for i, row in enumerate(data):
+        results = []
+        for row in data:
+            for field in self.fields:
                 obj = row
-                # handle nested fields. in that case, the obj points at the nested entity
+                field_path = utils.split_field(field)
+
                 for key in field_path[:-1]:
                     key = utils.unescape_field(key)
                     if key in obj:
                         obj = obj[key]
                     else:
                         obj[key] = {}
-                # assign the new values
-                obj[utils.unescape_field(field_path[-1:][0])] = expression_results[i]
 
-        return utils.all_success(data)
+                obj[utils.unescape_field(field_path[-1:][0])] = self.fields[field].search(row)
+            results.append(Result.SUCCESS)
+        return data, results
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/add_field/block.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/add_field/tests/test_add_field.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/tests/test_add_field.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import pytest
-from datayoga_core import utils
+from datayoga_core.block import Result
 from datayoga_core.blocks.add_field.block import Block
 
 
 @pytest.mark.asyncio
 async def test_add_field():
     block = Block({"field": "full_name",
                    "language": "jmespath",
                    "expression": "[fname,lname] | join(' ', @)"})
     block.init()
-    assert await block.run([{"fname": "john", "lname": "doe"}]) == utils.all_success([
-        {"fname": "john", "lname": "doe", "full_name": "john doe"}]
+    assert await block.run([{"fname": "john", "lname": "doe"}]) == ([
+        {"fname": "john", "lname": "doe", "full_name": "john doe"}], [Result.SUCCESS]
     )
 
 
 @pytest.mark.asyncio
 async def test_add_nested_field():
     block = Block({"field": "name.full_name",
                    "language": "jmespath",
                   "expression": "[name.fname,name.lname] | join(' ', @)"})
     block.init()
-    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == utils.all_success([
-        {"name": {"fname": "john", "lname": "doe", "full_name": "john doe"}}])
+    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == ([
+        {"name": {"fname": "john", "lname": "doe", "full_name": "john doe"}}], [Result.SUCCESS])
 
 
 @pytest.mark.asyncio
 async def test_add_multiple_fields():
     block = Block({"fields": [{"field": "name.full_name", "language": "jmespath", "expression": "concat([name.fname, ' ', name.lname])"}, {
                   "field": "name.fname_upper", "language": "jmespath", "expression": "upper(name.fname)"}]})
     block.init()
-    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == utils.all_success([
-        {"name": {"fname": "john", "lname": "doe", "full_name": "john doe", "fname_upper": "JOHN"}}])
+    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == ([
+        {"name": {"fname": "john", "lname": "doe", "full_name": "john doe", "fname_upper": "JOHN"}}], [Result.SUCCESS])
 
 
 @pytest.mark.asyncio
 async def test_add_field_with_dot():
     block = Block({"field": "name\.full_name",
                    "language": "jmespath",
                    "expression": "[fname,lname] | join(' ', @)"})
     block.init()
-    assert await block.run([{"fname": "john", "lname": "doe"}]) == utils.all_success([
-        {"fname": "john", "lname": "doe", "name.full_name": "john doe"}])
+    assert await block.run([{"fname": "john", "lname": "doe"}]) == ([
+        {"fname": "john", "lname": "doe", "name.full_name": "john doe"}], [Result.SUCCESS])
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/files/read_csv/block.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/resources/schemas/job.schema.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4375%*

 * *Differences: {"'definitions'": "OrderedDict([('block', OrderedDict([('type', 'object'), ('properties', "*

 * *                  "OrderedDict([('uses', OrderedDict([('description', 'Block type'), ('type', "*

 * *                  "'string')])), ('with', OrderedDict([('description', 'Properties'), ('type', "*

 * *                  "['object', 'array'])]))])), ('additionalProperties', False), ('required', "*

 * *                  "['uses']), ('examples', [OrderedDict([('uses', 'files.read_csv'), ('with', "*

 * *                  "OrderedDict([('fi […]*

```diff
@@ -1,73 +1,84 @@
 {
     "additionalProperties": false,
-    "description": "Read data from CSV",
-    "examples": [
-        {
-            "delimiter": ";",
-            "file": "archive.csv"
+    "definitions": {
+        "block": {
+            "additionalProperties": false,
+            "examples": [
+                {
+                    "uses": "files.read_csv",
+                    "with": {
+                        "batch_size": 2500,
+                        "file": "employees.csv"
+                    }
+                },
+                {
+                    "uses": "add_field",
+                    "with": {
+                        "expression": "concat([capitalize(fname), ' ' , capitalize(lname)])",
+                        "field": "full_name",
+                        "language": "jmespath"
+                    }
+                },
+                {
+                    "uses": "map",
+                    "with": {
+                        "expression": {
+                            "country": "country_code || ' - ' || UPPER(country_name)",
+                            "full_name": "full_name",
+                            "gender": "gender",
+                            "id": "id"
+                        }
+                    }
+                },
+                {
+                    "uses": "redis.write",
+                    "with": {
+                        "command": "HSET",
+                        "connection": "cache",
+                        "key_field": "id"
+                    }
+                }
+            ],
+            "properties": {
+                "uses": {
+                    "description": "Block type",
+                    "type": "string"
+                },
+                "with": {
+                    "description": "Properties",
+                    "type": [
+                        "object",
+                        "array"
+                    ]
+                }
+            },
+            "required": [
+                "uses"
+            ],
+            "type": "object"
         }
-    ],
+    },
+    "description": "Job descriptor",
     "properties": {
-        "batch_size": {
-            "default": 1000,
-            "description": "Number of records to read per batch",
-            "minimum": 1,
-            "type": "number"
-        },
-        "delimiter": {
-            "default": ",",
-            "description": "Delimiter to use for splitting the csv records",
-            "maxLength": 1,
-            "minLength": 1,
+        "error_handling": {
+            "default": "ignore",
+            "description": "Error handling strategy: abort - terminate job, ignore - skip",
+            "enum": [
+                "abort",
+                "ignore"
+            ],
             "type": "string"
         },
-        "encoding": {
-            "default": "utf-8",
-            "description": "Encoding to use for reading the file",
-            "type": "string"
+        "input": {
+            "$ref": "#/definitions/block"
         },
-        "fields": {
-            "additionalItems": true,
-            "default": null,
-            "description": "List of columns to use for extract",
-            "examples": [
-                [
-                    "fname",
-                    "lname"
-                ]
-            ],
+        "steps": {
             "items": {
-                "description": "field name",
-                "examples": [
-                    "fname"
-                ],
-                "type": "string"
+                "$ref": "#/definitions/block"
             },
-            "minLength": 1,
-            "title": "List of columns to use",
             "type": "array"
-        },
-        "file": {
-            "description": "Filename. Can contain a regexp or glob expression",
-            "type": "string"
-        },
-        "quotechar": {
-            "default": "\"",
-            "description": "A one-character string used to quote fields containing special characters, such as the delimiter or quotechar, or which contain new-line characters. It defaults to '",
-            "maxLength": 1,
-            "minLength": 1,
-            "type": "string"
-        },
-        "skip": {
-            "default": 0,
-            "description": "Number of lines to skip",
-            "minimum": 0,
-            "type": "number"
         }
     },
-    "required": [
-        "file"
-    ],
-    "title": "files.read_csv",
+    "title": "Job",
     "type": "object"
 }
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/filter/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/map/block.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,30 @@
+import json
 import logging
-from abc import ABCMeta
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Tuple
 
 from datayoga_core import expression
 from datayoga_core.block import Block as DyBlock
+from datayoga_core.block import Result
 from datayoga_core.context import Context
-from datayoga_core.result import BlockResult, Result, Status
 
 logger = logging.getLogger("dy")
 
 
-class Block(DyBlock, metaclass=ABCMeta):
-
-    def init(self, context: Optional[Context] = None):
+class Block(DyBlock):
+    def init(self, context: Context = None):
         logger.debug(f"Initializing {self.get_block_name()}")
-        self.expression = expression.compile(self.properties["language"], self.properties["expression"])
+        self.expression = expression.compile(self.properties["language"], json.dumps(self.properties["expression"]))
 
-    async def run(self, data: List[Dict[str, Any]]) -> BlockResult:
-        result = BlockResult()
+    async def run(self, data: List[Dict[str, Any]]) -> Tuple[List[Dict[str, Any]], List[Result]]:
         logger.debug(f"Running {self.get_block_name()}")
-        return_data = self.expression.filter(data, tombstone=True)
-        # mark filtered rows
-        for i, row in enumerate(return_data):
-            if row is None:
-                result.filtered.append(Result(Status.FILTERED, payload=data[i]))
-            else:
-                result.processed.append(Result(Status.SUCCESS, payload=row))
+        results = []
+        return_data = []
+        for row in data:
+            mapped_row = self.expression.search(row)
+            # we always add the msg_id back
+            if Block.MSG_ID_FIELD in row:
+                mapped_row[Block.MSG_ID_FIELD] = row[Block.MSG_ID_FIELD]
+            return_data.append(mapped_row)
 
-        return result
+        results.append(Result.SUCCESS)
+        return return_data, results
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/parquet/write/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/files/read_csv/block.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 import logging
 import os
-from abc import ABCMeta
-from typing import Any, Dict, List, Optional
+from csv import DictReader
+from typing import Generator, Optional
 
-from datayoga_core import utils
-from datayoga_core.block import Block as DyBlock
 from datayoga_core.context import Context
-from datayoga_core.result import BlockResult
-from datayoga_core.utils import remove_msg_id
-from fastparquet import write
-from pandas import DataFrame
+from datayoga_core.producer import Message
+from datayoga_core.producer import Producer as DyProducer
 
 logger = logging.getLogger("dy")
 
 
-class Block(DyBlock, metaclass=ABCMeta):
+class Block(DyProducer):
 
     def init(self, context: Optional[Context] = None):
         logger.debug(f"Initializing {self.get_block_name()}")
-        parquet_file = self.properties["file"]
+        csv_file = self.properties["file"]
 
-        if os.path.isabs(parquet_file) or context is None:
-            self.file = parquet_file
+        if os.path.isabs(csv_file) or context is None:
+            self.file = csv_file
         else:
-            self.file = os.path.join(context.properties.get("data_path"), parquet_file)
+            self.file = os.path.join(context.properties.get("data_path"), csv_file)
 
         logger.debug(f"file: {self.file}")
+        self.batch_size = self.properties.get("batch_size", 1000)
 
-    async def run(self, data: List[Dict[str, Any]]) -> BlockResult:
-        logger.debug("Writing parquet")
+    def produce(self) -> Generator[Message, None, None]:
+        logger.debug("Reading CSV")
 
-        out = [{"data": remove_msg_id(record)} for record in data]
-        append = os.path.exists(self.file)
-        write(self.file, DataFrame(out), append=append, has_nulls=True)
+        with open(self.file, "r") as read_obj:
+            records = list(DictReader(read_obj))
 
-        # if we made it here, it is a success. return the data and the success result
-        return utils.all_success(data)
+        for i, record in enumerate(records):
+            yield {self.MSG_ID_FIELD: str(i), **record}
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/redis/read_stream/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/redis/read_stream/block.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import json
 import logging
-from typing import AsyncGenerator, List, Optional
+from typing import Generator, List, Optional
 
 import datayoga_core.blocks.redis.utils as redis_utils
-import orjson
 from datayoga_core.context import Context
 from datayoga_core.producer import Message
 from datayoga_core.producer import Producer as DyProducer
 from datayoga_core.utils import get_connection_details
 
 logger = logging.getLogger("dy")
 
@@ -26,29 +26,29 @@
         self.consumer_group = f'datayoga_job_{context.properties.get("job_name", "") if context else ""}'
         self.requesting_consumer = "dy_consumer_a"
         stream_groups = self.redis_client.xinfo_groups(self.stream)
         if next(filter(lambda x: x["name"] == self.consumer_group, stream_groups), None) is None:
             logger.info(f"Creating a new {self.consumer_group} consumer group associated with the {self.stream}")
             self.redis_client.xgroup_create(self.stream, self.consumer_group, 0)
 
-    async def produce(self) -> AsyncGenerator[List[Message], None]:
+    def produce(self) -> Generator[Message, None, None]:
         logger.debug(f"Running {self.get_block_name()}")
 
         read_pending = True
         while True:
             # Read pending messages (fetched by us before but not acknowledged) in the first time, then consume new messages
             streams = self.redis_client.xreadgroup(self.consumer_group, self.requesting_consumer, {
-                self.stream: "0" if read_pending else ">"}, None, 100 if self.snapshot else 0)
+                                                   self.stream: "0" if read_pending else ">"}, None, 100 if self.snapshot else 0)
 
             for stream in streams:
                 logger.debug(f"Messages in {self.stream} stream (pending: {read_pending}):\n\t{stream}")
                 for key, value in stream[1]:
-                    payload = orjson.loads(value[next(iter(value))])
+                    payload = json.loads(value[next(iter(value))])
                     payload[self.MSG_ID_FIELD] = key
-                    yield [payload]
+                    yield payload
 
             # Quit after consuming pending current messages in case of snapshot
             if self.snapshot and not read_pending:
                 break
 
             read_pending = False
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/redis/read_stream/block.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/blocks/redis/read_stream/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/relational/read/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/relational/write/block.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 import logging
-from typing import AsyncGenerator, List, Optional
+from typing import Any, Dict, List, Optional, Tuple
 
 import sqlalchemy as sa
-from datayoga_core import utils
-from datayoga_core.blocks.relational import utils as relational_utils
+from datayoga_core.block import Block as DyBlock
+from datayoga_core.block import Result
 from datayoga_core.context import Context
-from datayoga_core.producer import Message
-from datayoga_core.producer import Producer as DyProducer
+from datayoga_core.utils import get_connection_details
 
 logger = logging.getLogger("dy")
 
 
-class Block(DyProducer):
-
+class Block(DyBlock):
     def init(self, context: Optional[Context] = None):
-        self.engine, self.db_type = relational_utils.get_engine(
-            self.properties.get("connection"),
-            context,
-            autocommit=False
+        logger.debug(f"Initializing {self.get_block_name()}")
+
+        connection = get_connection_details(self.properties.get("connection"), context)
+
+        engine_url = sa.engine.URL.create(
+            drivername=connection.get("type"),
+            host=connection.get("host"),
+            port=connection.get("port"),
+            username=connection.get("user"),
+            password=connection.get("password"),
+            database=connection.get("database")
         )
 
         self.schema = self.properties.get("schema")
         self.table = self.properties.get("table")
-        self.opcode_field = self.properties.get("opcode_field")
-        self.load_strategy = self.properties.get("load_strategy")
-        self.keys = self.properties.get("keys")
-        self.mapping = self.properties.get("mapping")
-
-        self.tbl = sa.Table(self.table, sa.MetaData(schema=self.schema), autoload_with=self.engine)
-
-        logger.debug(f"Connecting to {self.db_type}")
-        self.connection = self.engine.connect()
-
-    async def produce(self) -> AsyncGenerator[List[Message], None]:
-        result = self.connection.execution_options(stream_results=True).execute(self.tbl.select())
-
-        while True:
-            chunk = result.fetchmany(10000)
-            if not chunk:
-                break
-            for row in chunk:
-                yield [utils.add_uid(dict(row._asdict()))]
-
-    def stop(self):
-        self.connection.close()
-        self.engine.dispose()
+        self.engine = sa.create_engine(engine_url, echo=False)
+        logger.debug(f"Connecting to {connection.get('type')}")
+
+        self.conn = self.engine.connect()
+
+    async def run(self, data: List[Dict[str, Any]]) -> Tuple[List[Dict[str, Any]], List[Result]]:
+        logger.debug(f"Running {self.get_block_name()}")
+
+        logger.info(f"Inserting {len(data)} record(s) to {self.table} table")
+        tbl = sa.Table(self.table, sa.MetaData(schema=self.schema), autoload_with=self.engine)
+
+        self.conn.execute(tbl.insert(), data)
+        # if we made it here, it is a success. return the data and the success result
+        return data, [Result.SUCCESS]*len(data)
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/relational/write/block.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/blocks/relational/write/block.schema.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8391504329004329%*

 * *Differences: {"'examples'": "{0: {'properties': {'table_name': 'employees', 'table_schema': 'dbo', "*

 * *               "'target_type': 'database', delete: ['table', 'schema']}}}",*

 * * "'properties'": "{'business_keys': OrderedDict([('type', 'array'), ('title', 'Business keys to "*

 * *                 "use for upsert in case of an UPSERT'), ('items', OrderedDict([('type', "*

 * *                 "'string'), ('description', 'The business key is used for performing an upsert in "*

 * *                 "case the load strategy is UPSERT'), ('ti […]*

```diff
@@ -1,60 +1,51 @@
 {
     "additionalProperties": false,
-    "allOf": [
-        {
-            "not": {
-                "required": [
-                    "opcode_field",
-                    "load_strategy"
-                ]
-            }
-        }
-    ],
     "description": "Write into a SQL-compatible data store",
     "examples": [
         {
             "id": "load_snowflake",
             "properties": {
                 "connection": "eu_datalake",
                 "load_strategy": "APPEND",
-                "schema": "dbo",
-                "table": "employees"
+                "table_name": "employees",
+                "table_schema": "dbo",
+                "target_type": "database"
             },
             "type": "relational.write"
         }
     ],
     "properties": {
         "active_record_indicator": {
             "description": "Used for `TYPE2` load_strategy. An SQL expression used to identify which rows are active",
             "examples": [
                 "is_active='Y'",
                 "deletedAt is null"
             ],
             "type": "string"
         },
+        "business_keys": {
+            "items": {
+                "description": "The business key is used for performing an upsert in case the load strategy is UPSERT",
+                "title": "name of column",
+                "type": "string"
+            },
+            "title": "Business keys to use for upsert in case of an UPSERT",
+            "type": "array"
+        },
         "connection": {
             "description": "Logical connection name as defined in the connections.yaml",
             "examples": [
                 "europe_db",
                 "target",
                 "eu_dwh"
             ],
             "title": "The connection to use for loading",
             "type": "string"
         },
-        "foreach": {
-            "description": "Use a JMESPath expression to split a column into multiple records. The expression should be in the format column: expression.",
-            "examples": [
-                "order_line: lines[]"
-            ],
-            "pattern": "^(?!:).*:.*(?<!:)$",
-            "title": "Split a column into multiple records with a JMESPath expression",
-            "type": "string"
-        },
         "inactive_record_mapping": {
             "default": [],
             "description": "A list of columns to use. Use any valid SQL expression for the source. If 'target' is omitted, will default to the name of the source column",
             "examples": [
                 [
                     {
                         "source": "CURRENT_DATE",
@@ -65,69 +56,25 @@
                         "target": "is_active"
                     }
                 ]
             ],
             "title": "Used for `TYPE2` load_strategy. The columns mapping to use to close out an active record",
             "type": "array"
         },
-        "keys": {
-            "examples": [
-                [
-                    "fname",
-                    {
-                        "lname": "last_name"
-                    }
-                ]
-            ],
-            "items": {
-                "title": "name of column",
-                "type": [
-                    "string",
-                    "object"
-                ]
-            },
-            "title": "Business keys to use in case of `load_strategy` is UPSERT or working with `opcode_field`",
-            "type": "array"
-        },
         "load_strategy": {
             "default": "APPEND",
             "description": "type of target",
             "enum": [
                 "APPEND",
                 "REPLACE",
                 "UPSERT",
                 "TYPE2"
             ],
             "type": "string"
         },
-        "mapping": {
-            "examples": [
-                [
-                    "fname",
-                    {
-                        "lname": "last_name"
-                    },
-                    "address",
-                    "gender"
-                ]
-            ],
-            "items": {
-                "title": "name of column",
-                "type": [
-                    "string",
-                    "object"
-                ]
-            },
-            "title": "Fields to write",
-            "type": "array"
-        },
-        "opcode_field": {
-            "description": "Name of the field in the payload that holds the operation (c - create, d - delete, u - update) for this record in the DB",
-            "type": "string"
-        },
         "schema": {
             "description": "If left blank, the default schema of this connection will be used as defined in the connections.yaml",
             "examples": [
                 "dbo"
             ],
             "title": "The table schema of the target table",
             "type": "string"
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/remove_field/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/block.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import logging
-from abc import ABCMeta
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List
 
 from datayoga_core import utils
 from datayoga_core.block import Block as DyBlock
+from datayoga_core.block import Result
 from datayoga_core.context import Context
-from datayoga_core.result import BlockResult
 
 logger = logging.getLogger("dy")
 
 
-class Block(DyBlock, metaclass=ABCMeta):
-
-    def init(self, context: Optional[Context] = None):
+class Block(DyBlock):
+    def init(self, context: Context = None):
         logger.debug(f"Initializing {self.get_block_name()}")
         self.properties = utils.format_block_properties(self.properties)
 
-    async def run(self, data: List[Dict[str, Any]]) -> BlockResult:
+    async def run(self, data: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
         logger.debug(f"Running {self.get_block_name()}")
+        results = []
+
         for row in data:
-            for prop in self.properties["fields"]:
+            for property in self.properties["fields"]:
                 obj = row
-                from_field_path = utils.split_field(prop["field"])
+                from_field_path = utils.split_field(property["field"])
 
                 for index, key in enumerate(from_field_path):
                     key = utils.unescape_field(key)
                     if key in obj:
                         if len(from_field_path) == index + 1:
                             del obj[key]
                         else:
                             obj = obj[key]
+        results.append(Result.SUCCESS)
 
-        return utils.all_success(data)
+        return data, results
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/remove_field/block.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/remove_field/tests/test_remove_field.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/tests/test_remove_field.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 import pytest
-from datayoga_core import utils
+from datayoga_core.block import Result
 from datayoga_core.blocks.remove_field.block import Block
 
 
 @pytest.mark.asyncio
 async def test_remove_existing_field():
     block = Block({"field": "fname"})
     block.init()
-    assert await block.run([{"fname": "john", "lname": "doe"}]) == utils.all_success([{"lname": "doe"}])
+    assert await block.run([{"fname": "john", "lname": "doe"}]) == ([{"lname": "doe"}], [Result.SUCCESS])
 
 
 @pytest.mark.asyncio
 async def test_remove_missing_field():
     block = Block({"field": "mname"})
     block.init()
-    assert await block.run([{"fname": "john", "lname": "doe"}]) == utils.all_success([{"fname": "john", "lname": "doe"}])
+    assert await block.run([{"fname": "john", "lname": "doe"}]) == ([{"fname": "john", "lname": "doe"}], [Result.SUCCESS])
 
 
 @pytest.mark.asyncio
 async def test_remove_deep_nested_field():
     block = Block({"field": "employee.name.fname"})
     block.init()
-    assert await block.run([{"employee": {"name": {"fname": "john", "lname": "doe"}}}]) == utils.all_success([
-        {"employee": {"name": {"lname": "doe"}}}])
+    assert await block.run([{"employee": {"name": {"fname": "john", "lname": "doe"}}}]) == ([
+        {"employee": {"name": {"lname": "doe"}}}], [Result.SUCCESS])
 
 
 @pytest.mark.asyncio
 async def test_remove_nested_field():
     block = Block({"field": "name.fname"})
     block.init()
-    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == utils.all_success([{"name": {"lname": "doe"}}])
+    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == ([{"name": {"lname": "doe"}}], [Result.SUCCESS])
 
 
 @pytest.mark.asyncio
 async def test_remove_missing_nested_field():
     block = Block({"field": "full_name.fname"})
     block.init()
-    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == utils.all_success([{"name": {"fname": "john", "lname": "doe"}}])
+    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == ([{"name": {"fname": "john", "lname": "doe"}}], [Result.SUCCESS])
 
 
 @pytest.mark.asyncio
 async def test_remove_multiple_fields():
     block = Block({"fields": [{"field": "name.fname"}, {"field": "name.lname"}]})
     block.init()
-    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == utils.all_success([{"name": {}}])
+    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == ([{"name": {}}], [Result.SUCCESS])
 
 
 @pytest.mark.asyncio
 async def test_remove_field_with_dot():
     block = Block({"field": "name\.fname"})
     block.init()
-    assert await block.run([{"name.fname": "john", "lname": "doe"}]) == utils.all_success([{"lname": "doe"}])
+    assert await block.run([{"name.fname": "john", "lname": "doe"}]) == ([{"lname": "doe"}], [Result.SUCCESS])
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/rename_field/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/block.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import logging
-from abc import ABCMeta
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Tuple
 
 from datayoga_core import utils
 from datayoga_core.block import Block as DyBlock
+from datayoga_core.block import Result
 from datayoga_core.context import Context
-from datayoga_core.result import BlockResult
 
 logger = logging.getLogger("dy")
 
 
-class Block(DyBlock, metaclass=ABCMeta):
-
-    def init(self, context: Optional[Context] = None):
+class Block(DyBlock):
+    def init(self, context: Context = None):
         logger.debug(f"Initializing {self.get_block_name()}")
         self.properties = utils.format_block_properties(self.properties)
 
-    async def run(self, data: List[Dict[str, Any]]) -> BlockResult:
+    async def run(self, data: List[Dict[str, Any]]) -> Tuple[List[Dict[str, Any]], List[Result]]:
         logger.debug(f"Running {self.get_block_name()}")
+        results = []
+
         for row in data:
-            for prop in self.properties["fields"]:
+            for property in self.properties["fields"]:
                 key_found = True
                 obj = row
                 value = None
-                from_field_path = utils.split_field(prop["from_field"])
+                from_field_path = utils.split_field(property["from_field"])
 
                 for index, key in enumerate(from_field_path):
                     key = utils.unescape_field(key)
 
                     if key in obj:
                         if len(from_field_path) == index + 1:
                             value = obj[key]
@@ -36,23 +36,24 @@
                             obj = obj[key]
                     else:
                         key_found = False
                         break
 
                 if key_found:
                     obj = row
-                    to_field_path = utils.split_field(prop["to_field"])
+                    to_field_path = utils.split_field(property["to_field"])
 
                     for key in to_field_path[:-1]:
                         key = utils.unescape_field(key)
 
                         if key in obj:
                             obj = obj[key]
                         else:
                             obj[key] = {}
 
                     if key in obj:
                         obj = obj[key]
 
                     obj[utils.unescape_field(to_field_path[-1:][0])] = value
 
-        return utils.all_success(data)
+        results.append(Result.SUCCESS)
+        return data, results
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/rename_field/block.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/rename_field/tests/test_rename_field.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/tests/test_rename_field.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,78 @@
 import pytest
-from datayoga_core import utils
+from datayoga_core.block import Result
 from datayoga_core.blocks.rename_field.block import Block
 
 
 @pytest.mark.asyncio
 async def test_rename_existing_field():
     block = Block(
         {
             "from_field": "fname",
             "to_field": "first_name"
         }
     )
     block.init()
-    assert await block.run([{"fname": "john", "lname": "doe"}]) == utils.all_success([{"first_name": "john", "lname": "doe"}])
+    assert await block.run([{"fname": "john", "lname": "doe"}]) == ([{"first_name": "john", "lname": "doe"}], [Result.SUCCESS])
 
 
 @pytest.mark.asyncio
 async def test_rename_missing_field():
     block = Block(
         {
             "from_field": "mname",
             "to_field": "middle_name"
         }
     )
     block.init()
-    assert await block.run([{"fname": "john", "lname": "doe"}]) == utils.all_success([
-        {"fname": "john", "lname": "doe"}])
+    assert await block.run([{"fname": "john", "lname": "doe"}]) == ([{"fname": "john", "lname": "doe"}], [Result.SUCCESS])
 
 
 @pytest.mark.asyncio
 async def test_rename_deep_nested_field():
     block = Block(
         {
             "from_field": "employee.name.fname",
             "to_field": "employee.name.first_name"
         }
     )
     block.init()
-    assert await block.run([{"employee": {"name": {"fname": "john", "lname": "doe"}}}]) == utils.all_success([
-
-        {"employee": {"name": {"first_name": "john", "lname": "doe"}}}])
+    assert await block.run([{"employee": {"name": {"fname": "john", "lname": "doe"}}}]) == ([
+        {"employee": {"name": {"first_name": "john", "lname": "doe"}}}], [Result.SUCCESS])
 
 
 @pytest.mark.asyncio
 async def test_rename_nested_field():
     block = Block(
         {
             "from_field": "name.fname",
             "to_field": "name.first_name"
         }
     )
     block.init()
-    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == utils.all_success([
-        {"name": {"first_name": "john", "lname": "doe"}}])
+    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == ([
+        {"name": {"first_name": "john", "lname": "doe"}}], [Result.SUCCESS])
 
 
 @pytest.mark.asyncio
 async def test_rename_nested_field_missing_to_field_parent():
     block = Block(
         {
             "from_field": "name.fname",
             "to_field": "new_name.first_name"
         }
     )
     block.init()
-    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == utils.all_success([
-        {"name": {"lname": "doe"}, "new_name": {"first_name": "john"}}])
+    assert await block.run([{"name": {"fname": "john", "lname": "doe"}}]) == ([
+        {"name": {"lname": "doe"}, "new_name": {"first_name": "john"}}], [Result.SUCCESS])
 
 
 @pytest.mark.asyncio
 async def test_rename_field_with_dot():
     block = Block(
         {
             "from_field": "name\.fname",
             "to_field": "name\.first_name"
         }
     )
     block.init()
-    assert await block.run([{"name.fname": "john", "lname": "doe"}]) == utils.all_success([{"name.first_name": "john", "lname": "doe"}])
+    assert await block.run([{"name.fname": "john", "lname": "doe"}]) == ([{"name.first_name": "john", "lname": "doe"}], [Result.SUCCESS])
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/sequence/block.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/blocks/sequence/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.87.0/src/datayoga_core/blocks/std/read/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/std/read/block.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,41 @@
+import json
 import logging
 import select
 import sys
 import uuid
-from typing import Any, AsyncGenerator, Dict, List, Optional
+from typing import Any, Dict, Generator, List, Optional
 
-import orjson
 from datayoga_core.context import Context
 from datayoga_core.producer import Message
 from datayoga_core.producer import Producer as DyProducer
 
 logger = logging.getLogger("dy")
 
 
 class Block(DyProducer):
 
     def init(self, context: Optional[Context] = None):
         logger.debug(f"Initializing {self.get_block_name()}")
 
-    async def produce(self) -> AsyncGenerator[List[Message], None]:
+    def produce(self) -> Generator[Message, None, None]:
         if select.select([sys.stdin, ], [], [], 0.0)[0]:
             # piped data exists
             for data in sys.stdin:
                 for record in self.get_records(data):
-                    yield [self.get_message(record)]
+                    yield self.get_message(record)
         else:
             # interactive mode
             print("Enter data to process:")
             data = input()
             for record in self.get_records(data):
-                yield [self.get_message(record)]
+                yield self.get_message(record)
 
-    @staticmethod
-    def get_records(data: str) -> List[Dict[str, Any]]:
-        records = orjson.loads(data)
+    def get_records(self, data: str) -> List[Dict[str, Any]]:
+        records = json.loads(data)
 
         if isinstance(records, dict):
             records = [records]
 
         return records
 
     def get_message(self, record: Dict[str, Any]) -> Message:
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/jmespath_custom_functions.py` & `datayoga_core-1.9.0/src/datayoga_core/jmespath_custom_functions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-import base64
 import hashlib
-import re
 import string
 from datetime import datetime, timezone
-from typing import Any, Iterable, Union
+from typing import Union
 from uuid import uuid4
 
-import orjson
+import json
 from jmespath import functions
 
 
-# custom functions for JMESPath
+# custom functions for Jmespath
 class JmespathCustomFunctions(functions.Functions):
 
     @functions.signature({"types": ["string", "null"]})
     def _func_capitalize(self, arg):
         return string.capwords(str(arg)) if arg is not None else None
 
     @functions.signature({"types": ["array"]})
@@ -27,20 +25,15 @@
 
     @functions.signature({"types": ["string", "null"]})
     def _func_upper(self, element):
         return str(element).upper() if element is not None else None
 
     @functions.signature({"types": ["string", "null"]}, {"types": ["string"]}, {"types": ["string"]})
     def _func_replace(self, element, old_value, new_value):
-        if element is None:
-            return None
-
-        # Unexpected behavior when `old_value` is an empty string in Python's builtin replace
-        # https://bugs.python.org/issue28029
-        return str(element).replace(old_value, new_value) if old_value != "" else str(element)
+        return str(element).replace(old_value, new_value) if element is not None else None
 
     @functions.signature({"types": ["string", "null"]}, {"types": ["number"]})
     def _func_right(self, element, amount):
         return str(element)[-amount:] if element is not None else None
 
     @functions.signature({"types": ["string", "null"]}, {"types": ["number"]})
     def _func_left(self, element, amount):
@@ -58,15 +51,16 @@
     def _func_uuid(self):
         """Generates a random UUID4 and returns it as a string in standard format."""
 
         return str(uuid4())
 
     @functions.signature({"types": ["number", "string", "boolean", "array", "object", "null"], "variadic": True})
     def _func_hash(self, obj, hash_name="sha1"):
-        """Calculates a hash using given the `hash_name` hash function and returns its hexadecimal representation.
+        """\
+        Calculates a hash using given the `hash_name` hash function and returns its hexadecimal representation.
 
         Supported algorithms:
 
         - sha1(default)
         - sha256
         - md5
         - sha384
@@ -88,59 +82,42 @@
 
             if obj is None:
                 return b""
 
             if isinstance(obj, str):
                 return obj.encode()
 
-            return orjson.dumps(obj, option=orjson.OPT_SORT_KEYS)
+            # the 'separators' arg is needed to remove whitespace in the resulting string
+            return json.dumps(obj, separators=(',', ':')).encode("utf-8")
 
         h = hashlib.new(hash_name)
         h.update(prepare())
         return h.hexdigest()
 
     @functions.signature({"types": ["string", "number"]})
     def _func_time_delta_days(self, dt):
-        """Returns the number of days between given `dt` and now (positive)
+        """\
+        Returns the number of days between given `dt` and now (positive)
         or the number of days that have passed from now (negative).
 
         If `dt` is a string, ISO datetime (2011-11-04T00:05:23+04:00, for example) is assumed.
         If `dt` is a number, Unix timestamp (1320365123, for example) is assumed.
         """
 
         dt = datetime.fromisoformat(dt) if isinstance(dt, str) else datetime.fromtimestamp(dt, timezone.utc)
         delta = dt.now(dt.tzinfo) - dt
         return delta.days
 
     @functions.signature({"types": ["string", "number"]})
     def _func_time_delta_seconds(self, dt):
-        """Returns the number of seconds between given `dt` and now (positive)
+        """\
+        Returns the number of seconds between given `dt` and now (positive)
         or the number of seconds that have passed from now (negative).
 
         If `dt` is a string, ISO datetime (2011-11-04T00:05:23+04:00, for example) is assumed.
         If `dt` is a number, Unix timestamp (1320365123, for example) is assumed.
         """
 
         dt = datetime.fromisoformat(dt) if isinstance(dt, str) else datetime.fromtimestamp(dt, timezone.utc)
         delta = dt.now(dt.tzinfo) - dt
 
         return delta.days * 86400 + delta.seconds
-
-    @functions.signature({"types": ["string"]}, {"types": ["string"]}, {"types": ["string"]})
-    def _func_regex_replace(self, text: str, pattern: str, replacement: str) -> str:
-        """Replaces matched patterns in the string by the given replacement."""
-        return re.sub(pattern, replacement, text)
-
-    @functions.signature({"types": ["number", "string", "boolean", "array", "object", "null"]}, {"types": ["array"]})
-    def _func_in(self, element: Any, iterable: Iterable) -> bool:
-        """Returns True if the iterable contains the given element."""
-        return element in iterable
-
-    @functions.signature({"types": ["string"]})
-    def _func_json_parse(self, data: str) -> Any:
-        """Returns parsed object from the given json string."""
-        return orjson.loads(data)
-
-    @functions.signature({"types": ["string"]})
-    def _func_base64_decode(self, data: str) -> str:
-        """Returns decoded string from the given base64 encoded string."""
-        return base64.b64decode(data).decode()
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/producer.py` & `datayoga_core-1.9.0/src/datayoga_core/producer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-from abc import abstractmethod
-from typing import Any, AsyncGenerator, Dict, Generator, List
+import logging
+from typing import Any, Dict, Generator, List, TypedDict
 
 from .block import Block
 
-
-class Message:
-    def __init__(self, msg_id: str, value: Dict[str, Any]):
-        self.msg_id = msg_id
-        self.value = value
+logger = logging.getLogger("dy")
+Message = TypedDict("Message", msg_id=str, value=Dict[str, Any])
 
 
 class Producer(Block):
 
-    @abstractmethod
-    def produce(self) -> AsyncGenerator[List[Message], None]:
-        """Produces data
+    def produce(self) -> Generator[Message, None, None]:
+        """ Produces data (abstract, should be implemented by the sub class)
 
         Returns:
             Generator[Message]: Produced data
         """
-        raise NotImplementedError
+        pass
 
     def ack(self, msg_ids: List[str]):
-        """Sends acknowledge for the message IDs of the records that have been processed
+        """ Sends acknowledge for the message IDs of the records that have been processed (abstract, should be implemented by the sub class)
 
         Args:
             msg_ids (List[str]): Message IDs
         """
         pass
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/resources/scaffold/README.md` & `datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/README.md`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.87.0/src/datayoga_core/resources/schemas/connections/mysql.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/resources/schemas/connections.schema.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('title', 'Connections'), ('description', 'Connection catalog'), "*

 * *            "('type', ['object', 'null']), ('patternProperties', OrderedDict([('.', "*

 * *            "OrderedDict([('type', 'object'), ('anyOf', [OrderedDict([('description', 'SQL "*

 * *            "database'), ('properties', OrderedDict([('type', OrderedDict([('description', 'DB "*

 * *            "type'), ('type', 'string'), ('pattern', '^(?!redis$)')])), ('host', "*

 * *            "OrderedDict([('description', 'DB host'), ('type […]*

```diff
@@ -1,59 +1,107 @@
 {
-    "examples": [
-        {
-            "hr": {
-                "connect_args": {
-                    "ssl_ca": "/opt/ssl/ca.crt",
-                    "ssl_cert": "/opt/ssl/client.crt",
-                    "ssl_key": "/opt/ssl/client.key"
+    "additionalProperties": false,
+    "description": "Connection catalog",
+    "patternProperties": {
+        ".": {
+            "anyOf": [
+                {
+                    "additionalProperties": false,
+                    "description": "SQL database",
+                    "examples": [
+                        {
+                            "database": "postgres",
+                            "host": "localhost",
+                            "name": "hr",
+                            "password": "postgres",
+                            "port": 5432,
+                            "type": "postgresql",
+                            "user": "postgres"
+                        }
+                    ],
+                    "properties": {
+                        "database": {
+                            "description": "DB name",
+                            "type": "string"
+                        },
+                        "host": {
+                            "description": "DB host",
+                            "type": "string"
+                        },
+                        "password": {
+                            "description": "DB password",
+                            "type": "string"
+                        },
+                        "port": {
+                            "description": "DB port",
+                            "maximum": 65535,
+                            "minimum": 1,
+                            "type": "integer"
+                        },
+                        "type": {
+                            "description": "DB type",
+                            "pattern": "^(?!redis$)",
+                            "type": "string"
+                        },
+                        "user": {
+                            "description": "DB user",
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "type",
+                        "host",
+                        "database",
+                        "user"
+                    ]
                 },
-                "database": "hr",
-                "host": "localhost",
-                "password": "mypass",
-                "port": 3306,
-                "type": "mysql",
-                "user": "myuser"
-            }
-        }
-    ],
-    "properties": {
-        "connect_args": {
-            "additionalProperties": true,
-            "description": "Additional arguments to use when connecting to the DB",
-            "type": "object"
-        },
-        "database": {
-            "description": "DB name",
-            "type": "string"
-        },
-        "host": {
-            "description": "DB host",
-            "type": "string"
-        },
-        "password": {
-            "description": "DB password",
-            "type": "string"
-        },
-        "port": {
-            "description": "DB port",
-            "maximum": 65535,
-            "minimum": 1,
-            "type": "integer"
-        },
-        "query_args": {
-            "additionalProperties": true,
-            "description": "Additional query string arguments to use when connecting to the DB",
+                {
+                    "additionalProperties": false,
+                    "description": "Redis",
+                    "examples": [
+                        {
+                            "cache": {
+                                "host": "localhost",
+                                "port": 6379,
+                                "type": "redis"
+                            }
+                        }
+                    ],
+                    "properties": {
+                        "host": {
+                            "description": "Redis DB host",
+                            "type": "string"
+                        },
+                        "password": {
+                            "description": "Redis DB password",
+                            "type": "string"
+                        },
+                        "port": {
+                            "description": "Redis DB port",
+                            "maximum": 65535,
+                            "minimum": 1,
+                            "type": "integer"
+                        },
+                        "type": {
+                            "description": "DB type",
+                            "enum": [
+                                "redis"
+                            ],
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "type",
+                        "host",
+                        "port"
+                    ]
+                }
+            ],
             "type": "object"
-        },
-        "user": {
-            "description": "DB user",
-            "type": "string"
         }
     },
-    "required": [
-        "type",
-        "host",
-        "database",
-        "user"
+    "title": "Connections",
+    "type": [
+        "object",
+        "null"
     ]
 }
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/resources/schemas/connections/redis.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/blocks/map/block.schema.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.42857142857142855%*

 * *Differences: {"'description'": "'Maps a record into a new output based on expressions'",*

 * * "'examples'": "[OrderedDict([('expression', OrderedDict([('first_name', 'first_name'), "*

 * *               '(\'last_name\', \'last_name\'), (\'greeting\', "\'Hello \' || CASE WHEN gender = '*

 * *               "'F' THEN 'Ms.' WHEN gender = 'M' THEN 'Mr.' ELSE 'N/A' END || ' ' || "*

 * *               'full_name"), (\'country\', \'country\'), (\'full_name\', \'full_name\')])), '*

 * *               "('language', 'sql')])]",*

 * * "'properties'": "{replac […]*

```diff
@@ -1,41 +1,36 @@
 {
     "additionalProperties": false,
-    "description": "Redis",
+    "description": "Maps a record into a new output based on expressions",
     "examples": [
         {
-            "cache": {
-                "host": "localhost",
-                "port": 6379,
-                "type": "redis"
-            }
+            "expression": {
+                "country": "country",
+                "first_name": "first_name",
+                "full_name": "full_name",
+                "greeting": "'Hello ' || CASE WHEN gender = 'F' THEN 'Ms.' WHEN gender = 'M' THEN 'Mr.' ELSE 'N/A' END || ' ' || full_name",
+                "last_name": "last_name"
+            },
+            "language": "sql"
         }
     ],
     "properties": {
-        "host": {
-            "description": "Redis DB host",
-            "type": "string"
-        },
-        "password": {
-            "description": "Redis DB password",
-            "type": "string"
+        "expression": {
+            "description": "Expression",
+            "type": "object"
         },
-        "port": {
-            "description": "Redis DB port",
-            "maximum": 65535,
-            "minimum": 1,
-            "type": "integer"
-        },
-        "type": {
-            "description": "DB type",
+        "language": {
+            "description": "Language",
             "enum": [
-                "redis"
+                "jmespath",
+                "sql"
             ],
             "type": "string"
         }
     },
     "required": [
-        "type",
-        "host",
-        "port"
-    ]
+        "expression",
+        "language"
+    ],
+    "title": "map",
+    "type": "object"
 }
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/step.py` & `datayoga_core-1.9.0/src/datayoga_core/step.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,131 +1,110 @@
 from __future__ import annotations
 
 import asyncio
 import logging
-from asyncio import Task
 from typing import Any, Callable, Dict, List, Optional
 
-from datayoga_core import prometheus
-from datayoga_core.block import Block
+from datayoga_core.block import Block, Result
 from datayoga_core.context import Context
-from datayoga_core.result import Result, Status
 
 logger = logging.getLogger("dy")
 
 
-class Step:
-    def __init__(self, step_id: str, block: Optional[Block], concurrency=1):
-        self.id = step_id
+class Step():
+    def __init__(self, id: str, block: Block, concurrency=1):
+        self.id = id
         self.block = block
         self.next_step = None
         self.active_entries = set()
         self.concurrency = concurrency
-        self.workers: List[Optional[Task]] = [None]*self.concurrency
+        self.workers = [None]*self.concurrency
         self.done_callback = None
         self.initialized = False
 
     def init(self, context: Optional[Context] = None):
         # initialize the block
         self.block.init(context)
+        # start pool of workers for parallelization
 
     async def start_pool(self):
-        # start pool of workers for parallelization
         logger.debug("starting pool")
         self.queue = asyncio.Queue(maxsize=1)
-        for worker_id in range(self.concurrency):
-            worker = self.workers[worker_id]
+        for id in range(self.concurrency):
+            worker = self.workers[id]
             if worker is None or not worker.done():
-                self.workers[worker_id] = asyncio.create_task(self.run(worker_id))
+                self.workers[id] = asyncio.create_task(self.run(id))
             else:
-                logger.debug(f"worker {worker_id} is running: {not worker.done()}")
+                logger.debug(f"worker {id} is running: {not worker.done()}")
 
-    def add_done_callback(self, callback: Callable[[List[str], List[Result]], None]):
+    def add_done_callback(self, callback: Callable[[str], None]):
         self.done_callback = callback
 
     def __or__(self, other: Step):
         return self.append(other)
 
     def append(self, next_step: Step):
         self.next_step = next_step
         self.next_step.add_done_callback(self.done)
         return self.next_step
 
     async def process(self, messages: List[Dict[str, Any]]):
         if not self.initialized:
             await self.start_pool()
             self.initialized = True
+
         self.active_entries.update([x[Block.MSG_ID_FIELD] for x in messages])
         await self.queue.put(messages)
 
     async def run(self, worker_id: int):
         while True:
             entry = await self.queue.get()
             logger.debug(f"{self.id}-{worker_id} processing {[i[Block.MSG_ID_FIELD] for i in entry]}")
             try:
-                processed_entries, filtered_entries, rejected_entries = await self.block.run(entry)
-
-                prometheus.processed_entries.labels(step=self.id).inc(len(processed_entries))
-                prometheus.filtered_records.labels(step=self.id).inc(len(filtered_entries))
-                prometheus.rejected_records.labels(step=self.id).inc(len(rejected_entries))
-
-                # handle filtered. anything not processed or rejected
-                logger.debug(
-                    f"filtered entries: {filtered_entries}, processed entries: {processed_entries}, rejected entries: {rejected_entries}")
-                if filtered_entries:
-                    # ack the filtered entries
-                    self.done([row.payload[Block.MSG_ID_FIELD] for row in filtered_entries],
-                              [Result(Status.FILTERED)] * len(filtered_entries))
-
-                # handle rejected
-                if rejected_entries:
-                    # ack the rejected entries
-                    self.done([row.payload[Block.MSG_ID_FIELD] for row in rejected_entries], rejected_entries)
-
-                if processed_entries:
-                    # check if we have a next step
-                    if self.next_step:
-                        # process downstream
-                        await self.next_step.process([result.payload for result in processed_entries])
-                    else:
-                        # we are a last channel, propagate the ack upstream
-                        # TODO: verify that all entries have a msg id otherwise raise consistency error
-                        self.done([row.payload[Block.MSG_ID_FIELD] for row in processed_entries], processed_entries)
+                processed_entries, results = await self.block.run(entry)
 
+                # TODO: handle filtered. anything not processed or rejected
+                # check if we have a next step
+                if self.next_step:
+                    # process downstream
+                    await self.next_step.process(processed_entries)
+                else:
+                    # we are a last channel, propagate the ack upstream
+                    # TODO: verify that all entries have a msg id otherwise raise consistency error
+                    self.done([x[Block.MSG_ID_FIELD] for x in processed_entries], Result.SUCCESS)
+
+                    # indicate rejected records if any
+                    if Result.REJECTED in results:
+                        self.done([entry[i][Block.MSG_ID_FIELD]
+                                  for i, v in enumerate(results) if v == Result.REJECTED], Result.REJECTED)
             except Exception as e:
                 # we caught an exception. the entire batch is considered rejected
                 logger.exception(e)
                 # verify that all messages still have a msg_id property
                 # if next(filter(lambda x: not Block.MSG_ID_FIELD in x,entry),None) is not None
-                self.done([x[Block.MSG_ID_FIELD] for x in entry], [
-                          Result(Status.REJECTED, f"Error in step {self.id}: {repr(e)}")] * len(entry))
+                self.done([x[Block.MSG_ID_FIELD] for x in entry],
+                          Result.REJECTED, f"Error in step {self.id}: {repr(e)}")
             finally:
                 self.queue.task_done()
-            logger.debug(f"{self.id}-{worker_id} done processing {entry}")
+            logger.debug(f"{self.id}-{worker_id} done processing {entry[0][Block.MSG_ID_FIELD]}")
 
-    def done(self, msg_ids: List[str], results: List[Result]):
-        logger.debug(f"{self.id} acking {msg_ids}")
+    def done(self, msg_ids: List[str], result: Optional[Result] = None, reason: Optional[str] = None):
+        logger.debug(f"{self.id} acking {msg_ids} with result {result}")
         self.active_entries.difference_update(msg_ids)
         if self.done_callback is not None:
-            self.done_callback(msg_ids, results)
+            self.done_callback(msg_ids, result, reason)
 
     async def join(self):
         # wait for all active entries to be processed
         while len(self.active_entries) > 0:
-            logger.debug(f"{self.id} waiting for dangling messages: {self.active_entries}")
             await asyncio.sleep(0.2)
 
     async def stop(self):
         # wait for all tasks to finish
         await self.join()
-        logger.debug("joined")
-
-        # stop the block
-        if self.block:
-            self.block.stop()
 
         # stop any downstream workers
         if self.next_step:
             await self.next_step.stop()
 
         # stop all workers in the pool
         for worker in self.workers:
```

### Comparing `datayoga_core-1.87.0/src/datayoga_core/utils.py` & `datayoga_core-1.9.0/src/datayoga_core/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,30 @@
-import copy
+import json
 import os
 import re
 import sys
-import uuid
 from os import path
 from typing import Any, Dict, List
 
-import orjson
 import yaml
-from datayoga_core import result
-from datayoga_core.block import Block
 from datayoga_core.context import Context
-from datayoga_core.expression import JMESPathExpression
-from datayoga_core.result import BlockResult, Result, Status
 
 
 def read_json(filename: str) -> Any:
     """
     Loads a filename as a JSON object
 
     Args:
         filename (str): JSON filename to load
 
     Returns:
         Any: JSON object
     """
-    with open(filename, "r", encoding="utf8") as json_file:
-        return orjson.loads(json_file.read())
+    with open(filename, "r", encoding="utf8") as f:
+        return json.load(f)
 
 
 def read_yaml(filename: str) -> Dict[str, Any]:
     """
     Loads a filename as a YAML object
 
     Args:
@@ -39,16 +33,16 @@
     Raises:
         ValueError: In case of invalid YAML
 
     Returns:
          Dict[str, Any]: YAML python object
     """
     try:
-        with open(filename, "r", encoding="utf8") as yaml_file:
-            return yaml.safe_load(yaml_file)
+        with open(filename, "r", encoding="utf8") as stream:
+            return yaml.safe_load(stream)
     except Exception as e:
         raise ValueError(f"Malformed YAML: {e}")
 
 
 def format_block_properties(properties: Dict[str, Any]) -> Dict[str, Any]:
     """Adds `fields` array with the passed properties in case it's missing
 
@@ -62,15 +56,15 @@
 
 
 def is_bundled() -> bool:
     return getattr(sys, "frozen", False) and hasattr(sys, "_MEIPASS")
 
 
 def get_bundled_dir() -> str:
-    datayoga_dir = path.join(sys._MEIPASS, "datayoga_core")
+    datayoga_dir = path.join(sys._MEIPASS, "datayoga")
     return datayoga_dir if os.path.isdir(datayoga_dir) else sys._MEIPASS
 
 
 def get_resource_path(relative_path: str) -> str:
     if is_bundled():
         # we are running in a bundle
         return path.join(get_bundled_dir(), "resources", relative_path)
@@ -84,62 +78,13 @@
 
 
 def unescape_field(field: str) -> str:
     return field.replace("\\.", ".")
 
 
 def get_connection_details(connection_name: str, context: Context) -> Dict[str, Any]:
-    if context and context.properties:
-        connection = context.properties.get("connections", {}).get(connection_name)
+    if context:
+        connection = context.properties.get("connections").get(connection_name)
         if connection:
             return connection
 
     raise ValueError(f"{connection_name} connection not found")
-
-
-def all_success(records: List[Dict[str, Any]]) -> BlockResult:
-    return BlockResult(processed=[Result(Status.SUCCESS, payload=row) for row in records])
-
-
-def is_rejected(record: Dict[str, Any]) -> bool:
-    return record.get(Block.RESULT_FIELD, result.SUCCESS).status == Status.REJECTED
-
-
-def add_uid(record: Dict[str, Any]) -> Dict[str, Any]:
-    return {Block.MSG_ID_FIELD: f"{uuid.uuid4()}", **record}
-
-
-def remove_msg_id(record: dict) -> dict:
-    return {k: v for k, v in record.items() if k != Block.MSG_ID_FIELD}
-
-
-def explode_records(records: List[Dict[str, Any]], field_expression: str) -> List[Dict[str, Any]]:
-    """
-    Takes a list of records and a JMESPath expression specifying a field to be exploded, and returns a new list of records
-    where each record has been "exploded" into multiple records based on the values in the specified field.
-
-    Args:
-        records (List[Dict[str, Any]]): A list of dictionaries representing records.
-        field_expression (str): A string specifying the field to be exploded, in the form "field_name: expression".
-
-    Returns:
-        List[Dict[str, Any]]: A new list of dictionaries representing the exploded records.
-    """
-    field_name, expression = map(str.strip, field_expression.split(":", maxsplit=1))
-
-    jmespath_expr = JMESPathExpression()
-    jmespath_expr.compile(expression)
-
-    exploded_records = []
-
-    for record in records:
-        # Apply the JMESPath expression to the current record to obtain the values to be exploded.
-        field_values = jmespath_expr.search(record)
-
-        # If the JMESPath expression returned any values, create a new record for each value and add it to the output list.
-        if field_values:
-            for field_value in field_values:
-                new_record = copy.deepcopy(record)
-                new_record[field_name] = field_value
-                exploded_records.append(new_record)
-
-    return exploded_records
```

