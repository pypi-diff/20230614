# Comparing `tmp/databricks-feature-store-0.9.1a1.tar.gz` & `tmp/databricks-feature-store-0.9.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks-feature-store-0.9.1a1.tar", last modified: Fri Jan 20 23:51:54 2023, max compression
+gzip compressed data, was "databricks-feature-store-0.9.1a2.tar", last modified: Sat Jan 28 00:42:56 2023, max compression
```

## Comparing `databricks-feature-store-0.9.1a1.tar` & `databricks-feature-store-0.9.1a2.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-20 23:51:54.508381 databricks-feature-store-0.9.1a1/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2414 2022-10-06 23:48:00.000000 databricks-feature-store-0.9.1a1/LICENSE.md
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      495 2022-10-17 19:57:31.000000 databricks-feature-store-0.9.1a1/NOTICE.md
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3754 2023-01-20 23:51:54.508184 databricks-feature-store-0.9.1a1/PKG-INFO
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3433 2023-01-20 23:51:54.000000 databricks-feature-store-0.9.1a1/README.md
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-20 23:51:54.475053 databricks-feature-store-0.9.1a1/databricks/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      166 2022-07-20 05:31:47.000000 databricks-feature-store-0.9.1a1/databricks/__init__.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-20 23:51:54.475273 databricks-feature-store-0.9.1a1/databricks/_feature_store_pkg_metadata/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      166 2022-10-06 23:48:00.000000 databricks-feature-store-0.9.1a1/databricks/_feature_store_pkg_metadata/__init__.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-20 23:51:54.475533 databricks-feature-store-0.9.1a1/databricks/_feature_store_pkg_metadata/_core_client_pkg_metadata/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-10-06 23:48:00.000000 databricks-feature-store-0.9.1a1/databricks/_feature_store_pkg_metadata/_core_client_pkg_metadata/__init__.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-20 23:51:54.480746 databricks-feature-store-0.9.1a1/databricks/feature_store/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2409 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     5295 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/_catalog_client_helper.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-20 23:51:54.481387 databricks-feature-store-0.9.1a1/databricks/feature_store/_compute_client/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-10-06 23:48:00.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/_compute_client/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    50536 2023-01-18 22:59:35.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/_compute_client/_compute_client.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-20 23:51:54.481966 databricks-feature-store-0.9.1a1/databricks/feature_store/_publish_client/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-10-06 23:48:00.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/_publish_client/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    17391 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/_publish_client/_publish_client.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2161 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/_spark_client_helper.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-20 23:51:54.482416 databricks-feature-store-0.9.1a1/databricks/feature_store/_training_scoring_client/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-10-06 23:48:00.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/_training_scoring_client/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    29256 2023-01-20 22:49:39.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/_training_scoring_client/_training_scoring_client.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-20 23:51:54.482671 databricks-feature-store-0.9.1a1/databricks/feature_store/api/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-07-20 05:31:47.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/api/__init__.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-20 23:51:54.483118 databricks-feature-store-0.9.1a1/databricks/feature_store/api/proto/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-07-20 05:31:47.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/api/proto/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    76687 2023-01-20 23:51:27.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/api/proto/feature_catalog_pb2.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    18677 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/catalog_client.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    42539 2023-01-18 23:00:01.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/client.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      880 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/constants.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1414 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/databricks_client.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     6321 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/decorators.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-20 23:51:54.492730 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1297 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/_feature_store_object.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      902 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/_permission_level.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1489 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/_proto_enum_entity.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      444 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/cloud.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      257 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/column_info.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1092 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/consumer.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3270 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/data_type.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1222 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/feature.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2525 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/feature_column_info.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     6428 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/feature_lookup.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1221 2023-01-18 22:59:35.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/feature_serving_endpoint.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    13718 2023-01-13 00:17:50.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/feature_spec.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      378 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/feature_spec_constants.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     4366 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/feature_table.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1098 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/feature_table_info.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3635 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/feature_tables_for_serving.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1000 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/job.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1333 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/key_spec.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1182 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/notebook.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     6817 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/online_feature_table.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3424 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/online_store_detailed.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     5484 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/online_store_for_serving.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     6853 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/online_store_metadata.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      489 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/query_mode.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      715 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/source_data_column_info.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      607 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/store_type.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      506 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/entities/tag.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     9313 2023-01-20 22:49:39.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/feature_serving_endpoint_client.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      361 2022-07-20 05:31:47.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/feature_table_properties.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-20 23:51:54.493318 databricks-feature-store-0.9.1a1/databricks/feature_store/local_models/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        1 2023-01-18 22:59:35.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/local_models/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      506 2023-01-18 22:59:35.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/local_models/databricks_identity_model.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1638 2023-01-20 22:49:39.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/mlflow_model_constants.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     5240 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_publish_client.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      830 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_publish_client_factory.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     5279 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_publish_nosql_client.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    11991 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_publish_rdbms_client.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-20 23:51:54.495500 databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_spec/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      829 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_spec/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    10903 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_spec/amazon_dynamodb_online_store_spec.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     4125 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_spec/amazon_rds_mysql_online_store_spec.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     5354 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_spec/azure_cosmosdb_online_store_spec.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     4498 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_spec/azure_mysql_online_store_spec.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     4550 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_spec/azure_sql_server_online_store_spec.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1314 2022-10-06 23:48:00.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_spec/online_store_properties.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    20162 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_spec/online_store_spec.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-20 23:51:54.496187 databricks-feature-store-0.9.1a1/databricks/feature_store/protos/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-07-20 05:31:47.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/protos/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     4459 2023-01-20 23:51:27.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/protos/feature_spec_pb2.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    18242 2023-01-20 23:51:27.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/protos/feature_store_serving_pb2.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-20 23:51:54.497938 databricks-feature-store-0.9.1a1/databricks/feature_store/publish_engine/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      675 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/publish_engine/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    10407 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/publish_engine/publish_cosmosdb_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    10645 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/publish_engine/publish_dynamodb_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     5930 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/publish_engine/publish_mysql_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     4678 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/publish_engine/publish_sql_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     8406 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/publish_engine/publish_sql_server_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    10629 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/sagemaker.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    19778 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/spark_client.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2276 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/training_set.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-20 23:51:54.506415 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3877 2023-01-13 00:17:50.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/converter_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     7961 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/cosmosdb_type_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     4374 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/cosmosdb_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     7335 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/dynamodb_type_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     4955 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/dynamodb_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    11467 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/e2e_test_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    13758 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/feature_lookup_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1397 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/feature_spec_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1236 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/file_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      850 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/headers.yaml
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1204 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/logging_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1881 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/publish_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    10946 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/request_context.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     8891 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/rest_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     4687 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/schema_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     6415 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/spark_listener.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      192 2022-07-20 05:31:47.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/spark_test_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      923 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/spark_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     6876 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/test_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      318 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/test_utils_common.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     8595 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/uc_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     7953 2023-01-20 22:49:39.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      485 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/utils_common.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      864 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/utils/validation_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)       20 2023-01-20 22:49:15.000000 databricks-feature-store-0.9.1a1/databricks/feature_store/version.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-20 23:51:54.507845 databricks-feature-store-0.9.1a1/databricks_feature_store.egg-info/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3754 2023-01-20 23:51:54.000000 databricks-feature-store-0.9.1a1/databricks_feature_store.egg-info/PKG-INFO
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     5758 2023-01-20 23:51:54.000000 databricks-feature-store-0.9.1a1/databricks_feature_store.egg-info/SOURCES.txt
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        1 2023-01-20 23:51:54.000000 databricks-feature-store-0.9.1a1/databricks_feature_store.egg-info/dependency_links.txt
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      169 2023-01-20 23:51:54.000000 databricks-feature-store-0.9.1a1/databricks_feature_store.egg-info/requires.txt
--rw-r--r--   0 mingyang.ge   (502) staff       (20)       11 2023-01-20 23:51:54.000000 databricks-feature-store-0.9.1a1/databricks_feature_store.egg-info/top_level.txt
--rw-r--r--   0 mingyang.ge   (502) staff       (20)       38 2023-01-20 23:51:54.508556 databricks-feature-store-0.9.1a1/setup.cfg
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2236 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a1/setup.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-28 00:42:56.618357 databricks-feature-store-0.9.1a2/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2414 2022-10-06 23:48:00.000000 databricks-feature-store-0.9.1a2/LICENSE.md
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      495 2022-10-17 19:57:31.000000 databricks-feature-store-0.9.1a2/NOTICE.md
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3754 2023-01-28 00:42:56.618117 databricks-feature-store-0.9.1a2/PKG-INFO
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3433 2023-01-28 00:42:56.000000 databricks-feature-store-0.9.1a2/README.md
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-28 00:42:56.572221 databricks-feature-store-0.9.1a2/databricks/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      166 2022-07-20 05:31:47.000000 databricks-feature-store-0.9.1a2/databricks/__init__.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-28 00:42:56.572480 databricks-feature-store-0.9.1a2/databricks/_feature_store_pkg_metadata/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      166 2022-10-06 23:48:00.000000 databricks-feature-store-0.9.1a2/databricks/_feature_store_pkg_metadata/__init__.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-28 00:42:56.572754 databricks-feature-store-0.9.1a2/databricks/_feature_store_pkg_metadata/_core_client_pkg_metadata/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-10-06 23:48:00.000000 databricks-feature-store-0.9.1a2/databricks/_feature_store_pkg_metadata/_core_client_pkg_metadata/__init__.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-28 00:42:56.579554 databricks-feature-store-0.9.1a2/databricks/feature_store/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2409 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     5295 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/_catalog_client_helper.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-28 00:42:56.580241 databricks-feature-store-0.9.1a2/databricks/feature_store/_compute_client/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-10-06 23:48:00.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/_compute_client/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    50536 2023-01-18 22:59:35.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/_compute_client/_compute_client.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-28 00:42:56.580809 databricks-feature-store-0.9.1a2/databricks/feature_store/_publish_client/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-10-06 23:48:00.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/_publish_client/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    17391 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/_publish_client/_publish_client.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2161 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/_spark_client_helper.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-28 00:42:56.581342 databricks-feature-store-0.9.1a2/databricks/feature_store/_training_scoring_client/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-10-06 23:48:00.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/_training_scoring_client/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    29256 2023-01-27 23:46:29.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/_training_scoring_client/_training_scoring_client.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-28 00:42:56.581917 databricks-feature-store-0.9.1a2/databricks/feature_store/api/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-07-20 05:31:47.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/api/__init__.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-28 00:42:56.582529 databricks-feature-store-0.9.1a2/databricks/feature_store/api/proto/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-07-20 05:31:47.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/api/proto/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    76687 2023-01-20 23:51:27.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/api/proto/feature_catalog_pb2.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    18677 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/catalog_client.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    42539 2023-01-18 23:00:01.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/client.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      880 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/constants.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1414 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/databricks_client.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     6321 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/decorators.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-28 00:42:56.594497 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1297 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/_feature_store_object.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      902 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/_permission_level.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1489 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/_proto_enum_entity.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      444 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/cloud.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      257 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/column_info.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1092 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/consumer.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3270 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/data_type.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1222 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/feature.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2525 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/feature_column_info.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     6428 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/feature_lookup.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1221 2023-01-18 22:59:35.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/feature_serving_endpoint.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    13718 2023-01-13 00:17:50.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/feature_spec.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      378 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/feature_spec_constants.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     4366 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/feature_table.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1098 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/feature_table_info.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3635 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/feature_tables_for_serving.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1000 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/job.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1333 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/key_spec.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1182 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/notebook.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     6817 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/online_feature_table.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3424 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/online_store_detailed.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     5484 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/online_store_for_serving.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     6853 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/online_store_metadata.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      489 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/query_mode.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      715 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/source_data_column_info.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      607 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/store_type.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      506 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/entities/tag.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     9536 2023-01-28 00:42:20.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/feature_serving_endpoint_client.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      361 2022-07-20 05:31:47.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/feature_table_properties.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-28 00:42:56.595262 databricks-feature-store-0.9.1a2/databricks/feature_store/local_models/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        1 2023-01-18 22:59:35.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/local_models/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      506 2023-01-18 22:59:35.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/local_models/databricks_identity_model.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1638 2023-01-27 23:46:29.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/mlflow_model_constants.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     5240 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_publish_client.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      830 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_publish_client_factory.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     5279 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_publish_nosql_client.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    11991 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_publish_rdbms_client.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-28 00:42:56.597631 databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_spec/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      829 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_spec/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    10903 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_spec/amazon_dynamodb_online_store_spec.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     4125 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_spec/amazon_rds_mysql_online_store_spec.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     5354 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_spec/azure_cosmosdb_online_store_spec.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     4498 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_spec/azure_mysql_online_store_spec.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     4550 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_spec/azure_sql_server_online_store_spec.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1314 2022-10-06 23:48:00.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_spec/online_store_properties.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    20162 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_spec/online_store_spec.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-28 00:42:56.598497 databricks-feature-store-0.9.1a2/databricks/feature_store/protos/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-07-20 05:31:47.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/protos/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     4459 2023-01-20 23:51:27.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/protos/feature_spec_pb2.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    18242 2023-01-20 23:51:27.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/protos/feature_store_serving_pb2.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-28 00:42:56.600979 databricks-feature-store-0.9.1a2/databricks/feature_store/publish_engine/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      675 2022-10-19 00:33:31.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/publish_engine/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    10407 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/publish_engine/publish_cosmosdb_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    10645 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/publish_engine/publish_dynamodb_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     5930 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/publish_engine/publish_mysql_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     4678 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/publish_engine/publish_sql_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     8406 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/publish_engine/publish_sql_server_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    10629 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/sagemaker.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    19778 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/spark_client.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2276 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/training_set.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-28 00:42:56.616093 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3877 2023-01-13 00:17:50.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/converter_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     7961 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/cosmosdb_type_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     4374 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/cosmosdb_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     7335 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/dynamodb_type_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     4955 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/dynamodb_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    11467 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/e2e_test_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    13758 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/feature_lookup_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1397 2023-01-13 00:15:59.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/feature_spec_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1236 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/file_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      850 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/headers.yaml
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1204 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/logging_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1881 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/publish_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    10946 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/request_context.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     8891 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/rest_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     4687 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/schema_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     6415 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/spark_listener.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      192 2022-07-20 05:31:47.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/spark_test_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      923 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/spark_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     6876 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/test_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      318 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/test_utils_common.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     8595 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/uc_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     7953 2023-01-27 23:46:29.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      485 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/utils_common.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      864 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/utils/validation_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)       20 2023-01-28 00:42:20.000000 databricks-feature-store-0.9.1a2/databricks/feature_store/version.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-01-28 00:42:56.617756 databricks-feature-store-0.9.1a2/databricks_feature_store.egg-info/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3754 2023-01-28 00:42:56.000000 databricks-feature-store-0.9.1a2/databricks_feature_store.egg-info/PKG-INFO
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     5758 2023-01-28 00:42:56.000000 databricks-feature-store-0.9.1a2/databricks_feature_store.egg-info/SOURCES.txt
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        1 2023-01-28 00:42:56.000000 databricks-feature-store-0.9.1a2/databricks_feature_store.egg-info/dependency_links.txt
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      169 2023-01-28 00:42:56.000000 databricks-feature-store-0.9.1a2/databricks_feature_store.egg-info/requires.txt
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)       11 2023-01-28 00:42:56.000000 databricks-feature-store-0.9.1a2/databricks_feature_store.egg-info/top_level.txt
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)       38 2023-01-28 00:42:56.618531 databricks-feature-store-0.9.1a2/setup.cfg
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2236 2023-01-03 23:39:08.000000 databricks-feature-store-0.9.1a2/setup.py
```

### Comparing `databricks-feature-store-0.9.1a1/LICENSE.md` & `databricks-feature-store-0.9.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/PKG-INFO` & `databricks-feature-store-0.9.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-feature-store
-Version: 0.9.1a1
+Version: 0.9.1a2
 Summary: Databricks Feature Store Client
 Author: Databricks
 Author-email: feedback@databricks.com
 License: Databricks Proprietary License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `databricks-feature-store-0.9.1a1/README.md` & `databricks-feature-store-0.9.1a2/README.md`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/__init__.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/_catalog_client_helper.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/_catalog_client_helper.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/_compute_client/_compute_client.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/_compute_client/_compute_client.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/_publish_client/_publish_client.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/_publish_client/_publish_client.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/_spark_client_helper.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/_spark_client_helper.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/_training_scoring_client/_training_scoring_client.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/_training_scoring_client/_training_scoring_client.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/api/proto/feature_catalog_pb2.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/api/proto/feature_catalog_pb2.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/catalog_client.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/catalog_client.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/client.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/client.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/constants.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/constants.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/databricks_client.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/databricks_client.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/decorators.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/decorators.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/_feature_store_object.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/_feature_store_object.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/_permission_level.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/_permission_level.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/_proto_enum_entity.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/_proto_enum_entity.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/consumer.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/consumer.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/data_type.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/data_type.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/feature.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/feature.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/feature_column_info.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/feature_column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/feature_lookup.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/feature_lookup.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/feature_serving_endpoint.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/feature_serving_endpoint.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/feature_spec.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/feature_spec.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/feature_table.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/feature_table.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/feature_table_info.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/feature_table_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/feature_tables_for_serving.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/feature_tables_for_serving.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/job.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/job.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/key_spec.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/key_spec.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/notebook.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/notebook.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/online_feature_table.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/online_feature_table.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/online_store_detailed.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/online_store_detailed.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/online_store_for_serving.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/online_store_for_serving.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/online_store_metadata.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/online_store_metadata.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/source_data_column_info.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/source_data_column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/entities/store_type.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/entities/store_type.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/feature_serving_endpoint_client.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/feature_serving_endpoint_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 from pyspark.sql.types import StructType
 
 import databricks.feature_store.local_models as local_models
 from databricks.feature_store.entities.feature_lookup import FeatureLookup
 from databricks.feature_store.entities.feature_serving_endpoint import (
     FeatureServingEndpoint,
 )
