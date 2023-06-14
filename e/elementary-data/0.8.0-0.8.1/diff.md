# Comparing `tmp/elementary-data-0.8.0.tar.gz` & `tmp/elementary-data-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/elementary/elementary/dist/.tmp-y9leu538/elementary-data-0.8.0.tar", last modified: Wed May 31 20:23:43 2023, max compression
+gzip compressed data, was "/home/runner/work/elementary/elementary/dist/.tmp-9g4itmg2/elementary-data-0.8.1.tar", last modified: Wed Jun 14 16:47:58 2023, max compression
```

## Comparing `elementary-data-0.8.0.tar` & `elementary-data-0.8.1.tar`

### file list

```diff
@@ -1,297 +1,297 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-05-31 20:23:30.000000 elementary-data-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-31 20:23:30.000000 elementary-data-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14706 2023-05-31 20:23:43.000000 elementary-data-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13827 2023-05-31 20:23:30.000000 elementary-data-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/cli/upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/clients/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/clients/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/clients/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/clients/api/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/clients/dbt/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/clients/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/clients/dbt/base_dbt_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/clients/dbt/dbt_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     6428 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/clients/dbt/slim_dbt_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/clients/fetcher/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/clients/fetcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/clients/fetcher/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/clients/gcs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/clients/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3765 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/clients/gcs/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/clients/s3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/clients/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5360 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/clients/s3/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/clients/slack/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/clients/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8090 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/clients/slack/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/clients/slack/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     5714 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/clients/slack/slack_message_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/config/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8178 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4228 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7433 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/alerts/alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/alerts/alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)    13418 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/alerts/group_of_alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/alerts/malformed.py
--rw-r--r--   0 runner    (1001) docker     (122)     7697 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/alerts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/alerts/schema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/alerts/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/alerts/schema/alert.py
--rw-r--r--   0 runner    (1001) docker     (122)      418 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/alerts/schema/alert_group_component.py
--rw-r--r--   0 runner    (1001) docker     (122)      487 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/alerts/schema/test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6411 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/alerts/source_freshness.py
--rw-r--r--   0 runner    (1001) docker     (122)    16207 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/alerts/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4147 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/alerts/alert_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     8053 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/alerts/alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/api/filters/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4211 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/filters/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)      539 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/filters/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/api/invocations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/invocations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/invocations/invocations.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/invocations/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/api/lineage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/lineage/lineage.py
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/lineage/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/api/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9290 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/models/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/models/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/api/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7289 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/report/report.py
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/report/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/api/selector/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/selector/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/selector/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/api/sidebar/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/sidebar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/sidebar/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     3417 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/sidebar/sidebar.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/api/test_management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/test_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/test_management/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     1453 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/test_management/test_management.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3882 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)    19819 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/api/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)    19321 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/data_monitoring/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/data_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6583 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/data_monitoring/data_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    10398 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/data_monitoring/data_monitoring_alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/data_monitoring/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/data_monitoring/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11829 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/data_monitoring/report/data_monitoring_report.py
--rw-r--r--   0 runner    (1001) docker     (122)  1751556 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/data_monitoring/report/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     7918 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1718 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/data_monitoring/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     4355 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/data_monitoring/selector_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql
--rw-r--r--   0 runner    (1001) docker     (122)     6956 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql
--rw-r--r--   0 runner    (1001) docker     (122)     6387 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)     7562 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      611 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/base_queries/
--rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql
--rw-r--r--   0 runner    (1001) docker     (122)      827 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/base_queries/owners.sql
--rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/base_queries/resources.sql
--rw-r--r--   0 runner    (1001) docker     (122)      649 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/base_queries/tags.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/base_queries/tests.sql
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_adapter_type_and_unique_id.sql
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_alerts_time_limit.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_elementary_database_and_schema.sql
--rw-r--r--   0 runner    (1001) docker     (122)      324 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_elementary_table_nodes.sql
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_exposures.sql
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_invocations_by_ids.sql
--rw-r--r--   0 runner    (1001) docker     (122)      678 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_latest_invocation.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_models.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_models_runs.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_resources_latest_invocation.sql
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_result_rows_agate.sql
--rw-r--r--   0 runner    (1001) docker     (122)      991 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_sources.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql
--rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_test_results.sql
--rw-r--r--   0 runner    (1001) docker     (122)      683 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/internal_tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/internal_tests/validate_alert_statuses_are_updated.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (122)      494 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/materializations/nothing.sql
--rw-r--r--   0 runner    (1001) docker     (122)      927 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/test_conn.sql
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/macros/upload_source_freshness.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/models/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/models/alerts/alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/models/alerts/alerts_models.sql
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/models/update_alerts/
--rw-r--r--   0 runner    (1001) docker     (122)      300 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/models/update_alerts/update_sent_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/models/update_alerts/update_skipped_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/packages.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/dbt_project_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/fetchers/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6201 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/alerts/alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)     5173 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/alerts/normalized_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/base_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/fetchers/invocations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/invocations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/invocations/invocations.py
--rw-r--r--   0 runner    (1001) docker     (122)      906 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/invocations/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/fetchers/lineage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/lineage/lineage.py
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/lineage/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/fetchers/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/models/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2446 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/models/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/fetchers/selector/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/selector/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/selector/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/fetchers/test_management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/test_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1992 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/test_management/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     6808 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/test_management/test_management.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/monitor/fetchers/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/monitor/fetchers/tests/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/operations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/operations/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     2496 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/operations/upload_source_freshness.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/tracking/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6243 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/tracking/anonymous_tracking.py
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/tracking/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/tracking/tracking_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/utils/bucket_path.py
--rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/utils/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/utils/env_vars.py
--rw-r--r--   0 runner    (1001) docker     (122)     2281 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (122)      201 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/utils/ordered_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)      527 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/utils/package.py
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-05-31 20:23:30.000000 elementary-data-0.8.0/elementary/utils/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14706 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10322 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-31 20:23:43.000000 elementary-data-0.8.0/elementary_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 20:23:43.000000 elementary-data-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-05-31 20:23:30.000000 elementary-data-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/integration/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/integration/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/integration/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/integration/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/integration/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/integration/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/integration/monitor/api/alerts/test_alerts_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/integration/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/integration/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/integration/monitor/api/tests/test_tests_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/mocks/anonymous_tracking_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/mocks/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/mocks/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/mocks/api/alerts_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/mocks/api/invocations_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      784 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/mocks/api/tests_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/mocks/dbt_runner_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/mocks/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/mocks/fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19060 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/mocks/fetchers/alerts_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/mocks/fetchers/invocations_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/mocks/fetchers/selector_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/mocks/fetchers/tests_fetcher_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/unit/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/unit/monitor/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/alerts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/unit/monitor/alerts/group_alerts_by_table/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/alerts/group_alerts_by_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3180 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    12236 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/alerts/group_alerts_by_table/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      927 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/alerts/test_malformed_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     7565 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/alerts/test_normalized_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     7348 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/alerts/test_slack_alert_message_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/unit/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/unit/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12260 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/api/alerts/test_alert_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1919 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/api/alerts/test_alerts_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/unit/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/api/tests/test_tests_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/unit/monitor/data_monitoring/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/data_monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/unit/monitor/data_monitoring/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/data_monitoring/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7894 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     5152 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/data_monitoring/test_selector_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:43.000000 elementary-data-0.8.0/tests/unit/monitor/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2536 2023-05-31 20:23:30.000000 elementary-data-0.8.0/tests/unit/monitor/fetchers/test_alerts_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-06-14 16:47:44.000000 elementary-data-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-14 16:47:44.000000 elementary-data-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    14706 2023-06-14 16:47:58.000000 elementary-data-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13827 2023-06-14 16:47:44.000000 elementary-data-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/cli/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/clients/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/clients/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/clients/api/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/clients/dbt/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/clients/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/clients/dbt/base_dbt_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/clients/dbt/dbt_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6428 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/clients/dbt/slim_dbt_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/clients/fetcher/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/clients/fetcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/clients/fetcher/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/clients/gcs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/clients/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3765 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/clients/gcs/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/clients/s3/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/clients/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5360 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/clients/s3/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/clients/slack/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/clients/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8090 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/clients/slack/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/clients/slack/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5714 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/clients/slack/slack_message_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/config/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8178 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4228 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7443 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/alerts/alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/alerts/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13418 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/alerts/group_of_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/alerts/malformed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7697 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/alerts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/alerts/schema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/alerts/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/alerts/schema/alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      418 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/alerts/schema/alert_group_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)      487 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/alerts/schema/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6411 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/alerts/source_freshness.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16207 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/alerts/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4147 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/alerts/alert_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8053 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/alerts/alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/api/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4211 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/filters/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      539 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/filters/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/api/invocations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/invocations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/invocations/invocations.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/invocations/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/api/lineage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/lineage/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/lineage/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/api/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9290 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/models/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/api/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7289 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/report/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/api/selector/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/selector/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/selector/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/api/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/sidebar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/sidebar/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3417 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/sidebar/sidebar.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/api/test_management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/test_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/test_management/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1453 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/test_management/test_management.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3882 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19819 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/api/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19321 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/data_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/data_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6583 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/data_monitoring/data_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10398 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/data_monitoring/data_monitoring_alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/data_monitoring/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/data_monitoring/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11829 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/data_monitoring/report/data_monitoring_report.py
+-rw-r--r--   0 runner    (1001) docker     (122)  1751556 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/data_monitoring/report/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     7918 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1718 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/data_monitoring/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4355 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/data_monitoring/selector_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     6956 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     6387 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     7562 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/base_queries/
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/base_queries/owners.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/base_queries/resources.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      649 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/base_queries/tags.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/base_queries/tests.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_adapter_type_and_unique_id.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_alerts_time_limit.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_elementary_database_and_schema.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_elementary_table_nodes.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_exposures.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_invocations_by_ids.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_latest_invocation.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_models.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_models_runs.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_resources_latest_invocation.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_result_rows_agate.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      991 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_sources.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_test_results.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      683 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/internal_tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/internal_tests/validate_alert_statuses_are_updated.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      494 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/materializations/nothing.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      927 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/test_conn.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/macros/upload_source_freshness.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/models/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/models/alerts/alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/models/alerts/alerts_models.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/models/update_alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)      300 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/models/update_alerts/update_sent_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/models/update_alerts/update_skipped_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/packages.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/dbt_project_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/fetchers/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6201 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/alerts/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5167 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/alerts/normalized_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/base_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/fetchers/invocations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/invocations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/invocations/invocations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      906 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/invocations/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/fetchers/lineage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/lineage/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/lineage/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/fetchers/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2446 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/models/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/fetchers/selector/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/selector/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/selector/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/fetchers/test_management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/test_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1992 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/test_management/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6808 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/test_management/test_management.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/monitor/fetchers/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/monitor/fetchers/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/operations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/operations/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2496 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/operations/upload_source_freshness.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/tracking/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6243 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/tracking/anonymous_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/tracking/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/tracking/tracking_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/utils/bucket_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/utils/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/utils/env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2281 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/utils/ordered_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)      527 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/utils/package.py
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-06-14 16:47:44.000000 elementary-data-0.8.1/elementary/utils/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14706 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10322 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-14 16:47:58.000000 elementary-data-0.8.1/elementary_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-14 16:47:58.000000 elementary-data-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-06-14 16:47:44.000000 elementary-data-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/integration/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/integration/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/integration/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/integration/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/integration/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/integration/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/integration/monitor/api/alerts/test_alerts_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/integration/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/integration/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/integration/monitor/api/tests/test_tests_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/mocks/anonymous_tracking_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/mocks/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/mocks/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/mocks/api/alerts_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/mocks/api/invocations_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/mocks/api/tests_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/mocks/dbt_runner_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/mocks/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/mocks/fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19060 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/mocks/fetchers/alerts_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/mocks/fetchers/invocations_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/mocks/fetchers/selector_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/mocks/fetchers/tests_fetcher_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/unit/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/unit/monitor/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/alerts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/unit/monitor/alerts/group_alerts_by_table/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/alerts/group_alerts_by_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3180 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12236 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/alerts/group_alerts_by_table/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      927 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/alerts/test_malformed_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/alerts/test_normalized_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7348 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/alerts/test_slack_alert_message_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/unit/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/unit/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12260 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/api/alerts/test_alert_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1919 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/api/alerts/test_alerts_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/unit/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/api/tests/test_tests_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/unit/monitor/data_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/data_monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/unit/monitor/data_monitoring/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/data_monitoring/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7894 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5152 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/data_monitoring/test_selector_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:58.000000 elementary-data-0.8.1/tests/unit/monitor/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2536 2023-06-14 16:47:44.000000 elementary-data-0.8.1/tests/unit/monitor/fetchers/test_alerts_fetcher.py
```

### Comparing `elementary-data-0.8.0/LICENSE` & `elementary-data-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/PKG-INFO` & `elementary-data-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementary-data
-Version: 0.8.0
+Version: 0.8.1
 Summary: Data monitoring and lineage
 Home-page: https://github.com/elementary-data/elementary
 Author: Elementary
 Author-email: or@elementary-data.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: elementary-data Version: 0.8.0 Summary: Data
