# Comparing `tmp/syngenta_digital_dta-0.1.6.tar.gz` & `tmp/syngenta_digital_dta-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/syngenta_digital_dta-0.1.6.tar", last modified: Mon Mar  6 17:44:03 2023, max compression
+gzip compressed data, was "dist/syngenta_digital_dta-0.1.7.tar", last modified: Fri Mar 17 19:20:48 2023, max compression
```

## Comparing `syngenta_digital_dta-0.1.6.tar` & `syngenta_digital_dta-0.1.7.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.794024 syngenta_digital_dta-0.1.6/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20885 2023-03-06 17:44:03.794024 syngenta_digital_dta-0.1.6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20114 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2023-03-06 17:44:03.794024 syngenta_digital_dta-0.1.6/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1199 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.786024 syngenta_digital_dta-0.1.6/syngenta_digital_dta/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1452 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.786024 syngenta_digital_dta-0.1.6/syngenta_digital_dta/common/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/common/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1974 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/common/base_adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1867 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/common/dict_merger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      290 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/common/json_helper.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      279 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/common/logger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      880 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/common/publisher.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      298 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/common/schema_loader.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1602 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/common/schema_mapper.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.786024 syngenta_digital_dta-0.1.6/syngenta_digital_dta/dynamodb/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/dynamodb/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5733 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/dynamodb/adapter.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.790024 syngenta_digital_dta-0.1.6/syngenta_digital_dta/elasticsearch/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/elasticsearch/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4946 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/elasticsearch/adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      402 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/elasticsearch/es_connection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1834 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/elasticsearch/es_connector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2548 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/elasticsearch/es_mapper.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.790024 syngenta_digital_dta-0.1.6/syngenta_digital_dta/file_system/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/file_system/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3122 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/file_system/adapter.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.790024 syngenta_digital_dta-0.1.6/syngenta_digital_dta/mongo/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/mongo/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5377 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/mongo/adapter.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.790024 syngenta_digital_dta-0.1.6/syngenta_digital_dta/postgres/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/postgres/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11758 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/postgres/adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2585 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/postgres/json_formatting.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      640 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/postgres/sql_connection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1127 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/postgres/sql_connector.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.790024 syngenta_digital_dta-0.1.6/syngenta_digital_dta/s3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/s3/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9881 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta/s3/adapter.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.786024 syngenta_digital_dta-0.1.6/syngenta_digital_dta.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20885 2023-03-06 17:44:03.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2801 2023-03-06 17:44:03.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-06 17:44:03.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       83 2023-03-06 17:44:03.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2023-03-06 17:44:03.000000 syngenta_digital_dta-0.1.6/syngenta_digital_dta.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.790024 syngenta_digital_dta-0.1.6/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.790024 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.790024 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/common/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/common/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5690 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/common/test_base_adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1363 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/common/test_dict_merger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      628 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/common/test_publisher.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2126 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/common/test_schema_mapper.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.794024 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/dynamodb/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/dynamodb/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2598 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/dynamodb/mock_table.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12446 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/dynamodb/test_adapter.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.794024 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/elasticsearch/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/elasticsearch/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4440 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/elasticsearch/mocks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9386 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/elasticsearch/test_adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2056 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/elasticsearch/test_es_connector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2074 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/elasticsearch/test_es_mapper.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.794024 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/file_system/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/file_system/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3405 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/file_system/test_adapter.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.794024 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/mongo/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/mongo/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1441 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/mongo/mock_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6651 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/mongo/test_mongo.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.794024 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/postgres/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/postgres/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6675 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/postgres/test_json_formatting.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11884 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/postgres/test_postgres.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.794024 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/redshift/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/redshift/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10680 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/redshift/test_redshift.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:03.794024 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/s3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/s3/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8891 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/s3/test_s3.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3147 2023-03-06 17:43:51.000000 syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/test__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.875262 syngenta_digital_dta-0.1.7/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20885 2023-03-17 19:20:48.875262 syngenta_digital_dta-0.1.7/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20114 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2023-03-17 19:20:48.879262 syngenta_digital_dta-0.1.7/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1199 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.863262 syngenta_digital_dta-0.1.7/syngenta_digital_dta/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2842 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.863262 syngenta_digital_dta-0.1.7/syngenta_digital_dta/common/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/common/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2616 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/common/base_adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1867 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/common/dict_merger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      290 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/common/json_helper.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      279 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/common/logger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      880 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/common/publisher.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      298 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/common/schema_loader.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1602 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/common/schema_mapper.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.863262 syngenta_digital_dta-0.1.7/syngenta_digital_dta/dynamodb/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/dynamodb/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5733 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/dynamodb/adapter.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.867262 syngenta_digital_dta-0.1.7/syngenta_digital_dta/elasticsearch/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/elasticsearch/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8269 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/elasticsearch/adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      402 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/elasticsearch/es_connection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1834 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/elasticsearch/es_connector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2548 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/elasticsearch/es_mapper.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.867262 syngenta_digital_dta-0.1.7/syngenta_digital_dta/file_system/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/file_system/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3122 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/file_system/adapter.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.867262 syngenta_digital_dta-0.1.7/syngenta_digital_dta/mongo/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/mongo/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5377 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/mongo/adapter.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.867262 syngenta_digital_dta-0.1.7/syngenta_digital_dta/postgres/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/postgres/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11758 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/postgres/adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2585 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/postgres/json_formatting.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      640 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/postgres/sql_connection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1127 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/postgres/sql_connector.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.867262 syngenta_digital_dta-0.1.7/syngenta_digital_dta/s3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/s3/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10287 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta/s3/adapter.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.863262 syngenta_digital_dta-0.1.7/syngenta_digital_dta.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20885 2023-03-17 19:20:48.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2801 2023-03-17 19:20:48.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-17 19:20:48.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       83 2023-03-17 19:20:48.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2023-03-17 19:20:48.000000 syngenta_digital_dta-0.1.7/syngenta_digital_dta.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.867262 syngenta_digital_dta-0.1.7/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.867262 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.871262 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/common/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/common/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5690 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/common/test_base_adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1363 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/common/test_dict_merger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      628 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/common/test_publisher.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2126 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/common/test_schema_mapper.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.871262 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/dynamodb/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/dynamodb/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2598 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/dynamodb/mock_table.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12446 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/dynamodb/test_adapter.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.871262 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/elasticsearch/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/elasticsearch/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4440 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/elasticsearch/mocks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10020 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/elasticsearch/test_adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2056 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/elasticsearch/test_es_connector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2074 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/elasticsearch/test_es_mapper.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.871262 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/file_system/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/file_system/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3405 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/file_system/test_adapter.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.871262 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/mongo/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/mongo/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1441 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/mongo/mock_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6651 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/mongo/test_mongo.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.871262 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/postgres/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/postgres/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6675 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/postgres/test_json_formatting.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11884 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/postgres/test_postgres.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.875262 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/redshift/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/redshift/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10680 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/redshift/test_redshift.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:48.875262 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/s3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/s3/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8891 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/s3/test_s3.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3147 2023-03-17 19:20:33.000000 syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/test__init__.py
```

### Comparing `syngenta_digital_dta-0.1.6/LICENSE` & `syngenta_digital_dta-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/PKG-INFO` & `syngenta_digital_dta-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngenta_digital_dta
-Version: 0.1.6
+Version: 0.1.7
 Summary: A DRY multi-database normalizer.
 Home-page: https://github.com/syngenta-digital/package-python-dta.git
 Author: Paul Cruse III, Engineering Lead, Syngenta Digital
 Author-email: paul.cruse@syngenta.com
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
```

### Comparing `syngenta_digital_dta-0.1.6/README.md` & `syngenta_digital_dta-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/setup.py` & `syngenta_digital_dta-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/syngenta_digital_dta/common/dict_merger.py` & `syngenta_digital_dta-0.1.7/syngenta_digital_dta/common/dict_merger.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/syngenta_digital_dta/common/publisher.py` & `syngenta_digital_dta-0.1.7/syngenta_digital_dta/common/publisher.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/syngenta_digital_dta/common/schema_mapper.py` & `syngenta_digital_dta-0.1.7/syngenta_digital_dta/common/schema_mapper.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/syngenta_digital_dta/dynamodb/adapter.py` & `syngenta_digital_dta-0.1.7/syngenta_digital_dta/dynamodb/adapter.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/syngenta_digital_dta/elasticsearch/adapter.py` & `syngenta_digital_dta-0.1.7/syngenta_digital_dta/mongo/adapter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,136 +1,134 @@
-from syngenta_digital_dta.common import schema_mapper
+from functools import lru_cache
+
+from pymongo import MongoClient, operations
+
 from syngenta_digital_dta.common.base_adapter import BaseAdapter
