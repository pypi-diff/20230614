# Comparing `tmp/amundsen-databuilder-7.4.3.tar.gz` & `tmp/amundsen-databuilder-7.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amundsen-databuilder-7.4.3.tar", last modified: Fri Dec 16 05:07:09 2022, max compression
+gzip compressed data, was "dist/amundsen-databuilder-7.4.4.tar", last modified: Wed Jun 14 21:43:33 2023, max compression
```

## Comparing `amundsen-databuilder-7.4.3.tar` & `amundsen-databuilder-7.4.4.tar`

### file list

```diff
@@ -1,302 +1,302 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      869 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)   116500 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/amundsen_databuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/amundsen_databuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12729 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/amundsen_databuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/amundsen_databuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/amundsen_databuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/amundsen_databuilder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/callback/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/callback/call_back.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/clients/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/clients/neptune_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/extractor/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/athena_metadata_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17997 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/atlas_search_data_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/base_bigquery_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/base_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/base_postgres_metadata_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/base_teradata_metadata_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/bigquery_metadata_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/bigquery_usage_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/bigquery_watermark_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/cassandra_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12275 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/csv_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/apache_superset/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/apache_superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/apache_superset/apache_superset_chart_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/apache_superset/apache_superset_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/apache_superset/apache_superset_metadata_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/apache_superset/apache_superset_table_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/databricks_sql/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/databricks_sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/databricks_sql/databricks_sql_dashboard_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/databricks_sql/databricks_sql_dashboard_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_charts_batch_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_executions_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_last_modified_timestamp_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_last_successful_executions_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_owner_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_queries_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_usage_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_user_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/redash/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/redash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10333 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/redash/redash_dashboard_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/redash/redash_dashboard_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/tableau/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/tableau/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/tableau/tableau_dashboard_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/tableau/tableau_dashboard_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/tableau/tableau_dashboard_last_modified_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/tableau/tableau_dashboard_query_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/tableau/tableau_dashboard_table_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/tableau/tableau_dashboard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/tableau/tableau_external_table_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/db2_metadata_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/db_api_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14619 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dbt_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    23680 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/delta_lake_metadata_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/dremio_metadata_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/druid_metadata_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/es_base_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/es_column_stats_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/es_last_updated_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/es_metadata_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/es_watermark_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/eventbridge_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/feast_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/generic_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/generic_usage_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/glue_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15571 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/hive_table_last_updated_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/hive_table_metadata_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/kafka_schema_registry_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/kafka_source_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/mssql_metadata_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/mysql_metadata_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    19817 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/mysql_search_data_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/neo4j_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/neo4j_search_data_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11545 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/neptune_search_data_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/openlineage_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/oracle_metadata_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/pandas_profiling_column_stats_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/postgres_metadata_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/presto_view_metadata_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/redshift_metadata_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/extractor/restapi/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/restapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/restapi/rest_api_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/salesforce_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/snowflake_metadata_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/snowflake_table_last_updated_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/sql_alchemy_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/table_metadata_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/teradata_metadata_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/extractor/user/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/extractor/user/bamboohr/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/user/bamboohr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/user/bamboohr/bamboohr_user_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/extractor/vertica_metadata_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/filesystem/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/filesystem/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/filesystem/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/job/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/job/base_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/job/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/loader/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/loader/base_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/loader/file_system_atlas_csv_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/loader/file_system_csv_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/loader/file_system_elasticsearch_json_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/loader/file_system_mysql_csv_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/loader/file_system_neo4j_csv_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/loader/file_system_neptune_csv_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/loader/generic_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/models/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/atlas_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/atlas_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/atlas_serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7467 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/badge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/models/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/cluster/cluster_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/models/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/dashboard/dashboard_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/dashboard/dashboard_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/dashboard/dashboard_last_modified.py
--rw-r--r--   0 runner    (1001) docker     (123)    19183 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/dashboard/dashboard_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/dashboard/dashboard_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/dashboard/dashboard_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/dashboard/dashboard_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/dashboard/dashboard_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/dashboard_elasticsearch_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/description_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/elasticsearch_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/es_last_updated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/models/feature/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/feature/feature_elasticsearch_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/feature/feature_generation_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/feature/feature_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/feature/feature_watermark.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/graph_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/graph_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/graph_serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/owner.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/owner_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/models/query/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/query/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/query/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/query/query_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/query/query_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/query/query_where.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/models/schema/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/schema/schema_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/table_column_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/table_elasticsearch_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/table_last_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/table_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    31710 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/table_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/table_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/table_serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/table_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     8614 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/table_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/models/timestamp/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/timestamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/timestamp/timestamp_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    20307 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/type_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/models/usage/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/usage/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/usage/usage_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/user_elasticsearch_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/models/watermark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/publisher/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/publisher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16980 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/publisher/atlas_csv_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/publisher/base_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/publisher/elasticsearch_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/publisher/elasticsearch_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/publisher/mysql_csv_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)    22007 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/publisher/neo4j_csv_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)    18764 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/publisher/neo4j_csv_unwind_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/publisher/neo4j_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/publisher/neptune_csv_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/publisher/publisher_config_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/rest_api/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/rest_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/rest_api/base_rest_api_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/rest_api/mode_analytics/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/rest_api/mode_analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/rest_api/mode_analytics/mode_paginated_rest_api_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/rest_api/query_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/rest_api/rest_api_failure_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11926 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/rest_api/rest_api_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/serializers/atlas_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/serializers/mysql_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/serializers/neo4_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/serializers/neptune_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/task/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/task/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    10002 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/task/mysql_staleness_removal_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15185 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/task/neo4j_staleness_removal_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     9108 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/task/neptune_staleness_removal_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/task/search/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/task/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12199 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/task/search/document_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/task/search/search_data_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/task/search/search_metadata_to_elasticsearch_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/task/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/transformer/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/transformer/bigquery_usage_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/transformer/complex_type_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/transformer/dict_to_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/transformer/generic_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/transformer/regex_str_replace_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/transformer/remove_field_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/transformer/table_tag_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/transformer/template_variable_substitution_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/transformer/timestamp_string_to_epoch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/types/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/00_cluster_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      756 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_1_reader.json
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_2_table_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_3_bookmark.json
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_4_report.json
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_column_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      574 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_column_table_relation.json
--rw-r--r--   0 runner    (1001) docker     (123)      590 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_database_cluster_relation.json
--rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_database_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      582 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_schema_cluster_relation.json
--rw-r--r--   0 runner    (1001) docker     (123)      143 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_schema_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      417 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_source_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      583 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_table_schema_relation.json
--rw-r--r--   0 runner    (1001) docker     (123)      574 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_table_source_relation.json
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/02_user.json
--rw-r--r--   0 runner    (1001) docker     (123)      598 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/04_reader_referenceable_relation.json
--rw-r--r--   0 runner    (1001) docker     (123)      573 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/04_user_reader_relation.json
--rw-r--r--   0 runner    (1001) docker     (123)      245 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/05_1_hive_table_partition.json
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/05_table_partition_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      567 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/06_user_table_owner_relation.json
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/07_application_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      180 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/08_lineage_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/dashboard/01_group.json
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/dashboard/02_dashboard.json
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/dashboard/03_query.json
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/dashboard/04_chart.json
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/dashboard/05_execution.json
--rw-r--r--   0 runner    (1001) docker     (123)      594 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/dashboard/06_dashboard_cluster_relation.json
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/types/atlas/types_def.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/databuilder/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/utils/atlas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/utils/closer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/utils/hive_complex_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/utils/publisher_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/databuilder/utils/trino_complex_type_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/example/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      547 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2022-12-16 05:07:09.000000 amundsen-databuilder-7.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2022-12-16 05:07:06.000000 amundsen-databuilder-7.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   116465 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/amundsen_databuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/amundsen_databuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/amundsen_databuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/amundsen_databuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/amundsen_databuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/amundsen_databuilder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/callback/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/callback/call_back.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/clients/neptune_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/athena_metadata_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17997 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/atlas_search_data_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/base_bigquery_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/base_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/base_postgres_metadata_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/base_teradata_metadata_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/bigquery_metadata_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/bigquery_usage_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/bigquery_watermark_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/cassandra_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/csv_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/apache_superset/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/apache_superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/apache_superset/apache_superset_chart_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/apache_superset/apache_superset_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/apache_superset/apache_superset_metadata_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/apache_superset/apache_superset_table_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/databricks_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/databricks_sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/databricks_sql/databricks_sql_dashboard_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/databricks_sql/databricks_sql_dashboard_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_charts_batch_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_executions_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_last_modified_timestamp_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_last_successful_executions_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_owner_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_queries_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_usage_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_user_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/redash/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/redash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/redash/redash_dashboard_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/redash/redash_dashboard_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/tableau/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/tableau/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/tableau/tableau_dashboard_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/tableau/tableau_dashboard_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/tableau/tableau_dashboard_last_modified_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/tableau/tableau_dashboard_query_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/tableau/tableau_dashboard_table_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/tableau/tableau_dashboard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/tableau/tableau_external_table_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/db2_metadata_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/db_api_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dbt_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23680 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/delta_lake_metadata_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/dremio_metadata_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/druid_metadata_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/es_base_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/es_column_stats_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/es_last_updated_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/es_metadata_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/es_watermark_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/eventbridge_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/feast_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/generic_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/generic_usage_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/glue_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/hive_table_last_updated_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/hive_table_metadata_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/kafka_schema_registry_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/kafka_source_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/mssql_metadata_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/mysql_metadata_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19817 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/mysql_search_data_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/neo4j_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/neo4j_search_data_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/neptune_search_data_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/openlineage_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/oracle_metadata_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/pandas_profiling_column_stats_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/postgres_metadata_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/presto_view_metadata_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/redshift_metadata_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/extractor/restapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/restapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/restapi/rest_api_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/salesforce_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/snowflake_metadata_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/snowflake_table_last_updated_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/sql_alchemy_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/table_metadata_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/teradata_metadata_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/extractor/user/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/extractor/user/bamboohr/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/user/bamboohr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/user/bamboohr/bamboohr_user_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/extractor/vertica_metadata_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/filesystem/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/filesystem/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/job/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/job/base_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/job/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/loader/base_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/loader/file_system_atlas_csv_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/loader/file_system_csv_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/loader/file_system_elasticsearch_json_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/loader/file_system_mysql_csv_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/loader/file_system_neo4j_csv_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/loader/file_system_neptune_csv_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/loader/generic_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/atlas_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/atlas_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/atlas_serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/badge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/models/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/cluster/cluster_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/models/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/dashboard/dashboard_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/dashboard/dashboard_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/dashboard/dashboard_last_modified.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/dashboard/dashboard_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/dashboard/dashboard_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/dashboard/dashboard_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/dashboard/dashboard_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/dashboard/dashboard_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/dashboard_elasticsearch_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/description_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/elasticsearch_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/es_last_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/models/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/feature/feature_elasticsearch_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/feature/feature_generation_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/feature/feature_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/feature/feature_watermark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/graph_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/graph_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/graph_serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/owner_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/models/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/query/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/query/query_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/query/query_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/query/query_where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/models/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/schema/schema_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/table_column_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/table_elasticsearch_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/table_last_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/table_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31710 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/table_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/table_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/table_serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/table_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/table_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/models/timestamp/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/timestamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/timestamp/timestamp_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20307 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/type_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/models/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/usage/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/usage/usage_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/user_elasticsearch_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/models/watermark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/publisher/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/publisher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/publisher/atlas_csv_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/publisher/base_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/publisher/elasticsearch_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/publisher/elasticsearch_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/publisher/mysql_csv_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22007 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/publisher/neo4j_csv_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18764 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/publisher/neo4j_csv_unwind_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/publisher/neo4j_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/publisher/neptune_csv_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/publisher/publisher_config_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/rest_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/rest_api/base_rest_api_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/rest_api/mode_analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/rest_api/mode_analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/rest_api/mode_analytics/mode_paginated_rest_api_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/rest_api/query_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/rest_api/rest_api_failure_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/rest_api/rest_api_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/serializers/atlas_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/serializers/mysql_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/serializers/neo4_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/serializers/neptune_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/task/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/task/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/task/mysql_staleness_removal_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15185 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/task/neo4j_staleness_removal_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9108 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/task/neptune_staleness_removal_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/task/search/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/task/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12199 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/task/search/document_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/task/search/search_data_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/task/search/search_metadata_to_elasticsearch_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/task/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/transformer/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/transformer/bigquery_usage_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/transformer/complex_type_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/transformer/dict_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/transformer/generic_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/transformer/regex_str_replace_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/transformer/remove_field_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/transformer/table_tag_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/transformer/template_variable_substitution_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/transformer/timestamp_string_to_epoch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/00_cluster_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_1_reader.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_2_table_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_3_bookmark.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_4_report.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_column_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_column_table_relation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_database_cluster_relation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_database_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_schema_cluster_relation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_schema_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_source_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_table_schema_relation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_table_source_relation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/02_user.json
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/04_reader_referenceable_relation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/04_user_reader_relation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/05_1_hive_table_partition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/05_table_partition_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/06_user_table_owner_relation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/07_application_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/08_lineage_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/dashboard/01_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/dashboard/02_dashboard.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/dashboard/03_query.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/dashboard/04_chart.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/dashboard/05_execution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/dashboard/06_dashboard_cluster_relation.json
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/types/atlas/types_def.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/databuilder/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/utils/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/utils/closer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/utils/hive_complex_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/utils/publisher_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/databuilder/utils/trino_complex_type_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-14 21:43:33.000000 amundsen-databuilder-7.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-06-14 21:43:30.000000 amundsen-databuilder-7.4.4/setup.py
```

### Comparing `amundsen-databuilder-7.4.3/PKG-INFO` & `amundsen-databuilder-7.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amundsen-databuilder
-Version: 7.4.3
+Version: 7.4.4
 Summary: Amundsen Data builder
 Home-page: https://www.github.com/amundsen-io/amundsen/tree/main/databuilder
 Maintainer: Amundsen TSC
 Maintainer-email: amundsen-tsc@lists.lfai.foundation
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `amundsen-databuilder-7.4.3/README.md` & `amundsen-databuilder-7.4.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Amundsen Databuilder is a data ingestion library, which is inspired by [Apache Gobblin](https://gobblin.apache.org/). It could be used in an orchestration framework(e.g. Apache Airflow) to build data from Amundsen. You could use the library either with an adhoc python script([example](https://github.com/amundsen-io/amundsen/blob/main/databuilder/example/scripts/sample_data_loader.py)) or inside an Apache Airflow DAG([example](https://github.com/amundsen-io/amundsen/blob/main/databuilder/example/dags/hive_sample_dag.py)).
 
 For information about Amundsen and our other services, visit the [main repository](https://github.com/amundsen-io/amundsen#amundsen) `README.md` . Please also see our instructions for a [quick start](https://github.com/amundsen-io/amundsen/blob/master/docs/installation.md#bootstrap-a-default-version-of-amundsen-using-docker) setup  of Amundsen with dummy data, and an [overview of the architecture](https://github.com/amundsen-io/amundsen/blob/master/docs/architecture.md#architecture).
 
 ## Requirements
 - Python >= 3.6.x
-- elasticsearch 6.x (currently it doesn't support 7.x)
+- elasticsearch 7.x
 
 ## Doc
 - https://www.amundsen.io/amundsen/
 
 ## Concept
 ETL job consists of extraction of records from the source, transform records, if necessary, and load records into the sink. Amundsen Databuilder is a ETL framework for Amundsen and there are corresponding components for ETL called Extractor, Transformer, and Loader that deals with record level operation. A component called task controls all these three components.
 Job is the highest level component in Databuilder that controls task and publisher and is the one that client use to launch the ETL job.
```