+Metadata-Version: 2.1 Name: elementary-data Version: 0.8.1 Summary: Data
 monitoring and lineage Home-page: https://github.com/elementary-data/elementary
 Author: Elementary Author-email: or@elementary-data.com Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `elementary-data-0.8.0/README.md` & `elementary-data-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/cli/cli.py` & `elementary-data-0.8.1/elementary/cli/cli.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/cli/upgrade.py` & `elementary-data-0.8.1/elementary/cli/upgrade.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/clients/dbt/base_dbt_runner.py` & `elementary-data-0.8.1/elementary/clients/dbt/base_dbt_runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/clients/dbt/dbt_runner.py` & `elementary-data-0.8.1/elementary/clients/dbt/dbt_runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/clients/dbt/slim_dbt_runner.py` & `elementary-data-0.8.1/elementary/clients/dbt/slim_dbt_runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/clients/gcs/client.py` & `elementary-data-0.8.1/elementary/clients/gcs/client.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/clients/s3/client.py` & `elementary-data-0.8.1/elementary/clients/s3/client.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/clients/slack/client.py` & `elementary-data-0.8.1/elementary/clients/slack/client.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/clients/slack/schema.py` & `elementary-data-0.8.1/elementary/clients/slack/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/clients/slack/slack_message_builder.py` & `elementary-data-0.8.1/elementary/clients/slack/slack_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/config/config.py` & `elementary-data-0.8.1/elementary/config/config.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/exceptions/exceptions.py` & `elementary-data-0.8.1/elementary/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/alerts/alert.py` & `elementary-data-0.8.1/elementary/monitor/alerts/alert.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         tags: Optional[List[str]] = None,
         status: Optional[str] = None,
         subscribers: Optional[List[str]] = None,
         slack_channel: Optional[str] = None,
         alert_suppression_interval: int = 0,
         alert_fields: Optional[list] = None,
         timezone: Optional[str] = None,
-        meta: Optional[dict] = None,
+        test_meta: Optional[dict] = None,
         model_meta: Optional[str] = None,
         alerts_table: Optional[str] = None,
         slack_group_alerts_by: Optional[str] = None,
         **kwargs,
     ):
         self.slack_message_builder = SlackAlertMessageBuilder()
         self.id = id
@@ -57,15 +57,15 @@
                 )
             except Exception:
                 logger.error('Failed to parse "detected_at" field.')
         self.database_name = database_name
         self.schema_name = schema_name
         self.owners = owners
         self.tags = tags
-        self.meta = meta
+        self.meta = test_meta
         self.model_meta = try_load_json(model_meta) or {}
         self.status = status
         self.subscribers = subscribers
         self.slack_channel = slack_channel
         self.alert_suppression_interval = alert_suppression_interval
         self.alert_fields = alert_fields
         self.slack_group_alerts_by = slack_group_alerts_by
```