-from syngenta_digital_dta.elasticsearch.es_connection import es_connection
-from syngenta_digital_dta.elasticsearch import es_mapper
+from syngenta_digital_dta.common import dict_merger
+from syngenta_digital_dta.common import schema_mapper
 
 
-class ElasticsearchAdapter(BaseAdapter):
+class MongoAdapter(BaseAdapter):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.index = kwargs['index']
-        self.endpoint = kwargs['endpoint']
-        self.model_schema_file = kwargs['model_schema_file']
-        self.model_schema = kwargs['model_schema']
-        self.model_identifier = kwargs['model_identifier']
-        self.authentication = kwargs.get('authentication')
-        self.port = kwargs.get('port')
-        self.user = kwargs.get('user')
-        self.password = kwargs.get('password')
-        self.size = kwargs.get('size', 10)
-        self.connection = None
-        self.__connect()
-
-    @es_connection
-    def __connect(self):
-        # just need to call to invoke the decorator
-        pass
-
-    def create_template(self, **kwargs):
-        kwargs['use_patterns'] = True
-        body = self.__create_template_body(**kwargs)
-        self.connection.indices.put_template(
-            name=f'{kwargs["name"]}-template',
-            body=body
-        )
-
-    def create_index(self, **kwargs):
-        if not self.connection.indices.exists(self.index):
-            create_args = {}
-            create_args['index'] = self.index
-            if kwargs.get('template', True):
-                create_args['body'] = self.__create_template_body(**kwargs)
-            self.connection.indices.create(**create_args)
+        self.__collection = self.__connect(**kwargs)
+        self.__model_schema_file = kwargs['model_schema_file']
+        self.__model_schema = kwargs['model_schema']
+        self.__model_identifier = kwargs['model_identifier']
+        self.__allowed_queries = [
+            'find',
+            'find_one',
+            'aggregate',
+            'aggregate_raw_batches',
+            'find_raw_batches',
+            'count_documents',
+            'estimated_document_count',
+            'distinct',
+            'list_indexes'
+        ]
+
+    @lru_cache(maxsize=128)
+    def __connect(self, **kwargs):
+        client = MongoClient(kwargs['endpoint'], username=kwargs['user'], password=kwargs['password'])
+        db = client[kwargs['database']]
+        return db[kwargs['collection']]
 
     def create(self, **kwargs):
