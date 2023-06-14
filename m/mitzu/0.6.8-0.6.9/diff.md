# Comparing `tmp/mitzu-0.6.8.tar.gz` & `tmp/mitzu-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitzu-0.6.8.tar", max compression
+gzip compressed data, was "mitzu-0.6.9.tar", max compression
```

## Comparing `mitzu-0.6.8.tar` & `mitzu-0.6.9.tar`

### file list

```diff
@@ -1,138 +1,138 @@
--rw-r--r--   0        0        0     1082 2023-06-14 11:09:52.655983 mitzu-0.6.8/LICENSE.txt
--rw-r--r--   0        0        0     2235 2023-06-14 11:09:52.655983 mitzu-0.6.8/README.md
--rw-r--r--   0        0        0     6148 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/.DS_Store
--rw-r--r--   0        0        0      752 2023-06-14 11:10:47.345127 mitzu-0.6.8/mitzu/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/__init__.py
--rw-r--r--   0        0        0     1918 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/adapter_factory.py
--rw-r--r--   0        0        0     5148 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/athena_adapter.py
--rw-r--r--   0        0        0     6262 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/bigquery_adapter.py
--rw-r--r--   0        0        0     6026 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/databricks_adapter.py
--rw-r--r--   0        0        0     2261 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/file_adapter.py
--rw-r--r--   0        0        0     2533 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/generic_adapter.py
--rw-r--r--   0        0        0      898 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/helper.py
--rw-r--r--   0        0        0     3422 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/mysql_adapter.py
--rw-r--r--   0        0        0     6645 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/postgresql_adapter.py
--rw-r--r--   0        0        0     3765 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/redshift_adapter.py
--rw-r--r--   0        0        0     3298 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/snowflake_adapter.py
--rw-r--r--   0        0        0        0 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/athena/__init__.py
--rw-r--r--   0        0        0      701 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5071 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6415 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
--rw-r--r--   0        0        0     9751 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1844 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
--rw-r--r--   0        0        0        0 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/__init__.py
--rw-r--r--   0        0        0     2146 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2412 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py
--rw-r--r--   0        0        0     5071 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py
--rw-r--r--   0        0        0     4770 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py
--rw-r--r--   0        0        0    38550 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     8638 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py
--rw-r--r--   0        0        0     9854 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py
--rw-r--r--   0        0        0     7361 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py
--rw-r--r--   0        0        0     1131 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py
--rw-r--r--   0        0        0        0 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/databricks/__init__.py
--rw-r--r--   0        0        0      713 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5010 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6601 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
--rw-r--r--   0        0        0    10073 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1848 2023-06-14 11:09:53.051992 mitzu-0.6.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
--rw-r--r--   0        0        0    40466 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/adapters/sqlalchemy_adapter.py
--rw-r--r--   0        0        0     4963 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/adapters/sqlite_adapter.py
--rw-r--r--   0        0        0     7705 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/adapters/trino_adapter.py
--rw-r--r--   0        0        0     1835 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/helper.py
--rw-r--r--   0        0        0    53055 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/model.py
--rw-r--r--   0        0        0        0 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/notebook/__init__.py
--rw-r--r--   0        0        0     6845 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/notebook/model_loader.py
--rw-r--r--   0        0        0     2550 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/project_discovery.py
--rw-r--r--   0        0        0     2102 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/project_serialization.py
--rw-r--r--   0        0        0      785 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/samples/__init__.py
--rw-r--r--   0        0        0     3794 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/samples/data_ingestion.py
--rw-r--r--   0        0        0    10141 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/samples/sample_data_generator.py
--rw-r--r--   0        0        0    11933 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/serialization.py
--rw-r--r--   0        0        0        0 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/visualization/__init__.py
--rw-r--r--   0        0        0     7305 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/visualization/charts.py
--rw-r--r--   0        0        0     1866 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/visualization/common.py
--rw-r--r--   0        0        0      941 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/visualization/labels.py
--rw-r--r--   0        0        0     7802 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/visualization/plot.py
--rw-r--r--   0        0        0     5767 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/visualization/titles.py
--rw-r--r--   0        0        0     3181 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/visualization/tooltips.py
--rw-r--r--   0        0        0     3289 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/visualization/transform_conv.py
--rw-r--r--   0        0        0     1222 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/visualization/transform_retention.py
--rw-r--r--   0        0        0     6148 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/webapp/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/webapp/__init__.py
--rw-r--r--   0        0        0     5347 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/webapp/assets/explore_page.css
--rw-r--r--   0        0        0   147145 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/webapp/assets/favicon.ico
--rw-r--r--   0        0        0    46702 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/webapp/assets/logo.png
--rw-r--r--   0        0        0    43472 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/webapp/assets/mitzu-logo-light.svg
--rw-r--r--   0        0        0    49422 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/webapp/assets/warehouse/athena.png
--rw-r--r--   0        0        0    20802 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/webapp/assets/warehouse/bigquery.png
--rw-r--r--   0        0        0    10321 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/webapp/assets/warehouse/clickhouse.png
--rw-r--r--   0        0        0   119554 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/webapp/assets/warehouse/databricks.png
--rw-r--r--   0        0        0     3008 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/webapp/assets/warehouse/mysql.png
--rw-r--r--   0        0        0     2446 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/webapp/assets/warehouse/pandas.png
--rw-r--r--   0        0        0     5338 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/webapp/assets/warehouse/postgresql.png
--rw-r--r--   0        0        0     8512 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/webapp/assets/warehouse/redshift.png
--rw-r--r--   0        0        0    93500 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/webapp/assets/warehouse/snowflake.png
--rw-r--r--   0        0        0    48681 2023-06-14 11:09:53.055992 mitzu-0.6.8/mitzu/webapp/assets/warehouse/sqlite.png
--rw-r--r--   0        0        0    34219 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/assets/warehouse/trino.png
--rw-r--r--   0        0        0    15910 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/auth/authorizer.py
--rw-r--r--   0        0        0     3557 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/auth/cognito.py
--rw-r--r--   0        0        0     1305 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/auth/decorator.py
--rw-r--r--   0        0        0     2777 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/auth/google.py
--rw-r--r--   0        0        0     7481 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/cache.py
--rw-r--r--   0        0        0     2920 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/caching_dataset_adapter.py
--rw-r--r--   0        0        0     1664 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/configs.py
--rw-r--r--   0        0        0     3641 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/dependencies.py
--rw-r--r--   0        0        0     4984 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/helper.py
--rw-r--r--   0        0        0     8785 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/model.py
--rw-r--r--   0        0        0      309 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/navbar.py
--rw-r--r--   0        0        0     5435 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/offcanvas.py
--rw-r--r--   0        0        0     1606 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/onboarding_flow.py
--rw-r--r--   0        0        0        0 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/connections/__init__.py
--rw-r--r--   0        0        0    22704 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/connections/manage_connections_component.py
--rw-r--r--   0        0        0     4428 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/connections_page.py
--rw-r--r--   0        0        0        0 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/dashboards/__init__.py
--rw-r--r--   0        0        0    20561 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
--rw-r--r--   0        0        0     9628 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/dashboards_page.py
--rw-r--r--   0        0        0    14949 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/edit_user.py
--rw-r--r--   0        0        0        0 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/explore/__init__.py
--rw-r--r--   0        0        0     5929 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/explore/complex_segment_handler.py
--rw-r--r--   0        0        0     6488 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/explore/dates_selector_handler.py
--rw-r--r--   0        0        0     5790 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/explore/event_segment_handler.py
--rw-r--r--   0        0        0    22619 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/explore/explore_page.py
--rw-r--r--   0        0        0    10358 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/explore/graph_handler.py
--rw-r--r--   0        0        0    10698 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/explore/metric_config_handler.py
--rw-r--r--   0        0        0     2382 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/explore/metric_segments_handler.py
--rw-r--r--   0        0        0     1553 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/explore/metric_type_handler.py
--rw-r--r--   0        0        0    10285 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/explore/simple_segment_handler.py
--rw-r--r--   0        0        0     4644 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/explore/toolbar_handler.py
--rw-r--r--   0        0        0     1221 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/explore_project.py
--rw-r--r--   0        0        0    13959 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/home.py
--rw-r--r--   0        0        0     3947 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/login.py
--rw-r--r--   0        0        0     5023 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/manage_connection.py
--rw-r--r--   0        0        0     1288 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/manage_dashboard.py
--rw-r--r--   0        0        0    10095 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/manage_event_defs.py
--rw-r--r--   0        0        0    12087 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/manage_project.py
--rw-r--r--   0        0        0     9470 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/manage_saved_metrics.py
--rw-r--r--   0        0        0     1738 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/paths.py
--rw-r--r--   0        0        0        0 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/projects/__init__.py
--rw-r--r--   0        0        0    35694 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/projects/event_tables_config.py
--rw-r--r--   0        0        0      587 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/projects/helper.py
--rw-r--r--   0        0        0     9400 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/projects/manage_project_component.py
--rw-r--r--   0        0        0     5090 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/projects_page.py
--rw-r--r--   0        0        0     3114 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/pages/users.py
--rw-r--r--   0        0        0        0 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/service/__init__.py
--rw-r--r--   0        0        0     1955 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/service/events_service.py
--rw-r--r--   0        0        0     4974 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/service/navbar_service.py
--rw-r--r--   0        0        0      670 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/service/notification_service.py
--rw-r--r--   0        0        0     1647 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/service/onboarding_service.py
--rw-r--r--   0        0        0     2105 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/service/secret_service.py
--rw-r--r--   0        0        0     6708 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/service/tracking_service.py
--rw-r--r--   0        0        0     4756 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/service/user_service.py
--rw-r--r--   0        0        0    25283 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/storage.py
--rw-r--r--   0        0        0    25734 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/storage_model.py
--rw-r--r--   0        0        0     4700 2023-06-14 11:09:53.059992 mitzu-0.6.8/mitzu/webapp/webapp.py
--rw-r--r--   0        0        0     3422 2023-06-14 11:10:47.345127 mitzu-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 mitzu-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-14 14:01:24.644477 mitzu-0.6.9/LICENSE.txt
+-rw-r--r--   0        0        0     2235 2023-06-14 14:01:24.644477 mitzu-0.6.9/README.md
+-rw-r--r--   0        0        0     6148 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/.DS_Store
+-rw-r--r--   0        0        0      752 2023-06-14 14:02:33.588490 mitzu-0.6.9/mitzu/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/__init__.py
+-rw-r--r--   0        0        0     1918 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/adapter_factory.py
+-rw-r--r--   0        0        0     5148 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/athena_adapter.py
+-rw-r--r--   0        0        0     6262 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/bigquery_adapter.py
+-rw-r--r--   0        0        0     6026 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/databricks_adapter.py
+-rw-r--r--   0        0        0     2261 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/file_adapter.py
+-rw-r--r--   0        0        0     2533 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/generic_adapter.py
+-rw-r--r--   0        0        0      898 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/helper.py
+-rw-r--r--   0        0        0     3422 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/mysql_adapter.py
+-rw-r--r--   0        0        0     6645 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/postgresql_adapter.py
+-rw-r--r--   0        0        0     3765 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/redshift_adapter.py
+-rw-r--r--   0        0        0     3298 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/snowflake_adapter.py
+-rw-r--r--   0        0        0        0 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/athena/__init__.py
+-rw-r--r--   0        0        0      701 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5071 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6415 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0     9751 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1844 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
+-rw-r--r--   0        0        0        0 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/__init__.py
+-rw-r--r--   0        0        0     2146 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2412 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py
+-rw-r--r--   0        0        0     5071 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py
+-rw-r--r--   0        0        0     4770 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py
+-rw-r--r--   0        0        0    38550 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     8638 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py
+-rw-r--r--   0        0        0     9854 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py
+-rw-r--r--   0        0        0     7361 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0     1131 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py
+-rw-r--r--   0        0        0        0 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/databricks/__init__.py
+-rw-r--r--   0        0        0      713 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5010 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6601 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0    10073 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1848 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
+-rw-r--r--   0        0        0    40466 2023-06-14 14:01:25.060494 mitzu-0.6.9/mitzu/adapters/sqlalchemy_adapter.py
+-rw-r--r--   0        0        0     4963 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/adapters/sqlite_adapter.py
+-rw-r--r--   0        0        0     7705 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/adapters/trino_adapter.py
+-rw-r--r--   0        0        0     1835 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/helper.py
+-rw-r--r--   0        0        0    53053 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/model.py
+-rw-r--r--   0        0        0        0 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/notebook/__init__.py
+-rw-r--r--   0        0        0     6845 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/notebook/model_loader.py
+-rw-r--r--   0        0        0     2550 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/project_discovery.py
+-rw-r--r--   0        0        0     2102 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/project_serialization.py
+-rw-r--r--   0        0        0      785 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/samples/__init__.py
+-rw-r--r--   0        0        0     3794 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/samples/data_ingestion.py
+-rw-r--r--   0        0        0    10141 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/samples/sample_data_generator.py
+-rw-r--r--   0        0        0    11933 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/serialization.py
+-rw-r--r--   0        0        0        0 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/visualization/__init__.py
+-rw-r--r--   0        0        0     7305 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/visualization/charts.py
+-rw-r--r--   0        0        0     1866 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/visualization/common.py
+-rw-r--r--   0        0        0      941 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/visualization/labels.py
+-rw-r--r--   0        0        0     7802 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/visualization/plot.py
+-rw-r--r--   0        0        0     5767 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/visualization/titles.py
+-rw-r--r--   0        0        0     3181 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/visualization/tooltips.py
+-rw-r--r--   0        0        0     3289 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/visualization/transform_conv.py
+-rw-r--r--   0        0        0     1222 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/visualization/transform_retention.py
+-rw-r--r--   0        0        0     6148 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/webapp/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/webapp/__init__.py
+-rw-r--r--   0        0        0     5347 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/webapp/assets/explore_page.css
+-rw-r--r--   0        0        0   147145 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/webapp/assets/favicon.ico
+-rw-r--r--   0        0        0    46702 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/webapp/assets/logo.png
+-rw-r--r--   0        0        0    43472 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/webapp/assets/mitzu-logo-light.svg
+-rw-r--r--   0        0        0    49422 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/webapp/assets/warehouse/athena.png
+-rw-r--r--   0        0        0    20802 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/webapp/assets/warehouse/bigquery.png
+-rw-r--r--   0        0        0    10321 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/webapp/assets/warehouse/clickhouse.png
+-rw-r--r--   0        0        0   119554 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/webapp/assets/warehouse/databricks.png
+-rw-r--r--   0        0        0     3008 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/webapp/assets/warehouse/mysql.png
+-rw-r--r--   0        0        0     2446 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/webapp/assets/warehouse/pandas.png
+-rw-r--r--   0        0        0     5338 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/webapp/assets/warehouse/postgresql.png
+-rw-r--r--   0        0        0     8512 2023-06-14 14:01:25.064494 mitzu-0.6.9/mitzu/webapp/assets/warehouse/redshift.png
+-rw-r--r--   0        0        0    93500 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/assets/warehouse/snowflake.png
+-rw-r--r--   0        0        0    48681 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/assets/warehouse/sqlite.png
+-rw-r--r--   0        0        0    34219 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/assets/warehouse/trino.png
+-rw-r--r--   0        0        0    15910 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/auth/authorizer.py
+-rw-r--r--   0        0        0     3557 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/auth/cognito.py
+-rw-r--r--   0        0        0     1305 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/auth/decorator.py
+-rw-r--r--   0        0        0     2777 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/auth/google.py
+-rw-r--r--   0        0        0     7481 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/cache.py
+-rw-r--r--   0        0        0     2920 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/caching_dataset_adapter.py
+-rw-r--r--   0        0        0     1664 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/configs.py
+-rw-r--r--   0        0        0     3641 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/dependencies.py
+-rw-r--r--   0        0        0     4984 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/helper.py
+-rw-r--r--   0        0        0     8785 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/model.py
+-rw-r--r--   0        0        0      309 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/navbar.py
+-rw-r--r--   0        0        0     5435 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/offcanvas.py
+-rw-r--r--   0        0        0     1642 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/onboarding_flow.py
+-rw-r--r--   0        0        0        0 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/connections/__init__.py
+-rw-r--r--   0        0        0    25313 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/connections/manage_connections_component.py
+-rw-r--r--   0        0        0     4428 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/connections_page.py
+-rw-r--r--   0        0        0        0 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/dashboards/__init__.py
+-rw-r--r--   0        0        0    20561 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
+-rw-r--r--   0        0        0     9628 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/dashboards_page.py
+-rw-r--r--   0        0        0    14949 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/edit_user.py
+-rw-r--r--   0        0        0        0 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/explore/__init__.py
+-rw-r--r--   0        0        0     5929 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/explore/complex_segment_handler.py
+-rw-r--r--   0        0        0     6488 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/explore/dates_selector_handler.py
+-rw-r--r--   0        0        0     5790 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/explore/event_segment_handler.py
+-rw-r--r--   0        0        0    22619 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/explore/explore_page.py
+-rw-r--r--   0        0        0    10358 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/explore/graph_handler.py
+-rw-r--r--   0        0        0    10698 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/explore/metric_config_handler.py
+-rw-r--r--   0        0        0     2382 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/explore/metric_segments_handler.py
+-rw-r--r--   0        0        0     1553 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/explore/metric_type_handler.py
+-rw-r--r--   0        0        0    10285 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/explore/simple_segment_handler.py
+-rw-r--r--   0        0        0     4644 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/explore/toolbar_handler.py
+-rw-r--r--   0        0        0     1221 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/explore_project.py
+-rw-r--r--   0        0        0    13913 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/home.py
+-rw-r--r--   0        0        0     3947 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/login.py
+-rw-r--r--   0        0        0     9691 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/manage_connection.py
+-rw-r--r--   0        0        0     1288 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/manage_dashboard.py
+-rw-r--r--   0        0        0    10095 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/manage_event_defs.py
+-rw-r--r--   0        0        0    11804 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/manage_project.py
+-rw-r--r--   0        0        0     9470 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/manage_saved_metrics.py
+-rw-r--r--   0        0        0     1738 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/paths.py
+-rw-r--r--   0        0        0        0 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/projects/__init__.py
+-rw-r--r--   0        0        0    35398 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/projects/event_tables_config.py
+-rw-r--r--   0        0        0      587 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/projects/helper.py
+-rw-r--r--   0        0        0    19570 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/projects/manage_project_component.py
+-rw-r--r--   0        0        0     5090 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/projects_page.py
+-rw-r--r--   0        0        0     3114 2023-06-14 14:01:25.068494 mitzu-0.6.9/mitzu/webapp/pages/users.py
+-rw-r--r--   0        0        0        0 2023-06-14 14:01:25.072495 mitzu-0.6.9/mitzu/webapp/service/__init__.py
+-rw-r--r--   0        0        0     1955 2023-06-14 14:01:25.072495 mitzu-0.6.9/mitzu/webapp/service/events_service.py
+-rw-r--r--   0        0        0     4974 2023-06-14 14:01:25.072495 mitzu-0.6.9/mitzu/webapp/service/navbar_service.py
+-rw-r--r--   0        0        0      670 2023-06-14 14:01:25.072495 mitzu-0.6.9/mitzu/webapp/service/notification_service.py
+-rw-r--r--   0        0        0     1647 2023-06-14 14:01:25.072495 mitzu-0.6.9/mitzu/webapp/service/onboarding_service.py
+-rw-r--r--   0        0        0     2105 2023-06-14 14:01:25.072495 mitzu-0.6.9/mitzu/webapp/service/secret_service.py
+-rw-r--r--   0        0        0     6708 2023-06-14 14:01:25.072495 mitzu-0.6.9/mitzu/webapp/service/tracking_service.py
+-rw-r--r--   0        0        0     4756 2023-06-14 14:01:25.072495 mitzu-0.6.9/mitzu/webapp/service/user_service.py
+-rw-r--r--   0        0        0    25283 2023-06-14 14:01:25.072495 mitzu-0.6.9/mitzu/webapp/storage.py
+-rw-r--r--   0        0        0    25734 2023-06-14 14:01:25.072495 mitzu-0.6.9/mitzu/webapp/storage_model.py
+-rw-r--r--   0        0        0     4700 2023-06-14 14:01:25.072495 mitzu-0.6.9/mitzu/webapp/webapp.py
+-rw-r--r--   0        0        0     3422 2023-06-14 14:02:33.584490 mitzu-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 mitzu-0.6.9/PKG-INFO
```

### Comparing `mitzu-0.6.8/LICENSE.txt` & `mitzu-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/README.md` & `mitzu-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/.DS_Store` & `mitzu-0.6.9/mitzu/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/__init__.py` & `mitzu-0.6.9/mitzu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     TimeWindow,
     TimeGroup,
     DiscoverySettings,
     WebappSettings,
 )
 from mitzu.samples import get_sample_discovered_project
 
