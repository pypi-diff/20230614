# Comparing `tmp/mozilla-metric-config-parser-2023.6.3.tar.gz` & `tmp/mozilla-metric-config-parser-2023.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-metric-config-parser-2023.6.3.tar", last modified: Tue Jun  6 17:50:50 2023, max compression
+gzip compressed data, was "mozilla-metric-config-parser-2023.6.4.tar", last modified: Wed Jun 14 18:13:55 2023, max compression
```

## Comparing `mozilla-metric-config-parser-2023.6.3.tar` & `mozilla-metric-config-parser-2023.6.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:50:50.845125 mozilla-metric-config-parser-2023.6.3/
--rw-r--r--   0 root         (0) root         (0)    16725 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-06 17:50:50.845125 mozilla-metric-config-parser-2023.6.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      279 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:50:50.841125 mozilla-metric-config-parser-2023.6.3/metric_config_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7062 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/alert.py
--rw-r--r--   0 root         (0) root         (0)     7048 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/analysis.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/cli.py
--rw-r--r--   0 root         (0) root         (0)    27918 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/config.py
--rw-r--r--   0 root         (0) root         (0)     8172 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/data_source.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/definition.py
--rw-r--r--   0 root         (0) root         (0)     3493 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/dimension.py
--rw-r--r--   0 root         (0) root         (0)      804 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/errors.py
--rw-r--r--   0 root         (0) root         (0)     9608 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/experiment.py
--rw-r--r--   0 root         (0) root         (0)     2619 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/exposure_signal.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/function.py
--rw-r--r--   0 root         (0) root         (0)    12463 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/metric.py
--rw-r--r--   0 root         (0) root         (0)     3130 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/metric_group.py
--rw-r--r--   0 root         (0) root         (0)     6640 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/monitoring.py
--rw-r--r--   0 root         (0) root         (0)     1718 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/outcome.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/parameter.py
--rw-r--r--   0 root         (0) root         (0)     3278 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/population.py
--rw-r--r--   0 root         (0) root         (0)      317 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/pre_treatment.py
--rw-r--r--   0 root         (0) root         (0)     5138 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/project.py
--rw-r--r--   0 root         (0) root         (0)     8103 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/segment.py
--rw-r--r--   0 root         (0) root         (0)     4207 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/sql.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/statistic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:50:50.841125 mozilla-metric-config-parser-2023.6.3/metric_config_parser/templates/
--rw-r--r--   0 root         (0) root         (0)      145 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/templates/data_source_query.sql
--rw-r--r--   0 root         (0) root         (0)     2691 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/templates/metrics_query.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:50:50.845125 mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5118 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:50:50.845125 mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     4708 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/integration/test_config_integration.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_alert.py
--rw-r--r--   0 root         (0) root         (0)    19957 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_analysis.py
--rw-r--r--   0 root         (0) root         (0)    14533 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)     9856 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_experiment.py
--rw-r--r--   0 root         (0) root         (0)     1581 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_function.py
--rw-r--r--   0 root         (0) root         (0)     2608 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_metric.py
--rw-r--r--   0 root         (0) root         (0)     8522 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)    11358 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_outcomes.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_parameter.py
--rw-r--r--   0 root         (0) root         (0)     2035 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_population.py
--rw-r--r--   0 root         (0) root         (0)     2808 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_project.py
--rw-r--r--   0 root         (0) root         (0)     3322 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_sql.py
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/metric_config_parser/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:50:50.845125 mozilla-metric-config-parser-2023.6.3/mozilla_metric_config_parser.egg-info/
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-06 17:50:50.000000 mozilla-metric-config-parser-2023.6.3/mozilla_metric_config_parser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1941 2023-06-06 17:50:50.000000 mozilla-metric-config-parser-2023.6.3/mozilla_metric_config_parser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 17:50:50.000000 mozilla-metric-config-parser-2023.6.3/mozilla_metric_config_parser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-06-06 17:50:50.000000 mozilla-metric-config-parser-2023.6.3/mozilla_metric_config_parser.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-06 17:50:50.000000 mozilla-metric-config-parser-2023.6.3/mozilla_metric_config_parser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-06 17:50:50.000000 mozilla-metric-config-parser-2023.6.3/mozilla_metric_config_parser.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-06 17:50:50.845125 mozilla-metric-config-parser-2023.6.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1540 2023-06-06 17:50:41.000000 mozilla-metric-config-parser-2023.6.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:13:55.443258 mozilla-metric-config-parser-2023.6.4/
+-rw-r--r--   0 root         (0) root         (0)    16725 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-14 18:13:55.443258 mozilla-metric-config-parser-2023.6.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      279 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:13:55.439258 mozilla-metric-config-parser-2023.6.4/metric_config_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7062 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/alert.py
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/analysis.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/cli.py
+-rw-r--r--   0 root         (0) root         (0)    27669 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/config.py
+-rw-r--r--   0 root         (0) root         (0)     8172 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/data_source.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/definition.py
+-rw-r--r--   0 root         (0) root         (0)     3493 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/dimension.py
+-rw-r--r--   0 root         (0) root         (0)      804 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/errors.py
+-rw-r--r--   0 root         (0) root         (0)     9608 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/experiment.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/exposure_signal.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/function.py
+-rw-r--r--   0 root         (0) root         (0)    12463 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/metric.py
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/metric_group.py
+-rw-r--r--   0 root         (0) root         (0)     6640 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/outcome.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/parameter.py
+-rw-r--r--   0 root         (0) root         (0)     3278 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/population.py
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/pre_treatment.py
+-rw-r--r--   0 root         (0) root         (0)     5138 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/project.py
+-rw-r--r--   0 root         (0) root         (0)     8103 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/segment.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/sql.py
+-rw-r--r--   0 root         (0) root         (0)      129 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/statistic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:13:55.439258 mozilla-metric-config-parser-2023.6.4/metric_config_parser/templates/
+-rw-r--r--   0 root         (0) root         (0)      145 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/templates/data_source_query.sql
+-rw-r--r--   0 root         (0) root         (0)     2691 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/templates/metrics_query.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:13:55.439258 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5118 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:13:55.443258 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     4708 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/integration/test_config_integration.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_alert.py
+-rw-r--r--   0 root         (0) root         (0)    19957 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    14533 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     9856 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_experiment.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_function.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_metric.py
+-rw-r--r--   0 root         (0) root         (0)     8522 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_outcomes.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_population.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_project.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_sql.py
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:13:55.443258 mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-14 18:13:55.000000 mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-06-14 18:13:55.000000 mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 18:13:55.000000 mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-14 18:13:55.000000 mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-14 18:13:55.000000 mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-14 18:13:55.000000 mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-14 18:13:55.443258 mozilla-metric-config-parser-2023.6.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/setup.py
```

### Comparing `mozilla-metric-config-parser-2023.6.3/LICENSE` & `mozilla-metric-config-parser-2023.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/PKG-INFO` & `mozilla-metric-config-parser-2023.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2023.6.3
+Version: 2023.6.4
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/alert.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/alert.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/analysis.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/analysis.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/cli.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/cli.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/config.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -538,18 +538,14 @@
                                 tmp_repo,
                                 repo.path,
                                 self.is_private,
                                 repo.main_branch,
                                 is_tmp_repo=True,
                             )
                             could_load_configs = True