### Comparing `amundsen-databuilder-7.4.3/amundsen_databuilder.egg-info/PKG-INFO` & `amundsen-databuilder-7.4.4/amundsen_databuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amundsen-databuilder
-Version: 7.4.3
+Version: 7.4.4
 Summary: Amundsen Data builder
 Home-page: https://www.github.com/amundsen-io/amundsen/tree/main/databuilder
 Maintainer: Amundsen TSC
 Maintainer-email: amundsen-tsc@lists.lfai.foundation
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `amundsen-databuilder-7.4.3/amundsen_databuilder.egg-info/SOURCES.txt` & `amundsen-databuilder-7.4.4/amundsen_databuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/amundsen_databuilder.egg-info/requires.txt` & `amundsen-databuilder-7.4.4/amundsen_databuilder.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 sqlalchemy>=1.3.6
 wheel>=0.31.1
 pytz>=2018.4
 statsd>=3.2.1
 retrying>=1.3.3
 unicodecsv<1.0,>=0.14.1
 httplib2>=0.18.0
-unidecode
+text-unidecode>=1.3
 Jinja2<4,>=2.10.0
 pandas<1.5.0,>=0.21.0
 responses>=0.10.6
 jsonref==0.2
 amundsen-common>=0.16.0
-amundsen-rds==0.0.7
+amundsen-rds==0.0.8
 
 [all]
 elasticsearch<8.0,>=6.2.0
 elasticsearch-dsl==7.4.0
 neo4j-driver<5.0,>=4.4.5
 requests<3.0,>=2.25.0
 freezegun>=1.1.0
@@ -39,21 +39,21 @@
 sqlalchemy>=1.3.6
 wheel>=0.31.1
 pytz>=2018.4
 statsd>=3.2.1
 retrying>=1.3.3
 unicodecsv<1.0,>=0.14.1
 httplib2>=0.18.0
-unidecode
+text-unidecode>=1.3
 Jinja2<4,>=2.10.0
 pandas<1.5.0,>=0.21.0
 responses>=0.10.6
 jsonref==0.2
 amundsen-common>=0.16.0
-amundsen-rds==0.0.7
+amundsen-rds==0.0.8
 flake8>=3.9.2
 flake8-tidy-imports>=4.3.0
 isort[colors]~=5.8.0
 mock>=4.0.3
 mypy<0.900,>=0.812
 pytest>=6.2.4
 pytest-cov>=2.12.0
```