-__version__ = "0.6.8"
+__version__ = "0.6.9"
 
 
 __all__ = [
     "Connection",
     "ConnectionType",
     "Project",
     "EventDataTable",
```

### Comparing `mitzu-0.6.8/mitzu/adapters/adapter_factory.py` & `mitzu-0.6.9/mitzu/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/athena_adapter.py` & `mitzu-0.6.9/mitzu/adapters/athena_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/bigquery_adapter.py` & `mitzu-0.6.9/mitzu/adapters/bigquery_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/databricks_adapter.py` & `mitzu-0.6.9/mitzu/adapters/databricks_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/file_adapter.py` & `mitzu-0.6.9/mitzu/adapters/file_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/generic_adapter.py` & `mitzu-0.6.9/mitzu/adapters/generic_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/helper.py` & `mitzu-0.6.9/mitzu/adapters/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/mysql_adapter.py` & `mitzu-0.6.9/mitzu/adapters/mysql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/postgresql_adapter.py` & `mitzu-0.6.9/mitzu/adapters/postgresql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/redshift_adapter.py` & `mitzu-0.6.9/mitzu/adapters/redshift_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/snowflake_adapter.py` & `mitzu-0.6.9/mitzu/adapters/snowflake_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlalchemy_adapter.py` & `mitzu-0.6.9/mitzu/adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/sqlite_adapter.py` & `mitzu-0.6.9/mitzu/adapters/sqlite_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/adapters/trino_adapter.py` & `mitzu-0.6.9/mitzu/adapters/trino_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/helper.py` & `mitzu-0.6.9/mitzu/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/model.py` & `mitzu-0.6.9/mitzu/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -515,22 +515,22 @@
     def get_id(self) -> str:
         return self.id
 
 
 @dataclass(frozen=True)
 class DiscoverySettings:
     id: str = field(default_factory=helper.create_unique_id)
-    max_enum_cardinality: int = 300
+    max_enum_cardinality: int = 500
     max_map_key_cardinality: int = 1000
 
     end_dt: Optional[datetime] = None
     property_sample_rate: int = 0
 
-    lookback_days: int = 14
-    min_property_sample_size: int = 1000
+    lookback_days: int = 30
+    min_property_sample_size: int = 2000
 
 
 class WebappEndDateConfig(Enum):
     CUSTOM_DATE = auto()
     NOW = auto()
     START_OF_CURRENT_DAY = auto()
     END_OF_CURRENT_DAY = auto()
@@ -552,15 +552,15 @@
 
 
 @dataclass(frozen=True)
 class WebappSettings:
     id: str = field(default_factory=helper.create_unique_id)
     lookback_window: TimeWindow = TimeWindow(30, TimeGroup.DAY)
     auto_refresh_enabled: bool = True
-    end_date_config: WebappEndDateConfig = WebappEndDateConfig.START_OF_CURRENT_DAY
+    end_date_config: WebappEndDateConfig = WebappEndDateConfig.END_OF_CURRENT_DAY
     custom_end_date: Optional[datetime] = None
 
 
 class InvalidEventDataTableError(Exception):
     pass
```

### Comparing `mitzu-0.6.8/mitzu/notebook/model_loader.py` & `mitzu-0.6.9/mitzu/notebook/model_loader.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/project_discovery.py` & `mitzu-0.6.9/mitzu/project_discovery.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/project_serialization.py` & `mitzu-0.6.9/mitzu/project_serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/samples/__init__.py` & `mitzu-0.6.9/mitzu/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/samples/data_ingestion.py` & `mitzu-0.6.9/mitzu/samples/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/samples/sample_data_generator.py` & `mitzu-0.6.9/mitzu/samples/sample_data_generator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/serialization.py` & `mitzu-0.6.9/mitzu/serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/visualization/charts.py` & `mitzu-0.6.9/mitzu/visualization/charts.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/visualization/common.py` & `mitzu-0.6.9/mitzu/visualization/common.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/visualization/labels.py` & `mitzu-0.6.9/mitzu/visualization/labels.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/visualization/plot.py` & `mitzu-0.6.9/mitzu/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/visualization/titles.py` & `mitzu-0.6.9/mitzu/visualization/titles.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/visualization/tooltips.py` & `mitzu-0.6.9/mitzu/visualization/tooltips.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/visualization/transform_conv.py` & `mitzu-0.6.9/mitzu/visualization/transform_conv.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/visualization/transform_retention.py` & `mitzu-0.6.9/mitzu/visualization/transform_retention.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/.DS_Store` & `mitzu-0.6.9/mitzu/webapp/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/assets/explore_page.css` & `mitzu-0.6.9/mitzu/webapp/assets/explore_page.css`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/assets/favicon.ico` & `mitzu-0.6.9/mitzu/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/assets/logo.png` & `mitzu-0.6.9/mitzu/webapp/assets/logo.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/assets/mitzu-logo-light.svg` & `mitzu-0.6.9/mitzu/webapp/assets/mitzu-logo-light.svg`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/assets/warehouse/athena.png` & `mitzu-0.6.9/mitzu/webapp/assets/warehouse/athena.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/assets/warehouse/bigquery.png` & `mitzu-0.6.9/mitzu/webapp/assets/warehouse/bigquery.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/assets/warehouse/clickhouse.png` & `mitzu-0.6.9/mitzu/webapp/assets/warehouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/assets/warehouse/databricks.png` & `mitzu-0.6.9/mitzu/webapp/assets/warehouse/databricks.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/assets/warehouse/mysql.png` & `mitzu-0.6.9/mitzu/webapp/assets/warehouse/mysql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/assets/warehouse/pandas.png` & `mitzu-0.6.9/mitzu/webapp/assets/warehouse/pandas.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/assets/warehouse/postgresql.png` & `mitzu-0.6.9/mitzu/webapp/assets/warehouse/postgresql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/assets/warehouse/redshift.png` & `mitzu-0.6.9/mitzu/webapp/assets/warehouse/redshift.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/assets/warehouse/snowflake.png` & `mitzu-0.6.9/mitzu/webapp/assets/warehouse/snowflake.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/assets/warehouse/sqlite.png` & `mitzu-0.6.9/mitzu/webapp/assets/warehouse/sqlite.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/assets/warehouse/trino.png` & `mitzu-0.6.9/mitzu/webapp/assets/warehouse/trino.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/auth/authorizer.py` & `mitzu-0.6.9/mitzu/webapp/auth/authorizer.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/auth/cognito.py` & `mitzu-0.6.9/mitzu/webapp/auth/cognito.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/auth/decorator.py` & `mitzu-0.6.9/mitzu/webapp/auth/decorator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/auth/google.py` & `mitzu-0.6.9/mitzu/webapp/auth/google.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/cache.py` & `mitzu-0.6.9/mitzu/webapp/cache.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/caching_dataset_adapter.py` & `mitzu-0.6.9/mitzu/webapp/caching_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/configs.py` & `mitzu-0.6.9/mitzu/webapp/configs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/dependencies.py` & `mitzu-0.6.9/mitzu/webapp/dependencies.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/helper.py` & `mitzu-0.6.9/mitzu/webapp/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/model.py` & `mitzu-0.6.9/mitzu/webapp/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/offcanvas.py` & `mitzu-0.6.9/mitzu/webapp/offcanvas.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/onboarding_flow.py` & `mitzu-0.6.9/mitzu/webapp/onboarding_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import List
 from dataclasses import dataclass
 
 import mitzu.webapp.storage as S
 
 
 @dataclass(frozen=True)
```

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/connections_page.py` & `mitzu-0.6.9/mitzu/webapp/pages/connections_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/dashboards/manage_dashboards_component.py` & `mitzu-0.6.9/mitzu/webapp/pages/dashboards/manage_dashboards_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/dashboards_page.py` & `mitzu-0.6.9/mitzu/webapp/pages/dashboards_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/edit_user.py` & `mitzu-0.6.9/mitzu/webapp/pages/edit_user.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/explore/complex_segment_handler.py` & `mitzu-0.6.9/mitzu/webapp/pages/explore/complex_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/explore/dates_selector_handler.py` & `mitzu-0.6.9/mitzu/webapp/pages/explore/dates_selector_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/explore/event_segment_handler.py` & `mitzu-0.6.9/mitzu/webapp/pages/explore/event_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/explore/explore_page.py` & `mitzu-0.6.9/mitzu/webapp/pages/explore/explore_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/explore/graph_handler.py` & `mitzu-0.6.9/mitzu/webapp/pages/explore/graph_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/explore/metric_config_handler.py` & `mitzu-0.6.9/mitzu/webapp/pages/explore/metric_config_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/explore/metric_segments_handler.py` & `mitzu-0.6.9/mitzu/webapp/pages/explore/metric_segments_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/explore/metric_type_handler.py` & `mitzu-0.6.9/mitzu/webapp/pages/explore/metric_type_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/explore/simple_segment_handler.py` & `mitzu-0.6.9/mitzu/webapp/pages/explore/simple_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/explore/toolbar_handler.py` & `mitzu-0.6.9/mitzu/webapp/pages/explore/toolbar_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/explore_project.py` & `mitzu-0.6.9/mitzu/webapp/pages/explore_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/home.py` & `mitzu-0.6.9/mitzu/webapp/pages/home.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,16 +96,15 @@
                                 children=[
                                     dmc.StepperStep(
                                         label="Connect your data warehouse",
                                         children=[
                                             dbc.Row(
                                                 [
                                                     onboarding_step_description_row(
-                                                        """Create a new project and connect your data warehouse to Mitzu. 
-                                                        This should take no more than 5 minutes. 
+                                                        """Create a new project and connect your data warehouse to Mitzu.                                                     
                                                         If you don't have a data warehouse yet you can also explore our sample one.
                                                         """,
                                                     ),
                                                 ],
                                                 class_name="mt-3",
                                                 justify="center",
                                             ),
```

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/login.py` & `mitzu-0.6.9/mitzu/webapp/pages/login.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/manage_dashboard.py` & `mitzu-0.6.9/mitzu/webapp/pages/manage_dashboard.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/manage_event_defs.py` & `mitzu-0.6.9/mitzu/webapp/pages/manage_event_defs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/manage_project.py` & `mitzu-0.6.9/mitzu/webapp/pages/manage_project.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,27 +150,16 @@
 
     return html.Div(
         [
             NB.create_mitzu_navbar("create-project-navbar"),
             dbc.Container(
                 children=[
                     dcc.Location(id=PROJECT_LOCATION),
-                    dbc.Row(
-                        [
-                            dbc.Col(
-                                html.H4(
-                                    title, id=PROJECT_TITLE, className="card-title"
-                                ),
-                                width="auto",
-                            )
-                        ]
-                    ),
-                    html.Hr(),
+                    html.Div(title, id=PROJECT_TITLE, className="lead"),
                     MPC.create_project_settings(project, dependencies, **query_params),
-                    html.Hr(),
                     dbc.Button(
                         [html.B(className="bi bi-check-circle"), " Save"],
                         color="success",
                         id=SAVE_BUTTON,
                         class_name="d-inline-block me-3 mb-1",
                         size="sm",
                     ),
@@ -185,15 +174,14 @@
                         class_name="d-inline-block me-3 mb-1",
                     ),
                     html.Div(
                         children="",
                         className="mb-3 lead",
                         id=MANAGE_PROJECT_INFO,
                     ),
-                    html.Hr(),
                     create_delete_button(project),
                     create_confirm_dialog(project),
                 ],
                 class_name="mb-3",
             ),
         ]
     )
