# Comparing `tmp/vdk-core-0.3.896750818.tar.gz` & `tmp/vdk-core-0.3.899446293.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdk-core-0.3.896750818.tar", last modified: Mon Jun 12 08:43:34 2023, max compression
+gzip compressed data, was "dist/vdk-core-0.3.899446293.tar", last modified: Wed Jun 14 09:17:26 2023, max compression
```

## Comparing `vdk-core-0.3.896750818.tar` & `vdk-core-0.3.899446293.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2460 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1542 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1483 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      440 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/api/
--rw-rw-rw-   0 root         (0) root         (0)     2561 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/api/data_job.py
--rw-rw-rw-   0 root         (0) root         (0)    18539 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/api/job_input.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/api/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     6715 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/api/plugin/connection_hook_spec.py
--rw-rw-rw-   0 root         (0) root         (0)     7784 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/api/plugin/core_hook_spec.py
--rw-rw-rw-   0 root         (0) root         (0)     2586 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/api/plugin/hook_markers.py
--rw-rw-rw-   0 root         (0) root         (0)    25728 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/api/plugin/plugin_input.py
--rw-rw-rw-   0 root         (0) root         (0)     4057 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/api/plugin/plugin_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     3961 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/api/plugin/plugin_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/
--rw-rw-rw-   0 root         (0) root         (0)     5894 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/builtin_hook_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/config/
--rw-rw-rw-   0 root         (0) root         (0)     5112 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/config/config_help.py
--rw-rw-rw-   0 root         (0) root         (0)     9354 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/config/job_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11179 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/config/log_config.py
--rw-rw-rw-   0 root         (0) root         (0)    10141 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/config/vdk_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/
--rw-rw-rw-   0 root         (0) root         (0)     3123 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/connection_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1425 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/connection_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4661 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py
--rw-rw-rw-   0 root         (0) root         (0)     2316 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/execution_cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/impl/
--rw-rw-rw-   0 root         (0) root         (0)     6464 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/impl/router.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py
--rw-rw-rw-   0 root         (0) root         (0)    10056 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py
--rw-rw-rw-   0 root         (0) root         (0)    10048 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/managed_cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/pep249/
--rw-rw-rw-   0 root         (0) root         (0)     2958 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2274 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py
--rw-rw-rw-   0 root         (0) root         (0)     3980 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/debug/
--rw-rw-rw-   0 root         (0) root         (0)     5746 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/debug/debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/ingestion/
--rw-rw-rw-   0 root         (0) root         (0)    29371 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py
--rw-rw-rw-   0 root         (0) root         (0)     5646 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     4069 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)    13247 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py
--rw-rw-rw-   0 root         (0) root         (0)     4631 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1849 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/internal_hookspecs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/job_properties/
--rw-rw-rw-   0 root         (0) root         (0)      897 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py
--rw-rw-rw-   0 root         (0) root         (0)     3700 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2362 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/job_properties/properties_config.py
--rw-rw-rw-   0 root         (0) root         (0)     8208 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/job_properties/properties_router.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/notification/
--rw-rw-rw-   0 root         (0) root         (0)     4654 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/notification/notification.py
--rw-rw-rw-   0 root         (0) root         (0)    10656 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/notification/notification_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7985 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/notification/notification_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/
--rw-rw-rw-   0 root         (0) root         (0)     6225 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/cli_run.py
--rw-rw-rw-   0 root         (0) root         (0)    13573 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/execution_environment.py
--rw-rw-rw-   0 root         (0) root         (0)     5515 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/execution_results.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/execution_state.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/execution_tracking.py
--rw-rw-rw-   0 root         (0) root         (0)     7130 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/file_based_step.py
--rw-rw-rw-   0 root         (0) root         (0)     3911 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/job_context.py
--rw-rw-rw-   0 root         (0) root         (0)     7082 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/job_input.py
--rw-rw-rw-   0 root         (0) root         (0)     4856 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/run_status.py
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py
--rw-rw-rw-   0 root         (0) root         (0)     7959 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/standalone_data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/step.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3806 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/templates/template_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/termination_message/
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/termination_message/file_util.py
--rw-rw-rw-   0 root         (0) root         (0)     3119 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/termination_message/writer.py
--rw-rw-rw-   0 root         (0) root         (0)     1161 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/version/
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/version/new_version_check.py
--rw-rw-rw-   0 root         (0) root         (0)     4973 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2764 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/version/version.py
--rw-rw-rw-   0 root         (0) root         (0)     6471 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/cli_entry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/internal/core/
--rw-rw-rw-   0 root         (0) root         (0)     9586 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2355 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/core/context.py
--rw-rw-rw-   0 root         (0) root         (0)    21237 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/core/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     5683 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/core/statestore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/internal/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     5200 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/plugin/plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/plugin/plugin_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk/internal/util/
--rw-rw-rw-   0 root         (0) root         (0)     1234 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/util/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     2598 2023-06-12 08:43:11.000000 vdk-core-0.3.896750818/src/vdk/internal/util/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-06-12 08:43:32.000000 vdk-core-0.3.896750818/src/vdk/internal/vdk_build_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2460 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4333 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk_core.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk_core.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-12 08:43:34.000000 vdk-core-0.3.896750818/src/vdk_core.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-12 08:43:32.000000 vdk-core-0.3.896750818/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1542 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/api/
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/api/data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)    18539 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/api/job_input.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/api/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     6715 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/api/plugin/connection_hook_spec.py
+-rw-rw-rw-   0 root         (0) root         (0)     7784 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/api/plugin/core_hook_spec.py
+-rw-rw-rw-   0 root         (0) root         (0)     2586 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/api/plugin/hook_markers.py
+-rw-rw-rw-   0 root         (0) root         (0)    25728 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/api/plugin/plugin_input.py
+-rw-rw-rw-   0 root         (0) root         (0)     4057 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/api/plugin/plugin_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3961 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/api/plugin/plugin_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)     5894 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/builtin_hook_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/config/
+-rw-rw-rw-   0 root         (0) root         (0)     5112 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/config/config_help.py
+-rw-rw-rw-   0 root         (0) root         (0)     9354 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/config/job_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11179 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/config/log_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    10141 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/config/vdk_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/
+-rw-rw-rw-   0 root         (0) root         (0)     3123 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/connection_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/connection_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4661 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/execution_cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/impl/
+-rw-rw-rw-   0 root         (0) root         (0)     6464 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/impl/router.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10048 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/managed_cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/pep249/
+-rw-rw-rw-   0 root         (0) root         (0)     2958 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2274 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3980 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/debug/
+-rw-rw-rw-   0 root         (0) root         (0)     5746 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/debug/debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/ingestion/
+-rw-rw-rw-   0 root         (0) root         (0)    29371 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4069 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)    13247 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py
+-rw-rw-rw-   0 root         (0) root         (0)     4631 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/internal_hookspecs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/job_properties/
+-rw-rw-rw-   0 root         (0) root         (0)      897 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     3700 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2362 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/job_properties/properties_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8208 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/job_properties/properties_router.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/notification/
+-rw-rw-rw-   0 root         (0) root         (0)     4654 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/notification/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)    10656 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/notification/notification_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7985 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/notification/notification_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/
+-rw-rw-rw-   0 root         (0) root         (0)     9074 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/cli_run.py
+-rw-rw-rw-   0 root         (0) root         (0)    13573 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/execution_environment.py
+-rw-rw-rw-   0 root         (0) root         (0)     5515 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/execution_results.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/execution_state.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/execution_tracking.py
+-rw-rw-rw-   0 root         (0) root         (0)     7130 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/file_based_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     3911 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/job_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7082 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/job_input.py
+-rw-rw-rw-   0 root         (0) root         (0)     4856 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/run_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7959 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/standalone_data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3806 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/templates/template_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/termination_message/
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/termination_message/file_util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3119 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/termination_message/writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/version/
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/version/new_version_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     4973 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2764 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/version/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6471 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/cli_entry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/internal/core/
+-rw-rw-rw-   0 root         (0) root         (0)     9586 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/core/context.py
+-rw-rw-rw-   0 root         (0) root         (0)    21237 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/core/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5683 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/core/statestore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/internal/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     5200 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/plugin/plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/plugin/plugin_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk/internal/util/
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/util/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2598 2023-06-14 09:17:04.000000 vdk-core-0.3.899446293/src/vdk/internal/util/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-06-14 09:17:24.000000 vdk-core-0.3.899446293/src/vdk/internal/vdk_build_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk_core.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk_core.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-14 09:17:26.000000 vdk-core-0.3.899446293/src/vdk_core.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-14 09:17:24.000000 vdk-core-0.3.899446293/version.txt
```

### Comparing `vdk-core-0.3.896750818/PKG-INFO` & `vdk-core-0.3.899446293/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-core
-Version: 0.3.896750818
+Version: 0.3.899446293
 Summary: Versatile Data Kit SDK Core
 Home-page: https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Author: VMware Inc.
 Author-email: taurus@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/projects/vdk-core/README.md
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Platform: any
```

### Comparing `vdk-core-0.3.896750818/README.md` & `vdk-core-0.3.899446293/README.md`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/setup.cfg` & `vdk-core-0.3.899446293/setup.cfg`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/api/data_job.py` & `vdk-core-0.3.899446293/src/vdk/api/data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/api/job_input.py` & `vdk-core-0.3.899446293/src/vdk/api/job_input.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/api/plugin/connection_hook_spec.py` & `vdk-core-0.3.899446293/src/vdk/api/plugin/connection_hook_spec.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/api/plugin/core_hook_spec.py` & `vdk-core-0.3.899446293/src/vdk/api/plugin/core_hook_spec.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/api/plugin/hook_markers.py` & `vdk-core-0.3.899446293/src/vdk/api/plugin/hook_markers.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/api/plugin/plugin_input.py` & `vdk-core-0.3.899446293/src/vdk/api/plugin/plugin_input.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/api/plugin/plugin_registry.py` & `vdk-core-0.3.899446293/src/vdk/api/plugin/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/api/plugin/plugin_utils.py` & `vdk-core-0.3.899446293/src/vdk/api/plugin/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/builtin_hook_impl.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/builtin_hook_impl.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/config/config_help.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/config/config_help.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/config/job_config.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/config/job_config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/config/log_config.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/config/log_config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/config/vdk_config.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/config/vdk_config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/connection_hooks.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/connection_hooks.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/connection_plugin.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/connection_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/execution_cursor.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/execution_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/impl/router.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/impl/router.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/managed_cursor.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/managed_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/debug/debug.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/debug/debug.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/internal_hookspecs.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/internal_hookspecs.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/job_properties/properties_config.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/job_properties/properties_config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/job_properties/properties_router.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/job_properties/properties_router.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/notification/notification.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/notification/notification.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/notification/notification_base.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/notification/notification_base.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/notification/notification_configuration.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/notification/notification_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/cli_run.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/cli_run.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import json
 import logging
 import math
 import os
 import pathlib