-        data = schema_mapper.map_to_schema(kwargs['data'], self.model_schema_file, self.model_schema)
-        response = self.connection.index(
-            index=self.index,
-            id=data[self.model_identifier],
-            body=data,
-            op_type='create',
-            refresh=kwargs.get('refresh', True)
-        )
+        data = schema_mapper.map_to_schema(kwargs['data'], self.__model_schema_file, self.__model_schema)
+        data['_id'] = data[self.__model_identifier]
+        self.__collection.insert_one(data)
         super().publish('create', data, **kwargs)
-        return response
+        return data
+
+    def __map_documents(self, **kwargs):
+        items = []
+        for item in kwargs['data']:
+            item = schema_mapper.map_to_schema(item, self.__model_schema_file, self.__model_schema)
+            item['_id'] = item[self.__model_identifier]
+            items.append(item)
+        return items
+
+    def batch_create(self, **kwargs):
+        items = self.__map_documents(**kwargs)
+        insert_result = self.__collection.insert_many(items, **kwargs.get('params', {}))
+        super().publish('batch_create', items, **kwargs)
+        return insert_result
+
+    def batch_upsert(self, **kwargs):
+        data = kwargs['data']
+        batch_size = kwargs.get('batch_size', 25)
+
+        if not isinstance(data, list):
+            raise Exception('Batched data must be contained within a list')
+
+        batched_data = (data[pos:pos + batch_size] for pos in range(0, len(data), batch_size))
+        results = []
+        for items in batched_data:
+            bulk_operations = [
+                operations.ReplaceOne(filter={'_id': item[self.__model_identifier]}, replacement=item, upsert=True) for item in items
+            ]
+            batch_results = self.__collection.bulk_write(bulk_operations, **kwargs.get('params', {}))
+            results.append(batch_results)
+            super().publish('batch_upsert', items, **kwargs)
+
+        return results
+
+    def read(self, **kwargs):
+        if kwargs.get('operation') == 'query':
+            return self.find(**kwargs)
+        return self.find_one(**kwargs)
+
+    def query(self, **kwargs):
+        if kwargs['operation'] not in self.__allowed_queries:
+            raise Exception(
+                'query method is for read-only operations; please use another function for destructive operations')
+        query = getattr(self.__collection, kwargs['operation'])
+        return query(kwargs['query'])
+
+    def find_one(self, **kwargs):
+        return self.__collection.find_one(kwargs['query'])
+
+    def find(self, **kwargs):
+        results = self.__collection.find(kwargs['query'], **kwargs.get('params', {}))
+        return list(results)
+
+    def count(self, **kwargs):
+        return self.__collection.count_documents(kwargs.get('query', {}), **kwargs.get('params', {}))
 
     def update(self, **kwargs):