@@ -279,19 +267,25 @@
             id_val = prop["id"]
             if id_val.get("type") == MPH.PROJECT_INDEX_TYPE:
                 project_props[id_val.get("index")] = prop["value"]
 
         project_id = cast(str, project_props.get(MPC.PROP_PROJECT_ID))
         project_name = cast(str, project_props.get(MPC.PROP_PROJECT_NAME))
         if not project_name:
-            return html.P("Please name your project first!", className="text-danger")
+            return (
+                html.P("Please name your project!", className="text-danger"),
+                no_update,
+            )
 
         connection_id = cast(str, project_props.get(MPC.PROP_CONNECTION))
         if connection_id is None:
-            return html.P("Please select a connection first!", className="text-danger")
+            return (
+                html.P("Please select or add connection!", className="text-danger"),
+                no_update,
+            )
 
         description = cast(str, project_props.get(MPC.PROP_DESCRIPTION))
         disc_lookback_days = cast(int, project_props.get(MPC.PROP_DISC_LOOKBACK_DAYS))
         min_sample_size = cast(int, project_props.get(MPC.PROP_DISC_SAMPLE_SIZE))
         autorefresh_enabled = cast(
             bool, project_props.get(MPC.PROP_EXPLORE_AUTO_REFRESH)
         )