### Comparing `elementary-data-0.8.0/elementary/monitor/alerts/alerts.py` & `elementary-data-0.8.1/elementary/monitor/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/alerts/group_of_alerts.py` & `elementary-data-0.8.1/elementary/monitor/alerts/group_of_alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/alerts/malformed.py` & `elementary-data-0.8.1/elementary/monitor/alerts/malformed.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/alerts/model.py` & `elementary-data-0.8.1/elementary/monitor/alerts/model.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/alerts/source_freshness.py` & `elementary-data-0.8.1/elementary/monitor/alerts/source_freshness.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/alerts/test.py` & `elementary-data-0.8.1/elementary/monitor/alerts/test.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/api/alerts/alert_filters.py` & `elementary-data-0.8.1/elementary/monitor/api/alerts/alert_filters.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/api/alerts/alerts.py` & `elementary-data-0.8.1/elementary/monitor/api/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/api/filters/filters.py` & `elementary-data-0.8.1/elementary/monitor/api/filters/filters.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/api/filters/schema.py` & `elementary-data-0.8.1/elementary/monitor/api/filters/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/api/invocations/invocations.py` & `elementary-data-0.8.1/elementary/monitor/api/invocations/invocations.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/api/lineage/lineage.py` & `elementary-data-0.8.1/elementary/monitor/api/lineage/lineage.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/api/lineage/schema.py` & `elementary-data-0.8.1/elementary/monitor/api/lineage/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/api/models/models.py` & `elementary-data-0.8.1/elementary/monitor/api/models/models.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/api/models/schema.py` & `elementary-data-0.8.1/elementary/monitor/api/models/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/api/report/report.py` & `elementary-data-0.8.1/elementary/monitor/api/report/report.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/api/report/schema.py` & `elementary-data-0.8.1/elementary/monitor/api/report/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/api/selector/selector.py` & `elementary-data-0.8.1/elementary/monitor/api/selector/selector.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/api/sidebar/sidebar.py` & `elementary-data-0.8.1/elementary/monitor/api/sidebar/sidebar.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/api/test_management/test_management.py` & `elementary-data-0.8.1/elementary/monitor/api/test_management/test_management.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/api/tests/schema.py` & `elementary-data-0.8.1/elementary/monitor/api/tests/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/api/tests/tests.py` & `elementary-data-0.8.1/elementary/monitor/api/tests/tests.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/cli.py` & `elementary-data-0.8.1/elementary/monitor/cli.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/data_monitoring/data_monitoring.py` & `elementary-data-0.8.1/elementary/monitor/data_monitoring/data_monitoring.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/data_monitoring/data_monitoring_alerts.py` & `elementary-data-0.8.1/elementary/monitor/data_monitoring/data_monitoring_alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/data_monitoring/report/data_monitoring_report.py` & `elementary-data-0.8.1/elementary/monitor/data_monitoring/report/data_monitoring_report.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/data_monitoring/report/index.html` & `elementary-data-0.8.1/elementary/monitor/data_monitoring/report/index.html`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py` & `elementary-data-0.8.1/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/data_monitoring/schema.py` & `elementary-data-0.8.1/elementary/monitor/data_monitoring/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/data_monitoring/selector_filter.py` & `elementary-data-0.8.1/elementary/monitor/data_monitoring/selector_filter.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/README.md` & `elementary-data-0.8.1/elementary/monitor/dbt_project/README.md`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/dbt_project.yml` & `elementary-data-0.8.1/elementary/monitor/dbt_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/base_queries/owners.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/base_queries/owners.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/base_queries/resources.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/base_queries/resources.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/base_queries/tags.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/base_queries/tags.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/base_queries/tests.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/base_queries/tests.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_exposures.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_exposures.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_invocations_by_ids.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_invocations_by_ids.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_latest_invocation.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_latest_invocation.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_models.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_models.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_models_runs.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_models_runs.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_resources_latest_invocation.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_resources_latest_invocation.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_sources.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_sources.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_test_results.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_test_results.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/internal_tests/validate_alert_statuses_are_updated.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/internal_tests/validate_alert_statuses_are_updated.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/materializations/incremental.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/macros/materializations/table.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/models/alerts/alerts.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/models/alerts/alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/models/alerts/alerts_models.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/models/alerts/alerts_models.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql` & `elementary-data-0.8.1/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/dbt_project_utils.py` & `elementary-data-0.8.1/elementary/monitor/dbt_project_utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/debug.py` & `elementary-data-0.8.1/elementary/monitor/debug.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/fetchers/alerts/alerts.py` & `elementary-data-0.8.1/elementary/monitor/fetchers/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/fetchers/alerts/normalized_alert.py` & `elementary-data-0.8.1/elementary/monitor/fetchers/alerts/normalized_alert.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             ] = unpack_and_flatten_and_dedup_list_of_strings(
                 self._get_alert_meta_attrs(SUBSCRIBERS_KEY)
             )
             normalized_alert[OWNERS_KEY] = unpack_and_flatten_and_dedup_list_of_strings(
                 self._get_alert_meta_attrs("owner")
             )
             normalized_alert[TAGS_FIELD] = unpack_and_flatten_and_dedup_list_of_strings(
-                self._get_alert_meta_attrs(TAGS_FIELD)
+                normalized_alert.get(TAGS_FIELD)
             )
 
             normalized_alert["slack_channel"] = self._get_alert_channel()
             normalized_alert[
                 ALERT_SUPRESSION_INTERVAL_KEY
             ] = self._get_alert_suppression_interval()
             normalized_alert[ALERT_FIELDS_KEY] = self._get_alert_fields()