-        response = self.connection.update(
-            index=self.index,
-            id=kwargs['data'][self.model_identifier],
-            body={'doc': kwargs['data']},
-            refresh=kwargs.get('refresh', True)
-        )
-        super().publish('update', kwargs['data'], **kwargs)
-        return response
+        original_data = self.find_one(**kwargs)
+        if not original_data:
+            raise Exception(f'no document found by query: {kwargs["query"]}')
+        merged_data = dict_merger.merge(original_data, kwargs['data'], **kwargs)
+        updated_data = schema_mapper.map_to_schema(merged_data, self.__model_schema_file, self.__model_schema)
+        self.__collection.replace_one(kwargs['query'], updated_data, upsert=False)
+        super().publish('update', updated_data, **kwargs)
+        return updated_data
 
     def upsert(self, **kwargs):
-        if self.connection.exists(index=self.index, id=kwargs['data'][self.model_identifier]):
-            return self.update(**kwargs)
-        return self.create(**kwargs)
-
-    def delete(self, identifier_value, **kwargs):
-        response = self.connection.delete(
-            index=self.index,
-            id=identifier_value,
-            refresh=kwargs.get('refresh', True)
-        )
-        super().publish('delete', {self.model_identifier: identifier_value}, **kwargs)
-        return response
-
-    def get(self, identifier_value, **kwargs):
-        try:
-            response = self.connection.get(index=self.index, id=identifier_value)
-            if kwargs.get('normalize'):
-                response = response.get('_source')
-        except:
-            response = {}
-        return response
-
-    def query(self, **kwargs):
-        response = self.connection.search(
-            index=self.index,
-            size=self.size,
-            body={'query': kwargs['query']}
-        )
-        if kwargs.get('normalize'):
-            response = self.__normalize_hits(response)
-        return response
-
-    def __normalize_hits(self, hits):
-        normalized_hits = []
-        for hit in hits.get('hits', {}).get('hits', []):
-            normalized_hits.append(hit['_source'])
-        return normalized_hits
-
-    def __create_template_body(self, **kwargs):
-        body = {
-            'settings': self.__get_settings(**kwargs),
-            'mappings': self.__convert_openapi_mapping(self.model_schema_file, self.model_schema, kwargs.get('special'))
-        }
-        if kwargs.get('use_patterns') and isinstance(kwargs['index_patterns'], list):
-            body['index_patterns'] = kwargs['index_patterns']
-        elif kwargs.get('use_patterns'):
-            body['index_patterns'] = [kwargs['index_patterns']]
-        return body
-
-    def __get_settings(self, **kwargs):
-        if kwargs.get('settings'):
-            return kwargs['settings']
-        settings = {
-            'number_of_replicas': 1,
-            'number_of_shards': 1,
-            'analysis': {
-                'analyzer': {
-                    'url_email_analyzer': {
-                        'type': 'custom',
-                        'tokenizer': 'uax_url_email'
-                    }
-                }
-            }
-        }
-        return settings
-
-    def __convert_openapi_mapping(self, schema_file, schema_key, special=None):
-        mapping = es_mapper.convert_schema_to_mapping(schema_file, schema_key, special)
-        return mapping
+        original_data = self.find_one(**kwargs)
+        if original_data:
+            merged_data = dict_merger.merge(original_data, kwargs['data'], **kwargs)
+        else:
+            merged_data = kwargs['data']
+        data = schema_mapper.map_to_schema(merged_data, self.__model_schema_file, self.__model_schema)
+        data['_id'] = data[self.__model_identifier]
+        self.__collection.replace_one(kwargs['query'], data, upsert=True)
+        super().publish('upsert', data, **kwargs)
+        return data
+
+    def delete(self, **kwargs):
+        data = self.find_one(**kwargs)
+        result = self.__collection.delete_one(kwargs['query'])
+        super().publish('delete', data, **kwargs)
+        return result
+
+    def batch_delete(self, **kwargs):
+        items = self.__map_documents(**kwargs)
+        bulk_operations = []
+        for item in items:
+            bulk_operations.append(operations.DeleteOne(filter={'_id': item['_id']}))
+
+        results = self.__collection.bulk_write(bulk_operations, **kwargs.get('params', {}))
+        super().publish('batch_delete', items, **kwargs)
+        return results
```

### Comparing `syngenta_digital_dta-0.1.6/syngenta_digital_dta/elasticsearch/es_connector.py` & `syngenta_digital_dta-0.1.7/syngenta_digital_dta/elasticsearch/es_connector.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/syngenta_digital_dta/elasticsearch/es_mapper.py` & `syngenta_digital_dta-0.1.7/syngenta_digital_dta/elasticsearch/es_mapper.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/syngenta_digital_dta/file_system/adapter.py` & `syngenta_digital_dta-0.1.7/syngenta_digital_dta/file_system/adapter.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/syngenta_digital_dta/postgres/adapter.py` & `syngenta_digital_dta-0.1.7/syngenta_digital_dta/postgres/adapter.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/syngenta_digital_dta/postgres/json_formatting.py` & `syngenta_digital_dta-0.1.7/syngenta_digital_dta/postgres/json_formatting.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/syngenta_digital_dta/postgres/sql_connection.py` & `syngenta_digital_dta-0.1.7/syngenta_digital_dta/postgres/sql_connection.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/syngenta_digital_dta/postgres/sql_connector.py` & `syngenta_digital_dta-0.1.7/syngenta_digital_dta/postgres/sql_connector.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/syngenta_digital_dta/s3/adapter.py` & `syngenta_digital_dta-0.1.7/syngenta_digital_dta/s3/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,29 @@
                     },
                     Config=conf
                 )
 
         if kwargs.get('publish', True):
             super().publish('create', self.__generate_publish_data(**kwargs), **kwargs)
 