### Comparing `amundsen-databuilder-7.4.3/databuilder/__init__.py` & `amundsen-databuilder-7.4.4/databuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/callback/call_back.py` & `amundsen-databuilder-7.4.4/databuilder/callback/call_back.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/clients/neptune_client.py` & `amundsen-databuilder-7.4.4/databuilder/clients/neptune_client.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/athena_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/athena_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/atlas_search_data_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/atlas_search_data_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/base_bigquery_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/base_bigquery_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/base_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/base_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/base_postgres_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/base_postgres_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/base_teradata_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/base_teradata_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/bigquery_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/bigquery_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/bigquery_usage_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/bigquery_usage_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/bigquery_watermark_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/bigquery_watermark_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/cassandra_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/cassandra_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/csv_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/csv_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/apache_superset/apache_superset_chart_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/apache_superset/apache_superset_chart_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/apache_superset/apache_superset_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/apache_superset/apache_superset_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/apache_superset/apache_superset_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/apache_superset/apache_superset_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/apache_superset/apache_superset_table_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/apache_superset/apache_superset_table_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/databricks_sql/databricks_sql_dashboard_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/databricks_sql/databricks_sql_dashboard_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/databricks_sql/databricks_sql_dashboard_utils.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/databricks_sql/databricks_sql_dashboard_utils.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_charts_batch_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_charts_batch_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_executions_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_executions_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_last_modified_timestamp_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_last_modified_timestamp_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_last_successful_executions_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_last_successful_executions_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_owner_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_owner_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_queries_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_queries_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_usage_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_usage_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_user_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_user_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_utils.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/mode_analytics/mode_dashboard_utils.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/redash/redash_dashboard_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/redash/redash_dashboard_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/redash/redash_dashboard_utils.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/redash/redash_dashboard_utils.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/tableau/tableau_dashboard_constants.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/tableau/tableau_dashboard_constants.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/tableau/tableau_dashboard_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/tableau/tableau_dashboard_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/tableau/tableau_dashboard_last_modified_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/tableau/tableau_dashboard_last_modified_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/tableau/tableau_dashboard_query_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/tableau/tableau_dashboard_query_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/tableau/tableau_dashboard_table_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/tableau/tableau_dashboard_table_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/tableau/tableau_dashboard_utils.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/tableau/tableau_dashboard_utils.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dashboard/tableau/tableau_external_table_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dashboard/tableau/tableau_external_table_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/db2_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/db2_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/db_api_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/db_api_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dbt_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dbt_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/delta_lake_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/delta_lake_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/dremio_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/dremio_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/druid_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/druid_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/es_base_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/es_base_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/es_column_stats_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/es_column_stats_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/es_last_updated_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/es_last_updated_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/es_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/es_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/es_watermark_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/es_watermark_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/eventbridge_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/eventbridge_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/feast_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/feast_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/generic_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/generic_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/generic_usage_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/generic_usage_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/glue_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/glue_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/hive_table_last_updated_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/hive_table_last_updated_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/hive_table_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/hive_table_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/kafka_schema_registry_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/kafka_schema_registry_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/kafka_source_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/kafka_source_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/mssql_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/mssql_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/mysql_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/mysql_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/mysql_search_data_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/mysql_search_data_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/neo4j_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/neo4j_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/neo4j_search_data_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/neo4j_search_data_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/neptune_search_data_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/neptune_search_data_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/openlineage_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/openlineage_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/oracle_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/oracle_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/pandas_profiling_column_stats_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/pandas_profiling_column_stats_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/postgres_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/postgres_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/presto_view_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/presto_view_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/restapi/rest_api_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/restapi/rest_api_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/salesforce_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/salesforce_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/snowflake_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/snowflake_metadata_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from collections import namedtuple
 from itertools import groupby
 from typing import (
     Any, Dict, Iterator, Union,
 )
 
 from pyhocon import ConfigFactory, ConfigTree
