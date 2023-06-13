# Comparing `tmp/dlt-0.3.0.tar.gz` & `tmp/dlt-0.3.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.3.0.tar", max compression
+gzip compressed data, was "dlt-0.3.1a0.tar", max compression
```

## Comparing `dlt-0.3.0.tar` & `dlt-0.3.1a0.tar`

### file list

```diff
@@ -1,213 +1,214 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     4131 2023-06-07 09:55:25.911010 dlt-0.3.0/README.md
--rw-r--r--   0        0        0     1711 2023-04-30 21:17:44.388805 dlt-0.3.0/dlt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.3.0/dlt/cli/__init__.py
--rw-r--r--   0        0        0    16723 2023-06-07 09:55:25.911010 dlt-0.3.0/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     3886 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    14636 2023-05-29 18:11:09.008705 dlt-0.3.0/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0    14722 2023-05-29 18:11:09.008705 dlt-0.3.0/dlt/cli/deploy_command_helpers.py
--rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.3.0/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-06-07 09:55:25.911010 dlt-0.3.0/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    18756 2023-06-07 09:55:25.911010 dlt-0.3.0/dlt/cli/init_command.py
--rw-r--r--   0        0        0    10503 2023-05-28 13:56:42.331452 dlt-0.3.0/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0     9588 2023-06-07 09:55:25.911010 dlt-0.3.0/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     4505 2023-05-24 16:38:22.528779 dlt-0.3.0/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1899 2023-05-23 16:25:33.987923 dlt-0.3.0/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     3753 2023-05-29 18:11:09.008705 dlt-0.3.0/dlt/cli/utils.py
--rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.3.0/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      442 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     5078 2023-05-24 16:38:22.528779 dlt-0.3.0/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     3469 2023-06-03 16:59:51.259756 dlt-0.3.0/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     6741 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.3.0/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1791 2023-05-14 20:33:31.539348 dlt-0.3.0/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      306 2023-05-07 23:03:04.659469 dlt-0.3.0/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0      664 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1116 2023-05-07 23:03:04.659469 dlt-0.3.0/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1335 2023-05-07 23:03:04.659469 dlt-0.3.0/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     1981 2023-05-07 23:03:04.659469 dlt-0.3.0/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0     3662 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/providers/google_secrets.py
--rw-r--r--   0        0        0     1306 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0    12390 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    18788 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0      971 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1817 2023-05-07 23:03:04.659469 dlt-0.3.0/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0     2109 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/specs/aws_credentials.py
--rw-r--r--   0        0        0    14214 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     5483 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     3387 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     1818 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/configuration/specs/connection_string_credentials.py
--rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.3.0/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    12725 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/common/configuration/specs/gcp_credentials.py
--rw-r--r--   0        0        0      725 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.3.0/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0     6036 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.3.0/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     5893 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     2400 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0      189 2023-05-29 18:11:09.008705 dlt-0.3.0/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     2206 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0    11099 2023-05-29 18:11:09.008705 dlt-0.3.0/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     6461 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/exceptions.py
--rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/git.py
--rw-r--r--   0        0        0     5253 2023-05-14 20:33:31.539348 dlt-0.3.0/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.3.0/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.3.0/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.3.0/dlt/common/jsonpath.py
--rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1197 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.3.0/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    13382 2023-05-14 20:33:31.539348 dlt-0.3.0/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.3.0/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.3.0/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/pendulum.py
--rw-r--r--   0        0        0    18949 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.3.0/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.3.0/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.3.0/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      705 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     2635 2023-05-14 11:08:47.420838 dlt-0.3.0/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.3.0/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5590 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    13923 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     4501 2023-05-14 20:33:31.539348 dlt-0.3.0/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/common/runtime/logger.py
--rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     7170 2023-05-14 20:33:31.539348 dlt-0.3.0/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.3.0/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.3.0/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    25164 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.3.0/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    23080 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/schema/utils.py
--rw-r--r--   0        0        0     1467 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/source.py
--rw-r--r--   0        0        0      554 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1649 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/storages/configuration.py
--rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     3107 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0    10891 2023-05-14 20:33:31.539348 dlt-0.3.0/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2690 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    21812 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2409 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8600 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.3.0/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2634 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/common/time.py
--rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.3.0/dlt/common/typing.py
--rw-r--r--   0        0        0    14239 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/common/wei.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    12370 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0      386 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0    10342 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/destinations/duckdb/__init__.py
--rw-r--r--   0        0        0     7207 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/destinations/duckdb/configuration.py
--rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/destinations/duckdb/duck.py
--rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.3.0/dlt/destinations/duckdb/sql_client.py
--rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.3.0/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     4989 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     1270 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/destinations/filesystem/__init__.py
--rw-r--r--   0        0        0     2253 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/destinations/filesystem/configuration.py
--rw-r--r--   0        0        0     4935 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/destinations/filesystem/filesystem.py
--rw-r--r--   0        0        0     1419 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/destinations/filesystem/filesystem_client.py
--rw-r--r--   0        0        0     5005 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    15639 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0     1316 2023-05-29 18:11:09.008705 dlt-0.3.0/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     6074 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.3.0/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      570 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     7117 2023-05-28 13:56:42.341452 dlt-0.3.0/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    10090 2023-05-28 13:56:42.341452 dlt-0.3.0/dlt/destinations/sql_merge_job.py
--rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.3.0/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.0/dlt/extract/__init__.py
--rw-r--r--   0        0        0    26516 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/extract/decorators.py
--rw-r--r--   0        0        0    12995 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     8481 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/extract/extract.py
--rw-r--r--   0        0        0    14954 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/extract/incremental.py
--rw-r--r--   0        0        0    31816 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/extract/pipe.py
--rw-r--r--   0        0        0     9683 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/extract/schema.py
--rw-r--r--   0        0        0    38287 2023-06-07 08:32:53.271010 dlt-0.3.0/dlt/extract/source.py
--rw-r--r--   0        0        0     4308 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/extract/typing.py
--rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.3.0/dlt/extract/utils.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.3.0/dlt/helpers/__init__.py
--rw-r--r--   0        0        0    13783 2023-05-28 13:56:42.341452 dlt-0.3.0/dlt/helpers/airflow_helper.py
--rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     2490 2023-05-29 14:13:02.438979 dlt-0.3.0/dlt/helpers/pandas_helper.py
--rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/helpers/parquet.py
--rw-r--r--   0        0        0    13378 2023-05-29 14:13:02.438979 dlt-0.3.0/dlt/helpers/streamlit_helper.py
--rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/load/__init__.py
--rw-r--r--   0        0        0     1005 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/load/configuration.py
--rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/load/exceptions.py
--rw-r--r--   0        0        0    19925 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/load/load.py
--rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1101 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.0/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    16538 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/normalize/normalize.py
--rw-r--r--   0        0        0    13081 2023-05-28 13:56:42.341452 dlt-0.3.0/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     1858 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      379 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     3100 2023-05-28 13:56:42.341452 dlt-0.3.0/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     8733 2023-06-07 08:32:53.271010 dlt-0.3.0/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.3.0/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    59020 2023-06-07 08:32:53.271010 dlt-0.3.0/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     4186 2023-06-07 08:32:53.271010 dlt-0.3.0/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.3.0/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     4625 2023-05-29 18:11:09.018705 dlt-0.3.0/dlt/pipeline/track.py
--rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.3.0/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/reflection/names.py
--rw-r--r--   0        0        0     5617 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      124 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/sources/__init__.py
--rw-r--r--   0        0        0      320 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/sources/credentials.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.3.0/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0     9243 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.3.0/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.3.0/dlt/version.py
--rw-r--r--   0        0        0     4276 2023-06-07 09:58:58.281010 dlt-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7546 1970-01-01 00:00:00.000000 dlt-0.3.0/setup.py
--rw-r--r--   0        0        0     7544 1970-01-01 00:00:00.000000 dlt-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.3.1a0/LICENSE.txt
+-rw-r--r--   0        0        0     4131 2023-06-07 10:42:04.941010 dlt-0.3.1a0/README.md
+-rw-r--r--   0        0        0     1711 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    16723 2023-06-07 10:42:04.941010 dlt-0.3.1a0/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     3886 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    14636 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0    14722 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/cli/deploy_command_helpers.py
+-rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-06-07 10:42:04.941010 dlt-0.3.1a0/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    18756 2023-06-07 10:42:04.941010 dlt-0.3.1a0/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    10503 2023-05-28 13:56:42.331452 dlt-0.3.1a0/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0     9588 2023-06-07 10:42:04.941010 dlt-0.3.1a0/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     4505 2023-05-24 16:38:22.528779 dlt-0.3.1a0/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1899 2023-05-23 16:25:33.987923 dlt-0.3.1a0/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     3753 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/cli/utils.py
+-rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.3.1a0/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      442 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     5078 2023-05-24 16:38:22.528779 dlt-0.3.1a0/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     3469 2023-06-03 16:59:51.259756 dlt-0.3.1a0/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     6741 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.3.1a0/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1791 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      306 2023-05-07 23:03:04.659469 dlt-0.3.1a0/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0      664 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1116 2023-05-07 23:03:04.659469 dlt-0.3.1a0/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1335 2023-05-07 23:03:04.659469 dlt-0.3.1a0/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     1981 2023-05-07 23:03:04.659469 dlt-0.3.1a0/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0     3662 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/providers/google_secrets.py
+-rw-r--r--   0        0        0     1306 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0    12390 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    18788 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0      971 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1817 2023-05-07 23:03:04.659469 dlt-0.3.1a0/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0     2109 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/specs/aws_credentials.py
+-rw-r--r--   0        0        0    14214 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     5483 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     3387 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     1818 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/configuration/specs/connection_string_credentials.py
+-rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.3.1a0/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    12725 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/common/configuration/specs/gcp_credentials.py
+-rw-r--r--   0        0        0      725 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0     6036 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.3.1a0/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     5893 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     2400 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0      189 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     2228 2023-06-13 23:16:30.618251 dlt-0.3.1a0/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0    11099 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     6465 2023-06-08 07:50:27.863474 dlt-0.3.1a0/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/git.py
+-rw-r--r--   0        0        0     5253 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.3.1a0/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.3.1a0/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.3.1a0/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1197 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.3.1a0/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    13382 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.3.1a0/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.3.1a0/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    18949 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.3.1a0/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.3.1a0/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      705 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     2635 2023-05-14 11:08:47.420838 dlt-0.3.1a0/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5590 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    13923 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     4501 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/logger.py
+-rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     7170 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.3.1a0/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.3.1a0/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0    25164 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.3.1a0/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    23080 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0     1467 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/source.py
+-rw-r--r--   0        0        0      554 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     1649 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/storages/configuration.py
+-rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     3107 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0    10891 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0     2690 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    21812 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     2409 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     8600 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     9486 2023-06-08 07:50:27.863474 dlt-0.3.1a0/dlt/common/storages/transactional_file.py
+-rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.3.1a0/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     2634 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/common/time.py
+-rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.3.1a0/dlt/common/typing.py
+-rw-r--r--   0        0        0    14285 2023-06-13 23:16:30.618251 dlt-0.3.1a0/dlt/common/utils.py
+-rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/validation.py
+-rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/wei.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/bigquery/README.md
+-rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/bigquery/__init__.py
+-rw-r--r--   0        0        0    12370 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/bigquery/bigquery.py
+-rw-r--r--   0        0        0      386 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/destinations/bigquery/configuration.py
+-rw-r--r--   0        0        0    10342 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/destinations/bigquery/sql_client.py
+-rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/duckdb/__init__.py
+-rw-r--r--   0        0        0     7207 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/duckdb/configuration.py
+-rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/duckdb/duck.py
+-rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.3.1a0/dlt/destinations/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/dummy/__init__.py
+-rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.3.1a0/dlt/destinations/dummy/configuration.py
+-rw-r--r--   0        0        0     4989 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/dummy/dummy.py
+-rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0     1270 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/destinations/filesystem/__init__.py
+-rw-r--r--   0        0        0     2253 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/filesystem/configuration.py
+-rw-r--r--   0        0        0     4935 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/filesystem/filesystem.py
+-rw-r--r--   0        0        0     1419 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/filesystem/filesystem_client.py
+-rw-r--r--   0        0        0     5005 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    15639 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/postgres/README.md
+-rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/postgres/__init__.py
+-rw-r--r--   0        0        0     1316 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/destinations/postgres/configuration.py
+-rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/postgres/postgres.py
+-rw-r--r--   0        0        0     6074 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/destinations/postgres/sql_client.py
+-rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.3.1a0/dlt/destinations/redshift/README.md
+-rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/redshift/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/destinations/redshift/configuration.py
+-rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/redshift/redshift.py
+-rw-r--r--   0        0        0     7117 2023-05-28 13:56:42.341452 dlt-0.3.1a0/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    10090 2023-05-28 13:56:42.341452 dlt-0.3.1a0/dlt/destinations/sql_merge_job.py
+-rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.3.1a0/dlt/destinations/typing.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.1a0/dlt/extract/__init__.py
+-rw-r--r--   0        0        0    26516 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    12995 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0     8312 2023-06-13 20:43:40.978251 dlt-0.3.1a0/dlt/extract/extract.py
+-rw-r--r--   0        0        0    14954 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/extract/incremental.py
+-rw-r--r--   0        0        0    32327 2023-06-13 20:43:40.978251 dlt-0.3.1a0/dlt/extract/pipe.py
+-rw-r--r--   0        0        0     9683 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/extract/schema.py
+-rw-r--r--   0        0        0    38391 2023-06-13 20:43:40.978251 dlt-0.3.1a0/dlt/extract/source.py
+-rw-r--r--   0        0        0     4308 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/extract/typing.py
+-rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.3.1a0/dlt/extract/utils.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.3.1a0/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0    13783 2023-05-28 13:56:42.341452 dlt-0.3.1a0/dlt/helpers/airflow_helper.py
+-rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     2490 2023-05-29 14:13:02.438979 dlt-0.3.1a0/dlt/helpers/pandas_helper.py
+-rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/helpers/parquet.py
+-rw-r--r--   0        0        0    13378 2023-05-29 14:13:02.438979 dlt-0.3.1a0/dlt/helpers/streamlit_helper.py
+-rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/load/__init__.py
+-rw-r--r--   0        0        0     1005 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/load/configuration.py
+-rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    19925 2023-06-08 14:19:13.923473 dlt-0.3.1a0/dlt/load/load.py
+-rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1101 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.1a0/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    16538 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0    13081 2023-05-28 13:56:42.341452 dlt-0.3.1a0/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     1858 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      379 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     3100 2023-05-28 13:56:42.341452 dlt-0.3.1a0/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     8733 2023-06-07 08:32:53.271010 dlt-0.3.1a0/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.3.1a0/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    59020 2023-06-07 08:32:53.271010 dlt-0.3.1a0/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     4186 2023-06-07 08:32:53.271010 dlt-0.3.1a0/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.3.1a0/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     4625 2023-05-29 18:11:09.018705 dlt-0.3.1a0/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.3.1a0/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/reflection/names.py
+-rw-r--r--   0        0        0     5617 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      124 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/sources/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/sources/credentials.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.3.1a0/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0     9243 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.3.1a0/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.3.1a0/dlt/version.py
+-rw-r--r--   0        0        0     4278 2023-06-13 23:16:43.718251 dlt-0.3.1a0/pyproject.toml
+-rw-r--r--   0        0        0     7548 1970-01-01 00:00:00.000000 dlt-0.3.1a0/setup.py
+-rw-r--r--   0        0        0     7546 1970-01-01 00:00:00.000000 dlt-0.3.1a0/PKG-INFO
```

### Comparing `dlt-0.3.0/LICENSE.txt` & `dlt-0.3.1a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/README.md` & `dlt-0.3.1a0/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/__init__.py` & `dlt-0.3.1a0/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/cli/_dlt.py` & `dlt-0.3.1a0/dlt/cli/_dlt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/cli/config_toml_writer.py` & `dlt-0.3.1a0/dlt/cli/config_toml_writer.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/cli/deploy_command.py` & `dlt-0.3.1a0/dlt/cli/deploy_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/cli/deploy_command_helpers.py` & `dlt-0.3.1a0/dlt/cli/deploy_command_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/cli/echo.py` & `dlt-0.3.1a0/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/cli/init_command.py` & `dlt-0.3.1a0/dlt/cli/init_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/cli/pipeline_command.py` & `dlt-0.3.1a0/dlt/cli/pipeline_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/cli/pipeline_files.py` & `dlt-0.3.1a0/dlt/cli/pipeline_files.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/cli/source_detection.py` & `dlt-0.3.1a0/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/cli/telemetry_command.py` & `dlt-0.3.1a0/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/cli/utils.py` & `dlt-0.3.1a0/dlt/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/arithmetics.py` & `dlt-0.3.1a0/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/accessors.py` & `dlt-0.3.1a0/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/container.py` & `dlt-0.3.1a0/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/exceptions.py` & `dlt-0.3.1a0/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/inject.py` & `dlt-0.3.1a0/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/paths.py` & `dlt-0.3.1a0/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/providers/airflow.py` & `dlt-0.3.1a0/dlt/common/configuration/providers/airflow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/providers/context.py` & `dlt-0.3.1a0/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/providers/dictionary.py` & `dlt-0.3.1a0/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/providers/environ.py` & `dlt-0.3.1a0/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/providers/google_secrets.py` & `dlt-0.3.1a0/dlt/common/configuration/providers/google_secrets.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/providers/provider.py` & `dlt-0.3.1a0/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/providers/toml.py` & `dlt-0.3.1a0/dlt/common/configuration/providers/toml.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/resolve.py` & `dlt-0.3.1a0/dlt/common/configuration/resolve.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/specs/__init__.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/specs/aws_credentials.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/config_providers_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/specs/connection_string_credentials.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/specs/exceptions.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/specs/gcp_credentials.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/specs/known_sections.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/configuration/utils.py` & `dlt-0.3.1a0/dlt/common/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/data_types/type_helpers.py` & `dlt-0.3.1a0/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/data_writers/buffered.py` & `dlt-0.3.1a0/dlt/common/data_writers/buffered.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/data_writers/escape.py` & `dlt-0.3.1a0/dlt/common/data_writers/escape.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/data_writers/exceptions.py` & `dlt-0.3.1a0/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/data_writers/writers.py` & `dlt-0.3.1a0/dlt/common/data_writers/writers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/destination/capabilities.py` & `dlt-0.3.1a0/dlt/common/destination/capabilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Callable, ClassVar, List, Literal
 
 from dlt.common.configuration.utils import serialize_value
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import ContainerInjectableContext
+from dlt.common.utils import identity
 
 
 # known loader file formats
 # jsonl - new line separated json documents
 # puae-jsonl - internal extract -> normalize format bases on jsonl
 # insert_values - insert SQL statements
 # sql - any sql statement