+    def download_stream(self, **kwargs):
+        conf = boto3.s3.transfer.TransferConfig(
+            multipart_threshold=kwargs.get('threshold', 10000),
+            max_concurrency=kwargs.get('concurrency', 4)
+        )
+
+        self.client.download_fileobj(
+            self.bucket,
+            kwargs['s3_path'],
+            kwargs['io'],
+            Config=conf
+        )
+
+        kwargs['io'].seek(0)
+
     def delete(self, **kwargs):
         result = self.client.delete_object(
             Bucket=self.bucket,
             Key=kwargs['s3_path']
         )
         return result
 
@@ -260,15 +275,14 @@
         try:
             for key, value in tags.items():
                 result_tags.append({ 'Key' : key, 'Value': value})
             return result_tags
         except AttributeError as error:
             raise TypeError(' tags parameter is invalid, it should be Dict object') from error
 
-
     def __construct_tags_string(self, **kwargs):
         tags = kwargs.get('tags' , None)
         result_tags = ''
         if not tags:
             return result_tags
         try:
             for key, value in tags.items():
```

### Comparing `syngenta_digital_dta-0.1.6/syngenta_digital_dta.egg-info/PKG-INFO` & `syngenta_digital_dta-0.1.7/syngenta_digital_dta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngenta-digital-dta
-Version: 0.1.6
+Version: 0.1.7
 Summary: A DRY multi-database normalizer.
 Home-page: https://github.com/syngenta-digital/package-python-dta.git
 Author: Paul Cruse III, Engineering Lead, Syngenta Digital
 Author-email: paul.cruse@syngenta.com
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
```

### Comparing `syngenta_digital_dta-0.1.6/syngenta_digital_dta.egg-info/SOURCES.txt` & `syngenta_digital_dta-0.1.7/syngenta_digital_dta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/common/test_base_adapter.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/common/test_base_adapter.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/common/test_dict_merger.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/common/test_dict_merger.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/common/test_publisher.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/common/test_publisher.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/common/test_schema_mapper.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/common/test_schema_mapper.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/dynamodb/mock_table.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/dynamodb/mock_table.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/dynamodb/test_adapter.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/dynamodb/test_adapter.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/elasticsearch/mocks.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/elasticsearch/mocks.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/elasticsearch/test_adapter.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/elasticsearch/test_adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import uuid
 import unittest
 import warnings
 