@@ -337,26 +331,27 @@
         storage.set_project(project_id, project)
         tracking_service.track_project_saved(project)
         onboarding_service.mark_state_complete(
             OF.ConfigureMitzuOnboardingFlow.flow_id(),
             OF.CONNECT_WAREHOUSE,
         )
         if ctx.triggered_id == SAVE_BUTTON:
-            return ["Project succesfully saved", no_update]
+            return ("Project succesfully saved", no_update)
         else:
-            return [
+            return (
                 no_update,
                 P.create_path(
                     P.EVENTS_AND_PROPERTIES_PROJECT_PATH,
                     project_id=project_id,
                 ),
-            ]
+            )
     except Exception as exc:
+
         traceback.print_exc()
-        return [f"Something went wrong: {str(exc)}", no_update]
+        return (f"Something went wrong: {str(exc)}", no_update)
 
 
 register_page(
     __name__ + "_create",
     path=P.PROJECTS_CREATE_PATH,
     title="Mitzu - Create Project",
     layout=layout_create,
```

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/manage_saved_metrics.py` & `mitzu-0.6.9/mitzu/webapp/pages/manage_saved_metrics.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/paths.py` & `mitzu-0.6.9/mitzu/webapp/pages/paths.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/projects/event_tables_config.py` & `mitzu-0.6.9/mitzu/webapp/pages/projects/event_tables_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,30 +345,20 @@
 
 def create_event_tables(project: Optional[M.Project]) -> bc.Component:
     table = create_table_component(project)
     add_tables_modal = create_add_tables_modal()
     configure_tables_modal = create_configure_tables_modal()
     return html.Div(
         [
-            html.P(
-                children=[
-                    html.I(className="bi bi-info-circle me-1"),
-                    """Event tables are tables in the data warehouse that contain user events. 
-                The user id and event time columns are mandatory for the event tables. 
-                The event name column is optional and reserved for 
-                data warehouse tables that contain multiple event types.""",
-                ],
-                className="mb-3 lead",
-            ),
             dbc.Row(
                 [
                     dbc.Col(
                         dbc.Button(
                             [html.B(className="bi bi-plus-circle me-1"), "Add tables"],
-                            color="primary",
+                            color="secondary",
                             id=ADD_TABLES_BUTTON,
                             size="sm",
                         ),
                         width="auto",
                         class_name="mb-3",
                     ),
                     dbc.Col(
@@ -390,46 +380,49 @@
                             id=REMOVE_TABLES_BUTTON,
                             size="sm",
                         ),
                         class_name="mb-3",
                         width="auto",
                     ),
                     dbc.Col(
+                        dbc.Button(
+                            [
+                                html.B(className="bi bi-arrow-clockwise me-1"),
+                                "Validate",
+                            ],
+                            id=EDT_VALIDATE_BUTTON,
+                            color="secondary",
+                            size="sm",
+                            className="me-3 d-inline-block",
+                        ),
+                        class_name="mb-3",
+                        width="auto",
+                    ),
+                    dbc.Col(
                         dbc.Input(
                             id=TBL_SEARCH_INPUT,
                             placeholder="Search tables",
                             size="sm",
                         ),
                         class_name="ms-auto mb-3",
                         width="3",
                     ),
                 ],
                 class_name="me-auto",
             ),
             table,
-            html.Hr(),
-            dbc.Button(
-                [
-                    html.B(className="bi bi-check-circle me-1"),
-                    "Validate",
-                ],
-                id=EDT_VALIDATE_BUTTON,
-                color="primary",
-                size="sm",
-                className="me-3 d-inline-block shadow-sm mb-3",
-            ),
             html.Div(
                 children=[],
                 id=TBL_PROGRESS_INFO,
                 className="lead d-inline-block mb-3",
             ),
             add_tables_modal,
             configure_tables_modal,
         ],
-        className="overflow-auto mh-100 mt-3",
+        className="overflow-auto mh-100",
     )
 
 
 def get_checkbox_value_from_row(tr: html.Tr) -> bool:
     return (
         tr.get("props")
         .get("children")[0]
```

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/projects/helper.py` & `mitzu-0.6.9/mitzu/webapp/pages/projects/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/projects_page.py` & `mitzu-0.6.9/mitzu/webapp/pages/projects_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/pages/users.py` & `mitzu-0.6.9/mitzu/webapp/pages/users.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/service/events_service.py` & `mitzu-0.6.9/mitzu/webapp/service/events_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/service/navbar_service.py` & `mitzu-0.6.9/mitzu/webapp/service/navbar_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/service/notification_service.py` & `mitzu-0.6.9/mitzu/webapp/service/notification_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/service/onboarding_service.py` & `mitzu-0.6.9/mitzu/webapp/service/onboarding_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/service/secret_service.py` & `mitzu-0.6.9/mitzu/webapp/service/secret_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/service/tracking_service.py` & `mitzu-0.6.9/mitzu/webapp/service/tracking_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/service/user_service.py` & `mitzu-0.6.9/mitzu/webapp/service/user_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/storage.py` & `mitzu-0.6.9/mitzu/webapp/storage.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/storage_model.py` & `mitzu-0.6.9/mitzu/webapp/storage_model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/mitzu/webapp/webapp.py` & `mitzu-0.6.9/mitzu/webapp/webapp.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.8/pyproject.toml` & `mitzu-0.6.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mitzu"
-version = "0.6.8"
+version = "0.6.9"
 description = "Product analytics over your data warehouse"
 authors = ["Istvan Meszaros <istvan.meszaros.88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mitzu.io"
 repository = "https://github.com/mitzu-io/mitzu"
 documentation = "https://mitzu.io/documentation/"
```

### Comparing `mitzu-0.6.8/PKG-INFO` & `mitzu-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitzu
-Version: 0.6.8
+Version: 0.6.9
 Summary: Product analytics over your data warehouse
 Home-page: https://mitzu.io
 License: MIT
 Author: Istvan Meszaros
 Author-email: istvan.meszaros.88@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