+import re
+import sys
 from typing import cast
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import click
+from vdk.internal.builtin_plugins.config import vdk_config
+from vdk.internal.builtin_plugins.config.job_config import JobConfig
 from vdk.internal.builtin_plugins.run import job_input_error_classifier
 from vdk.internal.builtin_plugins.run.data_job import DataJobFactory
 from vdk.internal.builtin_plugins.run.execution_tracking import (
     ExecutionTrackingPlugin,
 )
 from vdk.internal.builtin_plugins.version import version
 from vdk.internal.core import errors
 from vdk.internal.core.context import CoreContext
+from vdk.internal.core.errors import VdkConfigurationError
 
 log = logging.getLogger(__name__)
 
 
 class CliRunImpl:
     def __init__(self, job_factory: DataJobFactory = None):
         self.__job_factory = job_factory if job_factory else DataJobFactory()
@@ -62,23 +67,76 @@
                 i if i < remainder else remainder
             ) + quotient * (0 if i < remainder else i - remainder)
             yield exec_steps[
                 subsequent_iteration : subsequent_iteration
                 + (quotient + 1 if i < remainder else quotient)
             ]
 
+    @staticmethod
+    def __warn_on_python_version_disparity(
+        context: CoreContext, job_directory: pathlib.Path
+    ):
+        log_config_type = context.configuration.get_value(vdk_config.LOG_CONFIG)
+        if log_config_type == "LOCAL":
+            # Get the local python installation's version.
+            python_env_version = sys.version_info
+            local_py_version = f"{python_env_version.major}.{python_env_version.minor}"
+
+            # Get the python_version set in the config.ini if any.
+            job_path = job_directory.resolve()
+            try:
+                config = JobConfig(data_job_path=job_path)
+            except VdkConfigurationError as e:
+                log.info(
+                    f"An exception occurred while loading job configuration. Error was {e}"
+                )
+                return
+            configured_python_version = config.get_python_version()
+
+            if not configured_python_version:
+                return
+
+            pattern = r"^\d+\.\d+"
+            version_match = re.match(pattern, configured_python_version)
+
+            if version_match:
+                extracted_configured_version = version_match.group()
+                if extracted_configured_version != local_py_version:
+                    log.warning(
+                        f"""
+                        {os.linesep + (' ' * 20) + ('*' * 80)}
+                        Python version ({configured_python_version}), set in the job's config.ini file, is different
+                        from the python version ({local_py_version}) used to execute the data job.
+                        WHAT: python_version is different from the version of the execution
+                        environment.
+                        WHY: The python_version set in the data job's config.ini file is
+                        different from the python version of the execution environment.
+                        CONSEQUENCES: Developing a data job with one python version, and
+                        using a different version for the deployed data job could lead to
+                        unexpected and hard to troubleshoot errors.
+                        COUNTERMEASURES: Please, make sure that the python version set in
+                        the python_version property of the config.ini file is the same as
+                        the python version of your execution environment.
+                        {os.linesep + (' ' * 20) + ('*' * 80)}
+                        """
+                    )
+
     def create_and_run_data_job(
         self,
         context: CoreContext,
         data_job_directory: pathlib.Path,
         arguments: Optional[str],
     ):
         log.info(f"Run job with directory {data_job_directory}")
         context.plugin_registry.load_plugin_with_hooks_impl(ExecutionTrackingPlugin())
 