```

### Comparing `elementary-data-0.8.0/elementary/monitor/fetchers/invocations/invocations.py` & `elementary-data-0.8.1/elementary/monitor/fetchers/invocations/invocations.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/fetchers/invocations/schema.py` & `elementary-data-0.8.1/elementary/monitor/fetchers/invocations/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/fetchers/lineage/lineage.py` & `elementary-data-0.8.1/elementary/monitor/fetchers/lineage/lineage.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/fetchers/lineage/schema.py` & `elementary-data-0.8.1/elementary/monitor/fetchers/lineage/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/fetchers/models/models.py` & `elementary-data-0.8.1/elementary/monitor/fetchers/models/models.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/fetchers/models/schema.py` & `elementary-data-0.8.1/elementary/monitor/fetchers/models/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/fetchers/test_management/schema.py` & `elementary-data-0.8.1/elementary/monitor/fetchers/test_management/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/fetchers/test_management/test_management.py` & `elementary-data-0.8.1/elementary/monitor/fetchers/test_management/test_management.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/fetchers/tests/schema.py` & `elementary-data-0.8.1/elementary/monitor/fetchers/tests/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/monitor/fetchers/tests/tests.py` & `elementary-data-0.8.1/elementary/monitor/fetchers/tests/tests.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/operations/cli.py` & `elementary-data-0.8.1/elementary/operations/cli.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/operations/upload_source_freshness.py` & `elementary-data-0.8.1/elementary/operations/upload_source_freshness.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/tracking/anonymous_tracking.py` & `elementary-data-0.8.1/elementary/tracking/anonymous_tracking.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/tracking/runner.py` & `elementary-data-0.8.1/elementary/tracking/runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/tracking/tracking_interface.py` & `elementary-data-0.8.1/elementary/tracking/tracking_interface.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/utils/cli_utils.py` & `elementary-data-0.8.1/elementary/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/utils/json_utils.py` & `elementary-data-0.8.1/elementary/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/utils/log.py` & `elementary-data-0.8.1/elementary/utils/log.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/utils/ordered_yaml.py` & `elementary-data-0.8.1/elementary/utils/ordered_yaml.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/utils/package.py` & `elementary-data-0.8.1/elementary/utils/package.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/utils/schema.py` & `elementary-data-0.8.1/elementary/utils/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary/utils/time.py` & `elementary-data-0.8.1/elementary/utils/time.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary_data.egg-info/PKG-INFO` & `elementary-data-0.8.1/elementary_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementary-data
-Version: 0.8.0
+Version: 0.8.1
 Summary: Data monitoring and lineage
 Home-page: https://github.com/elementary-data/elementary
 Author: Elementary
 Author-email: or@elementary-data.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: elementary-data Version: 0.8.0 Summary: Data