@@ -34,16 +35,16 @@
     can_create_default: ClassVar[bool] = False
 
     @staticmethod
     def generic_capabilities(preferred_loader_file_format: TLoaderFileFormat = None) -> "DestinationCapabilitiesContext":
         caps = DestinationCapabilitiesContext()
         caps.preferred_loader_file_format = preferred_loader_file_format
         caps.supported_loader_file_formats = ["jsonl", "insert_values"]
-        caps.escape_identifier = lambda x: x
-        caps.escape_literal = lambda x: serialize_value(x)
+        caps.escape_identifier = identity
+        caps.escape_literal = serialize_value
         caps.max_identifier_length = 65536
         caps.max_column_identifier_length = 65536
         caps.max_query_length = 32 * 1024 * 1024
         caps.is_max_query_length_in_bytes = True
         caps.max_text_data_type_length = 1024 * 1024 * 1024
         caps.is_max_text_data_type_length_in_bytes = True
         caps.supports_ddl_transactions = True
```

### Comparing `dlt-0.3.0/dlt/common/destination/reference.py` & `dlt-0.3.1a0/dlt/common/destination/reference.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/exceptions.py` & `dlt-0.3.1a0/dlt/common/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 {self._to_pip_install()}
 """
         if appendix:
             msg = msg + "\n" + appendix
         return msg
 
     def _to_pip_install(self) -> str:
-        return "\n".join([f"pip install {d}" for d in self.dependencies])
+        return "\n".join([f"pip install \"{d}\"" for d in self.dependencies])
 
 
 class DestinationException(DltException):
     pass
 
 
 class UnknownDestinationModule(DestinationException):
```

### Comparing `dlt-0.3.0/dlt/common/git.py` & `dlt-0.3.1a0/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/json/__init__.py` & `dlt-0.3.1a0/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/json/_orjson.py` & `dlt-0.3.1a0/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/json/_simplejson.py` & `dlt-0.3.1a0/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/jsonpath.py` & `dlt-0.3.1a0/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/normalizers/configuration.py` & `dlt-0.3.1a0/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/normalizers/json/__init__.py` & `dlt-0.3.1a0/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/normalizers/json/relational.py` & `dlt-0.3.1a0/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/normalizers/naming/direct.py` & `dlt-0.3.1a0/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.3.1a0/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.3.1a0/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/normalizers/naming/naming.py` & `dlt-0.3.1a0/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.3.1a0/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/normalizers/utils.py` & `dlt-0.3.1a0/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/pipeline.py` & `dlt-0.3.1a0/dlt/common/pipeline.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/reflection/spec.py` & `dlt-0.3.1a0/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/reflection/utils.py` & `dlt-0.3.1a0/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/runners/configuration.py` & `dlt-0.3.1a0/dlt/common/runners/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/runners/pool_runner.py` & `dlt-0.3.1a0/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/runners/runnable.py` & `dlt-0.3.1a0/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/runners/stdout.py` & `dlt-0.3.1a0/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/runners/synth_pickle.py` & `dlt-0.3.1a0/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/runners/venv.py` & `dlt-0.3.1a0/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/runtime/collector.py` & `dlt-0.3.1a0/dlt/common/runtime/collector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/runtime/exec_info.py` & `dlt-0.3.1a0/dlt/common/runtime/exec_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/runtime/init.py` & `dlt-0.3.1a0/dlt/common/runtime/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/runtime/logger.py` & `dlt-0.3.1a0/dlt/common/runtime/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/runtime/prometheus.py` & `dlt-0.3.1a0/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/runtime/segment.py` & `dlt-0.3.1a0/dlt/common/runtime/segment.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/runtime/sentry.py` & `dlt-0.3.1a0/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/runtime/signals.py` & `dlt-0.3.1a0/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/runtime/slack.py` & `dlt-0.3.1a0/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/runtime/telemetry.py` & `dlt-0.3.1a0/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/schema/detections.py` & `dlt-0.3.1a0/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/schema/exceptions.py` & `dlt-0.3.1a0/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/schema/schema.py` & `dlt-0.3.1a0/dlt/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/schema/typing.py` & `dlt-0.3.1a0/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/schema/utils.py` & `dlt-0.3.1a0/dlt/common/schema/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/source.py` & `dlt-0.3.1a0/dlt/common/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/storages/__init__.py` & `dlt-0.3.1a0/dlt/common/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/storages/configuration.py` & `dlt-0.3.1a0/dlt/common/storages/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/storages/data_item_storage.py` & `dlt-0.3.1a0/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/storages/exceptions.py` & `dlt-0.3.1a0/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/storages/file_storage.py` & `dlt-0.3.1a0/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/storages/live_schema_storage.py` & `dlt-0.3.1a0/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/storages/load_storage.py` & `dlt-0.3.1a0/dlt/common/storages/load_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/storages/normalize_storage.py` & `dlt-0.3.1a0/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/storages/schema_storage.py` & `dlt-0.3.1a0/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/storages/versioned_storage.py` & `dlt-0.3.1a0/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/time.py` & `dlt-0.3.1a0/dlt/common/time.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/typing.py` & `dlt-0.3.1a0/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/utils.py` & `dlt-0.3.1a0/dlt/common/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,7 +417,11 @@
     return base64.b64encode(zlib.compress(value, level=9)).decode('ascii')
 
 
 def compressed_b64decode(value: str) -> bytes:
     """Decode a bytestring encoded with `compressed_b64encode`"""
     value_bytes = base64.b64decode(value, validate=True)
     return zlib.decompress(value_bytes)
+
+
+def identity(x: TAny) -> TAny:
+    return x
```

### Comparing `dlt-0.3.0/dlt/common/validation.py` & `dlt-0.3.1a0/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/common/wei.py` & `dlt-0.3.1a0/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/bigquery/__init__.py` & `dlt-0.3.1a0/dlt/destinations/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/bigquery/bigquery.py` & `dlt-0.3.1a0/dlt/destinations/bigquery/bigquery.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/bigquery/sql_client.py` & `dlt-0.3.1a0/dlt/destinations/bigquery/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/duckdb/__init__.py` & `dlt-0.3.1a0/dlt/destinations/duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/duckdb/configuration.py` & `dlt-0.3.1a0/dlt/destinations/duckdb/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/duckdb/duck.py` & `dlt-0.3.1a0/dlt/destinations/duckdb/duck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/duckdb/sql_client.py` & `dlt-0.3.1a0/dlt/destinations/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/dummy/__init__.py` & `dlt-0.3.1a0/dlt/destinations/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/dummy/configuration.py` & `dlt-0.3.1a0/dlt/destinations/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/dummy/dummy.py` & `dlt-0.3.1a0/dlt/destinations/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/exceptions.py` & `dlt-0.3.1a0/dlt/destinations/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/filesystem/__init__.py` & `dlt-0.3.1a0/dlt/destinations/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/filesystem/configuration.py` & `dlt-0.3.1a0/dlt/destinations/filesystem/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/filesystem/filesystem.py` & `dlt-0.3.1a0/dlt/destinations/filesystem/filesystem.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/filesystem/filesystem_client.py` & `dlt-0.3.1a0/dlt/destinations/filesystem/filesystem_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/insert_job_client.py` & `dlt-0.3.1a0/dlt/destinations/insert_job_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/job_client_impl.py` & `dlt-0.3.1a0/dlt/destinations/job_client_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/job_impl.py` & `dlt-0.3.1a0/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/postgres/__init__.py` & `dlt-0.3.1a0/dlt/destinations/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/postgres/configuration.py` & `dlt-0.3.1a0/dlt/destinations/postgres/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/postgres/postgres.py` & `dlt-0.3.1a0/dlt/destinations/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/postgres/sql_client.py` & `dlt-0.3.1a0/dlt/destinations/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/redshift/README.md` & `dlt-0.3.1a0/dlt/destinations/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/redshift/__init__.py` & `dlt-0.3.1a0/dlt/destinations/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/redshift/configuration.py` & `dlt-0.3.1a0/dlt/destinations/redshift/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/redshift/redshift.py` & `dlt-0.3.1a0/dlt/destinations/redshift/redshift.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/sql_client.py` & `dlt-0.3.1a0/dlt/destinations/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/sql_merge_job.py` & `dlt-0.3.1a0/dlt/destinations/sql_merge_job.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/destinations/typing.py` & `dlt-0.3.1a0/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/extract/decorators.py` & `dlt-0.3.1a0/dlt/extract/decorators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/extract/exceptions.py` & `dlt-0.3.1a0/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/extract/extract.py` & `dlt-0.3.1a0/dlt/extract/extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,17 +165,14 @@
             # reset resource states
             for resource in source.resources.extracted.values():
                 with contextlib.suppress(DataItemRequiredForDynamicTableHints):
                     if resource.write_disposition == "replace":
                         _reset_resource_state(resource._name)
 
             extractor = extract(extract_id, source, storage, collector, max_parallel_items=max_parallel_items, workers=workers)
-            # source iterates
-            # TODO: implement a real check if source is exhausted. most of the resources should be not
-            source.exhausted = True
             # iterate over all items in the pipeline and update the schema if dynamic table hints were present
             for _, partials in extractor.items():
                 for partial in partials:
                     schema.update_schema(schema.normalize_table_identifiers(partial))
 
     return extract_id
```

### Comparing `dlt-0.3.0/dlt/extract/incremental.py` & `dlt-0.3.1a0/dlt/extract/incremental.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/extract/pipe.py` & `dlt-0.3.1a0/dlt/extract/pipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from copy import copy
 from threading import Thread
 from typing import Any, ContextManager, Optional, Sequence, Union, Callable, Iterable, Iterator, List, NamedTuple, Awaitable, Tuple, Type, TYPE_CHECKING
 
 from dlt.common import sleep
 from dlt.common.configuration import configspec
 from dlt.common.configuration.inject import with_config
-from dlt.common.configuration.specs import BaseConfiguration
+from dlt.common.configuration.specs import BaseConfiguration, ContainerInjectableContext
+from dlt.common.configuration.container import Container
 from dlt.common.exceptions import PipelineException
 from dlt.common.source import unset_current_pipe_name, set_current_pipe_name
 from dlt.common.typing import AnyFun, AnyType, TDataItems
 from dlt.common.utils import get_callable_name
 
 from dlt.extract.exceptions import CreatePipeException, DltSourceException, ExtractorException, InvalidResourceDataTypeFunctionNotAGenerator, InvalidStepFunctionArguments, InvalidTransformerGeneratorFunction, ParametrizedResourceUnbound, PipeException, PipeItemProcessingError, PipeNotBoundToData, ResourceExtractionError
 from dlt.extract.typing import DataItemWithMeta, ItemTransform, SupportsPipe, TPipedDataItems
@@ -720,27 +721,38 @@
                 clone = clone.parent
 
         return cloned_pipes
 
 
 class ManagedPipeIterator(PipeIterator):
     """A version of the pipe iterator that gets closed automatically on an exception in _next_"""
-    _context_manager: ContextManager[Any] = None
+    _ctx: List[ContainerInjectableContext] = None
+    _container: Container = None
 
-    def set_context_manager(self, ctx: ContextManager[Any]) -> None:
-        """Enters the context manager that will exit automatically when iterator is closed"""
-        ctx.__enter__()
-        self._context_manager = ctx
+    def set_context(self, ctx: List[ContainerInjectableContext]) -> None:
+        """Sets list of injectable contexts that will be injected into Container for each call to __next__"""
+        self._ctx = ctx
+        self._container = Container()
 
     def __next__(self) -> PipeItem:
+        if self._ctx:
+            managers = [self._container.injectable_context(ctx) for ctx in self._ctx]
+            for manager in managers:
+                manager.__enter__()
         try:
-            return super().__next__()
+            item = super().__next__()
         except Exception as ex:
             # release context manager
-            if self._context_manager:
+            if self._ctx:
                 if isinstance(ex, StopIteration):
-                    self._context_manager.__exit__(None, None, None)
+                    for manager in managers:
+                        manager.__exit__(None, None, None)
                 else:
-                    self._context_manager.__exit__(type(ex), ex, None)
+                    for manager in managers:
+                        manager.__exit__(type(ex), ex, None)
             # crash in next
             self.close()
             raise
+        if self._ctx:
+            for manager in managers:
+                manager.__exit__(None, None, None)
+        return item
```

### Comparing `dlt-0.3.0/dlt/extract/schema.py` & `dlt-0.3.1a0/dlt/extract/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/extract/source.py` & `dlt-0.3.1a0/dlt/extract/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import warnings
 import contextlib
 from copy import copy
 import makefun
 import inspect
 from typing import AsyncIterable, AsyncIterator, ClassVar, Callable, ContextManager, Dict, Iterable, Iterator, List, Sequence, Tuple, Union, Any
+import types
 
 from dlt.common.configuration.resolve import inject_section
 from dlt.common.configuration.specs import known_sections
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.normalizers.json.relational import DataItemNormalizer as RelationalNormalizer, RelationalNormalizerConfigPropagation
 from dlt.common.schema import Schema
 from dlt.common.schema.typing import TColumnName
@@ -295,15 +296,15 @@
         else:
             self._bound = True
         return self
 
     @property
     def state(self) -> StrAny:
         """Gets resource-scoped state from the active pipeline. PipelineStateNotAvailable is raised if pipeline context is not available"""
-        with self._get_config_section_context():
+        with inject_section(self._get_config_section_context()):
             return resource_state(self.name)
 
     def clone(self, clone_pipe: bool = True, keep_pipe_id: bool = True) -> "DltResource":
         """Creates a deep copy of a current resource, optionally cloning also pipe. Note that name of a containing source will not be cloned."""
         pipe = self._pipe
         if self._pipe and not self._pipe.is_empty and clone_pipe:
             pipe = pipe._clone(keep_pipe_id=keep_pipe_id)
@@ -335,49 +336,43 @@
         """Opens iterator that yields the data items from the resources in the same order as in Pipeline class.
 
             A read-only state is provided, initialized from active pipeline state. The state is discarded after the iterator is closed.
         """
         # use the same state dict when opening iterator and when iterator is iterated
         container = Container()
         state, _ = pipeline_state(container, {})
+        state_context = StateInjectableContext(state=state)
+        section_context = self._get_config_section_context()
 
-        def _get_context() -> List[ContextManager[Any]]:
-            return [
-                self._get_config_section_context(),
-                Container().injectable_context(StateInjectableContext(state=state))
-            ]
-
-        # managed pipe iterator will remove injected contexts when closing
-        with multi_context_manager(_get_context()):
+        # managed pipe iterator will set the context on each call to  __next__
+        with inject_section(section_context), Container().injectable_context(state_context):
             pipe_iterator: ManagedPipeIterator = ManagedPipeIterator.from_pipes([self._pipe])  # type: ignore
 
-        pipe_iterator.set_context_manager(multi_context_manager(_get_context()))
+        pipe_iterator.set_context([state_context, section_context])
         _iter = map(lambda item: item.item, pipe_iterator)
         return flatten_list_or_items(_iter)
 
-    def _get_config_section_context(self) -> ContextManager[ConfigSectionContext]:
+    def _get_config_section_context(self) -> ConfigSectionContext:
         container = Container()
         proxy = container[PipelineContext]
         pipeline = None if not proxy.is_active() else proxy.pipeline()
         if pipeline:
             pipeline_name = pipeline.pipeline_name
         else:
             pipeline_name = None
         if pipeline:
             default_schema_name = pipeline.default_schema_name
         else:
             default_schema_name = None
         if not default_schema_name and pipeline_name:
             default_schema_name = pipeline._make_schema_with_default_name().name
-        return inject_section(
-            ConfigSectionContext(
-                pipeline_name=pipeline_name,
-                sections=(known_sections.SOURCES, self.section or default_schema_name or uniq_id(), self.source_name or default_schema_name or self._name),
-                source_state_key=self.source_name or default_schema_name or self.section or uniq_id()
-            )
+        return ConfigSectionContext(
+            pipeline_name=pipeline_name,
+            sections=(known_sections.SOURCES, self.section or default_schema_name or uniq_id(), self.source_name or default_schema_name or self._name),
+            source_state_key=self.source_name or default_schema_name or self.section or uniq_id()
         )
 
     def __str__(self) -> str:
         info = f"DltResource [{self._name}]"
         if self.section:
             info += f" in section [{self.section}]"
         if self.source_name:
@@ -564,15 +559,14 @@
     * You can get the `schema` for the source and all the resources within it.
     * You can use a `run` method to load the data with a default instance of dlt pipeline.
     * You can get source read only state for the currently active Pipeline instance
     """
     def __init__(self, name: str, section: str, schema: Schema, resources: Sequence[DltResource] = None) -> None:
         self.name = name
         self.section = section