-                            print(
-                                f"Error parsing config files as of {timestamp}: {e}. "
-                                + f"Using newer version instead of commit {newer_commit.hexsha}"
-                            )
                             break
                         except Exception:
                             # continue searching
                             pass
 
                     if not could_load_configs:
                         # there is no newer commit, current state is broken
```

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/data_source.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/data_source.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/definition.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/definition.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/dimension.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/dimension.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/errors.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/errors.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/experiment.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/experiment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/exposure_signal.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/exposure_signal.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/function.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/function.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/metric.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/metric.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/metric_group.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/metric_group.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/monitoring.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/outcome.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/outcome.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/parameter.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/parameter.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/population.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/population.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/project.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/project.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/segment.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/segment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/sql.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/sql.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/templates/metrics_query.sql` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/templates/metrics_query.sql`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/conftest.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/integration/test_config_integration.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/integration/test_config_integration.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_alert.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_alert.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_analysis.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_config.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_experiment.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_function.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_metric.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_monitoring.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_outcomes.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_population.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_project.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/tests/test_sql.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/metric_config_parser/util.py` & `mozilla-metric-config-parser-2023.6.4/metric_config_parser/util.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/mozilla_metric_config_parser.egg-info/PKG-INFO` & `mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2023.6.3
+Version: 2023.6.4
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `mozilla-metric-config-parser-2023.6.3/mozilla_metric_config_parser.egg-info/SOURCES.txt` & `mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.3/setup.py` & `mozilla-metric-config-parser-2023.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,9 +60,9 @@
     long_description=text_from_file("README.md"),
     long_description_content_type="text/markdown",
     python_requires=">=3.6",
     entry_points="""
         [console_scripts]
         metric-config-parser=metric_config_parser.cli:cli
     """,
-    version="2023.6.3",
+    version="2023.6.4",
 )
```