-from databricks.feature_store.utils.rest_utils import http_request
+from databricks.feature_store.utils.rest_utils import http_request, verify_rest_response
 
 ENABLE_FEATURE_SERVING_ENDPOINT_CLIENT = True
-BASE_API_PATH = "/api/2.0/preview/inference-endpoints"
+BASE_API_PATH = "/api/2.0/serving-endpoints"
 MODEL_NAME_PREFIX = "feature-serving-model-"
 SERVED_MODEL_NAME_PREFIX = "feature-serving-served-model-"
 FEATURE_SERVING_DEFAULT_WORKLOAD_SIZE = "Large"
 FEATURE_SERVING_DEFAULT_SCALE_TO_ZERO = True
 
 # Must be one or more characters including alphanumeric and dash. The first and
 # last characters can only be alphanumeric.
@@ -112,15 +112,19 @@
         result = self._call_api(f"/{endpoint_name}", "DELETE", {})
         self._mlflow_client.delete_registered_model(
             name=self._get_model_name(endpoint_name)
         )
 
     def _list_endpoints(self):
         listresult = self._call_api(path="", method="GET", json_body=None)
-        return listresult["endpoints"]
+        if "endpoints" in listresult:
+            return listresult["endpoints"]
+        else:
+            # when the result is empty the key "endpoints" is missing.
+            return []
 
     def _create_model(self, model_name, feature_lookups) -> ModelVersion:
         # To prevent the FS client being added to the model dependency, import IdentityModel
         # with manipulation to sys.path so that the class is imported as
         # <databricks_identity_model.IdentityModel>. This is necessary for SRTI to import the
         # file directly from Python path while loading the model.
         model_file = os.path.dirname(local_models.__file__)
