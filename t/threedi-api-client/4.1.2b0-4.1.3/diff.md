# Comparing `tmp/threedi-api-client-4.1.2b0.tar.gz` & `tmp/threedi-api-client-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi-api-client-4.1.2b0.tar", last modified: Mon Mar 13 09:38:53 2023, max compression
+gzip compressed data, was "threedi-api-client-4.1.3.tar", last modified: Wed Jun 14 17:55:30 2023, max compression
```

## Comparing `threedi-api-client-4.1.2b0.tar` & `threedi-api-client-4.1.3.tar`

### file list

```diff
@@ -1,516 +1,516 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:53.886650 threedi-api-client-4.1.2b0/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-03-13 09:38:53.886650 threedi-api-client-4.1.2b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:53.766650 threedi-api-client-4.1.2b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/docs/files.rst
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:53.766650 threedi-api-client-4.1.2b0/openapi_client/
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15187 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:53.766650 threedi-api-client-4.1.2b0/openapi_client/aio/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/aio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:53.766650 threedi-api-client-4.1.2b0/openapi_client/aio/api/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/aio/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25524 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/aio/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13242 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/aio/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/aio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:53.770650 threedi-api-client-4.1.2b0/openapi_client/aio/models/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/aio/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/aio/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:53.774650 threedi-api-client-4.1.2b0/openapi_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34135 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    45337 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/api/contracts_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    48688 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/api/files_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    46426 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/api/inpy_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23195 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/api/organisations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33045 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/api/permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    57628 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/api/repositories_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    60230 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/api/revisions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/api/roles_api.py
--rw-r--r--   0 runner    (1001) docker     (123)  2103601 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/api/simulations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    61145 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/api/statuses_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   433273 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/api/threedimodels_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    51322 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/api/usage_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25427 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:53.818650 threedi-api-client-4.1.2b0/openapi_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    13775 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/aggregation_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/arrival_time_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/base_event_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/basic_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/boundary_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)    15799 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/breach.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/breach_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/breach_graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    15252 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/constant_lateral.py
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/constant_leakage.py
--rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/constant_local_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/constant_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/constant_sources_sinks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/constant_wind.py
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/current_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/damage_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/damage_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/extent.py
--rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/file_boundary_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/file_lateral.py
--rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/file_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    18364 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/file_raster_leakage.py
--rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/file_raster_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    18704 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/file_raster_sources_sinks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/file_read_only.py
--rw-r--r--   0 runner    (1001) docker     (123)    16650 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/file_timeseries_leakage.py
--rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/file_timeseries_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/file_timeseries_sources_sinks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/grid_event_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/ground_water_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/ground_water_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/initial_saved_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/initial_saved_state_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/initial_waterlevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response200.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response2001.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20010.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20011.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20012.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20013.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20014.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20015.py
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20016.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20017.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20018.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20019.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response2002.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20020.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20021.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20022.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20023.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20024.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20025.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20026.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20027.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20028.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20029.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response2003.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20030.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20031.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20032.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20033.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20034.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20035.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20036.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20037.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20038.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20039.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response2004.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20040.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20041.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20042.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20043.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20044.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20045.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20046.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20047.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20048.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20049.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response2005.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20050.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20051.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20052.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20053.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20054.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20055.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20056.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20057.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20058.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20059.py
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response2006.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20060.py
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response20061.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response2007.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response2008.py
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inline_response2009.py
--rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/inpy_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16461 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/lateral.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/linestring.py
--rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/lizard_raster_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    14807 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/lizard_raster_sources_sinks.py
--rw-r--r--   0 runner    (1001) docker     (123)    14188 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/lizard_timeseries_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/lizard_timeseries_sources_sinks.py
--rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/local_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/measure_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/measure_location_grid_event_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/measure_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    21660 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/memory_structure_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/net_cdf_raster_leakage.py
--rw-r--r--   0 runner    (1001) docker     (123)    16743 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/net_cdf_raster_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    17816 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/net_cdf_raster_sources_sinks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15750 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/net_cdf_timeseries_leakage.py
--rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/net_cdf_timeseries_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    16030 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/net_cdf_timeseries_sources_sinks.py
--rw-r--r--   0 runner    (1001) docker     (123)    44234 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/numerical_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/one_d_water_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/one_d_water_level_predefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/organisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/organisation_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/physical_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/post_processing_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/post_processing_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/post_processing_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    10682 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/potential_breach.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/pump_discharge_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/pump_discharge_graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/raster_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/raster_edit_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    31886 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/raster_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/result_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/saved_state_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/simulation_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/simulation_settings_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/simulation_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/simulation_status_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/simulation_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/stable_threshold_saved_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/table_structure_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    26110 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/threedi_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/threedi_model_saved_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/time_step_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/timed_saved_state_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    16698 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/timed_structure_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14768 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/timeseries_lateral.py
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/timeseries_leakage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/timeseries_leakage_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)    12462 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/timeseries_local_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/timeseries_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/timeseries_rain_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/timeseries_sources_sinks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/timeseries_sources_sinks_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/timeseries_wind.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/tms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/two_d_water_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/two_d_water_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/upload_event_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/usage_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/water_flow_graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/water_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/water_level_graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/water_level_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/water_level_profile_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/waterdepth.py
--rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/wind.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/models/wind_drag_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)    12662 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/openapi_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-13 09:38:53.886650 threedi-api-client-4.1.2b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:53.818650 threedi-api-client-4.1.2b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/tests/test_files_aio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/tests/test_threedi_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/tests/test_threedi_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/tests/test_threedi_api_client_aio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:53.822650 threedi-api-client-4.1.2b0/threedi_api_client/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:53.822650 threedi-api-client-4.1.2b0/threedi_api_client/aio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/aio/aiohttp_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19517 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/aio/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:53.826650 threedi-api-client-4.1.2b0/threedi_api_client/aio/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/aio/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26560 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/aio/openapi/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/aio/openapi/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/aio/openapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:53.826650 threedi-api-client-4.1.2b0/threedi_api_client/aio/openapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/aio/openapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/aio/openapi/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/aio/threedi_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13822 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:53.826650 threedi-api-client-4.1.2b0/threedi_api_client/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:53.830650 threedi-api-client-4.1.2b0/threedi_api_client/openapi/api/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  3446215 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/api/v3_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    92592 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/api/v3_beta_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26463 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:53.886650 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)    19035 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/aggregation_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/arrival_time_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/base_event_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/basic_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/boundary_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/breach.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/breach_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/breach_graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9830 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/constant_lateral.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/constant_leakage.py
--rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/constant_local_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/constant_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/constant_sources_sinks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17132 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/constant_wind.py
--rw-r--r--   0 runner    (1001) docker     (123)    13943 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/copy_to_threedi_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/create_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/create_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/current_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/current_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/damage_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/damage_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/destroy_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    34917 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/extent.py
--rw-r--r--   0 runner    (1001) docker     (123)    16293 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_boundary_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_lateral.py
--rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    18279 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_raster_leakage.py
--rw-r--r--   0 runner    (1001) docker     (123)    18075 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_raster_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_raster_sources_sinks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_read_only.py
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_structure_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    16634 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_timeseries_leakage.py
--rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_timeseries_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_timeseries_sources_sinks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/from_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/grid_event_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/ground_water_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/ground_water_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/initial_saved_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/initial_saved_state_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/initial_waterlevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response200.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2001.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20010.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20011.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20012.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20013.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20014.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20015.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20016.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20017.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20018.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20019.py
--rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2002.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20020.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20021.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20022.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20023.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20024.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20025.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20026.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20027.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20028.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20029.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2003.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20030.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20031.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20032.py
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20033.py
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20034.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20035.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20036.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20037.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20038.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20039.py
--rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2004.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20040.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20041.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20042.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20043.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20044.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20045.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20046.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20047.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20048.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20049.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2005.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20050.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20051.py
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20052.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20053.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20054.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20055.py
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20056.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20057.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20058.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20059.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2006.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20060.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20061.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20062.py
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20063.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20064.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20065.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20066.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20067.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20068.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20069.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2007.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20070.py
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20071.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20072.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2008.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2009.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inpy_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16495 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/lateral.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/linestring.py
--rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/lizard_raster_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/lizard_raster_sources_sinks.py
--rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/lizard_timeseries_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/lizard_timeseries_sources_sinks.py
--rw-r--r--   0 runner    (1001) docker     (123)    14352 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/local_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/measure_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/measure_location_grid_event_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/measure_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    21309 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/memory_structure_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    17462 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/net_cdf_raster_leakage.py
--rw-r--r--   0 runner    (1001) docker     (123)    16717 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/net_cdf_raster_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/net_cdf_raster_sources_sinks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/net_cdf_timeseries_leakage.py
--rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/net_cdf_timeseries_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/net_cdf_timeseries_sources_sinks.py
--rw-r--r--   0 runner    (1001) docker     (123)    48436 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/numerical_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/obstacle_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/one_d_water_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/one_d_water_level_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/one_d_water_level_predefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/organisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/organisation_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/organisation_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/organisation_user_role_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/personal_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/personal_api_key_with_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/physical_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/post_processing_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/post_processing_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/post_processing_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/potential_breach.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/pump_discharge_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/pump_discharge_graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/rain_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/rain_graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/raster_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/raster_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/raster_edit_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    30720 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/raster_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/result_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/revision.py
--rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/revision_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/revision_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/saved_state_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)    16381 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/schematisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16168 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/schematisation_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/simulation_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/simulation_settings_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)    15971 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/simulation_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/simulation_status_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19645 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/simulation_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/sqlite_file_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/stable_threshold_saved_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/table_structure_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    29939 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/threedi_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/threedi_model_saved_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/threedi_model_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/time_step_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timed_saved_state_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    16437 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timed_structure_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_lateral.py
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_leakage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_leakage_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_local_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_rain_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_sources_sinks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_sources_sinks_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_wind.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/tms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/two_d_water_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/two_d_water_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/upload_event_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/usage_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/user_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/water_flow_graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/water_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/water_level_graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/water_level_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/water_level_profile_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/waterdepth.py
--rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/wind.py
--rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/wind_drag_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/openapi/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/threedi_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-13 09:38:49.000000 threedi-api-client-4.1.2b0/threedi_api_client/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:38:53.822650 threedi-api-client-4.1.2b0/threedi_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-03-13 09:38:53.000000 threedi-api-client-4.1.2b0/threedi_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23477 2023-03-13 09:38:53.000000 threedi-api-client-4.1.2b0/threedi_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 09:38:53.000000 threedi-api-client-4.1.2b0/threedi_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 09:38:53.000000 threedi-api-client-4.1.2b0/threedi_api_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-13 09:38:53.000000 threedi-api-client-4.1.2b0/threedi_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-13 09:38:53.000000 threedi-api-client-4.1.2b0/threedi_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:30.654161 threedi-api-client-4.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13339 2023-06-14 17:55:30.654161 threedi-api-client-4.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:30.518191 threedi-api-client-4.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/docs/files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:30.518191 threedi-api-client-4.1.3/openapi_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15187 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:30.522190 threedi-api-client-4.1.3/openapi_client/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/aio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:30.522190 threedi-api-client-4.1.3/openapi_client/aio/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/aio/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25524 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/aio/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13242 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/aio/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/aio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:30.522190 threedi-api-client-4.1.3/openapi_client/aio/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/aio/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/aio/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:30.530188 threedi-api-client-4.1.3/openapi_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34135 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45337 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/api/contracts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48688 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/api/files_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46426 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/api/inpy_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23195 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/api/organisations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33045 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/api/permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57628 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/api/repositories_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60230 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/api/revisions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/api/roles_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2103601 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/api/simulations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61145 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/api/statuses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   433273 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/api/threedimodels_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51322 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/api/usage_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25427 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:30.574179 threedi-api-client-4.1.3/openapi_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    13775 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/aggregation_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/arrival_time_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/base_event_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/basic_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/boundary_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15799 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/breach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/breach_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/breach_graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15252 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/constant_lateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/constant_leakage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/constant_local_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/constant_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/constant_sources_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/constant_wind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/current_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/damage_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/damage_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/extent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/file_boundary_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/file_lateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/file_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18364 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/file_raster_leakage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/file_raster_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18704 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/file_raster_sources_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/file_read_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16650 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/file_timeseries_leakage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/file_timeseries_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/file_timeseries_sources_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/grid_event_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/ground_water_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/ground_water_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/initial_saved_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/initial_saved_state_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/initial_waterlevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response2001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20010.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20011.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20012.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20013.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20014.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20015.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20016.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20018.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20020.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20021.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20022.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20023.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20025.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20026.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20027.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20028.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20029.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20030.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20031.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20032.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20033.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20034.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20035.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20036.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20037.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20038.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20039.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response2004.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20040.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20041.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20042.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20043.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20044.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20045.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20046.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20047.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20049.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response2005.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20050.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20051.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20052.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20053.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20054.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20055.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20056.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20057.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20058.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20059.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response2006.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20060.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response20061.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response2007.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response2008.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inline_response2009.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/inpy_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16461 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/lateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/linestring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/lizard_raster_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14807 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/lizard_raster_sources_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14188 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/lizard_timeseries_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/lizard_timeseries_sources_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/local_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/measure_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/measure_location_grid_event_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/measure_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21660 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/memory_structure_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/net_cdf_raster_leakage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16743 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/net_cdf_raster_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17816 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/net_cdf_raster_sources_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15750 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/net_cdf_timeseries_leakage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/net_cdf_timeseries_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16030 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/net_cdf_timeseries_sources_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44234 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/numerical_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/one_d_water_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/one_d_water_level_predefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/organisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/organisation_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/physical_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/post_processing_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/post_processing_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/post_processing_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10682 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/potential_breach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/pump_discharge_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/pump_discharge_graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/raster_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/raster_edit_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31886 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/raster_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/result_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/saved_state_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/simulation_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/simulation_settings_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/simulation_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/simulation_status_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/simulation_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/stable_threshold_saved_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/table_structure_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26110 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/threedi_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/threedi_model_saved_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/time_step_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/timed_saved_state_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16698 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/timed_structure_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14768 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/timeseries_lateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/timeseries_leakage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/timeseries_leakage_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12462 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/timeseries_local_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/timeseries_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/timeseries_rain_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/timeseries_sources_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/timeseries_sources_sinks_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/timeseries_wind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/tms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/two_d_water_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/two_d_water_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/upload_event_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/usage_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/water_flow_graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/water_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/water_level_graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/water_level_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/water_level_profile_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/waterdepth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/wind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/models/wind_drag_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12662 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/openapi_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-14 17:55:30.654161 threedi-api-client-4.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:30.574179 threedi-api-client-4.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/tests/test_files_aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/tests/test_threedi_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/tests/test_threedi_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/tests/test_threedi_api_client_aio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:30.578178 threedi-api-client-4.1.3/threedi_api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:30.578178 threedi-api-client-4.1.3/threedi_api_client/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/aio/aiohttp_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19517 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/aio/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:30.578178 threedi-api-client-4.1.3/threedi_api_client/aio/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/aio/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26560 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/aio/openapi/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/aio/openapi/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/aio/openapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:30.578178 threedi-api-client-4.1.3/threedi_api_client/aio/openapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/aio/openapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/aio/openapi/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/aio/threedi_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13822 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:30.582177 threedi-api-client-4.1.3/threedi_api_client/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:30.586176 threedi-api-client-4.1.3/threedi_api_client/openapi/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  3447091 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/api/v3_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92552 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/api/v3_beta_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26463 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:30.654161 threedi-api-client-4.1.3/threedi_api_client/openapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    19035 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/aggregation_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/arrival_time_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/base_event_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/basic_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/boundary_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/breach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/breach_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/breach_graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9830 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/constant_lateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/constant_leakage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/constant_local_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/constant_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/constant_sources_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17132 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/constant_wind.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14616 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/copy_to_threedi_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/create_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/create_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/current_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/current_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/damage_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/damage_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/destroy_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34917 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/extent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16293 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_boundary_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_lateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18279 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_raster_leakage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18075 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_raster_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_raster_sources_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_read_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_structure_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16634 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_timeseries_leakage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_timeseries_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_timeseries_sources_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/from_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/grid_event_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/ground_water_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/ground_water_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/initial_saved_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/initial_saved_state_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/initial_waterlevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20010.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20011.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20012.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20013.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20014.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20015.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20016.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20018.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20020.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20021.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20022.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20023.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20025.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20026.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20027.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20028.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20029.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20030.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20031.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20032.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20033.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20034.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20035.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20036.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20037.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20038.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20039.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2004.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20040.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20041.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20042.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20043.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20044.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20045.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20046.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20047.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20049.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2005.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20050.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20051.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20052.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20053.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20054.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20055.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20056.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20057.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20058.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20059.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2006.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20060.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20061.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20062.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20063.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20064.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20065.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20066.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20067.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20068.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20069.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2007.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20070.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20071.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20072.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2008.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2009.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/inpy_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16495 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/lateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/linestring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/lizard_raster_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/lizard_raster_sources_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/lizard_timeseries_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/lizard_timeseries_sources_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14352 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/local_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/measure_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/measure_location_grid_event_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/measure_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21309 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/memory_structure_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17462 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/net_cdf_raster_leakage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16717 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/net_cdf_raster_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/net_cdf_raster_sources_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/net_cdf_timeseries_leakage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/net_cdf_timeseries_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/net_cdf_timeseries_sources_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48436 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/numerical_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10845 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/obstacle_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/one_d_water_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/one_d_water_level_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/one_d_water_level_predefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/organisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/organisation_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/organisation_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/organisation_user_role_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/personal_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/personal_api_key_with_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/physical_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/post_processing_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/post_processing_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/post_processing_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/potential_breach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/pump_discharge_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/pump_discharge_graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/rain_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/rain_graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/raster_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/raster_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/raster_edit_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37474 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/raster_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/result_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/revision_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/revision_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/saved_state_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16381 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/schematisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16168 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/schematisation_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/simulation_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/simulation_settings_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20123 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/simulation_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/simulation_status_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19645 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/simulation_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/sqlite_file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/stable_threshold_saved_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/table_structure_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29939 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/threedi_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/threedi_model_saved_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/threedi_model_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/time_step_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/timed_saved_state_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16437 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/timed_structure_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_lateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_leakage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_leakage_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_local_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_rain_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_sources_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_sources_sinks_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_wind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/tms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/two_d_water_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/two_d_water_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/upload_event_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/usage_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/user_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/water_flow_graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/water_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/water_level_graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/water_level_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/water_level_profile_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/waterdepth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/wind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/models/wind_drag_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/openapi/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/threedi_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-14 17:55:20.000000 threedi-api-client-4.1.3/threedi_api_client/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:55:30.578178 threedi-api-client-4.1.3/threedi_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13339 2023-06-14 17:55:30.000000 threedi-api-client-4.1.3/threedi_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23477 2023-06-14 17:55:30.000000 threedi-api-client-4.1.3/threedi_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 17:55:30.000000 threedi-api-client-4.1.3/threedi_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 17:55:30.000000 threedi-api-client-4.1.3/threedi_api_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-14 17:55:30.000000 threedi-api-client-4.1.3/threedi_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 17:55:30.000000 threedi-api-client-4.1.3/threedi_api_client.egg-info/top_level.txt
```

### Comparing `threedi-api-client-4.1.2b0/CONTRIBUTING.rst` & `threedi-api-client-4.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/HISTORY.rst` & `threedi-api-client-4.1.3/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 =======
 History
 =======
 
+4.1.3 (2023-06-14)
+------------------
+
+- Release 3.2.34
+- Build the release with the build package instead of setuptools.
+- Rewrite release workflow to use a supported github action for github release.
+
+
+4.1.2 (2023-04-25)
+------------------
+
+- Public release.
+
+
 4.1.2b (2023-03-13)
 -------------------
 
 - Updated to framework release 3.2.6
 
 - Fix timeout when retrying uploads.