-        self.exhausted = False
         """Tells if iterator associated with a source is exhausted"""
         self._schema = schema
         self._resources: DltResourceDict = DltResourceDict(self.name, self.section)
 
         if self.name != schema.name:
             # raise ValueError(f"Schema name {schema.name} differs from source name {name}! The explicit source name argument is deprecated and will be soon removed.")
             warnings.warn(f"Schema name {schema.name} differs from source name {name}! The explicit source name argument is deprecated and will be soon removed.")
@@ -605,20 +599,29 @@
         return RelationalNormalizer.get_normalizer_config(self._schema).get("max_nesting")
 
     @max_table_nesting.setter
     def max_table_nesting(self, value: int) -> None:
         RelationalNormalizer.update_normalizer_config(self._schema, {"max_nesting": value})
 
     @property
+    def exhausted(self) -> bool:
+        """check all selected pipes wether one of them has started. if so, the source is exhausted."""
+        for resource in self._resources.extracted.values():
+            item = resource._pipe.gen
+            if inspect.isgenerator(item):
+                if inspect.getgeneratorstate(item) != "GEN_CREATED":
+                    return True
+        return False
+
+    @property
     def root_key(self) -> bool:
         """Enables merging on all resources by propagating root foreign key to child tables. This option is most useful if you plan to change write disposition of a resource to disable/enable merge"""
         config = RelationalNormalizer.get_normalizer_config(self._schema).get("propagation")
         return config is not None and "root" in config and "_dlt_id" in config["root"] and config["root"]["_dlt_id"] == "_dlt_root_id"
 