+Metadata-Version: 2.1 Name: elementary-data Version: 0.8.1 Summary: Data
 monitoring and lineage Home-page: https://github.com/elementary-data/elementary
 Author: Elementary Author-email: or@elementary-data.com Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `elementary-data-0.8.0/elementary_data.egg-info/SOURCES.txt` & `elementary-data-0.8.1/elementary_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/elementary_data.egg-info/requires.txt` & `elementary-data-0.8.1/elementary_data.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/setup.py` & `elementary-data-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "spark": ["dbt-spark>=0.20,<2.0.0", "dbt-spark[PyHive]>=0.20,<2.0.0"],
 }
 
 
 setup(
     name="elementary-data",
     description="Data monitoring and lineage",
-    version="0.8.0",
+    version="0.8.1",
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.6.2",
     entry_points="""
         [console_scripts]
         edr=elementary.cli.cli:cli
     """,
```

### Comparing `elementary-data-0.8.0/tests/integration/monitor/api/alerts/test_alerts_fetcher.py` & `elementary-data-0.8.1/tests/integration/monitor/api/alerts/test_alerts_fetcher.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/tests/integration/monitor/api/tests/test_tests_api.py` & `elementary-data-0.8.1/tests/integration/monitor/api/tests/test_tests_api.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/tests/mocks/api/alerts_api_mock.py` & `elementary-data-0.8.1/tests/mocks/api/alerts_api_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/tests/mocks/api/tests_api_mock.py` & `elementary-data-0.8.1/tests/mocks/api/tests_api_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/tests/mocks/fetchers/alerts_fetcher_mock.py` & `elementary-data-0.8.1/tests/mocks/fetchers/alerts_fetcher_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/tests/mocks/fetchers/tests_fetcher_mock.py` & `elementary-data-0.8.1/tests/mocks/fetchers/tests_fetcher_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py` & `elementary-data-0.8.1/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py` & `elementary-data-0.8.1/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py` & `elementary-data-0.8.1/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/tests/unit/monitor/alerts/group_alerts_by_table/utils.py` & `elementary-data-0.8.1/tests/unit/monitor/alerts/group_alerts_by_table/utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/tests/unit/monitor/alerts/test_malformed_alert.py` & `elementary-data-0.8.1/tests/unit/monitor/alerts/test_malformed_alert.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/tests/unit/monitor/alerts/test_normalized_alert.py` & `elementary-data-0.8.1/tests/unit/monitor/alerts/test_normalized_alert.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     CHANNEL_KEY,
     COLUMN_FIELD,
     DEFAULT_ALERT_FIELDS,
     MODEL_META_KEY,
     OWNERS_FIELD,
     SUBSCRIBERS_KEY,
     TABLE_FIELD,