```

### Comparing `threedi-api-client-4.1.2b0/LICENSE` & `threedi-api-client-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/PKG-INFO` & `threedi-api-client-4.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-api-client
-Version: 4.1.2b0
+Version: 4.1.3
 Summary: client for the threedi API
 Home-page: https://github.com/nens/threedi-api-client
 Author: Lars Claussen
 Author-email: lars.claussen@nelen-schuurmans.nl
 License: BSD license
 Keywords: threedi-api-client
 Classifier: Development Status :: 4 - Beta
@@ -70,14 +70,28 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+4.1.3 (2023-06-14)
+------------------
+
+- Release 3.2.34
+- Build the release with the build package instead of setuptools.
+- Rewrite release workflow to use a supported github action for github release.
+
+
+4.1.2 (2023-04-25)
+------------------
+
+- Public release.
+
+
 4.1.2b (2023-03-13)
 -------------------
 
 - Updated to framework release 3.2.6
 
 - Fix timeout when retrying uploads.
```

### Comparing `threedi-api-client-4.1.2b0/README.rst` & `threedi-api-client-4.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/docs/Makefile` & `threedi-api-client-4.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/docs/conf.py` & `threedi-api-client-4.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/docs/examples.rst` & `threedi-api-client-4.1.3/docs/examples.rst`

 * *Files 4% similar despite different names*

```diff
@@ -135,51 +135,38 @@
                    'offset': 60,
                    'simulation': 'https://api.3di.live/v3.0/simulations/631/',
                    'units': 'm/s',
                    'url': 'https://api.3di.live/v3.0/simulations/631/events/rain/timeseries/17/',
                    'values': [[0.0, 0.0006], [5000.0, 0.0]]}],
    'timeseriessourcessinks': []}
 