+        self.__warn_on_python_version_disparity(
+            context=context, job_directory=data_job_directory
+        )
+
         job = self.__job_factory.new_datajob(
             data_job_directory=data_job_directory, core_context=context
         )
         args = self.__validate_and_parse_args(arguments)
 
         execution_result = None
         try:
```

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/data_job.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/execution_environment.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/execution_environment.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/execution_results.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/execution_results.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/execution_state.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/execution_state.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/execution_tracking.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/execution_tracking.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/file_based_step.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/file_based_step.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/job_context.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/job_context.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/job_input.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/job_input.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/standalone_data_job.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/standalone_data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/run/step.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/run/step.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/templates/template_impl.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/templates/template_impl.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/termination_message/file_util.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/termination_message/file_util.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/termination_message/writer.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/termination_message/writer.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/version/new_version_check.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/version/new_version_check.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/builtin_plugins/version/version.py` & `vdk-core-0.3.899446293/src/vdk/internal/builtin_plugins/version/version.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/cli_entry.py` & `vdk-core-0.3.899446293/src/vdk/internal/cli_entry.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/core/config.py` & `vdk-core-0.3.899446293/src/vdk/internal/core/config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/core/context.py` & `vdk-core-0.3.899446293/src/vdk/internal/core/context.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/core/errors.py` & `vdk-core-0.3.899446293/src/vdk/internal/core/errors.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/core/statestore.py` & `vdk-core-0.3.899446293/src/vdk/internal/core/statestore.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/plugin/plugin.py` & `vdk-core-0.3.899446293/src/vdk/internal/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/util/decorators.py` & `vdk-core-0.3.899446293/src/vdk/internal/util/decorators.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk/internal/util/utils.py` & `vdk-core-0.3.899446293/src/vdk/internal/util/utils.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.896750818/src/vdk_core.egg-info/PKG-INFO` & `vdk-core-0.3.899446293/src/vdk_core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-core
-Version: 0.3.896750818
+Version: 0.3.899446293
 Summary: Versatile Data Kit SDK Core
 Home-page: https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Author: VMware Inc.
 Author-email: taurus@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/projects/vdk-core/README.md
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Platform: any
```

### Comparing `vdk-core-0.3.896750818/src/vdk_core.egg-info/SOURCES.txt` & `vdk-core-0.3.899446293/src/vdk_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