-from unidecode import unidecode
+from text_unidecode import unidecode
 
 from databuilder.extractor import sql_alchemy_extractor
 from databuilder.extractor.base_extractor import Extractor
 from databuilder.models.table_metadata import ColumnMetadata, TableMetadata
 
 TableKey = namedtuple('TableKey', ['schema', 'table_name'])
```

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/snowflake_table_last_updated_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/snowflake_table_last_updated_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/sql_alchemy_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/sql_alchemy_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/teradata_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/teradata_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/user/bamboohr/bamboohr_user_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/user/bamboohr/bamboohr_user_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/extractor/vertica_metadata_extractor.py` & `amundsen-databuilder-7.4.4/databuilder/extractor/vertica_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/filesystem/filesystem.py` & `amundsen-databuilder-7.4.4/databuilder/filesystem/filesystem.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/filesystem/metadata.py` & `amundsen-databuilder-7.4.4/databuilder/filesystem/metadata.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/job/base_job.py` & `amundsen-databuilder-7.4.4/databuilder/job/base_job.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/job/job.py` & `amundsen-databuilder-7.4.4/databuilder/job/job.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/loader/file_system_atlas_csv_loader.py` & `amundsen-databuilder-7.4.4/databuilder/loader/file_system_atlas_csv_loader.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/loader/file_system_csv_loader.py` & `amundsen-databuilder-7.4.4/databuilder/loader/file_system_csv_loader.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/loader/file_system_elasticsearch_json_loader.py` & `amundsen-databuilder-7.4.4/databuilder/loader/file_system_elasticsearch_json_loader.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/loader/file_system_mysql_csv_loader.py` & `amundsen-databuilder-7.4.4/databuilder/loader/file_system_mysql_csv_loader.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/loader/file_system_neo4j_csv_loader.py` & `amundsen-databuilder-7.4.4/databuilder/loader/file_system_neo4j_csv_loader.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/loader/file_system_neptune_csv_loader.py` & `amundsen-databuilder-7.4.4/databuilder/loader/file_system_neptune_csv_loader.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/loader/generic_loader.py` & `amundsen-databuilder-7.4.4/databuilder/loader/generic_loader.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/application.py` & `amundsen-databuilder-7.4.4/databuilder/models/application.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/atlas_serializable.py` & `amundsen-databuilder-7.4.4/databuilder/models/atlas_serializable.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/badge.py` & `amundsen-databuilder-7.4.4/databuilder/models/badge.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/dashboard/dashboard_chart.py` & `amundsen-databuilder-7.4.4/databuilder/models/dashboard/dashboard_chart.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/dashboard/dashboard_execution.py` & `amundsen-databuilder-7.4.4/databuilder/models/dashboard/dashboard_execution.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/dashboard/dashboard_last_modified.py` & `amundsen-databuilder-7.4.4/databuilder/models/dashboard/dashboard_last_modified.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/dashboard/dashboard_metadata.py` & `amundsen-databuilder-7.4.4/databuilder/models/dashboard/dashboard_metadata.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/dashboard/dashboard_owner.py` & `amundsen-databuilder-7.4.4/databuilder/models/dashboard/dashboard_owner.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/dashboard/dashboard_query.py` & `amundsen-databuilder-7.4.4/databuilder/models/dashboard/dashboard_query.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/dashboard/dashboard_table.py` & `amundsen-databuilder-7.4.4/databuilder/models/dashboard/dashboard_table.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/dashboard/dashboard_usage.py` & `amundsen-databuilder-7.4.4/databuilder/models/dashboard/dashboard_usage.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/dashboard_elasticsearch_document.py` & `amundsen-databuilder-7.4.4/databuilder/models/dashboard_elasticsearch_document.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/description_metadata.py` & `amundsen-databuilder-7.4.4/databuilder/models/description_metadata.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/elasticsearch_document.py` & `amundsen-databuilder-7.4.4/databuilder/models/elasticsearch_document.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/es_last_updated.py` & `amundsen-databuilder-7.4.4/databuilder/models/es_last_updated.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/feature/feature_elasticsearch_document.py` & `amundsen-databuilder-7.4.4/databuilder/models/feature/feature_elasticsearch_document.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/feature/feature_generation_code.py` & `amundsen-databuilder-7.4.4/databuilder/models/feature/feature_generation_code.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/feature/feature_metadata.py` & `amundsen-databuilder-7.4.4/databuilder/models/feature/feature_metadata.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/feature/feature_watermark.py` & `amundsen-databuilder-7.4.4/databuilder/models/feature/feature_watermark.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/graph_serializable.py` & `amundsen-databuilder-7.4.4/databuilder/models/graph_serializable.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/owner.py` & `amundsen-databuilder-7.4.4/databuilder/models/owner.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/query/base.py` & `amundsen-databuilder-7.4.4/databuilder/models/query/base.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/query/query.py` & `amundsen-databuilder-7.4.4/databuilder/models/query/query.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/query/query_execution.py` & `amundsen-databuilder-7.4.4/databuilder/models/query/query_execution.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/query/query_join.py` & `amundsen-databuilder-7.4.4/databuilder/models/query/query_join.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/query/query_where.py` & `amundsen-databuilder-7.4.4/databuilder/models/query/query_where.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/report.py` & `amundsen-databuilder-7.4.4/databuilder/models/report.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/schema/schema.py` & `amundsen-databuilder-7.4.4/databuilder/models/schema/schema.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/table_column_usage.py` & `amundsen-databuilder-7.4.4/databuilder/models/table_column_usage.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/table_elasticsearch_document.py` & `amundsen-databuilder-7.4.4/databuilder/models/table_elasticsearch_document.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/table_last_updated.py` & `amundsen-databuilder-7.4.4/databuilder/models/table_last_updated.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/table_lineage.py` & `amundsen-databuilder-7.4.4/databuilder/models/table_lineage.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,39 +3,44 @@
 
 from abc import abstractmethod
 from typing import (
     Iterator, List, Union,
 )
 
 from amundsen_common.utils.atlas import AtlasCommonParams, AtlasTableTypes
+from amundsen_rds.models import RDSModel
+from amundsen_rds.models.column import ColumnLineage as RDSColumnLineage
+from amundsen_rds.models.table import TableLineage as RDSTableLineage
 
 from databuilder.models.atlas_entity import AtlasEntity
 from databuilder.models.atlas_relationship import AtlasRelationship
 from databuilder.models.atlas_serializable import AtlasSerializable
 from databuilder.models.graph_node import GraphNode
 from databuilder.models.graph_relationship import GraphRelationship
 from databuilder.models.graph_serializable import GraphSerializable
 from databuilder.models.table_metadata import ColumnMetadata, TableMetadata
+from databuilder.models.table_serializable import TableSerializable
 from databuilder.serializers.atlas_serializer import get_entity_attrs
 from databuilder.utils.atlas import AtlasRelationshipTypes, AtlasSerializedEntityOperation
 
 
-class BaseLineage(GraphSerializable, AtlasSerializable):
+class BaseLineage(GraphSerializable, AtlasSerializable, TableSerializable):
     """
     Generic Lineage Interface
     """
     LABEL = 'Lineage'
     ORIGIN_DEPENDENCY_RELATION_TYPE = 'HAS_DOWNSTREAM'
     DEPENDENCY_ORIGIN_RELATION_TYPE = 'HAS_UPSTREAM'
 
     def __init__(self) -> None:
         self._node_iter = self._create_node_iterator()
         self._relation_iter = self._create_rel_iterator()
         self._atlas_entity_iterator = self._create_next_atlas_entity()
         self._atlas_relation_iterator = self._create_next_atlas_relation()
+        self._record_iter = self._create_record_iterator()
 
     def create_next_node(self) -> Union[GraphNode, None]:
         # return the string representation of the data
         try:
             return next(self._node_iter)
         except StopIteration:
             return None
@@ -115,14 +120,24 @@
     def _get_atlas_process_key(self) -> str:
         pass
 
     @abstractmethod
     def _get_atlas_entity_type(self) -> str:
         pass
 
+    def create_next_record(self) -> Union[RDSModel, None]:
+        try:
+            return next(self._record_iter)
+        except StopIteration:
+            return None
+
+    @abstractmethod
+    def _create_record_iterator(self) -> Iterator[RDSModel]:
+        pass
+
 
 class TableLineage(BaseLineage):
     """
     Table Lineage Model. It won't create nodes but create upstream/downstream rels.
     """
 
     def __init__(self,
@@ -154,14 +169,26 @@
 
     def _get_atlas_process_key(self) -> str:
         return self.table_key
 
     def _get_atlas_entity_type(self) -> str:
         return AtlasTableTypes.table
 
+    def _create_record_iterator(self) -> Iterator[RDSModel]:
+        """
+        Create lineage records for source table and its all downstream tables.
+        :return:
+        """
+        for downstream_key in self.downstream_deps:
+            record = RDSTableLineage(
+                table_source_rk=self.table_key,
+                table_target_rk=downstream_key
+            )
+            yield record
+
     def __repr__(self) -> str:
         return f'TableLineage({self.table_key!r})'
 
 
 class ColumnLineage(BaseLineage):
     """
     Column Lineage Model. It won't create nodes but create upstream/downstream rels.
@@ -196,9 +223,21 @@
 
     def _get_atlas_process_key(self) -> str:
         return self.column_key
 
     def _get_atlas_entity_type(self) -> str:
         return AtlasTableTypes.column
 
+    def _create_record_iterator(self) -> Iterator[RDSModel]:
+        """
+        Create lineage records for source column and its all downstream columns.
+        :return:
+        """
+        for downstream_key in self.downstream_deps:
+            record = RDSColumnLineage(
+                column_source_rk=self.column_key,
+                column_target_rk=downstream_key
+            )
+            yield record
+
     def __repr__(self) -> str:
         return f'ColumnLineage({self.column_key!r})'
```

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/table_metadata.py` & `amundsen-databuilder-7.4.4/databuilder/models/table_metadata.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/table_owner.py` & `amundsen-databuilder-7.4.4/databuilder/models/table_owner.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/table_serializable.py` & `amundsen-databuilder-7.4.4/databuilder/models/table_serializable.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/table_source.py` & `amundsen-databuilder-7.4.4/databuilder/models/table_source.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/table_stats.py` & `amundsen-databuilder-7.4.4/databuilder/models/table_stats.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/type_metadata.py` & `amundsen-databuilder-7.4.4/databuilder/models/type_metadata.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/usage/usage.py` & `amundsen-databuilder-7.4.4/databuilder/models/usage/usage.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/user.py` & `amundsen-databuilder-7.4.4/databuilder/models/user.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/user_elasticsearch_document.py` & `amundsen-databuilder-7.4.4/databuilder/models/user_elasticsearch_document.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/models/watermark.py` & `amundsen-databuilder-7.4.4/databuilder/models/watermark.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/publisher/atlas_csv_publisher.py` & `amundsen-databuilder-7.4.4/databuilder/publisher/atlas_csv_publisher.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/publisher/base_publisher.py` & `amundsen-databuilder-7.4.4/databuilder/publisher/base_publisher.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/publisher/elasticsearch_constants.py` & `amundsen-databuilder-7.4.4/databuilder/publisher/elasticsearch_constants.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/publisher/elasticsearch_publisher.py` & `amundsen-databuilder-7.4.4/databuilder/publisher/elasticsearch_publisher.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def __init__(self) -> None:
         super(ElasticsearchPublisher, self).__init__()
 
     def init(self, conf: ConfigTree) -> None:
         self.conf = conf
 
         self.file_path = self.conf.get_string(ElasticsearchPublisher.FILE_PATH_CONFIG_KEY)