+    TAGS_FIELD,
     TEST_META_KEY,
     NormalizedAlert,
 )
 
 
 def test_flatten_meta():
     alert = dict(
@@ -275,7 +276,28 @@
     # No alert fields
     alert = dict(
         test_meta=json.dumps(dict()),
         model_meta=json.dumps(dict()),
     )
     normalized_alert = NormalizedAlert(alert)
     assert normalized_alert._get_alert_fields() == DEFAULT_ALERT_FIELDS
+
+
+def test_normalized_alert_tags():
+    tags = ["first", "second"]
+
+    alert = dict(tags=json.dumps(tags))
+    normalized_alert = NormalizedAlert(alert).get_normalized_alert()
+    assert json.dumps(normalized_alert.get(TAGS_FIELD).sort()) == json.dumps(
+        tags.sort()
+    )
+
+    alert = dict(tags=tags)
+    normalized_alert = NormalizedAlert(alert).get_normalized_alert()
+    assert json.dumps(normalized_alert.get(TAGS_FIELD).sort()) == json.dumps(
+        tags.sort()
+    )
+
+    # No tags return empty list
+    alert = dict()
+    normalized_alert = NormalizedAlert(alert).get_normalized_alert()
+    assert normalized_alert.get(TAGS_FIELD) == []
```

### Comparing `elementary-data-0.8.0/tests/unit/monitor/alerts/test_slack_alert_message_builder.py` & `elementary-data-0.8.1/tests/unit/monitor/alerts/test_slack_alert_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/tests/unit/monitor/api/alerts/test_alert_filters.py` & `elementary-data-0.8.1/tests/unit/monitor/api/alerts/test_alert_filters.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/tests/unit/monitor/api/alerts/test_alerts_api.py` & `elementary-data-0.8.1/tests/unit/monitor/api/alerts/test_alerts_api.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/tests/unit/monitor/api/tests/test_tests_api.py` & `elementary-data-0.8.1/tests/unit/monitor/api/tests/test_tests_api.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py` & `elementary-data-0.8.1/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/tests/unit/monitor/data_monitoring/test_selector_filter.py` & `elementary-data-0.8.1/tests/unit/monitor/data_monitoring/test_selector_filter.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.8.0/tests/unit/monitor/fetchers/test_alerts_fetcher.py` & `elementary-data-0.8.1/tests/unit/monitor/fetchers/test_alerts_fetcher.py`

 * *Files identical despite different names*