@@ -221,14 +225,15 @@
         else:
             response = http_request(
                 host_creds=host_creds,
                 endpoint=api,
                 method=method,
                 json=json_body,
             )
+        verify_rest_response(response=response, endpoint=api)
         return json.loads(response.text)
 
     def _convert_to_feature_serving_endpoint(
         self, json_result
     ) -> FeatureServingEndpoint:
         json_state = json_result["state"]["config_update"]
         return FeatureServingEndpoint(
```

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/mlflow_model_constants.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/mlflow_model_constants.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_publish_client.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_publish_client.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_publish_client_factory.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_publish_client_factory.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_publish_nosql_client.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_publish_nosql_client.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_publish_rdbms_client.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_publish_rdbms_client.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_spec/__init__.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_spec/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_spec/amazon_dynamodb_online_store_spec.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_spec/amazon_dynamodb_online_store_spec.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_spec/amazon_rds_mysql_online_store_spec.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_spec/amazon_rds_mysql_online_store_spec.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_spec/azure_cosmosdb_online_store_spec.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_spec/azure_cosmosdb_online_store_spec.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_spec/azure_mysql_online_store_spec.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_spec/azure_mysql_online_store_spec.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_spec/azure_sql_server_online_store_spec.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_spec/azure_sql_server_online_store_spec.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_spec/online_store_properties.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_spec/online_store_properties.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/online_store_spec/online_store_spec.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/online_store_spec/online_store_spec.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/protos/feature_spec_pb2.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/protos/feature_spec_pb2.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/protos/feature_store_serving_pb2.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/protos/feature_store_serving_pb2.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/publish_engine/__init__.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/publish_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/publish_engine/publish_cosmosdb_engine.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/publish_engine/publish_cosmosdb_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/publish_engine/publish_dynamodb_engine.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/publish_engine/publish_dynamodb_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/publish_engine/publish_mysql_engine.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/publish_engine/publish_mysql_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/publish_engine/publish_sql_engine.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/publish_engine/publish_sql_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/publish_engine/publish_sql_server_engine.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/publish_engine/publish_sql_server_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/sagemaker.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/sagemaker.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/spark_client.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/spark_client.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/training_set.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/training_set.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/converter_utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/converter_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/cosmosdb_type_utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/cosmosdb_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/cosmosdb_utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/cosmosdb_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/dynamodb_type_utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/dynamodb_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/dynamodb_utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/dynamodb_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/e2e_test_utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/e2e_test_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/feature_lookup_utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/feature_lookup_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/feature_spec_utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/feature_spec_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/file_utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/headers.yaml` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/headers.yaml`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/logging_utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/publish_utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/publish_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/request_context.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/request_context.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/rest_utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/rest_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/schema_utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/spark_listener.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/spark_listener.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/spark_utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/spark_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/test_utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/uc_utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/uc_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks/feature_store/utils/validation_utils.py` & `databricks-feature-store-0.9.1a2/databricks/feature_store/utils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/databricks_feature_store.egg-info/PKG-INFO` & `databricks-feature-store-0.9.1a2/databricks_feature_store.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-feature-store
-Version: 0.9.1a1
+Version: 0.9.1a2
 Summary: Databricks Feature Store Client
 Author: Databricks
 Author-email: feedback@databricks.com
 License: Databricks Proprietary License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `databricks-feature-store-0.9.1a1/databricks_feature_store.egg-info/SOURCES.txt` & `databricks-feature-store-0.9.1a2/databricks_feature_store.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `databricks-feature-store-0.9.1a1/setup.py` & `databricks-feature-store-0.9.1a2/setup.py`

 * *Files identical despite different names*