-To list all file resources, make use of the ``files_list`` method.
-
-.. code:: python
-
-       api.files_list()                                                                                                                
-       {'count': 3064,
-       'next': 'https://api.3di.live/v3.0/files/?limit=10&offset=10',
-       'previous': None,
-       'results': [{'bucket': '3di',
-               'etag': None,
-               'expiry_date': '2019-08-16',
-               'filename': 'precipitation_1.nc',
-               'id': 2,
-               ..
 
 Advanced usage
 ~~~~~~~~~~~~~~
 
 See below for an example of uploading a rain raster.
 
 .. code:: python
 
+   from pathlib import Path
    from threedi_api_client.files import upload_file
 
    simulation_pk = 1
    filename = 'bergermeer_rasters_from_geotiffs.nc'
-   local_file_path = './data/bergermeer_rasters_from_geotiffs.nc'
+   local_file_path = Path('./data/bergermeer_rasters_from_geotiffs.nc')
 
    # Create rain raster upload resource in API
    # returns a 'file_upload' instance containing a
    # put_url property which is the URL to the object
    # storage object to be uploaded with an HTTP PUT requests.
    file_upload = api.simulations_events_rain_rasters_upload(
        filename, simulation_pk)
 
    # Upload the file
-   upload_file(local_file_path, file_upload.put_url)
+   upload_file(file_upload.put_url, local_file_path)
 
 
 Async client
 ~~~~~~~~~~~~
 
 This project also provides an asynchronous api client. To use
 the async-client make sure you install the optional dependencies using
@@ -189,25 +176,24 @@
 
 For example, to asynchronously request files from the api:
 
 .. code:: python
 
    import asyncio
 
-   from threedi_api_client import ThreediApi
-
+   from threedi_api_client.api import ThreediApi
+   from threedi_api_client.openapi.api.v3_api import V3Api
 
    config = {
-       "THREEDI_API_HOST": "https://api.3di.live/v3.0",
-       "THREEDI_API_USERNAME": "black.sheep",
-       "THREEDI_API_PASSWORD": "myverysecretmehhh"
+       "THREEDI_API_HOST": "https://api.3di.live",
+       "THREEDI_API_PERSONAL_API_TOKEN": "your_personal_api_token_here"
    }
 
 
    async def main():
        async with ThreediApi(config=config) as api_client:
-           api = V3Api(api_client)
-           print(await api.files_list())
+           api_client: V3Api
+           print(await api_client.files_list())
 
 
    if __name__ == '__main__':
        asyncio.run(main())
```

### Comparing `threedi-api-client-4.1.2b0/docs/make.bat` & `threedi-api-client-4.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/docs/usage.rst` & `threedi-api-client-4.1.3/docs/usage.rst`

 * *Files 9% similar despite different names*

```diff
@@ -53,14 +53,13 @@
 Applying the changes listed above, it is refactored to this:
 
 .. code:: python
 
     from threedi_api_client import ThreediApi
 
     config = {
-        "THREEDI_API_HOST": "https://api.3di.live"  # no version!
-        "THREEDI_API_USERNAME": "your.username"
-        "THREEDI_API_PASSWORD": "your.password"
+        "THREEDI_API_HOST": "https://api.3di.live",  # no version!
+        "THREEDI_API_PERSONAL_API_TOKEN": "your_personal_api_token_here"
     }
 
     with ThreediApi(config=config) as api:
         result = api.simulations_list()
```

### Comparing `threedi-api-client-4.1.2b0/openapi_client/LICENSE` & `threedi-api-client-4.1.3/openapi_client/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/__init__.py` & `threedi-api-client-4.1.3/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/aio/__init__.py` & `threedi-api-client-4.1.3/openapi_client/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/aio/api_client.py` & `threedi-api-client-4.1.3/openapi_client/aio/api_client.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/aio/configuration.py` & `threedi-api-client-4.1.3/openapi_client/aio/configuration.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/aio/exceptions.py` & `threedi-api-client-4.1.3/openapi_client/aio/exceptions.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/aio/rest.py` & `threedi-api-client-4.1.3/openapi_client/aio/rest.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/api/__init__.py` & `threedi-api-client-4.1.3/openapi_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/api/auth_api.py` & `threedi-api-client-4.1.3/openapi_client/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/api/contracts_api.py` & `threedi-api-client-4.1.3/openapi_client/api/contracts_api.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/api/files_api.py` & `threedi-api-client-4.1.3/openapi_client/api/files_api.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/api/inpy_versions_api.py` & `threedi-api-client-4.1.3/openapi_client/api/inpy_versions_api.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/api/organisations_api.py` & `threedi-api-client-4.1.3/openapi_client/api/organisations_api.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/api/permissions_api.py` & `threedi-api-client-4.1.3/openapi_client/api/permissions_api.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/api/repositories_api.py` & `threedi-api-client-4.1.3/openapi_client/api/repositories_api.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/api/revisions_api.py` & `threedi-api-client-4.1.3/openapi_client/api/revisions_api.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/api/roles_api.py` & `threedi-api-client-4.1.3/openapi_client/api/roles_api.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/api/simulations_api.py` & `threedi-api-client-4.1.3/openapi_client/api/simulations_api.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/api/statuses_api.py` & `threedi-api-client-4.1.3/openapi_client/api/statuses_api.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/api/threedimodels_api.py` & `threedi-api-client-4.1.3/openapi_client/api/threedimodels_api.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/api/usage_api.py` & `threedi-api-client-4.1.3/openapi_client/api/usage_api.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/api_client.py` & `threedi-api-client-4.1.3/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/configuration.py` & `threedi-api-client-4.1.3/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/exceptions.py` & `threedi-api-client-4.1.3/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/__init__.py` & `threedi-api-client-4.1.3/openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/action.py` & `threedi-api-client-4.1.3/openapi_client/models/action.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/aggregation_settings.py` & `threedi-api-client-4.1.3/openapi_client/models/aggregation_settings.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/arrival_time_post_processing.py` & `threedi-api-client-4.1.3/openapi_client/models/arrival_time_post_processing.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/authenticate.py` & `threedi-api-client-4.1.3/openapi_client/models/authenticate.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/base_event_state.py` & `threedi-api-client-4.1.3/openapi_client/models/base_event_state.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/basic_post_processing.py` & `threedi-api-client-4.1.3/openapi_client/models/basic_post_processing.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/boundary_condition.py` & `threedi-api-client-4.1.3/openapi_client/models/boundary_condition.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/breach.py` & `threedi-api-client-4.1.3/openapi_client/models/breach.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/breach_graph.py` & `threedi-api-client-4.1.3/openapi_client/models/breach_graph.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/breach_graph_request.py` & `threedi-api-client-4.1.3/openapi_client/models/breach_graph_request.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/constant_lateral.py` & `threedi-api-client-4.1.3/openapi_client/models/constant_lateral.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/constant_leakage.py` & `threedi-api-client-4.1.3/openapi_client/models/constant_leakage.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/constant_local_rain.py` & `threedi-api-client-4.1.3/openapi_client/models/constant_local_rain.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/constant_rain.py` & `threedi-api-client-4.1.3/openapi_client/models/constant_rain.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/constant_sources_sinks.py` & `threedi-api-client-4.1.3/openapi_client/models/constant_sources_sinks.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/constant_wind.py` & `threedi-api-client-4.1.3/openapi_client/models/constant_wind.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/contract.py` & `threedi-api-client-4.1.3/openapi_client/models/contract.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/current_status.py` & `threedi-api-client-4.1.3/openapi_client/models/current_status.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/damage_estimation.py` & `threedi-api-client-4.1.3/openapi_client/models/damage_estimation.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/damage_post_processing.py` & `threedi-api-client-4.1.3/openapi_client/models/damage_post_processing.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/download.py` & `threedi-api-client-4.1.3/openapi_client/models/download.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/event.py` & `threedi-api-client-4.1.3/openapi_client/models/event.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/extent.py` & `threedi-api-client-4.1.3/openapi_client/models/extent.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/file.py` & `threedi-api-client-4.1.3/openapi_client/models/file.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/file_boundary_condition.py` & `threedi-api-client-4.1.3/openapi_client/models/file_boundary_condition.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/file_lateral.py` & `threedi-api-client-4.1.3/openapi_client/models/file_lateral.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/file_meta.py` & `threedi-api-client-4.1.3/openapi_client/models/file_meta.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/file_raster_leakage.py` & `threedi-api-client-4.1.3/openapi_client/models/file_raster_leakage.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/file_raster_rain.py` & `threedi-api-client-4.1.3/openapi_client/models/file_raster_rain.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/file_raster_sources_sinks.py` & `threedi-api-client-4.1.3/openapi_client/models/file_raster_sources_sinks.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/file_read_only.py` & `threedi-api-client-4.1.3/openapi_client/models/file_read_only.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/file_timeseries_leakage.py` & `threedi-api-client-4.1.3/openapi_client/models/file_timeseries_leakage.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/file_timeseries_rain.py` & `threedi-api-client-4.1.3/openapi_client/models/file_timeseries_rain.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/file_timeseries_sources_sinks.py` & `threedi-api-client-4.1.3/openapi_client/models/file_timeseries_sources_sinks.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/grid_event_state.py` & `threedi-api-client-4.1.3/openapi_client/models/grid_event_state.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/ground_water_level.py` & `threedi-api-client-4.1.3/openapi_client/models/ground_water_level.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/ground_water_raster.py` & `threedi-api-client-4.1.3/openapi_client/models/ground_water_raster.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/initial_saved_state.py` & `threedi-api-client-4.1.3/openapi_client/models/initial_saved_state.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/initial_saved_state_overview.py` & `threedi-api-client-4.1.3/openapi_client/models/initial_saved_state_overview.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/initial_waterlevel.py` & `threedi-api-client-4.1.3/openapi_client/models/initial_waterlevel.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response200.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response2001.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20010.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20010.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20011.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20011.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20012.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20012.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20013.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20013.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20014.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20014.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20015.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20015.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20016.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20016.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20017.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20017.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20018.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20018.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20019.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20019.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response2002.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20020.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20020.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20021.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20021.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20022.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20022.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20023.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20023.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20024.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20024.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20025.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20025.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20026.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20026.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20027.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20027.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20028.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20028.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20029.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20029.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response2003.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response2003.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20030.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20030.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20031.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20031.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20032.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20032.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20033.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20033.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20034.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20034.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20035.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20035.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20036.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20036.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20037.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20037.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20038.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20038.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20039.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20039.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response2004.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response2004.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20040.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20040.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20041.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20041.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20042.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20042.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20043.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20043.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20044.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20044.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20045.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20045.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20046.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20046.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20047.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20047.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20048.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20048.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20049.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20049.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response2005.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response2005.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20050.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20050.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20051.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20051.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20052.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20052.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20053.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20053.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20054.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20054.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20055.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20055.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20056.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20056.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20057.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20057.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20058.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20058.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20059.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20059.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response2006.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response2006.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20060.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20060.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response20061.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response20061.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response2007.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response2007.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response2008.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response2008.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inline_response2009.py` & `threedi-api-client-4.1.3/openapi_client/models/inline_response2009.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/inpy_version.py` & `threedi-api-client-4.1.3/openapi_client/models/inpy_version.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/lateral.py` & `threedi-api-client-4.1.3/openapi_client/models/lateral.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/linestring.py` & `threedi-api-client-4.1.3/openapi_client/models/linestring.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/lizard_raster_rain.py` & `threedi-api-client-4.1.3/openapi_client/models/lizard_raster_rain.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/lizard_raster_sources_sinks.py` & `threedi-api-client-4.1.3/openapi_client/models/lizard_raster_sources_sinks.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/lizard_timeseries_rain.py` & `threedi-api-client-4.1.3/openapi_client/models/lizard_timeseries_rain.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/lizard_timeseries_sources_sinks.py` & `threedi-api-client-4.1.3/openapi_client/models/lizard_timeseries_sources_sinks.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/local_rain.py` & `threedi-api-client-4.1.3/openapi_client/models/local_rain.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/measure_location.py` & `threedi-api-client-4.1.3/openapi_client/models/measure_location.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/measure_location_grid_event_state.py` & `threedi-api-client-4.1.3/openapi_client/models/measure_location_grid_event_state.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/measure_specification.py` & `threedi-api-client-4.1.3/openapi_client/models/measure_specification.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/memory_structure_control.py` & `threedi-api-client-4.1.3/openapi_client/models/memory_structure_control.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/net_cdf_raster_leakage.py` & `threedi-api-client-4.1.3/openapi_client/models/net_cdf_raster_leakage.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/net_cdf_raster_rain.py` & `threedi-api-client-4.1.3/openapi_client/models/net_cdf_raster_rain.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/net_cdf_raster_sources_sinks.py` & `threedi-api-client-4.1.3/openapi_client/models/net_cdf_raster_sources_sinks.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/net_cdf_timeseries_leakage.py` & `threedi-api-client-4.1.3/openapi_client/models/net_cdf_timeseries_leakage.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/net_cdf_timeseries_rain.py` & `threedi-api-client-4.1.3/openapi_client/models/net_cdf_timeseries_rain.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/net_cdf_timeseries_sources_sinks.py` & `threedi-api-client-4.1.3/openapi_client/models/net_cdf_timeseries_sources_sinks.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/numerical_settings.py` & `threedi-api-client-4.1.3/openapi_client/models/numerical_settings.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/one_d_water_level.py` & `threedi-api-client-4.1.3/openapi_client/models/one_d_water_level.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/one_d_water_level_predefined.py` & `threedi-api-client-4.1.3/openapi_client/models/one_d_water_level_predefined.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/organisation.py` & `threedi-api-client-4.1.3/openapi_client/models/organisation.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/organisation_role.py` & `threedi-api-client-4.1.3/openapi_client/models/organisation_role.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/physical_settings.py` & `threedi-api-client-4.1.3/openapi_client/models/physical_settings.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/point.py` & `threedi-api-client-4.1.3/openapi_client/models/point.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/polygon.py` & `threedi-api-client-4.1.3/openapi_client/models/polygon.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/post_processing_overview.py` & `threedi-api-client-4.1.3/openapi_client/models/post_processing_overview.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/post_processing_queue.py` & `threedi-api-client-4.1.3/openapi_client/models/post_processing_queue.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/post_processing_status.py` & `threedi-api-client-4.1.3/openapi_client/models/post_processing_status.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/potential_breach.py` & `threedi-api-client-4.1.3/openapi_client/models/potential_breach.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/profile.py` & `threedi-api-client-4.1.3/openapi_client/models/profile.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/progress.py` & `threedi-api-client-4.1.3/openapi_client/models/progress.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/pump_discharge_graph.py` & `threedi-api-client-4.1.3/openapi_client/models/pump_discharge_graph.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/pump_discharge_graph_request.py` & `threedi-api-client-4.1.3/openapi_client/models/pump_discharge_graph_request.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/raster.py` & `threedi-api-client-4.1.3/openapi_client/models/raster.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/raster_edit.py` & `threedi-api-client-4.1.3/openapi_client/models/raster_edit.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/raster_edit_urls.py` & `threedi-api-client-4.1.3/openapi_client/models/raster_edit_urls.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/raster_options.py` & `threedi-api-client-4.1.3/openapi_client/models/raster_options.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/refresh.py` & `threedi-api-client-4.1.3/openapi_client/models/refresh.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/repository.py` & `threedi-api-client-4.1.3/openapi_client/models/repository.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/result.py` & `threedi-api-client-4.1.3/openapi_client/models/result.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/result_file.py` & `threedi-api-client-4.1.3/openapi_client/models/result_file.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/revision.py` & `threedi-api-client-4.1.3/openapi_client/models/revision.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/role.py` & `threedi-api-client-4.1.3/openapi_client/models/role.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/saved_state_overview.py` & `threedi-api-client-4.1.3/openapi_client/models/saved_state_overview.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/settings.py` & `threedi-api-client-4.1.3/openapi_client/models/settings.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/simulation.py` & `threedi-api-client-4.1.3/openapi_client/models/simulation.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/simulation_channel.py` & `threedi-api-client-4.1.3/openapi_client/models/simulation_channel.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/simulation_settings_overview.py` & `threedi-api-client-4.1.3/openapi_client/models/simulation_settings_overview.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/simulation_status.py` & `threedi-api-client-4.1.3/openapi_client/models/simulation_status.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/simulation_status_statistics.py` & `threedi-api-client-4.1.3/openapi_client/models/simulation_status_statistics.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/simulation_update.py` & `threedi-api-client-4.1.3/openapi_client/models/simulation_update.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/stable_threshold_saved_state.py` & `threedi-api-client-4.1.3/openapi_client/models/stable_threshold_saved_state.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/table_structure_control.py` & `threedi-api-client-4.1.3/openapi_client/models/table_structure_control.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/threedi_model.py` & `threedi-api-client-4.1.3/openapi_client/models/threedi_model.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/threedi_model_saved_state.py` & `threedi-api-client-4.1.3/openapi_client/models/threedi_model_saved_state.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/threshold.py` & `threedi-api-client-4.1.3/openapi_client/models/threshold.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/time_step_settings.py` & `threedi-api-client-4.1.3/openapi_client/models/time_step_settings.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/timed_saved_state_update.py` & `threedi-api-client-4.1.3/openapi_client/models/timed_saved_state_update.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/timed_structure_control.py` & `threedi-api-client-4.1.3/openapi_client/models/timed_structure_control.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/timeout.py` & `threedi-api-client-4.1.3/openapi_client/models/timeout.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/timeseries_lateral.py` & `threedi-api-client-4.1.3/openapi_client/models/timeseries_lateral.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/timeseries_leakage.py` & `threedi-api-client-4.1.3/openapi_client/models/timeseries_leakage.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/timeseries_leakage_overview.py` & `threedi-api-client-4.1.3/openapi_client/models/timeseries_leakage_overview.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/timeseries_local_rain.py` & `threedi-api-client-4.1.3/openapi_client/models/timeseries_local_rain.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/timeseries_rain.py` & `threedi-api-client-4.1.3/openapi_client/models/timeseries_rain.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/timeseries_rain_overview.py` & `threedi-api-client-4.1.3/openapi_client/models/timeseries_rain_overview.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/timeseries_sources_sinks.py` & `threedi-api-client-4.1.3/openapi_client/models/timeseries_sources_sinks.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/timeseries_sources_sinks_overview.py` & `threedi-api-client-4.1.3/openapi_client/models/timeseries_sources_sinks_overview.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/timeseries_wind.py` & `threedi-api-client-4.1.3/openapi_client/models/timeseries_wind.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/tms.py` & `threedi-api-client-4.1.3/openapi_client/models/tms.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/tokens.py` & `threedi-api-client-4.1.3/openapi_client/models/tokens.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/two_d_water_level.py` & `threedi-api-client-4.1.3/openapi_client/models/two_d_water_level.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/two_d_water_raster.py` & `threedi-api-client-4.1.3/openapi_client/models/two_d_water_raster.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/upload.py` & `threedi-api-client-4.1.3/openapi_client/models/upload.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/upload_event_file.py` & `threedi-api-client-4.1.3/openapi_client/models/upload_event_file.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/usage.py` & `threedi-api-client-4.1.3/openapi_client/models/usage.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/usage_statistics.py` & `threedi-api-client-4.1.3/openapi_client/models/usage_statistics.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/user.py` & `threedi-api-client-4.1.3/openapi_client/models/user.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/water_flow_graph_request.py` & `threedi-api-client-4.1.3/openapi_client/models/water_flow_graph_request.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/water_graph.py` & `threedi-api-client-4.1.3/openapi_client/models/water_graph.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/water_level_graph_request.py` & `threedi-api-client-4.1.3/openapi_client/models/water_level_graph_request.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/water_level_profile.py` & `threedi-api-client-4.1.3/openapi_client/models/water_level_profile.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/water_level_profile_request.py` & `threedi-api-client-4.1.3/openapi_client/models/water_level_profile_request.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/waterdepth.py` & `threedi-api-client-4.1.3/openapi_client/models/waterdepth.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/wind.py` & `threedi-api-client-4.1.3/openapi_client/models/wind.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/models/wind_drag_coefficient.py` & `threedi-api-client-4.1.3/openapi_client/models/wind_drag_coefficient.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/openapi_client/rest.py` & `threedi-api-client-4.1.3/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/setup.py` & `threedi-api-client-4.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
 
 requirements = [
     'certifi>=2019.3.9',
-    'urllib3>=1.24,<2.1',
+    'urllib3>=1.24,<2.0',
     'six>=1.10',
     'python-dateutil',
 ]
 
 aio_requirements = ["aiohttp>=3.6.3", "aiofiles>=0.6"]
 
 # Note: mock contains a backport of AsyncMock
```

### Comparing `threedi-api-client-4.1.2b0/tests/test_auth.py` & `threedi-api-client-4.1.3/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/tests/test_files.py` & `threedi-api-client-4.1.3/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/tests/test_files_aio.py` & `threedi-api-client-4.1.3/tests/test_files_aio.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/tests/test_threedi_api.py` & `threedi-api-client-4.1.3/tests/test_threedi_api.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/tests/test_threedi_api_client.py` & `threedi-api-client-4.1.3/tests/test_threedi_api_client.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/tests/test_threedi_api_client_aio.py` & `threedi-api-client-4.1.3/tests/test_threedi_api_client_aio.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/aio/aiohttp_retry.py` & `threedi-api-client-4.1.3/threedi_api_client/aio/aiohttp_retry.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/aio/files.py` & `threedi-api-client-4.1.3/threedi_api_client/aio/files.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/aio/openapi/api_client.py` & `threedi-api-client-4.1.3/threedi_api_client/aio/openapi/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/aio/openapi/configuration.py` & `threedi-api-client-4.1.3/threedi_api_client/aio/openapi/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/aio/openapi/rest.py` & `threedi-api-client-4.1.3/threedi_api_client/aio/openapi/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/aio/threedi_api_client.py` & `threedi-api-client-4.1.3/threedi_api_client/aio/threedi_api_client.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/api.py` & `threedi-api-client-4.1.3/threedi_api_client/api.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/auth.py` & `threedi-api-client-4.1.3/threedi_api_client/auth.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/config.py` & `threedi-api-client-4.1.3/threedi_api_client/config.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/files.py` & `threedi-api-client-4.1.3/threedi_api_client/files.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/__init__.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/api/v3_api.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/api/v3_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -3544,14 +3544,16 @@
         :param str unique_id__icontains:
         :param str unique_id__in: Multiple values may be separated by commas.
         :param str unique_id__startswith:
         :param str unique_id__istartswith:
         :param str unique_id__endswith:
         :param str unique_id__regex:
         :param str valid_contracts_only:
+        :param str logged_in_user_has_role:
+        :param str contract__scope__in: Multiple values may be separated by commas.
         :param int limit: Number of results to return per page.
         :param int offset: The initial index from which to return the results.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -3589,14 +3591,16 @@
         :param str unique_id__icontains:
         :param str unique_id__in: Multiple values may be separated by commas.
         :param str unique_id__startswith:
         :param str unique_id__istartswith:
         :param str unique_id__endswith:
         :param str unique_id__regex:
         :param str valid_contracts_only:
+        :param str logged_in_user_has_role:
+        :param str contract__scope__in: Multiple values may be separated by commas.
         :param int limit: Number of results to return per page.
         :param int offset: The initial index from which to return the results.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -3627,14 +3631,16 @@
             'unique_id__icontains',
             'unique_id__in',
             'unique_id__startswith',
             'unique_id__istartswith',
             'unique_id__endswith',
             'unique_id__regex',
             'valid_contracts_only',
+            'logged_in_user_has_role',
+            'contract__scope__in',
             'limit',
             'offset'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -3691,14 +3697,18 @@
             query_params.append(('unique_id__istartswith', local_var_params['unique_id__istartswith']))  # noqa: E501
         if 'unique_id__endswith' in local_var_params and local_var_params['unique_id__endswith'] is not None:  # noqa: E501
             query_params.append(('unique_id__endswith', local_var_params['unique_id__endswith']))  # noqa: E501
         if 'unique_id__regex' in local_var_params and local_var_params['unique_id__regex'] is not None:  # noqa: E501
             query_params.append(('unique_id__regex', local_var_params['unique_id__regex']))  # noqa: E501
         if 'valid_contracts_only' in local_var_params and local_var_params['valid_contracts_only'] is not None:  # noqa: E501
             query_params.append(('valid_contracts_only', local_var_params['valid_contracts_only']))  # noqa: E501
+        if 'logged_in_user_has_role' in local_var_params and local_var_params['logged_in_user_has_role'] is not None:  # noqa: E501
+            query_params.append(('logged_in_user_has_role', local_var_params['logged_in_user_has_role']))  # noqa: E501
+        if 'contract__scope__in' in local_var_params and local_var_params['contract__scope__in'] is not None:  # noqa: E501
+            query_params.append(('contract__scope__in', local_var_params['contract__scope__in']))  # noqa: E501
         if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
             query_params.append(('limit', local_var_params['limit']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
 
         header_params = {}
 
@@ -59292,17 +59302,17 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def threedimodels_initial_waterlevels_create(self, threedimodel_pk, data, **kwargs):  # noqa: E501
-        """### Adding (extra) 1D initial waterlevels Extra 1D initial waterlevels can be added by posting:  # noqa: E501
+        """Add new initial waterlevels  # noqa: E501
 
-        {\"dimension\": \"one_d\"}  Using the 'id' value from the response, a JSON file needs to be uploaded via the PUT_URL retrieved from `initial_waterlevels/{id}/upload/` in the following JSON format:  Python code:      import json     file_contents = json.dumps({         \"node_ids\": [node_id_1, node_id2, ....],         \"values\" : [value_for_node_id_1, value_for_node_id_2, ...]     })      # Notes:     # - Omitted values are considered dry.     # - `node_ids` need to be sorted and unique     # - Make sure that the positions of the node_id's and values match.  ### Adding (extra) 2D initial waterlevels 2D initial waterlevels can be added by uploading an 'initial_waterlevel_file' Geotiff raster via `rasters/{id}/upload/`. This automatically triggers the creation of a 2D initial waterlevel. The source raster is linked as 'source_raster'. The values in the `source_raster` are aggregated per node using max, min and mean operators. The resulting values are stored in a file linked under `file`.  # noqa: E501
+        ### Adding (extra) 1D initial waterlevels Extra 1D initial waterlevels can be added by posting:  {\"dimension\": \"one_d\"}  Using the 'id' value from the response, a JSON file needs to be uploaded via the PUT_URL retrieved from `initial_waterlevels/{id}/upload/` in the following JSON format:  Python code:      import json     file_contents = json.dumps({         \"node_ids\": [node_id_1, node_id2, ....],         \"values\" : [value_for_node_id_1, value_for_node_id_2, ...]     })      # Notes:     # - Omitted values are considered dry.     # - `node_ids` need to be sorted and unique     # - Make sure that the positions of the node_id's and values match.  ### Adding (extra) 2D initial waterlevels 2D initial waterlevels can be added by uploading an 'initial_waterlevel_file' Geotiff raster via `rasters/{id}/upload/`. This automatically triggers the creation of a 2D initial waterlevel. The source raster is linked as 'source_raster'. The values in the `source_raster` are aggregated per node using max, min and mean operators. The resulting values are stored in a file linked under `file`.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.threedimodels_initial_waterlevels_create(threedimodel_pk, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str threedimodel_pk: (required)
@@ -59318,17 +59328,17 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.threedimodels_initial_waterlevels_create_with_http_info(threedimodel_pk, data, **kwargs)  # noqa: E501
 
     def threedimodels_initial_waterlevels_create_with_http_info(self, threedimodel_pk, data, **kwargs):  # noqa: E501
-        """### Adding (extra) 1D initial waterlevels Extra 1D initial waterlevels can be added by posting:  # noqa: E501
+        """Add new initial waterlevels  # noqa: E501
 
-        {\"dimension\": \"one_d\"}  Using the 'id' value from the response, a JSON file needs to be uploaded via the PUT_URL retrieved from `initial_waterlevels/{id}/upload/` in the following JSON format:  Python code:      import json     file_contents = json.dumps({         \"node_ids\": [node_id_1, node_id2, ....],         \"values\" : [value_for_node_id_1, value_for_node_id_2, ...]     })      # Notes:     # - Omitted values are considered dry.     # - `node_ids` need to be sorted and unique     # - Make sure that the positions of the node_id's and values match.  ### Adding (extra) 2D initial waterlevels 2D initial waterlevels can be added by uploading an 'initial_waterlevel_file' Geotiff raster via `rasters/{id}/upload/`. This automatically triggers the creation of a 2D initial waterlevel. The source raster is linked as 'source_raster'. The values in the `source_raster` are aggregated per node using max, min and mean operators. The resulting values are stored in a file linked under `file`.  # noqa: E501
+        ### Adding (extra) 1D initial waterlevels Extra 1D initial waterlevels can be added by posting:  {\"dimension\": \"one_d\"}  Using the 'id' value from the response, a JSON file needs to be uploaded via the PUT_URL retrieved from `initial_waterlevels/{id}/upload/` in the following JSON format:  Python code:      import json     file_contents = json.dumps({         \"node_ids\": [node_id_1, node_id2, ....],         \"values\" : [value_for_node_id_1, value_for_node_id_2, ...]     })      # Notes:     # - Omitted values are considered dry.     # - `node_ids` need to be sorted and unique     # - Make sure that the positions of the node_id's and values match.  ### Adding (extra) 2D initial waterlevels 2D initial waterlevels can be added by uploading an 'initial_waterlevel_file' Geotiff raster via `rasters/{id}/upload/`. This automatically triggers the creation of a 2D initial waterlevel. The source raster is linked as 'source_raster'. The values in the `source_raster` are aggregated per node using max, min and mean operators. The resulting values are stored in a file linked under `file`.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.threedimodels_initial_waterlevels_create_with_http_info(threedimodel_pk, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str threedimodel_pk: (required)
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/api/v3_beta_api.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/api/v3_beta_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -734,15 +734,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def simulations_events_obstacle_edits_create(self, simulation_pk, data, **kwargs):  # noqa: E501
         """simulations_events_obstacle_edits_create  # noqa: E501
 
-        A simple ViewSet for viewing obstacle edits  # noqa: E501
+        Create an obstacle edit  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.simulations_events_obstacle_edits_create(simulation_pk, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str simulation_pk: (required)
@@ -760,15 +760,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.simulations_events_obstacle_edits_create_with_http_info(simulation_pk, data, **kwargs)  # noqa: E501
 
     def simulations_events_obstacle_edits_create_with_http_info(self, simulation_pk, data, **kwargs):  # noqa: E501
         """simulations_events_obstacle_edits_create  # noqa: E501
 
-        A simple ViewSet for viewing obstacle edits  # noqa: E501
+        Create an obstacle edit  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.simulations_events_obstacle_edits_create_with_http_info(simulation_pk, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str simulation_pk: (required)
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/api_client.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/configuration.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/exceptions.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/__init__.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 
 # flake8: noqa
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/action.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/action.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -36,50 +36,55 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'name': 'str',
         'duration': 'int',
         'timeout': 'int',
         'max_rate': 'float',
-        'compute_cluster': 'str'
+        'compute_cluster': 'str',
+        'simulation_runner': 'str'
     }
 
     attribute_map = {
         'name': 'name',
         'duration': 'duration',
         'timeout': 'timeout',
         'max_rate': 'max_rate',
-        'compute_cluster': 'compute_cluster'
+        'compute_cluster': 'compute_cluster',
+        'simulation_runner': 'simulation_runner'
     }
 
-    def __init__(self, name=None, duration=None, timeout=None, max_rate=None, compute_cluster=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
+    def __init__(self, name=None, duration=None, timeout=None, max_rate=None, compute_cluster=None, simulation_runner=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
         """Action - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         # True if data is coming from API
         self._fetched_from_api = fetched_from_api
 
         self._name = None
         self._duration = None
         self._timeout = None
         self._max_rate = None
         self._compute_cluster = None
+        self._simulation_runner = None
         self.discriminator = None
 
         self.name = name
         if duration is not None:
             self.duration = duration
         if timeout is not None:
             self.timeout = timeout
         if max_rate is not None:
             self.max_rate = max_rate
         if compute_cluster is not None:
             self.compute_cluster = compute_cluster
+        if simulation_runner is not None:
+            self.simulation_runner = simulation_runner
 
     @property
     def name(self):
         """Gets the name of this Action.  # noqa: E501
 
 
         :return: The name of this Action.  # noqa: E501
@@ -203,14 +208,43 @@
 
         :param compute_cluster: The compute_cluster of this Action.  # noqa: E501
         :type: str
         """
 
         self._compute_cluster = compute_cluster
 
+    @property
+    def simulation_runner(self):
+        """Gets the simulation_runner of this Action.  # noqa: E501
+
+        Only allowed for name values: 'start', 'initialize' or 'queue Simulation runner version used to execute the simulation. If not filled in the default version is used. (Note: used for testing new calccore releases on the staging environment. On production only the default version can be picked)  # noqa: E501
+
+        :return: The simulation_runner of this Action.  # noqa: E501
+        :rtype: str
+        """
+        return self._simulation_runner
+
+    @simulation_runner.setter
+    def simulation_runner(self, simulation_runner):
+        """Sets the simulation_runner of this Action.
+
+        Only allowed for name values: 'start', 'initialize' or 'queue Simulation runner version used to execute the simulation. If not filled in the default version is used. (Note: used for testing new calccore releases on the staging environment. On production only the default version can be picked)  # noqa: E501
+
+        :param simulation_runner: The simulation_runner of this Action.  # noqa: E501
+        :type: str
+        """
+        allowed_values = ["3.2.34-2.4.3"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and simulation_runner not in allowed_values:  # noqa: E501
+            self.__handle_validation_error(
+                "Invalid value for `simulation_runner` ({0}), must be one of {1}"  # noqa: E501
+                .format(simulation_runner, allowed_values)
+            )
+
+        self._simulation_runner = simulation_runner
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/aggregation_settings.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/aggregation_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/arrival_time_post_processing.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/arrival_time_post_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/authenticate.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/authenticate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/base_event_state.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/base_event_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/basic_post_processing.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/basic_post_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/boundary_condition.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/boundary_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/breach.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/breach.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/breach_graph.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/breach_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/breach_graph_request.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/breach_graph_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/commit.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/commit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/constant_lateral.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/constant_lateral.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/constant_leakage.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/constant_leakage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/constant_local_rain.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/constant_local_rain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/constant_rain.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/constant_rain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/constant_sources_sinks.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/constant_sources_sinks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/constant_wind.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/constant_wind.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/contract.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -37,50 +37,53 @@
     """
     openapi_types = {
         'url': 'str',
         'id': 'int',
         'organisation': 'str',
         'organisation_name': 'str',
         'scope': 'str',
+        'start_date': 'date',
         'hours_bought': 'int',
         'hours_used': 'float',
         'session_limit': 'int',
         'current_sessions': 'str',
         'threedimodel_limit': 'int',
         'created_by': 'str'
     }
 
     attribute_map = {
         'url': 'url',
         'id': 'id',
         'organisation': 'organisation',
         'organisation_name': 'organisation_name',
         'scope': 'scope',
+        'start_date': 'start_date',
         'hours_bought': 'hours_bought',
         'hours_used': 'hours_used',
         'session_limit': 'session_limit',
         'current_sessions': 'current_sessions',
         'threedimodel_limit': 'threedimodel_limit',
         'created_by': 'created_by'
     }
 
-    def __init__(self, url=None, id=None, organisation=None, organisation_name=None, scope=None, hours_bought=None, hours_used=None, session_limit=None, current_sessions=None, threedimodel_limit=None, created_by=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
+    def __init__(self, url=None, id=None, organisation=None, organisation_name=None, scope=None, start_date=None, hours_bought=None, hours_used=None, session_limit=None, current_sessions=None, threedimodel_limit=None, created_by=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
         """Contract - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         # True if data is coming from API
         self._fetched_from_api = fetched_from_api
 
         self._url = None
         self._id = None
         self._organisation = None
         self._organisation_name = None
         self._scope = None
+        self._start_date = None
         self._hours_bought = None
         self._hours_used = None
         self._session_limit = None
         self._current_sessions = None
         self._threedimodel_limit = None
         self._created_by = None
         self.discriminator = None
@@ -90,14 +93,15 @@
         if id is not None:
             self.id = id
         self.organisation = organisation
         if organisation_name is not None:
             self.organisation_name = organisation_name
         if scope is not None:
             self.scope = scope
+        self.start_date = start_date
         self.hours_bought = hours_bought
         if hours_used is not None:
             self.hours_used = hours_used
         self.session_limit = session_limit
         if current_sessions is not None:
             self.current_sessions = current_sessions
         if threedimodel_limit is not None:
@@ -192,37 +196,58 @@
 
         self._organisation_name = organisation_name
 
     @property
     def scope(self):
         """Gets the scope of this Contract.  # noqa: E501
 
-        A space-separated list of scopes (options: basic simulate create lizardrain lizardprocess manageusers managecontracts)  # noqa: E501
+        A space-separated list of scopes (options: basic simulate create lizardrain lizardprocess manageusers managecontracts test livesite)  # noqa: E501
 
         :return: The scope of this Contract.  # noqa: E501
         :rtype: str
         """
         return self._scope
 
     @scope.setter
     def scope(self, scope):
         """Sets the scope of this Contract.
 
-        A space-separated list of scopes (options: basic simulate create lizardrain lizardprocess manageusers managecontracts)  # noqa: E501
+        A space-separated list of scopes (options: basic simulate create lizardrain lizardprocess manageusers managecontracts test livesite)  # noqa: E501
 
         :param scope: The scope of this Contract.  # noqa: E501
         :type: str
         """
         if (self.local_vars_configuration.client_side_validation and
                 scope is not None and len(scope) < 1):
             self.__handle_validation_error("Invalid value for `scope`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._scope = scope
 
     @property
+    def start_date(self):
+        """Gets the start_date of this Contract.  # noqa: E501
+
+
+        :return: The start_date of this Contract.  # noqa: E501
+        :rtype: date
+        """
+        return self._start_date
+
+    @start_date.setter
+    def start_date(self, start_date):
+        """Sets the start_date of this Contract.
+
+
+        :param start_date: The start_date of this Contract.  # noqa: E501
+        :type: date
+        """
+
+        self._start_date = start_date
+
+    @property
     def hours_bought(self):
         """Gets the hours_bought of this Contract.  # noqa: E501
 
 
         :return: The hours_bought of this Contract.  # noqa: E501
         :rtype: int
         """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/copy_to_threedi_model.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/copy_to_threedi_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/create_revision.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/create_revision.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/create_template.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/create_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/current_status.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/current_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/current_version.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/current_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/damage_estimation.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/damage_estimation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/damage_post_processing.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/damage_post_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/destroy_revision.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/destroy_revision.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/download.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/event.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/extent.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/extent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_boundary_condition.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_boundary_condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_lateral.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_lateral.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_meta.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_raster_leakage.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_raster_leakage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_raster_rain.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_raster_rain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_raster_sources_sinks.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_raster_sources_sinks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_read_only.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_read_only.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_structure_control.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_structure_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_timeseries_leakage.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_timeseries_leakage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_timeseries_rain.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_timeseries_rain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/file_timeseries_sources_sinks.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/file_timeseries_sources_sinks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/from_template.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/from_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/grid_event_state.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/grid_event_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/ground_water_level.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/ground_water_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/ground_water_raster.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/ground_water_raster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/initial_saved_state.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/initial_saved_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/initial_saved_state_overview.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/initial_saved_state_overview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/initial_waterlevel.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/initial_waterlevel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response200.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response200.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2001.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2001.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20010.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20010.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20011.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20011.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20012.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20012.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20013.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20013.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20014.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20014.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20015.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20015.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20016.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20016.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20017.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20017.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20018.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20018.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20019.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20019.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2002.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2002.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20020.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20020.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20021.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20021.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20022.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20022.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20023.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20023.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20024.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20024.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20025.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20025.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20026.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20026.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20027.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20027.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20028.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20028.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20029.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20029.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2003.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2003.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20030.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20030.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20031.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20031.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20032.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20032.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20033.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20033.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20034.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20034.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20035.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20035.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20036.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20036.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20037.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20037.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20038.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20038.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20039.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20039.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2004.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2004.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20040.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20040.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20041.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20071.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -17,15 +17,15 @@
 
 import six
 
 from threedi_api_client.openapi.configuration import Configuration
 
 logger = logging.getLogger(__name__)
 
-class InlineResponse20041(object):
+class InlineResponse20071(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,26 +35,26 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'count': 'int',
         'next': 'str',
         'previous': 'str',
-        'results': 'list[NetCDFRasterSourcesSinks]'
+        'results': 'list[ThreediModelTask]'
     }
 
     attribute_map = {
         'count': 'count',
         'next': 'next',
         'previous': 'previous',
         'results': 'results'
     }
 
     def __init__(self, count=None, next=None, previous=None, results=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
-        """InlineResponse20041 - a model defined in OpenAPI"""  # noqa: E501
+        """InlineResponse20071 - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         # True if data is coming from API
         self._fetched_from_api = fetched_from_api
 
@@ -67,94 +67,94 @@
         self.count = count
         self.next = next
         self.previous = previous
         self.results = results
 
     @property
     def count(self):
-        """Gets the count of this InlineResponse20041.  # noqa: E501
+        """Gets the count of this InlineResponse20071.  # noqa: E501
 
 
-        :return: The count of this InlineResponse20041.  # noqa: E501
+        :return: The count of this InlineResponse20071.  # noqa: E501
         :rtype: int
         """
         return self._count
 
     @count.setter
     def count(self, count):
-        """Sets the count of this InlineResponse20041.
+        """Sets the count of this InlineResponse20071.
 
 
-        :param count: The count of this InlineResponse20041.  # noqa: E501
+        :param count: The count of this InlineResponse20071.  # noqa: E501
         :type: int
         """
         if self.local_vars_configuration.client_side_validation and count is None:  # noqa: E501
             self.__handle_validation_error("Invalid value for `count`, must not be `None`")  # noqa: E501
 
         self._count = count
 
     @property
     def next(self):
-        """Gets the next of this InlineResponse20041.  # noqa: E501
+        """Gets the next of this InlineResponse20071.  # noqa: E501
 
 
-        :return: The next of this InlineResponse20041.  # noqa: E501
+        :return: The next of this InlineResponse20071.  # noqa: E501
         :rtype: str
         """
         return self._next
 
     @next.setter
     def next(self, next):
-        """Sets the next of this InlineResponse20041.
+        """Sets the next of this InlineResponse20071.
 
 
-        :param next: The next of this InlineResponse20041.  # noqa: E501
+        :param next: The next of this InlineResponse20071.  # noqa: E501
         :type: str
         """
 
         self._next = next
 
     @property
     def previous(self):
-        """Gets the previous of this InlineResponse20041.  # noqa: E501
+        """Gets the previous of this InlineResponse20071.  # noqa: E501
 
 
-        :return: The previous of this InlineResponse20041.  # noqa: E501
+        :return: The previous of this InlineResponse20071.  # noqa: E501
         :rtype: str
         """
         return self._previous
 
     @previous.setter
     def previous(self, previous):
-        """Sets the previous of this InlineResponse20041.
+        """Sets the previous of this InlineResponse20071.
 
 
-        :param previous: The previous of this InlineResponse20041.  # noqa: E501
+        :param previous: The previous of this InlineResponse20071.  # noqa: E501
         :type: str
         """
 
         self._previous = previous
 
     @property
     def results(self):
-        """Gets the results of this InlineResponse20041.  # noqa: E501
+        """Gets the results of this InlineResponse20071.  # noqa: E501
 
 
-        :return: The results of this InlineResponse20041.  # noqa: E501
-        :rtype: list[NetCDFRasterSourcesSinks]
+        :return: The results of this InlineResponse20071.  # noqa: E501
+        :rtype: list[ThreediModelTask]
         """
         return self._results
 
     @results.setter
     def results(self, results):
-        """Sets the results of this InlineResponse20041.
+        """Sets the results of this InlineResponse20071.
 
 
-        :param results: The results of this InlineResponse20041.  # noqa: E501
-        :type: list[NetCDFRasterSourcesSinks]
+        :param results: The results of this InlineResponse20071.  # noqa: E501
+        :type: list[ThreediModelTask]
         """
         if self.local_vars_configuration.client_side_validation and results is None:  # noqa: E501
             self.__handle_validation_error("Invalid value for `results`, must not be `None`")  # noqa: E501
 
         self._results = results
 
     def to_dict(self):
@@ -195,18 +195,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, InlineResponse20041):
+        if not isinstance(other, InlineResponse20071):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, InlineResponse20041):
+        if not isinstance(other, InlineResponse20071):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20042.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20042.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20043.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20043.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20044.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20044.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20045.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20045.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20046.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20046.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20047.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20047.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20048.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20048.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20049.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20049.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2005.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2005.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20050.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20050.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20051.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20051.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20052.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20052.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20053.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20053.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20054.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20054.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20055.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20055.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20056.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20056.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20057.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20057.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20058.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20058.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20059.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20059.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2006.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2006.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20060.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20060.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20061.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20061.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20062.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20062.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20063.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20063.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20064.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20064.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20065.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20065.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20066.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20066.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20067.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20067.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20068.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20068.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20069.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20069.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2007.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2007.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20070.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20070.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20071.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20041.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -17,15 +17,15 @@
 
 import six
 
 from threedi_api_client.openapi.configuration import Configuration
 
 logger = logging.getLogger(__name__)
 
-class InlineResponse20071(object):
+class InlineResponse20041(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,26 +35,26 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'count': 'int',
         'next': 'str',
         'previous': 'str',
-        'results': 'list[ThreediModelTask]'
+        'results': 'list[NetCDFRasterSourcesSinks]'
     }
 
     attribute_map = {
         'count': 'count',
         'next': 'next',
         'previous': 'previous',
         'results': 'results'
     }
 
     def __init__(self, count=None, next=None, previous=None, results=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
-        """InlineResponse20071 - a model defined in OpenAPI"""  # noqa: E501
+        """InlineResponse20041 - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         # True if data is coming from API
         self._fetched_from_api = fetched_from_api
 
@@ -67,94 +67,94 @@
         self.count = count
         self.next = next
         self.previous = previous
         self.results = results
 
     @property
     def count(self):
-        """Gets the count of this InlineResponse20071.  # noqa: E501
+        """Gets the count of this InlineResponse20041.  # noqa: E501
 
 
-        :return: The count of this InlineResponse20071.  # noqa: E501
+        :return: The count of this InlineResponse20041.  # noqa: E501
         :rtype: int
         """
         return self._count
 
     @count.setter
     def count(self, count):
-        """Sets the count of this InlineResponse20071.
+        """Sets the count of this InlineResponse20041.
 
 
-        :param count: The count of this InlineResponse20071.  # noqa: E501
+        :param count: The count of this InlineResponse20041.  # noqa: E501
         :type: int
         """
         if self.local_vars_configuration.client_side_validation and count is None:  # noqa: E501
             self.__handle_validation_error("Invalid value for `count`, must not be `None`")  # noqa: E501
 
         self._count = count
 
     @property
     def next(self):
-        """Gets the next of this InlineResponse20071.  # noqa: E501
+        """Gets the next of this InlineResponse20041.  # noqa: E501
 
 
-        :return: The next of this InlineResponse20071.  # noqa: E501
+        :return: The next of this InlineResponse20041.  # noqa: E501
         :rtype: str
         """
         return self._next
 
     @next.setter
     def next(self, next):
-        """Sets the next of this InlineResponse20071.
+        """Sets the next of this InlineResponse20041.
 
 
-        :param next: The next of this InlineResponse20071.  # noqa: E501
+        :param next: The next of this InlineResponse20041.  # noqa: E501
         :type: str
         """
 
         self._next = next
 
     @property
     def previous(self):
-        """Gets the previous of this InlineResponse20071.  # noqa: E501
+        """Gets the previous of this InlineResponse20041.  # noqa: E501
 
 
-        :return: The previous of this InlineResponse20071.  # noqa: E501
+        :return: The previous of this InlineResponse20041.  # noqa: E501
         :rtype: str
         """
         return self._previous
 
     @previous.setter
     def previous(self, previous):
-        """Sets the previous of this InlineResponse20071.
+        """Sets the previous of this InlineResponse20041.
 
 
-        :param previous: The previous of this InlineResponse20071.  # noqa: E501
+        :param previous: The previous of this InlineResponse20041.  # noqa: E501
         :type: str
         """
 
         self._previous = previous
 
     @property
     def results(self):
-        """Gets the results of this InlineResponse20071.  # noqa: E501
+        """Gets the results of this InlineResponse20041.  # noqa: E501
 
 
-        :return: The results of this InlineResponse20071.  # noqa: E501
-        :rtype: list[ThreediModelTask]
+        :return: The results of this InlineResponse20041.  # noqa: E501
+        :rtype: list[NetCDFRasterSourcesSinks]
         """
         return self._results
 
     @results.setter
     def results(self, results):
-        """Sets the results of this InlineResponse20071.
+        """Sets the results of this InlineResponse20041.
 
 
-        :param results: The results of this InlineResponse20071.  # noqa: E501
-        :type: list[ThreediModelTask]
+        :param results: The results of this InlineResponse20041.  # noqa: E501
+        :type: list[NetCDFRasterSourcesSinks]
         """
         if self.local_vars_configuration.client_side_validation and results is None:  # noqa: E501
             self.__handle_validation_error("Invalid value for `results`, must not be `None`")  # noqa: E501
 
         self._results = results
 
     def to_dict(self):
@@ -195,18 +195,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, InlineResponse20071):
+        if not isinstance(other, InlineResponse20041):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, InlineResponse20071):
+        if not isinstance(other, InlineResponse20041):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response20072.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response20072.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2008.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2008.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inline_response2009.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inline_response2009.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/inpy_version.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/inpy_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/lateral.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/lateral.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/linestring.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/linestring.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/lizard_raster_rain.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/lizard_raster_rain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/lizard_raster_sources_sinks.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/lizard_raster_sources_sinks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/lizard_timeseries_rain.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/lizard_timeseries_rain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/lizard_timeseries_sources_sinks.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/lizard_timeseries_sources_sinks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/local_rain.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/local_rain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/measure_location.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/measure_location.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/measure_location_grid_event_state.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/measure_location_grid_event_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/measure_specification.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/measure_specification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/memory_structure_control.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/memory_structure_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/net_cdf_raster_leakage.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/net_cdf_raster_leakage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/net_cdf_raster_rain.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/net_cdf_raster_rain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/net_cdf_raster_sources_sinks.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/net_cdf_raster_sources_sinks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/net_cdf_timeseries_leakage.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/net_cdf_timeseries_leakage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/net_cdf_timeseries_rain.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/net_cdf_timeseries_rain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/net_cdf_timeseries_sources_sinks.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/net_cdf_timeseries_sources_sinks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/numerical_settings.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/numerical_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/obstacle_edit.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/obstacle_edit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -37,64 +37,59 @@
     """
     openapi_types = {
         'url': 'str',
         'simulation': 'str',
         'offset': 'int',
         'value': 'float',
         'linestring': 'Linestring',
-        'relative': 'bool',
         'state': 'str',
         'state_detail': 'object',
         'uid': 'str',
         'id': 'int'
     }
 
     attribute_map = {
         'url': 'url',
         'simulation': 'simulation',
         'offset': 'offset',
         'value': 'value',
         'linestring': 'linestring',
-        'relative': 'relative',
         'state': 'state',
         'state_detail': 'state_detail',
         'uid': 'uid',
         'id': 'id'
     }
 
-    def __init__(self, url=None, simulation=None, offset=None, value=None, linestring=None, relative=None, state=None, state_detail=None, uid=None, id=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
+    def __init__(self, url=None, simulation=None, offset=None, value=None, linestring=None, state=None, state_detail=None, uid=None, id=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
         """ObstacleEdit - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         # True if data is coming from API
         self._fetched_from_api = fetched_from_api
 
         self._url = None
         self._simulation = None
         self._offset = None
         self._value = None
         self._linestring = None
-        self._relative = None
         self._state = None
         self._state_detail = None
         self._uid = None
         self._id = None
         self.discriminator = None
 
         if url is not None:
             self.url = url
         if simulation is not None:
             self.simulation = simulation
         self.offset = offset
         self.value = value
         self.linestring = linestring
-        if relative is not None:
-            self.relative = relative
         if state is not None:
             self.state = state
         if state_detail is not None:
             self.state_detail = state_detail
         if uid is not None:
             self.uid = uid
         if id is not None:
@@ -218,37 +213,14 @@
         """
         if self.local_vars_configuration.client_side_validation and linestring is None:  # noqa: E501
             self.__handle_validation_error("Invalid value for `linestring`, must not be `None`")  # noqa: E501
 
         self._linestring = linestring
 
     @property
-    def relative(self):
-        """Gets the relative of this ObstacleEdit.  # noqa: E501
-
-        Process the value as a relative height, default is absolute  # noqa: E501
-
-        :return: The relative of this ObstacleEdit.  # noqa: E501
-        :rtype: bool
-        """
-        return self._relative
-
-    @relative.setter
-    def relative(self, relative):
-        """Sets the relative of this ObstacleEdit.
-
-        Process the value as a relative height, default is absolute  # noqa: E501
-
-        :param relative: The relative of this ObstacleEdit.  # noqa: E501
-        :type: bool
-        """
-
-        self._relative = relative
-
-    @property
     def state(self):
         """Gets the state of this ObstacleEdit.  # noqa: E501
 
 
         :return: The state of this ObstacleEdit.  # noqa: E501
         :rtype: str
         """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/one_d_water_level.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/one_d_water_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/one_d_water_level_file.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/one_d_water_level_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/one_d_water_level_predefined.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/one_d_water_level_predefined.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/organisation.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/organisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/organisation_role.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/organisation_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/organisation_user.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/organisation_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/organisation_user_role_patch.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/organisation_user_role_patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/personal_api_key.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/personal_api_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -109,26 +109,26 @@
 
         self._prefix = prefix
 
     @property
     def scope(self):
         """Gets the scope of this PersonalAPIKey.  # noqa: E501
 
-        A space-separated list of scopes (options: basic simulate create lizardrain lizardprocess manageusers managecontracts). Alternatively, use '*:readwrite' for all scopes.  # noqa: E501
+        A space-separated list of scopes (options: basic simulate create lizardrain lizardprocess manageusers managecontracts test livesite). Alternatively, use '*:readwrite' for all scopes.  # noqa: E501
 
         :return: The scope of this PersonalAPIKey.  # noqa: E501
         :rtype: str
         """
         return self._scope
 
     @scope.setter
     def scope(self, scope):
         """Sets the scope of this PersonalAPIKey.
 
-        A space-separated list of scopes (options: basic simulate create lizardrain lizardprocess manageusers managecontracts). Alternatively, use '*:readwrite' for all scopes.  # noqa: E501
+        A space-separated list of scopes (options: basic simulate create lizardrain lizardprocess manageusers managecontracts test livesite). Alternatively, use '*:readwrite' for all scopes.  # noqa: E501
 
         :param scope: The scope of this PersonalAPIKey.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and scope is None:  # noqa: E501
             self.__handle_validation_error("Invalid value for `scope`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/personal_api_key_with_secret.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/personal_api_key_with_secret.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -119,26 +119,26 @@
 
         self._prefix = prefix
 
     @property
     def scope(self):
         """Gets the scope of this PersonalAPIKeyWithSecret.  # noqa: E501
 
-        A space-separated list of scopes (options: basic simulate create lizardrain lizardprocess manageusers managecontracts). Alternatively, use '*:readwrite' for all scopes.  # noqa: E501
+        A space-separated list of scopes (options: basic simulate create lizardrain lizardprocess manageusers managecontracts test livesite). Alternatively, use '*:readwrite' for all scopes.  # noqa: E501
 
         :return: The scope of this PersonalAPIKeyWithSecret.  # noqa: E501
         :rtype: str
         """
         return self._scope
 
     @scope.setter
     def scope(self, scope):
         """Sets the scope of this PersonalAPIKeyWithSecret.
 
-        A space-separated list of scopes (options: basic simulate create lizardrain lizardprocess manageusers managecontracts). Alternatively, use '*:readwrite' for all scopes.  # noqa: E501
+        A space-separated list of scopes (options: basic simulate create lizardrain lizardprocess manageusers managecontracts test livesite). Alternatively, use '*:readwrite' for all scopes.  # noqa: E501
 
         :param scope: The scope of this PersonalAPIKeyWithSecret.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and scope is None:  # noqa: E501
             self.__handle_validation_error("Invalid value for `scope`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/physical_settings.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/physical_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/point.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/point.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/polygon.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/polygon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/post_processing_overview.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/post_processing_overview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/post_processing_queue.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/post_processing_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/post_processing_status.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/post_processing_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/potential_breach.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/potential_breach.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/profile.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/progress.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/pump_discharge_graph.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/pump_discharge_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/pump_discharge_graph_request.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/pump_discharge_graph_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/rain_graph.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/rain_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/rain_graph_request.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/rain_graph_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/raster.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -135,15 +135,15 @@
 
 
         :param type: The type of this Raster.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
             self.__handle_validation_error("Invalid value for `type`, must not be `None`")  # noqa: E501
-        allowed_values = ["dem_file", "dem_raw_file", "equilibrium_infiltration_rate_file", "frict_coef_file", "initial_groundwater_level_file", "initial_waterlevel_file", "groundwater_hydro_connectivity_file", "groundwater_impervious_layer_level_file", "infiltration_decay_period_file", "initial_infiltration_rate_file", "leakage_file", "phreatic_storage_capacity_file", "hydraulic_conductivity_file", "porosity_file", "infiltration_rate_file", "max_infiltration_capacity_file", "interception_file"]  # noqa: E501
+        allowed_values = ["dem_file", "dem_raw_file", "equilibrium_infiltration_rate_file", "frict_coef_file", "initial_groundwater_level_file", "initial_waterlevel_file", "groundwater_hydro_connectivity_file", "groundwater_impervious_layer_level_file", "infiltration_decay_period_file", "initial_infiltration_rate_file", "leakage_file", "phreatic_storage_capacity_file", "hydraulic_conductivity_file", "porosity_file", "infiltration_rate_file", "max_infiltration_capacity_file", "interception_file", "vegetation_height_file", "vegetation_drag_coefficient_file", "vegetation_stem_count_file", "vegetation_stem_diameter_file"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
             self.__handle_validation_error(
                 "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
                 .format(type, allowed_values)
             )
 
         self._type = type
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/raster_create.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/raster_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -132,15 +132,15 @@
 
 
         :param type: The type of this RasterCreate.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
             self.__handle_validation_error("Invalid value for `type`, must not be `None`")  # noqa: E501
-        allowed_values = ["dem_file", "equilibrium_infiltration_rate_file", "frict_coef_file", "initial_groundwater_level_file", "initial_waterlevel_file", "groundwater_hydro_connectivity_file", "groundwater_impervious_layer_level_file", "infiltration_decay_period_file", "initial_infiltration_rate_file", "leakage_file", "phreatic_storage_capacity_file", "hydraulic_conductivity_file", "porosity_file", "infiltration_rate_file", "max_infiltration_capacity_file", "interception_file"]  # noqa: E501
+        allowed_values = ["dem_file", "equilibrium_infiltration_rate_file", "frict_coef_file", "initial_groundwater_level_file", "initial_waterlevel_file", "groundwater_hydro_connectivity_file", "groundwater_impervious_layer_level_file", "infiltration_decay_period_file", "initial_infiltration_rate_file", "leakage_file", "phreatic_storage_capacity_file", "hydraulic_conductivity_file", "porosity_file", "infiltration_rate_file", "max_infiltration_capacity_file", "interception_file", "vegetation_height_file", "vegetation_drag_coefficient_file", "vegetation_stem_count_file", "vegetation_stem_diameter_file"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
             self.__handle_validation_error(
                 "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
                 .format(type, allowed_values)
             )
 
         self._type = type
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/raster_edit.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/raster_edit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/raster_edit_urls.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/raster_edit_urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/raster_options.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/raster_options.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -48,15 +48,19 @@
         'initial_infiltration_rate_file': 'str',
         'leakage_file': 'str',
         'phreatic_storage_capacity_file': 'str',
         'hydraulic_conductivity_file': 'str',
         'porosity_file': 'str',
         'infiltration_rate_file': 'str',
         'max_infiltration_capacity_file': 'str',
-        'interception_file': 'str'
+        'interception_file': 'str',
+        'vegetation_height_file': 'str',
+        'vegetation_drag_coefficient_file': 'str',
+        'vegetation_stem_count_file': 'str',
+        'vegetation_stem_diameter_file': 'str'
     }
 
     attribute_map = {
         'dem_file': 'dem_file',
         'dem_raw_file': 'dem_raw_file',
         'equilibrium_infiltration_rate_file': 'equilibrium_infiltration_rate_file',
         'frict_coef_file': 'frict_coef_file',
@@ -68,18 +72,22 @@
         'initial_infiltration_rate_file': 'initial_infiltration_rate_file',
         'leakage_file': 'leakage_file',
         'phreatic_storage_capacity_file': 'phreatic_storage_capacity_file',
         'hydraulic_conductivity_file': 'hydraulic_conductivity_file',
         'porosity_file': 'porosity_file',
         'infiltration_rate_file': 'infiltration_rate_file',
         'max_infiltration_capacity_file': 'max_infiltration_capacity_file',
-        'interception_file': 'interception_file'
+        'interception_file': 'interception_file',
+        'vegetation_height_file': 'vegetation_height_file',
+        'vegetation_drag_coefficient_file': 'vegetation_drag_coefficient_file',
+        'vegetation_stem_count_file': 'vegetation_stem_count_file',
+        'vegetation_stem_diameter_file': 'vegetation_stem_diameter_file'
     }
 
-    def __init__(self, dem_file=None, dem_raw_file=None, equilibrium_infiltration_rate_file=None, frict_coef_file=None, initial_groundwater_level_file=None, initial_waterlevel_file=None, groundwater_hydro_connectivity_file=None, groundwater_impervious_layer_level_file=None, infiltration_decay_period_file=None, initial_infiltration_rate_file=None, leakage_file=None, phreatic_storage_capacity_file=None, hydraulic_conductivity_file=None, porosity_file=None, infiltration_rate_file=None, max_infiltration_capacity_file=None, interception_file=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
+    def __init__(self, dem_file=None, dem_raw_file=None, equilibrium_infiltration_rate_file=None, frict_coef_file=None, initial_groundwater_level_file=None, initial_waterlevel_file=None, groundwater_hydro_connectivity_file=None, groundwater_impervious_layer_level_file=None, infiltration_decay_period_file=None, initial_infiltration_rate_file=None, leakage_file=None, phreatic_storage_capacity_file=None, hydraulic_conductivity_file=None, porosity_file=None, infiltration_rate_file=None, max_infiltration_capacity_file=None, interception_file=None, vegetation_height_file=None, vegetation_drag_coefficient_file=None, vegetation_stem_count_file=None, vegetation_stem_diameter_file=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
         """RasterOptions - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         # True if data is coming from API
         self._fetched_from_api = fetched_from_api
@@ -97,14 +105,18 @@
         self._leakage_file = None
         self._phreatic_storage_capacity_file = None
         self._hydraulic_conductivity_file = None
         self._porosity_file = None
         self._infiltration_rate_file = None
         self._max_infiltration_capacity_file = None
         self._interception_file = None
+        self._vegetation_height_file = None
+        self._vegetation_drag_coefficient_file = None
+        self._vegetation_stem_count_file = None
+        self._vegetation_stem_diameter_file = None
         self.discriminator = None
 
         if dem_file is not None:
             self.dem_file = dem_file
         if dem_raw_file is not None:
             self.dem_raw_file = dem_raw_file
         if equilibrium_infiltration_rate_file is not None:
@@ -133,14 +145,22 @@
             self.porosity_file = porosity_file
         if infiltration_rate_file is not None:
             self.infiltration_rate_file = infiltration_rate_file
         if max_infiltration_capacity_file is not None:
             self.max_infiltration_capacity_file = max_infiltration_capacity_file
         if interception_file is not None:
             self.interception_file = interception_file
+        if vegetation_height_file is not None:
+            self.vegetation_height_file = vegetation_height_file
+        if vegetation_drag_coefficient_file is not None:
+            self.vegetation_drag_coefficient_file = vegetation_drag_coefficient_file
+        if vegetation_stem_count_file is not None:
+            self.vegetation_stem_count_file = vegetation_stem_count_file
+        if vegetation_stem_diameter_file is not None:
+            self.vegetation_stem_diameter_file = vegetation_stem_diameter_file
 
     @property
     def dem_file(self):
         """Gets the dem_file of this RasterOptions.  # noqa: E501
 
 
         :return: The dem_file of this RasterOptions.  # noqa: E501
@@ -593,14 +613,122 @@
             self.__handle_validation_error("Invalid value for `interception_file`, length must be less than or equal to `80`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 interception_file is not None and len(interception_file) < 1):
             self.__handle_validation_error("Invalid value for `interception_file`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._interception_file = interception_file
 
+    @property
+    def vegetation_height_file(self):
+        """Gets the vegetation_height_file of this RasterOptions.  # noqa: E501
+
+
+        :return: The vegetation_height_file of this RasterOptions.  # noqa: E501
+        :rtype: str
+        """
+        return self._vegetation_height_file
+
+    @vegetation_height_file.setter
+    def vegetation_height_file(self, vegetation_height_file):
+        """Sets the vegetation_height_file of this RasterOptions.
+
+
+        :param vegetation_height_file: The vegetation_height_file of this RasterOptions.  # noqa: E501
+        :type: str
+        """
+        if (self.local_vars_configuration.client_side_validation and
+                vegetation_height_file is not None and len(vegetation_height_file) > 80):
+            self.__handle_validation_error("Invalid value for `vegetation_height_file`, length must be less than or equal to `80`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                vegetation_height_file is not None and len(vegetation_height_file) < 1):
+            self.__handle_validation_error("Invalid value for `vegetation_height_file`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._vegetation_height_file = vegetation_height_file
+
+    @property
+    def vegetation_drag_coefficient_file(self):
+        """Gets the vegetation_drag_coefficient_file of this RasterOptions.  # noqa: E501
+
+
+        :return: The vegetation_drag_coefficient_file of this RasterOptions.  # noqa: E501
+        :rtype: str
+        """
+        return self._vegetation_drag_coefficient_file
+
+    @vegetation_drag_coefficient_file.setter
+    def vegetation_drag_coefficient_file(self, vegetation_drag_coefficient_file):
+        """Sets the vegetation_drag_coefficient_file of this RasterOptions.
+
+
+        :param vegetation_drag_coefficient_file: The vegetation_drag_coefficient_file of this RasterOptions.  # noqa: E501
+        :type: str
+        """
+        if (self.local_vars_configuration.client_side_validation and
+                vegetation_drag_coefficient_file is not None and len(vegetation_drag_coefficient_file) > 80):
+            self.__handle_validation_error("Invalid value for `vegetation_drag_coefficient_file`, length must be less than or equal to `80`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                vegetation_drag_coefficient_file is not None and len(vegetation_drag_coefficient_file) < 1):
+            self.__handle_validation_error("Invalid value for `vegetation_drag_coefficient_file`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._vegetation_drag_coefficient_file = vegetation_drag_coefficient_file
+
+    @property
+    def vegetation_stem_count_file(self):
+        """Gets the vegetation_stem_count_file of this RasterOptions.  # noqa: E501
+
+
+        :return: The vegetation_stem_count_file of this RasterOptions.  # noqa: E501
+        :rtype: str
+        """
+        return self._vegetation_stem_count_file
+
+    @vegetation_stem_count_file.setter
+    def vegetation_stem_count_file(self, vegetation_stem_count_file):
+        """Sets the vegetation_stem_count_file of this RasterOptions.
+
+
+        :param vegetation_stem_count_file: The vegetation_stem_count_file of this RasterOptions.  # noqa: E501
+        :type: str
+        """
+        if (self.local_vars_configuration.client_side_validation and
+                vegetation_stem_count_file is not None and len(vegetation_stem_count_file) > 80):
+            self.__handle_validation_error("Invalid value for `vegetation_stem_count_file`, length must be less than or equal to `80`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                vegetation_stem_count_file is not None and len(vegetation_stem_count_file) < 1):
+            self.__handle_validation_error("Invalid value for `vegetation_stem_count_file`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._vegetation_stem_count_file = vegetation_stem_count_file
+
+    @property
+    def vegetation_stem_diameter_file(self):
+        """Gets the vegetation_stem_diameter_file of this RasterOptions.  # noqa: E501
+
+
+        :return: The vegetation_stem_diameter_file of this RasterOptions.  # noqa: E501
+        :rtype: str
+        """
+        return self._vegetation_stem_diameter_file
+
+    @vegetation_stem_diameter_file.setter
+    def vegetation_stem_diameter_file(self, vegetation_stem_diameter_file):
+        """Sets the vegetation_stem_diameter_file of this RasterOptions.
+
+
+        :param vegetation_stem_diameter_file: The vegetation_stem_diameter_file of this RasterOptions.  # noqa: E501
+        :type: str
+        """
+        if (self.local_vars_configuration.client_side_validation and
+                vegetation_stem_diameter_file is not None and len(vegetation_stem_diameter_file) > 80):
+            self.__handle_validation_error("Invalid value for `vegetation_stem_diameter_file`, length must be less than or equal to `80`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                vegetation_stem_diameter_file is not None and len(vegetation_stem_diameter_file) < 1):
+            self.__handle_validation_error("Invalid value for `vegetation_stem_diameter_file`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._vegetation_stem_diameter_file = vegetation_stem_diameter_file
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/refresh.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/refresh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/repository.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/result.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/result_file.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/result_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/revision.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/revision.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/revision_raster.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/revision_raster.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -132,15 +132,15 @@
 
 
         :param type: The type of this RevisionRaster.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
             self.__handle_validation_error("Invalid value for `type`, must not be `None`")  # noqa: E501
-        allowed_values = ["dem_file", "equilibrium_infiltration_rate_file", "frict_coef_file", "initial_groundwater_level_file", "initial_waterlevel_file", "groundwater_hydro_connectivity_file", "groundwater_impervious_layer_level_file", "infiltration_decay_period_file", "initial_infiltration_rate_file", "leakage_file", "phreatic_storage_capacity_file", "hydraulic_conductivity_file", "porosity_file", "infiltration_rate_file", "max_infiltration_capacity_file", "interception_file"]  # noqa: E501
+        allowed_values = ["dem_file", "equilibrium_infiltration_rate_file", "frict_coef_file", "initial_groundwater_level_file", "initial_waterlevel_file", "groundwater_hydro_connectivity_file", "groundwater_impervious_layer_level_file", "infiltration_decay_period_file", "initial_infiltration_rate_file", "leakage_file", "phreatic_storage_capacity_file", "hydraulic_conductivity_file", "porosity_file", "infiltration_rate_file", "max_infiltration_capacity_file", "interception_file", "vegetation_height_file", "vegetation_drag_coefficient_file", "vegetation_stem_count_file", "vegetation_stem_diameter_file"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
             self.__handle_validation_error(
                 "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
                 .format(type, allowed_values)
             )
 
         self._type = type
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/revision_task.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/revision_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/role.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/role.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/saved_state_overview.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/saved_state_overview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/schematisation.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/schematisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/schematisation_revision.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/schematisation_revision.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/settings.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/simulation.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/simulation_channel.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/simulation_channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/simulation_settings_overview.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/simulation_settings_overview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/simulation_status.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_lateral.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -17,15 +17,15 @@
 
 import six
 
 from threedi_api_client.openapi.configuration import Configuration
 
 logger = logging.getLogger(__name__)
 
-class SimulationStatus(object):
+class TimeseriesLateral(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -33,457 +33,400 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'url': 'str',
-        'name': 'str',
         'simulation': 'str',
-        'simulation_id': 'int',
-        'simulation_name': 'str',
-        'simulation_tags': 'list[str]',
-        'threedimodel_slug': 'str',
-        'threedimodel_id': 'int',
-        'has_results': 'bool',
-        'created': 'datetime',
-        'expiry': 'datetime',
-        'time': 'int',
-        'paused': 'bool',
-        'detail': 'object',
-        'exit_code': 'int',
-        'id': 'int'
+        'offset': 'int',
+        'interpolate': 'bool',
+        'values': 'list[list[float]]',
+        'units': 'str',
+        'point': 'Point',
+        'connection_node': 'int',
+        'state': 'str',
+        'state_detail': 'object',
+        'grid_id': 'int',
+        'id': 'int',
+        'uid': 'str'
     }
 
     attribute_map = {
         'url': 'url',
-        'name': 'name',
         'simulation': 'simulation',
-        'simulation_id': 'simulation_id',
-        'simulation_name': 'simulation_name',
-        'simulation_tags': 'simulation_tags',
-        'threedimodel_slug': 'threedimodel_slug',
-        'threedimodel_id': 'threedimodel_id',
-        'has_results': 'has_results',
-        'created': 'created',
-        'expiry': 'expiry',
-        'time': 'time',
-        'paused': 'paused',
-        'detail': 'detail',
-        'exit_code': 'exit_code',
-        'id': 'id'
+        'offset': 'offset',
+        'interpolate': 'interpolate',
+        'values': 'values',
+        'units': 'units',
+        'point': 'point',
+        'connection_node': 'connection_node',
+        'state': 'state',
+        'state_detail': 'state_detail',
+        'grid_id': 'grid_id',
+        'id': 'id',
+        'uid': 'uid'
     }
 
-    def __init__(self, url=None, name=None, simulation=None, simulation_id=None, simulation_name=None, simulation_tags=None, threedimodel_slug=None, threedimodel_id=None, has_results=None, created=None, expiry=None, time=None, paused=None, detail=None, exit_code=None, id=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
-        """SimulationStatus - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, url=None, simulation=None, offset=None, interpolate=None, values=None, units=None, point=None, connection_node=None, state=None, state_detail=None, grid_id=None, id=None, uid=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
+        """TimeseriesLateral - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         # True if data is coming from API
         self._fetched_from_api = fetched_from_api
 
         self._url = None
-        self._name = None
         self._simulation = None
-        self._simulation_id = None
-        self._simulation_name = None
-        self._simulation_tags = None
-        self._threedimodel_slug = None
-        self._threedimodel_id = None
-        self._has_results = None
-        self._created = None
-        self._expiry = None
-        self._time = None
-        self._paused = None
-        self._detail = None
-        self._exit_code = None
+        self._offset = None
+        self._interpolate = None
+        self._values = None
+        self._units = None
+        self._point = None
+        self._connection_node = None
+        self._state = None
+        self._state_detail = None
+        self._grid_id = None
         self._id = None
+        self._uid = None
         self.discriminator = None
 
         if url is not None:
             self.url = url
-        self.name = name
         if simulation is not None:
             self.simulation = simulation
-        if simulation_id is not None:
-            self.simulation_id = simulation_id
-        if simulation_name is not None:
-            self.simulation_name = simulation_name
-        if simulation_tags is not None:
-            self.simulation_tags = simulation_tags
-        if threedimodel_slug is not None:
-            self.threedimodel_slug = threedimodel_slug
-        if threedimodel_id is not None:
-            self.threedimodel_id = threedimodel_id
-        self.has_results = has_results
-        if created is not None:
-            self.created = created
-        self.expiry = expiry
-        self.time = time
-        self.paused = paused
-        self.detail = detail
-        self.exit_code = exit_code
+        self.offset = offset
+        if interpolate is not None:
+            self.interpolate = interpolate
+        self.values = values
+        self.units = units
+        if point is not None:
+            self.point = point
+        self.connection_node = connection_node
+        if state is not None:
+            self.state = state
+        if state_detail is not None:
+            self.state_detail = state_detail
+        if grid_id is not None:
+            self.grid_id = grid_id
         if id is not None:
             self.id = id
+        if uid is not None:
+            self.uid = uid
 
     @property
     def url(self):
-        """Gets the url of this SimulationStatus.  # noqa: E501
+        """Gets the url of this TimeseriesLateral.  # noqa: E501
 
 
-        :return: The url of this SimulationStatus.  # noqa: E501
+        :return: The url of this TimeseriesLateral.  # noqa: E501
         :rtype: str
         """
         return self._url
 
     @url.setter
     def url(self, url):
-        """Sets the url of this SimulationStatus.
+        """Sets the url of this TimeseriesLateral.
 
 
-        :param url: The url of this SimulationStatus.  # noqa: E501
+        :param url: The url of this TimeseriesLateral.  # noqa: E501
         :type: str
         """
 
         self._url = url
 
     @property
-    def name(self):
-        """Gets the name of this SimulationStatus.  # noqa: E501
-
-
-        :return: The name of this SimulationStatus.  # noqa: E501
-        :rtype: str
-        """
-        return self._name
-
-    @name.setter
-    def name(self, name):
-        """Sets the name of this SimulationStatus.
-
-
-        :param name: The name of this SimulationStatus.  # noqa: E501
-        :type: str
-        """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            self.__handle_validation_error("Invalid value for `name`, must not be `None`")  # noqa: E501
-        allowed_values = ["created", "starting", "initialized", "queued", "ended", "postprocessing", "finished", "crashed"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and name not in allowed_values:  # noqa: E501
-            self.__handle_validation_error(
-                "Invalid value for `name` ({0}), must be one of {1}"  # noqa: E501
-                .format(name, allowed_values)
-            )
-
-        self._name = name
-
-    @property
     def simulation(self):
-        """Gets the simulation of this SimulationStatus.  # noqa: E501
+        """Gets the simulation of this TimeseriesLateral.  # noqa: E501
 
 
-        :return: The simulation of this SimulationStatus.  # noqa: E501
+        :return: The simulation of this TimeseriesLateral.  # noqa: E501
         :rtype: str
         """
         return self._simulation
 
     @simulation.setter
     def simulation(self, simulation):
-        """Sets the simulation of this SimulationStatus.
+        """Sets the simulation of this TimeseriesLateral.
 
 
-        :param simulation: The simulation of this SimulationStatus.  # noqa: E501
+        :param simulation: The simulation of this TimeseriesLateral.  # noqa: E501
         :type: str
         """
 
         self._simulation = simulation
 
     @property
-    def simulation_id(self):
-        """Gets the simulation_id of this SimulationStatus.  # noqa: E501
+    def offset(self):
+        """Gets the offset of this TimeseriesLateral.  # noqa: E501
 
+        offset of event in simulation in seconds  # noqa: E501
 
-        :return: The simulation_id of this SimulationStatus.  # noqa: E501
+        :return: The offset of this TimeseriesLateral.  # noqa: E501
         :rtype: int
         """
-        return self._simulation_id
+        return self._offset
 
-    @simulation_id.setter
-    def simulation_id(self, simulation_id):
-        """Sets the simulation_id of this SimulationStatus.
+    @offset.setter
+    def offset(self, offset):
+        """Sets the offset of this TimeseriesLateral.
 
+        offset of event in simulation in seconds  # noqa: E501
 
-        :param simulation_id: The simulation_id of this SimulationStatus.  # noqa: E501
+        :param offset: The offset of this TimeseriesLateral.  # noqa: E501
         :type: int
         """
+        if self.local_vars_configuration.client_side_validation and offset is None:  # noqa: E501
+            self.__handle_validation_error("Invalid value for `offset`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                offset is not None and offset > 2147483647):  # noqa: E501
+            self.__handle_validation_error("Invalid value for `offset`, must be a value less than or equal to `2147483647`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                offset is not None and offset < 0):  # noqa: E501
+            self.__handle_validation_error("Invalid value for `offset`, must be a value greater than or equal to `0`")  # noqa: E501
 
-        self._simulation_id = simulation_id
+        self._offset = offset
 
     @property
-    def simulation_name(self):
-        """Gets the simulation_name of this SimulationStatus.  # noqa: E501
+    def interpolate(self):
+        """Gets the interpolate of this TimeseriesLateral.  # noqa: E501
 
 
-        :return: The simulation_name of this SimulationStatus.  # noqa: E501
-        :rtype: str
+        :return: The interpolate of this TimeseriesLateral.  # noqa: E501
+        :rtype: bool
         """
-        return self._simulation_name
+        return self._interpolate
 
-    @simulation_name.setter
-    def simulation_name(self, simulation_name):
-        """Sets the simulation_name of this SimulationStatus.
+    @interpolate.setter
+    def interpolate(self, interpolate):
+        """Sets the interpolate of this TimeseriesLateral.
 
 
-        :param simulation_name: The simulation_name of this SimulationStatus.  # noqa: E501
-        :type: str
+        :param interpolate: The interpolate of this TimeseriesLateral.  # noqa: E501
+        :type: bool
         """
 
-        self._simulation_name = simulation_name
+        self._interpolate = interpolate
 
     @property
-    def simulation_tags(self):
-        """Gets the simulation_tags of this SimulationStatus.  # noqa: E501
+    def values(self):
+        """Gets the values of this TimeseriesLateral.  # noqa: E501
 
+        Timeseries provided as a nested list. The inner list consists of exactly 2 values: timestamp, value  # noqa: E501
 
-        :return: The simulation_tags of this SimulationStatus.  # noqa: E501
-        :rtype: list[str]
+        :return: The values of this TimeseriesLateral.  # noqa: E501
+        :rtype: list[list[float]]
         """
-        return self._simulation_tags
+        return self._values
 
-    @simulation_tags.setter
-    def simulation_tags(self, simulation_tags):
-        """Sets the simulation_tags of this SimulationStatus.
+    @values.setter
+    def values(self, values):
+        """Sets the values of this TimeseriesLateral.
 
+        Timeseries provided as a nested list. The inner list consists of exactly 2 values: timestamp, value  # noqa: E501
 
-        :param simulation_tags: The simulation_tags of this SimulationStatus.  # noqa: E501
-        :type: list[str]
+        :param values: The values of this TimeseriesLateral.  # noqa: E501
+        :type: list[list[float]]
         """
+        if self.local_vars_configuration.client_side_validation and values is None:  # noqa: E501
+            self.__handle_validation_error("Invalid value for `values`, must not be `None`")  # noqa: E501
 
-        self._simulation_tags = simulation_tags
+        self._values = values
 
     @property
-    def threedimodel_slug(self):
-        """Gets the threedimodel_slug of this SimulationStatus.  # noqa: E501
+    def units(self):
+        """Gets the units of this TimeseriesLateral.  # noqa: E501
 
+        'm3/s' (only option for now)  # noqa: E501
 
-        :return: The threedimodel_slug of this SimulationStatus.  # noqa: E501
+        :return: The units of this TimeseriesLateral.  # noqa: E501
         :rtype: str
         """
-        return self._threedimodel_slug
+        return self._units
 
-    @threedimodel_slug.setter
-    def threedimodel_slug(self, threedimodel_slug):
-        """Sets the threedimodel_slug of this SimulationStatus.
+    @units.setter
+    def units(self, units):
+        """Sets the units of this TimeseriesLateral.
 
+        'm3/s' (only option for now)  # noqa: E501
 
-        :param threedimodel_slug: The threedimodel_slug of this SimulationStatus.  # noqa: E501
+        :param units: The units of this TimeseriesLateral.  # noqa: E501
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and units is None:  # noqa: E501
+            self.__handle_validation_error("Invalid value for `units`, must not be `None`")  # noqa: E501
+        allowed_values = ["m3/s"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and units not in allowed_values:  # noqa: E501
+            self.__handle_validation_error(
+                "Invalid value for `units` ({0}), must be one of {1}"  # noqa: E501
+                .format(units, allowed_values)
+            )
 
-        self._threedimodel_slug = threedimodel_slug
-
-    @property
-    def threedimodel_id(self):
-        """Gets the threedimodel_id of this SimulationStatus.  # noqa: E501
-
-
-        :return: The threedimodel_id of this SimulationStatus.  # noqa: E501
-        :rtype: int
-        """
-        return self._threedimodel_id
-
-    @threedimodel_id.setter
-    def threedimodel_id(self, threedimodel_id):
-        """Sets the threedimodel_id of this SimulationStatus.
-
-
-        :param threedimodel_id: The threedimodel_id of this SimulationStatus.  # noqa: E501
-        :type: int
-        """
-
-        self._threedimodel_id = threedimodel_id
-
-    @property
-    def has_results(self):
-        """Gets the has_results of this SimulationStatus.  # noqa: E501
-
-
-        :return: The has_results of this SimulationStatus.  # noqa: E501
-        :rtype: bool
-        """
-        return self._has_results
-
-    @has_results.setter
-    def has_results(self, has_results):
-        """Sets the has_results of this SimulationStatus.
-
-
-        :param has_results: The has_results of this SimulationStatus.  # noqa: E501
-        :type: bool
-        """
-
-        self._has_results = has_results
-
-    @property
-    def created(self):
-        """Gets the created of this SimulationStatus.  # noqa: E501
-
-
-        :return: The created of this SimulationStatus.  # noqa: E501
-        :rtype: datetime
-        """
-        return self._created
-
-    @created.setter
-    def created(self, created):
-        """Sets the created of this SimulationStatus.
-
-
-        :param created: The created of this SimulationStatus.  # noqa: E501
-        :type: datetime
-        """
-
-        self._created = created
+        self._units = units
 
     @property
-    def expiry(self):
-        """Gets the expiry of this SimulationStatus.  # noqa: E501
+    def point(self):
+        """Gets the point of this TimeseriesLateral.  # noqa: E501
 
 
-        :return: The expiry of this SimulationStatus.  # noqa: E501
-        :rtype: datetime
+        :return: The point of this TimeseriesLateral.  # noqa: E501
+        :rtype: Point
         """
-        return self._expiry
+        return self._point
 
-    @expiry.setter
-    def expiry(self, expiry):
-        """Sets the expiry of this SimulationStatus.
+    @point.setter
+    def point(self, point):
+        """Sets the point of this TimeseriesLateral.
 
 
-        :param expiry: The expiry of this SimulationStatus.  # noqa: E501
-        :type: datetime
+        :param point: The point of this TimeseriesLateral.  # noqa: E501
+        :type: Point
         """
 
-        self._expiry = expiry
+        self._point = point
 
     @property
-    def time(self):
-        """Gets the time of this SimulationStatus.  # noqa: E501
+    def connection_node(self):
+        """Gets the connection_node of this TimeseriesLateral.  # noqa: E501
 
-        simulation time in seconds  # noqa: E501
 
-        :return: The time of this SimulationStatus.  # noqa: E501
+        :return: The connection_node of this TimeseriesLateral.  # noqa: E501
         :rtype: int
         """
-        return self._time
+        return self._connection_node
 
-    @time.setter
-    def time(self, time):
-        """Sets the time of this SimulationStatus.
+    @connection_node.setter
+    def connection_node(self, connection_node):
+        """Sets the connection_node of this TimeseriesLateral.
 
-        simulation time in seconds  # noqa: E501
 
-        :param time: The time of this SimulationStatus.  # noqa: E501
+        :param connection_node: The connection_node of this TimeseriesLateral.  # noqa: E501
         :type: int
         """
         if (self.local_vars_configuration.client_side_validation and
-                time is not None and time > 2147483647):  # noqa: E501
-            self.__handle_validation_error("Invalid value for `time`, must be a value less than or equal to `2147483647`")  # noqa: E501
+                connection_node is not None and connection_node > 2147483647):  # noqa: E501
+            self.__handle_validation_error("Invalid value for `connection_node`, must be a value less than or equal to `2147483647`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                time is not None and time < 0):  # noqa: E501
-            self.__handle_validation_error("Invalid value for `time`, must be a value greater than or equal to `0`")  # noqa: E501
+                connection_node is not None and connection_node < -2147483648):  # noqa: E501
+            self.__handle_validation_error("Invalid value for `connection_node`, must be a value greater than or equal to `-2147483648`")  # noqa: E501
 
-        self._time = time
+        self._connection_node = connection_node
 
     @property
-    def paused(self):
-        """Gets the paused of this SimulationStatus.  # noqa: E501
+    def state(self):
+        """Gets the state of this TimeseriesLateral.  # noqa: E501
 
 
-        :return: The paused of this SimulationStatus.  # noqa: E501
-        :rtype: bool
+        :return: The state of this TimeseriesLateral.  # noqa: E501
+        :rtype: str
         """
-        return self._paused
+        return self._state
 
-    @paused.setter
-    def paused(self, paused):
-        """Sets the paused of this SimulationStatus.
+    @state.setter
+    def state(self, state):
+        """Sets the state of this TimeseriesLateral.
 
 
-        :param paused: The paused of this SimulationStatus.  # noqa: E501
-        :type: bool
+        :param state: The state of this TimeseriesLateral.  # noqa: E501
+        :type: str
         """
+        allowed_values = ["processing", "valid", "invalid"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and state not in allowed_values:  # noqa: E501
+            self.__handle_validation_error(
+                "Invalid value for `state` ({0}), must be one of {1}"  # noqa: E501
+                .format(state, allowed_values)
+            )
 
-        self._paused = paused
+        self._state = state
 
     @property
-    def detail(self):
-        """Gets the detail of this SimulationStatus.  # noqa: E501
+    def state_detail(self):
+        """Gets the state_detail of this TimeseriesLateral.  # noqa: E501
 
 
-        :return: The detail of this SimulationStatus.  # noqa: E501
+        :return: The state_detail of this TimeseriesLateral.  # noqa: E501
         :rtype: object
         """
-        return self._detail
+        return self._state_detail
 
-    @detail.setter
-    def detail(self, detail):
-        """Sets the detail of this SimulationStatus.
+    @state_detail.setter
+    def state_detail(self, state_detail):
+        """Sets the state_detail of this TimeseriesLateral.
 
 
-        :param detail: The detail of this SimulationStatus.  # noqa: E501
+        :param state_detail: The state_detail of this TimeseriesLateral.  # noqa: E501
         :type: object
         """
 
-        self._detail = detail
+        self._state_detail = state_detail
 
     @property
-    def exit_code(self):
-        """Gets the exit_code of this SimulationStatus.  # noqa: E501
+    def grid_id(self):
+        """Gets the grid_id of this TimeseriesLateral.  # noqa: E501
 
-        only available for final statuses like 'finished' or 'crashed'. Gives detailed insight to the application state when the simulation finished  # noqa: E501
 
-        :return: The exit_code of this SimulationStatus.  # noqa: E501
+        :return: The grid_id of this TimeseriesLateral.  # noqa: E501
         :rtype: int
         """
-        return self._exit_code
+        return self._grid_id
 
-    @exit_code.setter
-    def exit_code(self, exit_code):
-        """Sets the exit_code of this SimulationStatus.
+    @grid_id.setter
+    def grid_id(self, grid_id):
+        """Sets the grid_id of this TimeseriesLateral.
 
-        only available for final statuses like 'finished' or 'crashed'. Gives detailed insight to the application state when the simulation finished  # noqa: E501
 
-        :param exit_code: The exit_code of this SimulationStatus.  # noqa: E501
+        :param grid_id: The grid_id of this TimeseriesLateral.  # noqa: E501
         :type: int
         """
 
-        self._exit_code = exit_code
+        self._grid_id = grid_id
 
     @property
     def id(self):
-        """Gets the id of this SimulationStatus.  # noqa: E501
+        """Gets the id of this TimeseriesLateral.  # noqa: E501
 
 
-        :return: The id of this SimulationStatus.  # noqa: E501
+        :return: The id of this TimeseriesLateral.  # noqa: E501
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this SimulationStatus.
+        """Sets the id of this TimeseriesLateral.
 
 
-        :param id: The id of this SimulationStatus.  # noqa: E501
+        :param id: The id of this TimeseriesLateral.  # noqa: E501
         :type: int
         """
 
         self._id = id
 
+    @property
+    def uid(self):
+        """Gets the uid of this TimeseriesLateral.  # noqa: E501
+
+
+        :return: The uid of this TimeseriesLateral.  # noqa: E501
+        :rtype: str
+        """
+        return self._uid
+
+    @uid.setter
+    def uid(self, uid):
+        """Sets the uid of this TimeseriesLateral.
+
+
+        :param uid: The uid of this TimeseriesLateral.  # noqa: E501
+        :type: str
+        """
+
+        self._uid = uid
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -518,18 +461,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SimulationStatus):
+        if not isinstance(other, TimeseriesLateral):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SimulationStatus):
+        if not isinstance(other, TimeseriesLateral):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/simulation_status_statistics.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/simulation_status_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/simulation_update.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/simulation_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/sqlite.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/sqlite_file_upload.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/sqlite_file_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/stable_threshold_saved_state.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/stable_threshold_saved_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/status.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/table_structure_control.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/table_structure_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/template.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/threedi_model.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/threedi_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/threedi_model_saved_state.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/threedi_model_saved_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/threedi_model_task.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/threedi_model_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/threshold.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/threshold.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/time_step_settings.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/time_step_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timed_saved_state_update.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/timed_saved_state_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timed_structure_control.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/timed_structure_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeout.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_lateral.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_rain_overview.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -17,15 +17,15 @@
 
 import six
 
 from threedi_api_client.openapi.configuration import Configuration
 
 logger = logging.getLogger(__name__)
 
-class TimeseriesLateral(object):
+class TimeseriesRainOverview(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,398 +35,311 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'url': 'str',
         'simulation': 'str',
         'offset': 'int',
+        'duration': 'int',
         'interpolate': 'bool',
         'values': 'list[list[float]]',
         'units': 'str',
-        'point': 'Point',
-        'connection_node': 'int',
-        'state': 'str',
-        'state_detail': 'object',
-        'grid_id': 'int',
-        'id': 'int',
-        'uid': 'str'
+        'constant': 'bool',
+        'uid': 'str',
+        'id': 'int'
     }
 
     attribute_map = {
         'url': 'url',
         'simulation': 'simulation',
         'offset': 'offset',
+        'duration': 'duration',
         'interpolate': 'interpolate',
         'values': 'values',
         'units': 'units',
-        'point': 'point',
-        'connection_node': 'connection_node',
-        'state': 'state',
-        'state_detail': 'state_detail',
-        'grid_id': 'grid_id',
-        'id': 'id',
-        'uid': 'uid'
+        'constant': 'constant',
+        'uid': 'uid',
+        'id': 'id'
     }
 
-    def __init__(self, url=None, simulation=None, offset=None, interpolate=None, values=None, units=None, point=None, connection_node=None, state=None, state_detail=None, grid_id=None, id=None, uid=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
-        """TimeseriesLateral - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, url=None, simulation=None, offset=None, duration=None, interpolate=None, values=None, units=None, constant=None, uid=None, id=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
+        """TimeseriesRainOverview - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         # True if data is coming from API
         self._fetched_from_api = fetched_from_api
 
         self._url = None
         self._simulation = None
         self._offset = None
+        self._duration = None
         self._interpolate = None
         self._values = None
         self._units = None
-        self._point = None
-        self._connection_node = None
-        self._state = None
-        self._state_detail = None
-        self._grid_id = None
-        self._id = None
+        self._constant = None
         self._uid = None
+        self._id = None
         self.discriminator = None
 
         if url is not None:
             self.url = url
         if simulation is not None:
             self.simulation = simulation
         self.offset = offset
+        if duration is not None:
+            self.duration = duration
         if interpolate is not None:
             self.interpolate = interpolate
         self.values = values
         self.units = units
-        if point is not None:
-            self.point = point
-        self.connection_node = connection_node
-        if state is not None:
-            self.state = state
-        if state_detail is not None:
-            self.state_detail = state_detail
-        if grid_id is not None:
-            self.grid_id = grid_id
-        if id is not None:
-            self.id = id
+        if constant is not None:
+            self.constant = constant
         if uid is not None:
             self.uid = uid
+        if id is not None:
+            self.id = id
 
     @property
     def url(self):
-        """Gets the url of this TimeseriesLateral.  # noqa: E501
+        """Gets the url of this TimeseriesRainOverview.  # noqa: E501
 
 
-        :return: The url of this TimeseriesLateral.  # noqa: E501
+        :return: The url of this TimeseriesRainOverview.  # noqa: E501
         :rtype: str
         """
         return self._url
 
     @url.setter
     def url(self, url):
-        """Sets the url of this TimeseriesLateral.
+        """Sets the url of this TimeseriesRainOverview.
 
 
-        :param url: The url of this TimeseriesLateral.  # noqa: E501
+        :param url: The url of this TimeseriesRainOverview.  # noqa: E501
         :type: str
         """
 
         self._url = url
 
     @property
     def simulation(self):
-        """Gets the simulation of this TimeseriesLateral.  # noqa: E501
+        """Gets the simulation of this TimeseriesRainOverview.  # noqa: E501
 
 
-        :return: The simulation of this TimeseriesLateral.  # noqa: E501
+        :return: The simulation of this TimeseriesRainOverview.  # noqa: E501
         :rtype: str
         """
         return self._simulation
 
     @simulation.setter
     def simulation(self, simulation):
-        """Sets the simulation of this TimeseriesLateral.
+        """Sets the simulation of this TimeseriesRainOverview.
 
 
-        :param simulation: The simulation of this TimeseriesLateral.  # noqa: E501
+        :param simulation: The simulation of this TimeseriesRainOverview.  # noqa: E501
         :type: str
         """
 
         self._simulation = simulation
 
     @property
     def offset(self):
-        """Gets the offset of this TimeseriesLateral.  # noqa: E501
+        """Gets the offset of this TimeseriesRainOverview.  # noqa: E501
 
         offset of event in simulation in seconds  # noqa: E501
 
-        :return: The offset of this TimeseriesLateral.  # noqa: E501
+        :return: The offset of this TimeseriesRainOverview.  # noqa: E501
         :rtype: int
         """
         return self._offset
 
     @offset.setter
     def offset(self, offset):
-        """Sets the offset of this TimeseriesLateral.
+        """Sets the offset of this TimeseriesRainOverview.
 
         offset of event in simulation in seconds  # noqa: E501
 
-        :param offset: The offset of this TimeseriesLateral.  # noqa: E501
+        :param offset: The offset of this TimeseriesRainOverview.  # noqa: E501
         :type: int
         """
         if self.local_vars_configuration.client_side_validation and offset is None:  # noqa: E501
             self.__handle_validation_error("Invalid value for `offset`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 offset is not None and offset > 2147483647):  # noqa: E501
             self.__handle_validation_error("Invalid value for `offset`, must be a value less than or equal to `2147483647`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 offset is not None and offset < 0):  # noqa: E501
             self.__handle_validation_error("Invalid value for `offset`, must be a value greater than or equal to `0`")  # noqa: E501
 
         self._offset = offset
 
     @property
+    def duration(self):
+        """Gets the duration of this TimeseriesRainOverview.  # noqa: E501
+
+        event duration in seconds. -9999 is the 'infinite duration' value (only allowed in conjunction with infinite simulations  # noqa: E501
+
+        :return: The duration of this TimeseriesRainOverview.  # noqa: E501
+        :rtype: int
+        """
+        return self._duration
+
+    @duration.setter
+    def duration(self, duration):
+        """Sets the duration of this TimeseriesRainOverview.
+
+        event duration in seconds. -9999 is the 'infinite duration' value (only allowed in conjunction with infinite simulations  # noqa: E501
+
+        :param duration: The duration of this TimeseriesRainOverview.  # noqa: E501
+        :type: int
+        """
+
+        self._duration = duration
+
+    @property
     def interpolate(self):
-        """Gets the interpolate of this TimeseriesLateral.  # noqa: E501
+        """Gets the interpolate of this TimeseriesRainOverview.  # noqa: E501
 
 
-        :return: The interpolate of this TimeseriesLateral.  # noqa: E501
+        :return: The interpolate of this TimeseriesRainOverview.  # noqa: E501
         :rtype: bool
         """
         return self._interpolate
 
     @interpolate.setter
     def interpolate(self, interpolate):
-        """Sets the interpolate of this TimeseriesLateral.
+        """Sets the interpolate of this TimeseriesRainOverview.
 
 
-        :param interpolate: The interpolate of this TimeseriesLateral.  # noqa: E501
+        :param interpolate: The interpolate of this TimeseriesRainOverview.  # noqa: E501
         :type: bool
         """
 
         self._interpolate = interpolate
 
     @property
     def values(self):
-        """Gets the values of this TimeseriesLateral.  # noqa: E501
+        """Gets the values of this TimeseriesRainOverview.  # noqa: E501
 
         Timeseries provided as a nested list. The inner list consists of exactly 2 values: timestamp, value  # noqa: E501
 
-        :return: The values of this TimeseriesLateral.  # noqa: E501
+        :return: The values of this TimeseriesRainOverview.  # noqa: E501
         :rtype: list[list[float]]
         """
         return self._values
 
     @values.setter
     def values(self, values):
-        """Sets the values of this TimeseriesLateral.
+        """Sets the values of this TimeseriesRainOverview.
 
         Timeseries provided as a nested list. The inner list consists of exactly 2 values: timestamp, value  # noqa: E501
 
-        :param values: The values of this TimeseriesLateral.  # noqa: E501
+        :param values: The values of this TimeseriesRainOverview.  # noqa: E501
         :type: list[list[float]]
         """
         if self.local_vars_configuration.client_side_validation and values is None:  # noqa: E501
             self.__handle_validation_error("Invalid value for `values`, must not be `None`")  # noqa: E501
 
         self._values = values
 
     @property
     def units(self):
-        """Gets the units of this TimeseriesLateral.  # noqa: E501
+        """Gets the units of this TimeseriesRainOverview.  # noqa: E501
 
-        'm3/s' (only option for now)  # noqa: E501
+        m/s is only option for now  # noqa: E501
 
-        :return: The units of this TimeseriesLateral.  # noqa: E501
+        :return: The units of this TimeseriesRainOverview.  # noqa: E501
         :rtype: str
         """
         return self._units
 
     @units.setter
     def units(self, units):
-        """Sets the units of this TimeseriesLateral.
+        """Sets the units of this TimeseriesRainOverview.
 
-        'm3/s' (only option for now)  # noqa: E501
+        m/s is only option for now  # noqa: E501
 
-        :param units: The units of this TimeseriesLateral.  # noqa: E501
+        :param units: The units of this TimeseriesRainOverview.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and units is None:  # noqa: E501
             self.__handle_validation_error("Invalid value for `units`, must not be `None`")  # noqa: E501
-        allowed_values = ["m3/s"]  # noqa: E501
+        allowed_values = ["m/s"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and units not in allowed_values:  # noqa: E501
             self.__handle_validation_error(
                 "Invalid value for `units` ({0}), must be one of {1}"  # noqa: E501
                 .format(units, allowed_values)
             )
 
         self._units = units
 
     @property
-    def point(self):
-        """Gets the point of this TimeseriesLateral.  # noqa: E501
-
-
-        :return: The point of this TimeseriesLateral.  # noqa: E501
-        :rtype: Point
-        """
-        return self._point
-
-    @point.setter
-    def point(self, point):
-        """Sets the point of this TimeseriesLateral.
-
-
-        :param point: The point of this TimeseriesLateral.  # noqa: E501
-        :type: Point
-        """
-
-        self._point = point
-
-    @property
-    def connection_node(self):
-        """Gets the connection_node of this TimeseriesLateral.  # noqa: E501
+    def constant(self):
+        """Gets the constant of this TimeseriesRainOverview.  # noqa: E501
 
 
-        :return: The connection_node of this TimeseriesLateral.  # noqa: E501
-        :rtype: int
+        :return: The constant of this TimeseriesRainOverview.  # noqa: E501
+        :rtype: bool
         """
-        return self._connection_node
+        return self._constant
 
-    @connection_node.setter
-    def connection_node(self, connection_node):
-        """Sets the connection_node of this TimeseriesLateral.
+    @constant.setter
+    def constant(self, constant):
+        """Sets the constant of this TimeseriesRainOverview.
 
 
-        :param connection_node: The connection_node of this TimeseriesLateral.  # noqa: E501
-        :type: int
+        :param constant: The constant of this TimeseriesRainOverview.  # noqa: E501
+        :type: bool
         """
-        if (self.local_vars_configuration.client_side_validation and
-                connection_node is not None and connection_node > 2147483647):  # noqa: E501
-            self.__handle_validation_error("Invalid value for `connection_node`, must be a value less than or equal to `2147483647`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                connection_node is not None and connection_node < -2147483648):  # noqa: E501
-            self.__handle_validation_error("Invalid value for `connection_node`, must be a value greater than or equal to `-2147483648`")  # noqa: E501
 
-        self._connection_node = connection_node
+        self._constant = constant
 
     @property
-    def state(self):
-        """Gets the state of this TimeseriesLateral.  # noqa: E501
+    def uid(self):
+        """Gets the uid of this TimeseriesRainOverview.  # noqa: E501
 
 
-        :return: The state of this TimeseriesLateral.  # noqa: E501
+        :return: The uid of this TimeseriesRainOverview.  # noqa: E501
         :rtype: str
         """
-        return self._state
+        return self._uid
 
-    @state.setter
-    def state(self, state):
-        """Sets the state of this TimeseriesLateral.
+    @uid.setter
+    def uid(self, uid):
+        """Sets the uid of this TimeseriesRainOverview.
 
 
-        :param state: The state of this TimeseriesLateral.  # noqa: E501
+        :param uid: The uid of this TimeseriesRainOverview.  # noqa: E501
         :type: str
         """
-        allowed_values = ["processing", "valid", "invalid"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and state not in allowed_values:  # noqa: E501
-            self.__handle_validation_error(
-                "Invalid value for `state` ({0}), must be one of {1}"  # noqa: E501
-                .format(state, allowed_values)
-            )
-
-        self._state = state
-
-    @property
-    def state_detail(self):
-        """Gets the state_detail of this TimeseriesLateral.  # noqa: E501
-
-
-        :return: The state_detail of this TimeseriesLateral.  # noqa: E501
-        :rtype: object
-        """
-        return self._state_detail
-
-    @state_detail.setter
-    def state_detail(self, state_detail):
-        """Sets the state_detail of this TimeseriesLateral.
-
-
-        :param state_detail: The state_detail of this TimeseriesLateral.  # noqa: E501
-        :type: object
-        """
-
-        self._state_detail = state_detail
-
-    @property
-    def grid_id(self):
-        """Gets the grid_id of this TimeseriesLateral.  # noqa: E501
-
-
-        :return: The grid_id of this TimeseriesLateral.  # noqa: E501
-        :rtype: int
-        """
-        return self._grid_id
-
-    @grid_id.setter
-    def grid_id(self, grid_id):
-        """Sets the grid_id of this TimeseriesLateral.
-
-
-        :param grid_id: The grid_id of this TimeseriesLateral.  # noqa: E501
-        :type: int
-        """
 
-        self._grid_id = grid_id
+        self._uid = uid
 
     @property
     def id(self):
-        """Gets the id of this TimeseriesLateral.  # noqa: E501
+        """Gets the id of this TimeseriesRainOverview.  # noqa: E501
 
 
-        :return: The id of this TimeseriesLateral.  # noqa: E501
+        :return: The id of this TimeseriesRainOverview.  # noqa: E501
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this TimeseriesLateral.
+        """Sets the id of this TimeseriesRainOverview.
 
 
-        :param id: The id of this TimeseriesLateral.  # noqa: E501
+        :param id: The id of this TimeseriesRainOverview.  # noqa: E501
         :type: int
         """
 
         self._id = id
 
-    @property
-    def uid(self):
-        """Gets the uid of this TimeseriesLateral.  # noqa: E501
-
-
-        :return: The uid of this TimeseriesLateral.  # noqa: E501
-        :rtype: str
-        """
-        return self._uid
-
-    @uid.setter
-    def uid(self, uid):
-        """Sets the uid of this TimeseriesLateral.
-
-
-        :param uid: The uid of this TimeseriesLateral.  # noqa: E501
-        :type: str
-        """
-
-        self._uid = uid
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -461,18 +374,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TimeseriesLateral):
+        if not isinstance(other, TimeseriesRainOverview):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TimeseriesLateral):
+        if not isinstance(other, TimeseriesRainOverview):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_leakage.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_leakage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_leakage_overview.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_leakage_overview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_local_rain.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_local_rain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_rain.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_rain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_rain_overview.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_sources_sinks_overview.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -17,15 +17,15 @@
 
 import six
 
 from threedi_api_client.openapi.configuration import Configuration
 
 logger = logging.getLogger(__name__)
 
-class TimeseriesRainOverview(object):
+class TimeseriesSourcesSinksOverview(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,235 +35,207 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'url': 'str',
         'simulation': 'str',
         'offset': 'int',
-        'duration': 'int',
         'interpolate': 'bool',
         'values': 'list[list[float]]',
         'units': 'str',
         'constant': 'bool',
         'uid': 'str',
         'id': 'int'
     }
 
     attribute_map = {
         'url': 'url',
         'simulation': 'simulation',
         'offset': 'offset',
-        'duration': 'duration',
         'interpolate': 'interpolate',
         'values': 'values',
         'units': 'units',
         'constant': 'constant',
         'uid': 'uid',
         'id': 'id'
     }
 
-    def __init__(self, url=None, simulation=None, offset=None, duration=None, interpolate=None, values=None, units=None, constant=None, uid=None, id=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
-        """TimeseriesRainOverview - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, url=None, simulation=None, offset=None, interpolate=None, values=None, units=None, constant=None, uid=None, id=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
+        """TimeseriesSourcesSinksOverview - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         # True if data is coming from API
         self._fetched_from_api = fetched_from_api
 
         self._url = None
         self._simulation = None
         self._offset = None
-        self._duration = None
         self._interpolate = None
         self._values = None
         self._units = None
         self._constant = None
         self._uid = None
         self._id = None
         self.discriminator = None
 
         if url is not None:
             self.url = url
         if simulation is not None:
             self.simulation = simulation
         self.offset = offset
-        if duration is not None:
-            self.duration = duration
         if interpolate is not None:
             self.interpolate = interpolate
         self.values = values
         self.units = units
         if constant is not None:
             self.constant = constant
         if uid is not None:
             self.uid = uid
         if id is not None:
             self.id = id
 
     @property
     def url(self):
-        """Gets the url of this TimeseriesRainOverview.  # noqa: E501
+        """Gets the url of this TimeseriesSourcesSinksOverview.  # noqa: E501
 
 
-        :return: The url of this TimeseriesRainOverview.  # noqa: E501
+        :return: The url of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :rtype: str
         """
         return self._url
 
     @url.setter
     def url(self, url):
-        """Sets the url of this TimeseriesRainOverview.
+        """Sets the url of this TimeseriesSourcesSinksOverview.
 
 
-        :param url: The url of this TimeseriesRainOverview.  # noqa: E501
+        :param url: The url of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :type: str
         """
 
         self._url = url
 
     @property
     def simulation(self):
-        """Gets the simulation of this TimeseriesRainOverview.  # noqa: E501
+        """Gets the simulation of this TimeseriesSourcesSinksOverview.  # noqa: E501
 
 
-        :return: The simulation of this TimeseriesRainOverview.  # noqa: E501
+        :return: The simulation of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :rtype: str
         """
         return self._simulation
 
     @simulation.setter
     def simulation(self, simulation):
-        """Sets the simulation of this TimeseriesRainOverview.
+        """Sets the simulation of this TimeseriesSourcesSinksOverview.
 
 
-        :param simulation: The simulation of this TimeseriesRainOverview.  # noqa: E501
+        :param simulation: The simulation of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :type: str
         """
 
         self._simulation = simulation
 
     @property
     def offset(self):
-        """Gets the offset of this TimeseriesRainOverview.  # noqa: E501
+        """Gets the offset of this TimeseriesSourcesSinksOverview.  # noqa: E501
 
         offset of event in simulation in seconds  # noqa: E501
 
-        :return: The offset of this TimeseriesRainOverview.  # noqa: E501
+        :return: The offset of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :rtype: int
         """
         return self._offset
 
     @offset.setter
     def offset(self, offset):
-        """Sets the offset of this TimeseriesRainOverview.
+        """Sets the offset of this TimeseriesSourcesSinksOverview.
 
         offset of event in simulation in seconds  # noqa: E501
 
-        :param offset: The offset of this TimeseriesRainOverview.  # noqa: E501
+        :param offset: The offset of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :type: int
         """
         if self.local_vars_configuration.client_side_validation and offset is None:  # noqa: E501
             self.__handle_validation_error("Invalid value for `offset`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 offset is not None and offset > 2147483647):  # noqa: E501
             self.__handle_validation_error("Invalid value for `offset`, must be a value less than or equal to `2147483647`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 offset is not None and offset < 0):  # noqa: E501
             self.__handle_validation_error("Invalid value for `offset`, must be a value greater than or equal to `0`")  # noqa: E501
 
         self._offset = offset
 
     @property
-    def duration(self):
-        """Gets the duration of this TimeseriesRainOverview.  # noqa: E501
-
-        event duration in seconds. -9999 is the 'infinite duration' value (only allowed in conjunction with infinite simulations  # noqa: E501
-
-        :return: The duration of this TimeseriesRainOverview.  # noqa: E501
-        :rtype: int
-        """
-        return self._duration
-
-    @duration.setter
-    def duration(self, duration):
-        """Sets the duration of this TimeseriesRainOverview.
-
-        event duration in seconds. -9999 is the 'infinite duration' value (only allowed in conjunction with infinite simulations  # noqa: E501
-
-        :param duration: The duration of this TimeseriesRainOverview.  # noqa: E501
-        :type: int
-        """
-
-        self._duration = duration
-
-    @property
     def interpolate(self):
-        """Gets the interpolate of this TimeseriesRainOverview.  # noqa: E501
+        """Gets the interpolate of this TimeseriesSourcesSinksOverview.  # noqa: E501
 
 
-        :return: The interpolate of this TimeseriesRainOverview.  # noqa: E501
+        :return: The interpolate of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :rtype: bool
         """
         return self._interpolate
 
     @interpolate.setter
     def interpolate(self, interpolate):
-        """Sets the interpolate of this TimeseriesRainOverview.
+        """Sets the interpolate of this TimeseriesSourcesSinksOverview.
 
 
-        :param interpolate: The interpolate of this TimeseriesRainOverview.  # noqa: E501
+        :param interpolate: The interpolate of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :type: bool
         """
 
         self._interpolate = interpolate
 
     @property
     def values(self):
-        """Gets the values of this TimeseriesRainOverview.  # noqa: E501
+        """Gets the values of this TimeseriesSourcesSinksOverview.  # noqa: E501
 
         Timeseries provided as a nested list. The inner list consists of exactly 2 values: timestamp, value  # noqa: E501
 
-        :return: The values of this TimeseriesRainOverview.  # noqa: E501
+        :return: The values of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :rtype: list[list[float]]
         """
         return self._values
 
     @values.setter
     def values(self, values):
-        """Sets the values of this TimeseriesRainOverview.
+        """Sets the values of this TimeseriesSourcesSinksOverview.
 
         Timeseries provided as a nested list. The inner list consists of exactly 2 values: timestamp, value  # noqa: E501
 
-        :param values: The values of this TimeseriesRainOverview.  # noqa: E501
+        :param values: The values of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :type: list[list[float]]
         """
         if self.local_vars_configuration.client_side_validation and values is None:  # noqa: E501
             self.__handle_validation_error("Invalid value for `values`, must not be `None`")  # noqa: E501
 
         self._values = values
 
     @property
     def units(self):
-        """Gets the units of this TimeseriesRainOverview.  # noqa: E501
+        """Gets the units of this TimeseriesSourcesSinksOverview.  # noqa: E501
 
-        m/s is only option for now  # noqa: E501
+        'm/s' (only option for now)  # noqa: E501
 
-        :return: The units of this TimeseriesRainOverview.  # noqa: E501
+        :return: The units of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :rtype: str
         """
         return self._units
 
     @units.setter
     def units(self, units):
-        """Sets the units of this TimeseriesRainOverview.
+        """Sets the units of this TimeseriesSourcesSinksOverview.
 
-        m/s is only option for now  # noqa: E501
+        'm/s' (only option for now)  # noqa: E501
 
-        :param units: The units of this TimeseriesRainOverview.  # noqa: E501
+        :param units: The units of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and units is None:  # noqa: E501
             self.__handle_validation_error("Invalid value for `units`, must not be `None`")  # noqa: E501
         allowed_values = ["m/s"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and units not in allowed_values:  # noqa: E501
             self.__handle_validation_error(
@@ -271,70 +243,70 @@
                 .format(units, allowed_values)
             )
 
         self._units = units
 
     @property
     def constant(self):
-        """Gets the constant of this TimeseriesRainOverview.  # noqa: E501
+        """Gets the constant of this TimeseriesSourcesSinksOverview.  # noqa: E501
 
 
-        :return: The constant of this TimeseriesRainOverview.  # noqa: E501
+        :return: The constant of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :rtype: bool
         """
         return self._constant
 
     @constant.setter
     def constant(self, constant):
-        """Sets the constant of this TimeseriesRainOverview.
+        """Sets the constant of this TimeseriesSourcesSinksOverview.
 
 
-        :param constant: The constant of this TimeseriesRainOverview.  # noqa: E501
+        :param constant: The constant of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :type: bool
         """
 
         self._constant = constant
 
     @property
     def uid(self):
-        """Gets the uid of this TimeseriesRainOverview.  # noqa: E501
+        """Gets the uid of this TimeseriesSourcesSinksOverview.  # noqa: E501
 
 
-        :return: The uid of this TimeseriesRainOverview.  # noqa: E501
+        :return: The uid of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :rtype: str
         """
         return self._uid
 
     @uid.setter
     def uid(self, uid):
-        """Sets the uid of this TimeseriesRainOverview.
+        """Sets the uid of this TimeseriesSourcesSinksOverview.
 
 
-        :param uid: The uid of this TimeseriesRainOverview.  # noqa: E501
+        :param uid: The uid of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :type: str
         """
 
         self._uid = uid
 
     @property
     def id(self):
-        """Gets the id of this TimeseriesRainOverview.  # noqa: E501
+        """Gets the id of this TimeseriesSourcesSinksOverview.  # noqa: E501
 
 
-        :return: The id of this TimeseriesRainOverview.  # noqa: E501
+        :return: The id of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this TimeseriesRainOverview.
+        """Sets the id of this TimeseriesSourcesSinksOverview.
 
 
-        :param id: The id of this TimeseriesRainOverview.  # noqa: E501
+        :param id: The id of this TimeseriesSourcesSinksOverview.  # noqa: E501
         :type: int
         """
 
         self._id = id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -374,18 +346,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TimeseriesRainOverview):
+        if not isinstance(other, TimeseriesSourcesSinksOverview):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TimeseriesRainOverview):
+        if not isinstance(other, TimeseriesSourcesSinksOverview):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_sources_sinks.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_sources_sinks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_sources_sinks_overview.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/wind.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
 
 
@@ -17,300 +17,358 @@
 
 import six
 
 from threedi_api_client.openapi.configuration import Configuration
 
 logger = logging.getLogger(__name__)
 
-class TimeseriesSourcesSinksOverview(object):
+class Wind(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'id': 'int',
+        'uid': 'str',
         'url': 'str',
         'simulation': 'str',
         'offset': 'int',
-        'interpolate': 'bool',
         'values': 'list[list[float]]',
         'units': 'str',
-        'constant': 'bool',
-        'uid': 'str',
-        'id': 'int'
+        'speed_interpolate': 'bool',
+        'speed_constant': 'bool',
+        'direction_interpolate': 'bool',
+        'direction_constant': 'bool'
     }
 
     attribute_map = {
+        'id': 'id',
+        'uid': 'uid',
         'url': 'url',
         'simulation': 'simulation',
         'offset': 'offset',
-        'interpolate': 'interpolate',
         'values': 'values',
         'units': 'units',
-        'constant': 'constant',
-        'uid': 'uid',
-        'id': 'id'
+        'speed_interpolate': 'speed_interpolate',
+        'speed_constant': 'speed_constant',
+        'direction_interpolate': 'direction_interpolate',
+        'direction_constant': 'direction_constant'
     }
 
-    def __init__(self, url=None, simulation=None, offset=None, interpolate=None, values=None, units=None, constant=None, uid=None, id=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
-        """TimeseriesSourcesSinksOverview - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, id=None, uid=None, url=None, simulation=None, offset=None, values=None, units=None, speed_interpolate=None, speed_constant=None, direction_interpolate=None, direction_constant=None, local_vars_configuration=None, fetched_from_api=False):  # noqa: E501
+        """Wind - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         # True if data is coming from API
         self._fetched_from_api = fetched_from_api
 
+        self._id = None
+        self._uid = None
         self._url = None
         self._simulation = None
         self._offset = None
-        self._interpolate = None
         self._values = None
         self._units = None
-        self._constant = None
-        self._uid = None
-        self._id = None
+        self._speed_interpolate = None
+        self._speed_constant = None
+        self._direction_interpolate = None
+        self._direction_constant = None
         self.discriminator = None
 
+        if id is not None:
+            self.id = id
+        if uid is not None:
+            self.uid = uid
         if url is not None:
             self.url = url
         if simulation is not None:
             self.simulation = simulation
         self.offset = offset
-        if interpolate is not None:
-            self.interpolate = interpolate
-        self.values = values
-        self.units = units
-        if constant is not None:
-            self.constant = constant
-        if uid is not None:
-            self.uid = uid
-        if id is not None:
-            self.id = id
+        if values is not None:
+            self.values = values
+        if units is not None:
+            self.units = units
+        if speed_interpolate is not None:
+            self.speed_interpolate = speed_interpolate
+        if speed_constant is not None:
+            self.speed_constant = speed_constant
+        if direction_interpolate is not None:
+            self.direction_interpolate = direction_interpolate
+        if direction_constant is not None:
+            self.direction_constant = direction_constant
+
+    @property
+    def id(self):
+        """Gets the id of this Wind.  # noqa: E501
+
+
+        :return: The id of this Wind.  # noqa: E501
+        :rtype: int
+        """
+        return self._id
+
+    @id.setter
+    def id(self, id):
+        """Sets the id of this Wind.
+
+
+        :param id: The id of this Wind.  # noqa: E501
+        :type: int
+        """
+
+        self._id = id
+
+    @property
+    def uid(self):
+        """Gets the uid of this Wind.  # noqa: E501
+
+
+        :return: The uid of this Wind.  # noqa: E501
+        :rtype: str
+        """
+        return self._uid
+
+    @uid.setter
+    def uid(self, uid):
+        """Sets the uid of this Wind.
+
+
+        :param uid: The uid of this Wind.  # noqa: E501
+        :type: str
+        """
+
+        self._uid = uid
 
     @property
     def url(self):
-        """Gets the url of this TimeseriesSourcesSinksOverview.  # noqa: E501
+        """Gets the url of this Wind.  # noqa: E501
 
 
-        :return: The url of this TimeseriesSourcesSinksOverview.  # noqa: E501
+        :return: The url of this Wind.  # noqa: E501
         :rtype: str
         """
         return self._url
 
     @url.setter
     def url(self, url):
-        """Sets the url of this TimeseriesSourcesSinksOverview.
+        """Sets the url of this Wind.
 
 
-        :param url: The url of this TimeseriesSourcesSinksOverview.  # noqa: E501
+        :param url: The url of this Wind.  # noqa: E501
         :type: str
         """
 
         self._url = url
 
     @property
     def simulation(self):
-        """Gets the simulation of this TimeseriesSourcesSinksOverview.  # noqa: E501
+        """Gets the simulation of this Wind.  # noqa: E501
 
 
-        :return: The simulation of this TimeseriesSourcesSinksOverview.  # noqa: E501
+        :return: The simulation of this Wind.  # noqa: E501
         :rtype: str
         """
         return self._simulation
 
     @simulation.setter
     def simulation(self, simulation):
-        """Sets the simulation of this TimeseriesSourcesSinksOverview.
+        """Sets the simulation of this Wind.
 
 
-        :param simulation: The simulation of this TimeseriesSourcesSinksOverview.  # noqa: E501
+        :param simulation: The simulation of this Wind.  # noqa: E501
         :type: str
         """
 
         self._simulation = simulation
 
     @property
     def offset(self):
-        """Gets the offset of this TimeseriesSourcesSinksOverview.  # noqa: E501
+        """Gets the offset of this Wind.  # noqa: E501
 
         offset of event in simulation in seconds  # noqa: E501
 
-        :return: The offset of this TimeseriesSourcesSinksOverview.  # noqa: E501
+        :return: The offset of this Wind.  # noqa: E501
         :rtype: int
         """
         return self._offset
 
     @offset.setter
     def offset(self, offset):
-        """Sets the offset of this TimeseriesSourcesSinksOverview.
+        """Sets the offset of this Wind.
 
         offset of event in simulation in seconds  # noqa: E501
 
-        :param offset: The offset of this TimeseriesSourcesSinksOverview.  # noqa: E501
+        :param offset: The offset of this Wind.  # noqa: E501
         :type: int
         """
         if self.local_vars_configuration.client_side_validation and offset is None:  # noqa: E501
             self.__handle_validation_error("Invalid value for `offset`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 offset is not None and offset > 2147483647):  # noqa: E501
             self.__handle_validation_error("Invalid value for `offset`, must be a value less than or equal to `2147483647`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 offset is not None and offset < 0):  # noqa: E501
             self.__handle_validation_error("Invalid value for `offset`, must be a value greater than or equal to `0`")  # noqa: E501
 
         self._offset = offset
 
     @property
-    def interpolate(self):
-        """Gets the interpolate of this TimeseriesSourcesSinksOverview.  # noqa: E501
-
-
-        :return: The interpolate of this TimeseriesSourcesSinksOverview.  # noqa: E501
-        :rtype: bool
-        """
-        return self._interpolate
-
-    @interpolate.setter
-    def interpolate(self, interpolate):
-        """Sets the interpolate of this TimeseriesSourcesSinksOverview.
-
-
-        :param interpolate: The interpolate of this TimeseriesSourcesSinksOverview.  # noqa: E501
-        :type: bool
-        """
-
-        self._interpolate = interpolate
-
-    @property
     def values(self):
-        """Gets the values of this TimeseriesSourcesSinksOverview.  # noqa: E501
+        """Gets the values of this Wind.  # noqa: E501
 
-        Timeseries provided as a nested list. The inner list consists of exactly 2 values: timestamp, value  # noqa: E501
+        [time, speed, direction]  # noqa: E501
 
-        :return: The values of this TimeseriesSourcesSinksOverview.  # noqa: E501
+        :return: The values of this Wind.  # noqa: E501
         :rtype: list[list[float]]
         """
         return self._values
 
     @values.setter
     def values(self, values):
-        """Sets the values of this TimeseriesSourcesSinksOverview.
+        """Sets the values of this Wind.
 
-        Timeseries provided as a nested list. The inner list consists of exactly 2 values: timestamp, value  # noqa: E501
+        [time, speed, direction]  # noqa: E501
 
-        :param values: The values of this TimeseriesSourcesSinksOverview.  # noqa: E501
+        :param values: The values of this Wind.  # noqa: E501
         :type: list[list[float]]
         """
-        if self.local_vars_configuration.client_side_validation and values is None:  # noqa: E501
-            self.__handle_validation_error("Invalid value for `values`, must not be `None`")  # noqa: E501
 
         self._values = values
 
     @property
     def units(self):
-        """Gets the units of this TimeseriesSourcesSinksOverview.  # noqa: E501
+        """Gets the units of this Wind.  # noqa: E501
 
-        'm/s' (only option for now)  # noqa: E501
+        wind speed unit (default 'm/s')  # noqa: E501
 
-        :return: The units of this TimeseriesSourcesSinksOverview.  # noqa: E501
+        :return: The units of this Wind.  # noqa: E501
         :rtype: str
         """
         return self._units
 
     @units.setter
     def units(self, units):
-        """Sets the units of this TimeseriesSourcesSinksOverview.
+        """Sets the units of this Wind.
 
-        'm/s' (only option for now)  # noqa: E501
+        wind speed unit (default 'm/s')  # noqa: E501
 
-        :param units: The units of this TimeseriesSourcesSinksOverview.  # noqa: E501
+        :param units: The units of this Wind.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and units is None:  # noqa: E501
-            self.__handle_validation_error("Invalid value for `units`, must not be `None`")  # noqa: E501
-        allowed_values = ["m/s"]  # noqa: E501
+        allowed_values = ["m/s", "km/h"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and units not in allowed_values:  # noqa: E501
             self.__handle_validation_error(
                 "Invalid value for `units` ({0}), must be one of {1}"  # noqa: E501
                 .format(units, allowed_values)
             )
 
         self._units = units
 
     @property
-    def constant(self):
-        """Gets the constant of this TimeseriesSourcesSinksOverview.  # noqa: E501
+    def speed_interpolate(self):
+        """Gets the speed_interpolate of this Wind.  # noqa: E501
 
+        interpolate wind speed  # noqa: E501
 
-        :return: The constant of this TimeseriesSourcesSinksOverview.  # noqa: E501
+        :return: The speed_interpolate of this Wind.  # noqa: E501
         :rtype: bool
         """
-        return self._constant
+        return self._speed_interpolate
 
-    @constant.setter
-    def constant(self, constant):
-        """Sets the constant of this TimeseriesSourcesSinksOverview.
+    @speed_interpolate.setter
+    def speed_interpolate(self, speed_interpolate):
+        """Sets the speed_interpolate of this Wind.
 
+        interpolate wind speed  # noqa: E501
 
-        :param constant: The constant of this TimeseriesSourcesSinksOverview.  # noqa: E501
+        :param speed_interpolate: The speed_interpolate of this Wind.  # noqa: E501
         :type: bool
         """
 
-        self._constant = constant
+        self._speed_interpolate = speed_interpolate
 
     @property
-    def uid(self):
-        """Gets the uid of this TimeseriesSourcesSinksOverview.  # noqa: E501
+    def speed_constant(self):
+        """Gets the speed_constant of this Wind.  # noqa: E501
 
+        constant wind speed  # noqa: E501
 
-        :return: The uid of this TimeseriesSourcesSinksOverview.  # noqa: E501
-        :rtype: str
+        :return: The speed_constant of this Wind.  # noqa: E501
+        :rtype: bool
         """
-        return self._uid
+        return self._speed_constant
 
-    @uid.setter
-    def uid(self, uid):
-        """Sets the uid of this TimeseriesSourcesSinksOverview.
+    @speed_constant.setter
+    def speed_constant(self, speed_constant):
+        """Sets the speed_constant of this Wind.
 
+        constant wind speed  # noqa: E501
 
-        :param uid: The uid of this TimeseriesSourcesSinksOverview.  # noqa: E501
-        :type: str
+        :param speed_constant: The speed_constant of this Wind.  # noqa: E501
+        :type: bool
         """
 
-        self._uid = uid
+        self._speed_constant = speed_constant
 
     @property
-    def id(self):
-        """Gets the id of this TimeseriesSourcesSinksOverview.  # noqa: E501
+    def direction_interpolate(self):
+        """Gets the direction_interpolate of this Wind.  # noqa: E501
 
+        interpolate wind direction  # noqa: E501
 
-        :return: The id of this TimeseriesSourcesSinksOverview.  # noqa: E501
-        :rtype: int
+        :return: The direction_interpolate of this Wind.  # noqa: E501
+        :rtype: bool
         """
-        return self._id
+        return self._direction_interpolate
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this TimeseriesSourcesSinksOverview.
+    @direction_interpolate.setter
+    def direction_interpolate(self, direction_interpolate):
+        """Sets the direction_interpolate of this Wind.
 
+        interpolate wind direction  # noqa: E501
 
-        :param id: The id of this TimeseriesSourcesSinksOverview.  # noqa: E501
-        :type: int
+        :param direction_interpolate: The direction_interpolate of this Wind.  # noqa: E501
+        :type: bool
         """
 
-        self._id = id
+        self._direction_interpolate = direction_interpolate
+
+    @property
+    def direction_constant(self):
+        """Gets the direction_constant of this Wind.  # noqa: E501
+
+        constant wind direction  # noqa: E501
+
+        :return: The direction_constant of this Wind.  # noqa: E501
+        :rtype: bool
+        """
+        return self._direction_constant
+
+    @direction_constant.setter
+    def direction_constant(self, direction_constant):
+        """Sets the direction_constant of this Wind.
+
+        constant wind direction  # noqa: E501
+
+        :param direction_constant: The direction_constant of this Wind.  # noqa: E501
+        :type: bool
+        """
+
+        self._direction_constant = direction_constant
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -346,18 +404,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TimeseriesSourcesSinksOverview):
+        if not isinstance(other, Wind):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TimeseriesSourcesSinksOverview):
+        if not isinstance(other, Wind):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/timeseries_wind.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/timeseries_wind.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/tms.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/tms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/tokens.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/tokens.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/two_d_water_level.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/two_d_water_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/two_d_water_raster.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/two_d_water_raster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/upload.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/upload_event_file.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/upload_event_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/usage.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/usage_statistics.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/usage_statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/user.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/user_tokens.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/user_tokens.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/water_flow_graph_request.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/water_flow_graph_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/water_graph.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/water_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/water_level_graph_request.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/water_level_graph_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/water_level_profile.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/water_level_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/water_level_profile_request.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/water_level_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/waterdepth.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/waterdepth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/models/wind_drag_coefficient.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/models/wind_drag_coefficient.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/openapi/rest.py` & `threedi-api-client-4.1.3/threedi_api_client/openapi/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     3Di API
 
-    3Di simulation API (latest stable version: v3)   Framework release: 3.2.6   3Di core release: 2.3.6  deployed on:  07:54AM (UTC) on March 10, 2023  # noqa: E501
+    3Di simulation API (latest stable version: v3)   Framework release: 3.2.34   3Di core release: 2.4.3  deployed on:  05:50PM (UTC) on June 14, 2023  # noqa: E501
 
     The version of the OpenAPI document: v3
     Contact: info@nelen-schuurmans.nl
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/threedi_api_client.py` & `threedi-api-client-4.1.3/threedi_api_client/threedi_api_client.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client/versions.py` & `threedi-api-client-4.1.3/threedi_api_client/versions.py`

 * *Files identical despite different names*

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client.egg-info/PKG-INFO` & `threedi-api-client-4.1.3/threedi_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-api-client
-Version: 4.1.2b0
+Version: 4.1.3
 Summary: client for the threedi API
 Home-page: https://github.com/nens/threedi-api-client
 Author: Lars Claussen
 Author-email: lars.claussen@nelen-schuurmans.nl
 License: BSD license
 Keywords: threedi-api-client
 Classifier: Development Status :: 4 - Beta
@@ -70,14 +70,28 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+4.1.3 (2023-06-14)
+------------------
+
+- Release 3.2.34
+- Build the release with the build package instead of setuptools.
+- Rewrite release workflow to use a supported github action for github release.
+
+
+4.1.2 (2023-04-25)
+------------------
+
+- Public release.
+
+
 4.1.2b (2023-03-13)
 -------------------
 
 - Updated to framework release 3.2.6
 
 - Fix timeout when retrying uploads.
```

### Comparing `threedi-api-client-4.1.2b0/threedi_api_client.egg-info/SOURCES.txt` & `threedi-api-client-4.1.3/threedi_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