-
     @root_key.setter
     def root_key(self, value: bool) -> None:
         if value is True:
             propagation_config: RelationalNormalizerConfigPropagation = {
                 "root": {
                     "_dlt_id": TColumnName("_dlt_root_id")
                 },
@@ -702,15 +705,15 @@
         """A convenience method that will call `run` run on the currently active `dlt` pipeline. If pipeline instance is not found, one with default settings will be created."""
         self_run: SupportsPipelineRun = makefun.partial(Container()[PipelineContext].pipeline().run, *(), data=self)
         return self_run
 
     @property
     def state(self) -> StrAny:
         """Gets source-scoped state from the active pipeline. PipelineStateNotAvailable is raised if no pipeline is active"""
-        with self._get_config_section_context():
+        with inject_section(self._get_config_section_context()):
             return source_state()
 
     def clone(self) -> "DltSource":
         """Creates a deep copy of the source where copies of schema, resources and pipes are created"""
         # mind that resources and pipes are cloned when added to the DltResourcesDict in the source constructor
         return DltSource(self.name, self.section, self.schema.clone(), list(self._resources.values()))
 
@@ -719,38 +722,31 @@
 
             A read-only state is provided, initialized from active pipeline state. The state is discarded after the iterator is closed.
 
             A source config section is injected to allow secrets/config injection as during regular extraction.
         """
         # use the same state dict when opening iterator and when iterator is iterated
         mock_state, _ = pipeline_state(Container(), {})
+        state_context = StateInjectableContext(state=mock_state)
+        section_context = self._get_config_section_context()
 
-        def _get_context() -> List[ContextManager[Any]]:
-            return [
-                self._get_config_section_context(),
-                Container().injectable_context(StateInjectableContext(state=mock_state))
-            ]
-
-        # managed pipe iterator will remove injected contexts when closing
-        with multi_context_manager(_get_context()):
+        # managed pipe iterator will set the context on each call to  __next__
+        with inject_section(section_context), Container().injectable_context(state_context):
             pipe_iterator: ManagedPipeIterator = ManagedPipeIterator.from_pipes(self._resources.selected_pipes)  # type: ignore
-        pipe_iterator.set_context_manager(multi_context_manager(_get_context()))
+        pipe_iterator.set_context([section_context, state_context])
         _iter = map(lambda item: item.item, pipe_iterator)
-        self.exhausted = True
         return flatten_list_or_items(_iter)
 
-    def _get_config_section_context(self) -> ContextManager[ConfigSectionContext]:
+    def _get_config_section_context(self) -> ConfigSectionContext:
         proxy = Container()[PipelineContext]
         pipeline_name = None if not proxy.is_active() else proxy.pipeline().pipeline_name
-        return inject_section(
-            ConfigSectionContext(
-                pipeline_name=pipeline_name,
-                sections=(known_sections.SOURCES, self.section, self.name),
-                source_state_key=self.name
-            )
+        return ConfigSectionContext(
+            pipeline_name=pipeline_name,
+            sections=(known_sections.SOURCES, self.section, self.name),
+            source_state_key=self.name
         )
 
     def _add_resource(self, name: str, resource: DltResource) -> None:
         if self.exhausted:
             raise SourceExhausted(self.name)
 
         if name in self._resources:
```

### Comparing `dlt-0.3.0/dlt/extract/typing.py` & `dlt-0.3.1a0/dlt/extract/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/extract/utils.py` & `dlt-0.3.1a0/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/helpers/airflow_helper.py` & `dlt-0.3.1a0/dlt/helpers/airflow_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/helpers/dbt/__init__.py` & `dlt-0.3.1a0/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/helpers/dbt/configuration.py` & `dlt-0.3.1a0/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.3.1a0/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/helpers/dbt/exceptions.py` & `dlt-0.3.1a0/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/helpers/dbt/profiles.yml` & `dlt-0.3.1a0/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/helpers/dbt/runner.py` & `dlt-0.3.1a0/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/helpers/pandas_helper.py` & `dlt-0.3.1a0/dlt/helpers/pandas_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/helpers/parquet.py` & `dlt-0.3.1a0/dlt/helpers/parquet.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/helpers/streamlit_helper.py` & `dlt-0.3.1a0/dlt/helpers/streamlit_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/load/configuration.py` & `dlt-0.3.1a0/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/load/exceptions.py` & `dlt-0.3.1a0/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/load/load.py` & `dlt-0.3.1a0/dlt/load/load.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/normalize/configuration.py` & `dlt-0.3.1a0/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/normalize/normalize.py` & `dlt-0.3.1a0/dlt/normalize/normalize.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/pipeline/__init__.py` & `dlt-0.3.1a0/dlt/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/pipeline/configuration.py` & `dlt-0.3.1a0/dlt/pipeline/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/pipeline/dbt.py` & `dlt-0.3.1a0/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/pipeline/exceptions.py` & `dlt-0.3.1a0/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/pipeline/helpers.py` & `dlt-0.3.1a0/dlt/pipeline/helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/pipeline/pipeline.py` & `dlt-0.3.1a0/dlt/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/pipeline/progress.py` & `dlt-0.3.1a0/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/pipeline/state_sync.py` & `dlt-0.3.1a0/dlt/pipeline/state_sync.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/pipeline/trace.py` & `dlt-0.3.1a0/dlt/pipeline/trace.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/pipeline/track.py` & `dlt-0.3.1a0/dlt/pipeline/track.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/reflection/names.py` & `dlt-0.3.1a0/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/reflection/script_inspector.py` & `dlt-0.3.1a0/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/reflection/script_visitor.py` & `dlt-0.3.1a0/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/sources/helpers/requests/__init__.py` & `dlt-0.3.1a0/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/sources/helpers/requests/retry.py` & `dlt-0.3.1a0/dlt/sources/helpers/requests/retry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/sources/helpers/requests/session.py` & `dlt-0.3.1a0/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/sources/helpers/transform.py` & `dlt-0.3.1a0/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/dlt/version.py` & `dlt-0.3.1a0/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.0/pyproject.toml` & `dlt-0.3.1a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.3.0"
+version = "0.3.1a0"
 description = "DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
```

### Comparing `dlt-0.3.0/setup.py` & `dlt-0.3.1a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
  's3': ['s3fs>=2023.5.0,<2024.0.0', 'boto3>=1.26']}
 
 entry_points = \
 {'console_scripts': ['dlt = dlt.cli._dlt:_main']}
 
 setup_kwargs = {
     'name': 'dlt',
-    'version': '0.3.0',
+    'version': '0.3.1a0',
     'description': 'DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.',
     'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nfrom chess import chess # a utility function that grabs data from the chess.com API\n\n# create a dlt pipeline that will load chess game data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'games_data\'\n)\n\n# use chess.com API to grab data about a few players\ndata = chess([\'magnuscarlsen\', \'rpragchess\'], start_month=\'2022/11\', end_month=\'2022/12\')\n\n# extract, normalize, and load the data\npipeline.run(data)\n```\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Sources and Destinations\n\nExplore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/verified-sources/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Verified Sources**: Contribute your custom sources to the [dlt-hub/verified-sources](https://github.com/dlt-hub/verified-sources) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
     'author': 'dltHub Inc.',
     'author_email': 'services@dlthub.com',
     'maintainer': 'Marcin Rudolf',
     'maintainer_email': 'marcin@dlthub.com',
     'url': 'https://github.com/dlt-hub',
```

### Comparing `dlt-0.3.0/PKG-INFO` & `dlt-0.3.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.3.0
+Version: 0.3.1a0
 Summary: DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
```