-import syngenta_digital_dta
+import syngenta_digital_dta, syngenta_digital_dta.elasticsearch.adapter
 
 
 class ElasticsearchAdapterTest(unittest.TestCase):
 
-    def setUp(self, *args, **kwargs):
+    def setUp(self):
         warnings.simplefilter('ignore', ResourceWarning)
         self.maxDiff = None
         self.adapter = syngenta_digital_dta.adapter(
             engine='elasticsearch',
             index='users',
             endpoint='localhost',
             model_schema='test-elasticsearch-user-model',
@@ -288,7 +288,30 @@
             query={
                 'match': {
                     'first': 'Failure'
                 }
             }
         )
         self.assertEqual(len(response), 0)
+
+    def test_query_search_type(self):
+        query = {
+            "bool": {
+                "must": [
+                    {
+                        "range": {
+                            "start_date_time": {
+                                "gte": "2022-01-01T00:00:00"
+                            }
+                        }
+                    }
+                ]
+            }
+        }
+        self.adapter.query(
+            query=query,
+            search_type='query_then_fetch'
+        )
+        self.adapter.query(
+            query=query,
+            search_type='dfs_query_then_fetch'
+        )
```

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/elasticsearch/test_es_connector.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/elasticsearch/test_es_connector.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/elasticsearch/test_es_mapper.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/elasticsearch/test_es_mapper.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/file_system/test_adapter.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/file_system/test_adapter.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/mongo/mock_data.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/mongo/mock_data.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/mongo/test_mongo.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/mongo/test_mongo.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/postgres/test_json_formatting.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/postgres/test_json_formatting.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/postgres/test_postgres.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/postgres/test_postgres.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/redshift/test_redshift.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/redshift/test_redshift.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/s3/test_s3.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/s3/test_s3.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.6/tests/syngenta_digital_dta/test__init__.py` & `syngenta_digital_dta-0.1.7/tests/syngenta_digital_dta/test__init__.py`

 * *Files identical despite different names*