-        self.file_mode = self.conf.get_string(ElasticsearchPublisher.FILE_MODE_CONFIG_KEY, 'w')
+        self.file_mode = self.conf.get_string(ElasticsearchPublisher.FILE_MODE_CONFIG_KEY, 'r')
 
         self.elasticsearch_type = self.conf.get_string(ElasticsearchPublisher.ELASTICSEARCH_DOC_TYPE_CONFIG_KEY)
         self.elasticsearch_client = self.conf.get(ElasticsearchPublisher.ELASTICSEARCH_CLIENT_CONFIG_KEY)
         self.elasticsearch_new_index = self.conf.get(ElasticsearchPublisher.ELASTICSEARCH_NEW_INDEX_CONFIG_KEY)
         self.elasticsearch_alias = self.conf.get(ElasticsearchPublisher.ELASTICSEARCH_ALIAS_CONFIG_KEY)
 
         self.elasticsearch_mapping = self.conf.get(ElasticsearchPublisher.ELASTICSEARCH_MAPPING_CONFIG_KEY,
@@ -131,9 +131,17 @@
         actions.extend(delete_actions)
 
         update_action = {"actions": actions}
 
         # perform alias update and index delete in single atomic operation
         self.elasticsearch_client.indices.update_aliases(update_action)
 
+    def close(self) -> None:
+        """
+        close the file handler
+        :return:
+        """
+        if self.file_handler:
+            self.file_handler.close()
+
     def get_scope(self) -> str:
         return 'publisher.elasticsearch'
```

### Comparing `amundsen-databuilder-7.4.3/databuilder/publisher/mysql_csv_publisher.py` & `amundsen-databuilder-7.4.4/databuilder/publisher/mysql_csv_publisher.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/publisher/neo4j_csv_publisher.py` & `amundsen-databuilder-7.4.4/databuilder/publisher/neo4j_csv_publisher.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/publisher/neo4j_csv_unwind_publisher.py` & `amundsen-databuilder-7.4.4/databuilder/publisher/neo4j_csv_unwind_publisher.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/publisher/neo4j_preprocessor.py` & `amundsen-databuilder-7.4.4/databuilder/publisher/neo4j_preprocessor.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/publisher/neptune_csv_publisher.py` & `amundsen-databuilder-7.4.4/databuilder/publisher/neptune_csv_publisher.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/publisher/publisher_config_constants.py` & `amundsen-databuilder-7.4.4/databuilder/publisher/publisher_config_constants.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/rest_api/base_rest_api_query.py` & `amundsen-databuilder-7.4.4/databuilder/rest_api/base_rest_api_query.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/rest_api/mode_analytics/mode_paginated_rest_api_query.py` & `amundsen-databuilder-7.4.4/databuilder/rest_api/mode_analytics/mode_paginated_rest_api_query.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/rest_api/query_merger.py` & `amundsen-databuilder-7.4.4/databuilder/rest_api/query_merger.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/rest_api/rest_api_failure_handlers.py` & `amundsen-databuilder-7.4.4/databuilder/rest_api/rest_api_failure_handlers.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/rest_api/rest_api_query.py` & `amundsen-databuilder-7.4.4/databuilder/rest_api/rest_api_query.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/serializers/atlas_serializer.py` & `amundsen-databuilder-7.4.4/databuilder/serializers/atlas_serializer.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/serializers/neo4_serializer.py` & `amundsen-databuilder-7.4.4/databuilder/serializers/neo4_serializer.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/serializers/neptune_serializer.py` & `amundsen-databuilder-7.4.4/databuilder/serializers/neptune_serializer.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/task/base_task.py` & `amundsen-databuilder-7.4.4/databuilder/task/base_task.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/task/mysql_staleness_removal_task.py` & `amundsen-databuilder-7.4.4/databuilder/task/mysql_staleness_removal_task.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/task/neo4j_staleness_removal_task.py` & `amundsen-databuilder-7.4.4/databuilder/task/neo4j_staleness_removal_task.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/task/neptune_staleness_removal_task.py` & `amundsen-databuilder-7.4.4/databuilder/task/neptune_staleness_removal_task.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/task/search/document_mappings.py` & `amundsen-databuilder-7.4.4/databuilder/task/search/document_mappings.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/task/search/search_data_queries.py` & `amundsen-databuilder-7.4.4/databuilder/task/search/search_data_queries.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/task/search/search_metadata_to_elasticsearch_task.py` & `amundsen-databuilder-7.4.4/databuilder/task/search/search_metadata_to_elasticsearch_task.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/task/task.py` & `amundsen-databuilder-7.4.4/databuilder/task/task.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/transformer/base_transformer.py` & `amundsen-databuilder-7.4.4/databuilder/transformer/base_transformer.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/transformer/bigquery_usage_transformer.py` & `amundsen-databuilder-7.4.4/databuilder/transformer/bigquery_usage_transformer.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/transformer/complex_type_transformer.py` & `amundsen-databuilder-7.4.4/databuilder/transformer/complex_type_transformer.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/transformer/dict_to_model.py` & `amundsen-databuilder-7.4.4/databuilder/transformer/dict_to_model.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/transformer/generic_transformer.py` & `amundsen-databuilder-7.4.4/databuilder/transformer/generic_transformer.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/transformer/regex_str_replace_transformer.py` & `amundsen-databuilder-7.4.4/databuilder/transformer/regex_str_replace_transformer.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/transformer/remove_field_transformer.py` & `amundsen-databuilder-7.4.4/databuilder/transformer/remove_field_transformer.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/transformer/table_tag_transformer.py` & `amundsen-databuilder-7.4.4/databuilder/transformer/table_tag_transformer.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/transformer/template_variable_substitution_transformer.py` & `amundsen-databuilder-7.4.4/databuilder/transformer/template_variable_substitution_transformer.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/transformer/timestamp_string_to_epoch.py` & `amundsen-databuilder-7.4.4/databuilder/transformer/timestamp_string_to_epoch.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/__init__.py` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/__init__.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_1_reader.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_1_reader.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_2_table_schema.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_2_table_schema.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_3_bookmark.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_3_bookmark.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_4_report.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_4_report.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_column_schema.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_column_schema.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_column_table_relation.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_column_table_relation.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_database_cluster_relation.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_database_cluster_relation.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_schema_cluster_relation.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_schema_cluster_relation.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_table_schema_relation.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_table_schema_relation.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/01_table_source_relation.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/01_table_source_relation.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/02_user.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/02_user.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/04_reader_referenceable_relation.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/04_reader_referenceable_relation.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/04_user_reader_relation.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/04_user_reader_relation.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/05_table_partition_schema.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/05_table_partition_schema.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/06_user_table_owner_relation.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/06_user_table_owner_relation.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/07_application_schema.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/07_application_schema.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/dashboard/01_group.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/dashboard/01_group.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/dashboard/02_dashboard.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/dashboard/02_dashboard.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/dashboard/03_query.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/dashboard/03_query.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/dashboard/04_chart.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/dashboard/04_chart.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/dashboard/05_execution.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/dashboard/05_execution.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/schema/dashboard/06_dashboard_cluster_relation.json` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/schema/dashboard/06_dashboard_cluster_relation.json`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/types/atlas/types_def.py` & `amundsen-databuilder-7.4.4/databuilder/types/atlas/types_def.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/utils/atlas.py` & `amundsen-databuilder-7.4.4/databuilder/utils/atlas.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/utils/closer.py` & `amundsen-databuilder-7.4.4/databuilder/utils/closer.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/utils/hive_complex_type_parser.py` & `amundsen-databuilder-7.4.4/databuilder/utils/hive_complex_type_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,32 +19,32 @@
 
 field_name = Word(alphanums + "_")
 field_type = Forward()
 
 # Scalar types
 union_list = delimitedList(field_type)
 union_type = nestedExpr(
-    opener=union_keyword + "<", closer=">", content=union_list, ignoreExpr=None
+    opener=union_keyword + "<", closer=">", content=union_list, ignoreExpr=None  # type: ignore
 )
 scalar_quantifier = "(" + Word(nums) + Optional(")" | "," + Word(nums) + ")")
 scalar_type = union_type | OneOrMore(Word(alphanums + "_")) + Optional(scalar_quantifier)
 
 # Complex types
 array_field = "<" + field_type("type")
 map_field = originalTextFor(scalar_type)("key") + "," + field_type("type")
 struct_field = field_name("name") + ":" + field_type("type")
 struct_list = delimitedList(Group(struct_field))
 array_type = nestedExpr(
-    opener=array_keyword, closer=">", content=array_field, ignoreExpr=None
+    opener=array_keyword, closer=">", content=array_field, ignoreExpr=None  # type: ignore
 )
 map_type = nestedExpr(
-    opener=map_keyword + "<", closer=">", content=map_field, ignoreExpr=None
+    opener=map_keyword + "<", closer=">", content=map_field, ignoreExpr=None  # type: ignore
 )
 struct_type = nestedExpr(
-    opener=struct_keyword + "<", closer=">", content=struct_list, ignoreExpr=None
+    opener=struct_keyword + "<", closer=">", content=struct_list, ignoreExpr=None  # type: ignore
 )
 
 field_type <<= originalTextFor(array_type | map_type | struct_type | scalar_type)
 
 complex_type = (array_type("array_type") | map_type("map_type") | struct_type("struct_type") |
                 scalar_type("scalar_type"))
```

### Comparing `amundsen-databuilder-7.4.3/databuilder/utils/publisher_utils.py` & `amundsen-databuilder-7.4.4/databuilder/utils/publisher_utils.py`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/databuilder/utils/trino_complex_type_parser.py` & `amundsen-databuilder-7.4.4/databuilder/utils/trino_complex_type_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 
 # Complex types
 array_field = "(" + field_type("type")
 map_field = originalTextFor(scalar_type)("key") + "," + field_type("type")
 struct_field = field_name("name") + field_type("type")
 struct_list = delimitedList(Group(struct_field))
 array_type = nestedExpr(
-    opener=array_keyword, closer=")", content=array_field, ignoreExpr=None
+    opener=array_keyword, closer=")", content=array_field, ignoreExpr=None  # type: ignore
 )
 map_type = nestedExpr(
-    opener=map_keyword + "(", closer=")", content=map_field, ignoreExpr=None
+    opener=map_keyword + "(", closer=")", content=map_field, ignoreExpr=None  # type: ignore
 )
 struct_type = nestedExpr(
-    opener=struct_keyword + "(", closer=")", content=struct_list, ignoreExpr=None
+    opener=struct_keyword + "(", closer=")", content=struct_list, ignoreExpr=None  # type: ignore
 )
 
 field_type <<= originalTextFor(array_type | map_type | struct_type | scalar_type)
 
 complex_type = (array_type("array_type") | map_type("map_type") | struct_type("struct_type") |
                 scalar_type("scalar_type"))
```

### Comparing `amundsen-databuilder-7.4.3/requirements.txt` & `amundsen-databuilder-7.4.4/requirements.txt`

 * *Files 27% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 sqlalchemy>=1.3.6
 wheel>=0.31.1
 pytz>=2018.4
 statsd>=3.2.1
 retrying>=1.3.3
 unicodecsv>=0.14.1,<1.0
 httplib2>=0.18.0
-unidecode
+text-unidecode>=1.3
 Jinja2>=2.10.0,<4
 pandas>=0.21.0,<1.5.0
 responses>=0.10.6
 jsonref==0.2
 
 amundsen-common>=0.16.0
-amundsen-rds==0.0.7
+amundsen-rds==0.0.8
```

### Comparing `amundsen-databuilder-7.4.3/setup.cfg` & `amundsen-databuilder-7.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `amundsen-databuilder-7.4.3/setup.py` & `amundsen-databuilder-7.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright Contributors to the Amundsen project.
 # SPDX-License-Identifier: Apache-2.0
 
 import os
 
 from setuptools import find_packages, setup
 
-__version__ = '7.4.3'
+__version__ = '7.4.4'
 
 requirements_path = os.path.join(os.path.dirname(os.path.realpath(__file__)),
                                  'requirements.txt')
 with open(requirements_path, 'r') as requirements_file:
     requirements = requirements_file.readlines()
 
 requirements_path = os.path.join(os.path.dirname(os.path.realpath(__file__)),
```

