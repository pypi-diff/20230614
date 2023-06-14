# Comparing `tmp/bigeye_sdk-0.4.54.tar.gz` & `tmp/bigeye_sdk-0.4.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigeye_sdk-0.4.54.tar", max compression
+gzip compressed data, was "bigeye_sdk-0.4.55.tar", max compression
```

## Comparing `bigeye_sdk-0.4.54.tar` & `bigeye_sdk-0.4.55.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     2092 2023-01-13 19:29:40.987774 bigeye_sdk-0.4.54/LICENSE
--rw-r--r--   0        0        0      873 2022-09-21 14:26:02.564243 bigeye_sdk-0.4.54/README.md
--rw-r--r--   0        0        0     3727 2022-09-21 19:14:17.084238 bigeye_sdk-0.4.54/bigeye_sdk/__init__.py
--rw-r--r--   0        0        0       82 2022-09-21 19:14:17.084343 bigeye_sdk-0.4.54/bigeye_sdk/__version__.py
--rw-r--r--   0        0        0        0 2022-09-21 14:26:02.564505 bigeye_sdk-0.4.54/bigeye_sdk/authentication/__init__.py
--rw-r--r--   0        0        0    17489 2023-06-08 16:16:24.658685 bigeye_sdk-0.4.54/bigeye_sdk/authentication/api_authentication.py
--rw-r--r--   0        0        0     2009 2023-06-08 16:16:18.009998 bigeye_sdk-0.4.54/bigeye_sdk/authentication/credentials.py
--rw-r--r--   0        0        0      734 2022-09-21 14:26:02.564714 bigeye_sdk-0.4.54/bigeye_sdk/authentication/enums.py
--rw-r--r--   0        0        0        0 2022-09-21 19:14:17.084676 bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/__init__.py
--rw-r--r--   0        0        0    10264 2023-06-08 16:16:24.658832 bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/big_config_reports.py
--rw-r--r--   0        0        0     8116 2023-06-08 16:16:24.658990 bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/validation_context.py
--rw-r--r--   0        0        0     1579 2023-06-08 16:16:24.659119 bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/validation_functions.py
--rw-r--r--   0        0        0      701 2022-09-21 19:14:17.085326 bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/validation_models.py
--rw-r--r--   0        0        0     9206 2023-06-08 16:16:24.659227 bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/yaml_model_base.py
--rw-r--r--   0        0        0     3042 2023-06-08 16:16:24.659331 bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
--rw-r--r--   0        0        0        0 2022-09-21 14:26:02.565379 bigeye_sdk-0.4.54/bigeye_sdk/class_ext/__init__.py
--rw-r--r--   0        0        0      233 2022-09-21 14:26:02.565502 bigeye_sdk-0.4.54/bigeye_sdk/class_ext/dataclass_ext.py
--rw-r--r--   0        0        0      402 2022-10-11 14:47:52.093321 bigeye_sdk-0.4.54/bigeye_sdk/class_ext/enum_ext.py
--rw-r--r--   0        0        0        0 2022-09-21 14:26:02.565649 bigeye_sdk-0.4.54/bigeye_sdk/client/__init__.py
--rw-r--r--   0        0        0      389 2022-12-01 16:53:45.901990 bigeye_sdk-0.4.54/bigeye_sdk/client/base_client.py
--rw-r--r--   0        0        0    39770 2023-06-08 16:16:24.659558 bigeye_sdk-0.4.54/bigeye_sdk/client/datawatch_client.py
--rw-r--r--   0        0        0      201 2022-09-21 14:26:02.566284 bigeye_sdk-0.4.54/bigeye_sdk/client/enum.py
--rw-r--r--   0        0        0    38235 2023-06-08 16:16:24.659795 bigeye_sdk-0.4.54/bigeye_sdk/client/generated_datawatch_client.py
--rw-r--r--   0        0        0        0 2022-09-21 19:14:17.086145 bigeye_sdk-0.4.54/bigeye_sdk/controller/__init__.py
--rw-r--r--   0        0        0      390 2022-11-30 18:19:48.731219 bigeye_sdk-0.4.54/bigeye_sdk/controller/metric_controller.py
--rw-r--r--   0        0        0    32893 2023-06-08 16:16:24.660068 bigeye_sdk-0.4.54/bigeye_sdk/controller/metric_suite_controller.py
--rw-r--r--   0        0        0        0 2022-09-21 14:26:02.566925 bigeye_sdk-0.4.54/bigeye_sdk/decorators/__init__.py
--rw-r--r--   0        0        0      307 2022-09-21 19:14:17.086414 bigeye_sdk-0.4.54/bigeye_sdk/decorators/dataclass_decorators.py
--rw-r--r--   0        0        0       97 2022-09-21 14:26:02.567122 bigeye_sdk-0.4.54/bigeye_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0     1018 2023-06-08 16:16:24.660218 bigeye_sdk-0.4.54/bigeye_sdk/exceptions/exceptions.py
--rw-r--r--   0        0        0        0 2022-09-21 14:26:02.567221 bigeye_sdk-0.4.54/bigeye_sdk/functions/__init__.py
--rw-r--r--   0        0        0     4469 2023-01-13 19:29:40.988379 bigeye_sdk-0.4.54/bigeye_sdk/functions/athena.py
--rw-r--r--   0        0        0     5202 2022-10-18 15:49:05.166354 bigeye_sdk-0.4.54/bigeye_sdk/functions/aws.py
--rw-r--r--   0        0        0     3343 2023-02-03 22:21:16.752839 bigeye_sdk-0.4.54/bigeye_sdk/functions/bigconfig_functions.py
--rw-r--r--   0        0        0     3469 2022-09-21 14:26:02.567414 bigeye_sdk-0.4.54/bigeye_sdk/functions/casing.py
--rw-r--r--   0        0        0     3215 2022-09-21 19:14:17.086730 bigeye_sdk-0.4.54/bigeye_sdk/functions/core_py_functs.py
--rw-r--r--   0        0        0     4517 2022-11-30 18:19:48.731507 bigeye_sdk-0.4.54/bigeye_sdk/functions/delta_functions.py
--rw-r--r--   0        0        0     2544 2023-06-08 16:16:24.660379 bigeye_sdk-0.4.54/bigeye_sdk/functions/file_functs.py
--rw-r--r--   0        0        0      117 2023-06-08 16:16:24.660510 bigeye_sdk-0.4.54/bigeye_sdk/functions/helpers.py
--rw-r--r--   0        0        0    20235 2023-06-08 16:16:24.660721 bigeye_sdk-0.4.54/bigeye_sdk/functions/metric_functions.py
--rw-r--r--   0        0        0     1554 2023-06-08 16:16:18.012698 bigeye_sdk-0.4.54/bigeye_sdk/functions/metric_run_functions.py
--rw-r--r--   0        0        0     1227 2022-10-11 14:47:52.094658 bigeye_sdk-0.4.54/bigeye_sdk/functions/s3.py
--rw-r--r--   0        0        0     1676 2023-01-13 19:29:40.988609 bigeye_sdk-0.4.54/bigeye_sdk/functions/schema_functions.py
--rw-r--r--   0        0        0     5089 2023-06-08 16:16:24.660877 bigeye_sdk-0.4.54/bigeye_sdk/functions/search_and_match_functions.py
--rw-r--r--   0        0        0     4032 2023-06-08 16:16:24.661012 bigeye_sdk-0.4.54/bigeye_sdk/functions/table_functions.py
--rw-r--r--   0        0        0     1701 2023-06-08 16:16:24.661143 bigeye_sdk-0.4.54/bigeye_sdk/functions/urlfuncts.py
--rw-r--r--   0        0        0        0 2023-06-08 15:07:54.354138 bigeye_sdk-0.4.54/bigeye_sdk/generated/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 15:07:54.354225 bigeye_sdk-0.4.54/bigeye_sdk/generated/com/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 15:07:54.354300 bigeye_sdk-0.4.54/bigeye_sdk/generated/com/bigeye/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 15:07:54.354356 bigeye_sdk-0.4.54/bigeye_sdk/generated/com/bigeye/models/__init__.py
--rw-r--r--   0        0        0   213399 2023-06-08 16:16:24.661924 bigeye_sdk-0.4.54/bigeye_sdk/generated/com/bigeye/models/generated.py
--rw-r--r--   0        0        0        0 2023-06-08 15:07:54.354553 bigeye_sdk-0.4.54/bigeye_sdk/generated/google/__init__.py
--rw-r--r--   0        0        0    14816 2023-06-08 15:07:54.354602 bigeye_sdk-0.4.54/bigeye_sdk/generated/google/api.py
--rw-r--r--   0        0        0      507 2022-09-21 14:26:02.569285 bigeye_sdk-0.4.54/bigeye_sdk/log/__init__.py
--rw-r--r--   0        0        0        1 2022-09-21 19:14:17.088368 bigeye_sdk-0.4.54/bigeye_sdk/model/__init__.py
--rw-r--r--   0        0        0      489 2022-09-21 19:14:17.088495 bigeye_sdk-0.4.54/bigeye_sdk/model/base_datawatch_facade.py
--rw-r--r--   0        0        0    22303 2023-06-08 16:16:24.662241 bigeye_sdk-0.4.54/bigeye_sdk/model/big_config.py
--rw-r--r--   0        0        0      778 2023-02-23 17:53:03.561875 bigeye_sdk-0.4.54/bigeye_sdk/model/collection_models.py
--rw-r--r--   0        0        0     3948 2023-06-08 16:16:24.662434 bigeye_sdk-0.4.54/bigeye_sdk/model/dbt_schema.py
--rw-r--r--   0        0        0     3504 2023-06-08 16:16:24.662568 bigeye_sdk-0.4.54/bigeye_sdk/model/delta_facade.py
--rw-r--r--   0        0        0     9456 2023-01-13 19:29:40.989263 bigeye_sdk-0.4.54/bigeye_sdk/model/metric_facade.py
--rw-r--r--   0        0        0     8396 2023-06-08 16:16:24.662714 bigeye_sdk-0.4.54/bigeye_sdk/model/protobuf_enum_facade.py
--rw-r--r--   0        0        0      220 2022-11-30 18:19:48.733054 bigeye_sdk-0.4.54/bigeye_sdk/model/protobuf_extensions.py
--rw-r--r--   0        0        0    44904 2023-06-08 16:16:24.662961 bigeye_sdk-0.4.54/bigeye_sdk/model/protobuf_message_facade.py
--rw-r--r--   0        0        0      865 2023-02-22 23:48:15.904646 bigeye_sdk-0.4.54/bigeye_sdk/model/sla_models.py
--rw-r--r--   0        0        0     7114 2023-06-08 16:16:24.663118 bigeye_sdk-0.4.54/bigeye_sdk/serializable.py
--rw-r--r--   0        0        0     3709 2023-06-08 16:16:24.664385 bigeye_sdk-0.4.54/pyproject.toml
--rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.54/PKG-INFO
+-rw-r--r--   0        0        0     2092 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/LICENSE
+-rw-r--r--   0        0        0      873 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/README.md
+-rw-r--r--   0        0        0     3727 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/__init__.py
+-rw-r--r--   0        0        0       82 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/__version__.py
+-rw-r--r--   0        0        0        0 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/authentication/__init__.py
+-rw-r--r--   0        0        0    17489 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/authentication/api_authentication.py
+-rw-r--r--   0        0        0     1182 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/authentication/credentials.py
+-rw-r--r--   0        0        0      734 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/authentication/enums.py
+-rw-r--r--   0        0        0        0 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/__init__.py
+-rw-r--r--   0        0        0    10264 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/big_config_reports.py
+-rw-r--r--   0        0        0     8116 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/validation_context.py
+-rw-r--r--   0        0        0     1579 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/validation_functions.py
+-rw-r--r--   0        0        0      701 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/validation_models.py
+-rw-r--r--   0        0        0     9206 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/yaml_model_base.py
+-rw-r--r--   0        0        0     3042 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
+-rw-r--r--   0        0        0        0 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/class_ext/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/class_ext/dataclass_ext.py
+-rw-r--r--   0        0        0      402 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/class_ext/enum_ext.py
+-rw-r--r--   0        0        0        0 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/client/__init__.py
+-rw-r--r--   0        0        0      389 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/client/base_client.py
+-rw-r--r--   0        0        0    39917 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/client/datawatch_client.py
+-rw-r--r--   0        0        0      201 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/client/enum.py
+-rw-r--r--   0        0        0    38282 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/client/generated_datawatch_client.py
+-rw-r--r--   0        0        0        0 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/controller/__init__.py
+-rw-r--r--   0        0        0      390 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/controller/metric_controller.py
+-rw-r--r--   0        0        0    33079 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/controller/metric_suite_controller.py
+-rw-r--r--   0        0        0        0 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/decorators/__init__.py
+-rw-r--r--   0        0        0      307 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/decorators/dataclass_decorators.py
+-rw-r--r--   0        0        0       97 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0     1018 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/exceptions/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/__init__.py
+-rw-r--r--   0        0        0     4469 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/athena.py
+-rw-r--r--   0        0        0     5202 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/aws.py
+-rw-r--r--   0        0        0     3343 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/bigconfig_functions.py
+-rw-r--r--   0        0        0     3469 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/casing.py
+-rw-r--r--   0        0        0     3215 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/core_py_functs.py
+-rw-r--r--   0        0        0     4517 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/delta_functions.py
+-rw-r--r--   0        0        0     2544 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/file_functs.py
+-rw-r--r--   0        0        0      117 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/helpers.py
+-rw-r--r--   0        0        0    20235 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/metric_functions.py
+-rw-r--r--   0        0        0     2540 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/metric_run_functions.py
+-rw-r--r--   0        0        0     1227 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/s3.py
+-rw-r--r--   0        0        0     1676 2023-06-14 21:08:17.837777 bigeye_sdk-0.4.55/bigeye_sdk/functions/schema_functions.py
+-rw-r--r--   0        0        0     5088 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/functions/search_and_match_functions.py
+-rw-r--r--   0        0        0     4031 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/functions/table_functions.py
+-rw-r--r--   0        0        0     1701 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/functions/urlfuncts.py
+-rw-r--r--   0        0        0        0 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/generated/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/generated/com/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/generated/com/bigeye/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/generated/com/bigeye/models/__init__.py
+-rw-r--r--   0        0        0   220193 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/generated/com/bigeye/models/generated.py
+-rw-r--r--   0        0        0        0 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/generated/google/__init__.py
+-rw-r--r--   0        0        0    14816 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/generated/google/api.py
+-rw-r--r--   0        0        0      507 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/log/__init__.py
+-rw-r--r--   0        0        0        1 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/base_datawatch_facade.py
+-rw-r--r--   0        0        0    22303 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/big_config.py
+-rw-r--r--   0        0        0      778 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/collection_models.py
+-rw-r--r--   0        0        0     3948 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/dbt_schema.py
+-rw-r--r--   0        0        0     3504 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/delta_facade.py
+-rw-r--r--   0        0        0     9456 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/metric_facade.py
+-rw-r--r--   0        0        0     8396 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/protobuf_enum_facade.py
+-rw-r--r--   0        0        0      220 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/protobuf_extensions.py
+-rw-r--r--   0        0        0    50205 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/protobuf_message_facade.py
+-rw-r--r--   0        0        0      865 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/model/sla_models.py
+-rw-r--r--   0        0        0     7114 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/bigeye_sdk/serializable.py
+-rw-r--r--   0        0        0     3685 2023-06-14 21:08:17.841777 bigeye_sdk-0.4.55/pyproject.toml
+-rw-r--r--   0        0        0     2090 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.55/PKG-INFO
```

### Comparing `bigeye_sdk-0.4.54/LICENSE` & `bigeye_sdk-0.4.55/LICENSE`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/README.md` & `bigeye_sdk-0.4.55/README.md`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/__init__.py` & `bigeye_sdk-0.4.55/bigeye_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/authentication/api_authentication.py` & `bigeye_sdk-0.4.55/bigeye_sdk/authentication/api_authentication.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/authentication/enums.py` & `bigeye_sdk-0.4.55/bigeye_sdk/authentication/enums.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/big_config_reports.py` & `bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/big_config_reports.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/validation_context.py` & `bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/validation_context.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/validation_functions.py` & `bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/validation_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/validation_models.py` & `bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/validation_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/yaml_model_base.py` & `bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/yaml_model_base.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py` & `bigeye_sdk-0.4.55/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/client/datawatch_client.py` & `bigeye_sdk-0.4.55/bigeye_sdk/client/datawatch_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,18 +404,19 @@
                     m.metrics.extend(all_column_metrics)
 
             response_as_ctc.group_bys = [gb.to_datawatch_object() for gb in sdc.group_bys]
             response_as_ctc.source_filters = sdc.source_filters
             response_as_ctc.target_filters = sdc.target_filters
 
             schedules = self.get_named_schedule().named_schedules
-
             for s in schedules:
                 """Matches on cron value."""
-                if s.cron == sdc.cron_schedule.cron or s.name == sdc.cron_schedule.name:
+                if sdc.cron_schedule is None:
+                    response_as_ctc.named_schedule = IdAndDisplayName(id=s.id, display_name=s.name)
+                elif s.cron == sdc.cron_schedule.cron or s.name == sdc.cron_schedule.name:
                     response_as_ctc.named_schedule = IdAndDisplayName(id=s.id, display_name=s.name)
 
             if response_as_ctc.named_schedule.id == 0:
                 ns = self.create_named_schedule(name=sdc.cron_schedule.name, cron=sdc.cron_schedule.cron)
                 response_as_ctc.named_schedule = IdAndDisplayName(id=ns.id, display_name=ns.name)
 
             response = self.create_delta(comparison_table_configuration=response_as_ctc)
```

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/client/generated_datawatch_client.py` & `bigeye_sdk-0.4.55/bigeye_sdk/client/generated_datawatch_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,15 +341,15 @@
 
         return EditCollectionResponse().from_dict(response)
 
     def update_collection(self, collection: Collection) -> EditCollectionResponse:
 
         request: EditCollectionRequest = EditCollectionRequest()
         request.collection_name = collection.name
-        request.description = collection.description
+        request.description = collection.description if collection.description else collection.name
         request.metric_ids = collection.metric_ids
         request.notification_channels = collection.notification_channels
         request.muted_until_timestamp = collection.muted_until_timestamp
 
         url = f"/api/v1/collections/{collection.id}"
 
         log.info(f'Query: {url}; Body: {request.to_json()}')
```

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/controller/metric_suite_controller.py` & `bigeye_sdk-0.4.55/bigeye_sdk/controller/metric_suite_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,23 +65,28 @@
 
     if not files:
         """No YAML files were found at the given input path or current working directory, raise error for user to fix input paths."""
         raise FileNotFoundException(f'No YAML files for the given input paths or current working directory were found.')
 
     bigeye_files: List[BIGCONFIG_FILE] = []
     file: BIGCONFIG_FILE
+    load_errs = []
     for file in files:
         try:
             """Loading Bigconfig YAML.  If file is not of Bigconfig type then the error will be caught and passed."""
             bigeye_files.append(File.load(str(file)))
         except FileLoadException as e:
-            log.warning(f'File {file} failed to load with error: {str(e.message)}')
+            load_err = f'File {file} failed to load with error: {str(e.message)}'
+            load_errs.append(load_err)
+            log.warning(load_err)
 
     if len(bigeye_files) == 0:
-        raise BigConfigValidationException(f'No conforming files found. There may be a formatting issue with the yaml.')
+        errors = "\n\n=========\n\n".join(load_errs)
+        err = f'No conforming files found. There may be a formatting issue with the yaml.\nErrors found:\n{errors}'
+        raise BigConfigValidationException(err)
 
     else:
         return bigeye_files
 
 
 class MetricSuiteController:
```

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/exceptions/exceptions.py` & `bigeye_sdk-0.4.55/bigeye_sdk/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/functions/athena.py` & `bigeye_sdk-0.4.55/bigeye_sdk/functions/athena.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/functions/aws.py` & `bigeye_sdk-0.4.55/bigeye_sdk/functions/aws.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/functions/bigconfig_functions.py` & `bigeye_sdk-0.4.55/bigeye_sdk/functions/bigconfig_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/functions/casing.py` & `bigeye_sdk-0.4.55/bigeye_sdk/functions/casing.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/functions/core_py_functs.py` & `bigeye_sdk-0.4.55/bigeye_sdk/functions/core_py_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/functions/delta_functions.py` & `bigeye_sdk-0.4.55/bigeye_sdk/functions/delta_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/functions/file_functs.py` & `bigeye_sdk-0.4.55/bigeye_sdk/functions/file_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/functions/metric_functions.py` & `bigeye_sdk-0.4.55/bigeye_sdk/functions/metric_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/functions/metric_run_functions.py` & `bigeye_sdk-0.4.55/bigeye_sdk/functions/metric_run_functions.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,44 @@
 
 @dataclass
 class UpperLower:
     upper: float = 0.0
     lower: float = 0.0
 
 
+def get_most_recent_run_point(metric_info: MetricInfo) -> MetricRun:
+    """
+        Returns the most recent MetricRun object from the Metric Info based on the grain start of a lookback window or
+        the run at time.
+        Args:
+            metric_info: a MetricInfo object
+
+        Returns: the most recent MetricRun.
+
+    """
+    try:
+        return max(metric_info.latest_metric_runs, key=attrgetter('grain_start_epoch_seconds'))
+    except AttributeError:
+        return get_most_recent_run(metric_info=metric_info)
+
+
+def get_most_recent_run_by_id(metric_info: MetricInfo) -> MetricRun:
+    """
+    Returns the most recent MetricRun object from the Metric Info based on the max MetricRun id.
+        Args:
+            metric_info: a MetricInfo object
+
+        Returns: the most recent MetricRun.
+    """
+    try:
+        return max(metric_info.latest_metric_runs, key=attrgetter('id'))
+    except AttributeError:
+        return get_most_recent_run(metric_info=metric_info)
+
+
 def get_most_recent_run(metric_info: MetricInfo) -> MetricRun:
     """
     Returns the most recent MetricRun object from the Metric Info.
     Args:
         metric_info: a MetricInfo object
 
     Returns: the most recent MetricRun.
@@ -48,8 +78,8 @@
 
     for t in most_recent_run.thresholds:
         if t.bound.bound_type == SimpleBoundType.UPPER_BOUND_SIMPLE_BOUND_TYPE:
             ul.upper = t.bound.value
         elif t.bound.bound_type == SimpleBoundType.LOWER_BOUND_SIMPLE_BOUND_TYPE:
             ul.lower = t.bound.value
 
-    return ul
+    return ul
```

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/functions/s3.py` & `bigeye_sdk-0.4.55/bigeye_sdk/functions/s3.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/functions/schema_functions.py` & `bigeye_sdk-0.4.55/bigeye_sdk/functions/schema_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/functions/search_and_match_functions.py` & `bigeye_sdk-0.4.55/bigeye_sdk/functions/search_and_match_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import re
 from itertools import product
 from typing import List, Tuple, Dict
 
-from fuzzywuzzy import fuzz
+from rapidfuzz import fuzz
 
 
 def wildcard_search(search_string: str, content: List[str]) -> List[str]:
     r: List[str] = []
     search_string = f"^{search_string.replace('*', '.+')}$"
     for s in content:
         if re.search(search_string, s):
```

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/functions/table_functions.py` & `bigeye_sdk-0.4.55/bigeye_sdk/functions/table_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import List, Union, Tuple
 
-from fuzzywuzzy import process
+from rapidfuzz import process
 
 from bigeye_sdk.generated.com.bigeye.models.generated import Table, TableColumn
 from bigeye_sdk.log import get_logger
 
 log = get_logger(__file__)
```

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/functions/urlfuncts.py` & `bigeye_sdk-0.4.55/bigeye_sdk/functions/urlfuncts.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/generated/com/bigeye/models/generated.py` & `bigeye_sdk-0.4.55/bigeye_sdk/generated/com/bigeye/models/generated.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,15 @@
     TAGGABLE_ENTITY_TYPE_DELTA = 5
     TAGGABLE_ENTITY_TYPE_COLUMN = 6
     TAGGABLE_ENTITY_TYPE_SLA = 7
     TAGGABLE_ENTITY_TYPE_BI_TOOL = 8
     TAGGABLE_ENTITY_TYPE_TABLEAU_WORKBOOK = 9
     TAGGABLE_ENTITY_TYPE_N_WAY_DELTA = 10
     TAGGABLE_ENTITY_TYPE_VIRTUAL_TABLE = 11
+    TAGGABLE_ENTITY_TYPE_DBT_PROJECT = 12
 
 
 class TableType(betterproto.Enum):
     TABLE_TYPE_UNSPECIFIED = 0
     TABLE_TYPE_TABLE = 1
     TABLE_TYPE_VIEW = 2
     TABLE_TYPE_VIRTUAL = 3
@@ -328,14 +329,28 @@
     DATA_NODE_TYPE_TABLE = 1
     DATA_NODE_TYPE_TABLEAU_WORKBOOK = 2
 
 
 class IntegrationPartner(betterproto.Enum):
     INTEGRATION_PARTNER_UNSPECIFIED = 0
     INTEGRATION_PARTNER_TABLEAU = 1
+    INTEGRATION_PARTNER_DBT_CLOUD = 2
+
+
+class IntegrationType(betterproto.Enum):
+    INTEGRATION_TYPE_UNSPECIFIED = 0
+    INTEGRATION_TYPE_BI_TOOL = 1
+    INTEGRATION_TYPE_ETL_TOOL = 2
+
+
+class DbtProjectSortField(betterproto.Enum):
+    DBT_PROJECT_SORT_FIELD_UNSPECIFIED = 0
+    DBT_PROJECT_SORT_FIELD_NAME = 1
+    DBT_PROJECT_SORT_FIELD_FAVORITE = 2
+    DBT_PROJECT_SORT_FIELD_UPDATED_AT = 3
 
 
 class ThreeLeggedBoolean(betterproto.Enum):
     """
     We need this for isMuted filters as unspecified == no filter, but the
     generated typescript file is setting null to false so there is no way for
     the receiver to tell if there is no filter, or if the filter is set to
@@ -1094,25 +1109,31 @@
 
 @dataclass
 class GetCollectionInfoResponse(betterproto.Message):
     collection_info: "CollectionInfo" = betterproto.message_field(1)
 
 
 @dataclass
+class GetAllCollectionInfosRequest(betterproto.Message):
+    workspace_id: int = betterproto.int32_field(1)
+
+
+@dataclass
 class GetAllCollectionInfosResponse(betterproto.Message):
     collection_infos: List["CollectionInfo"] = betterproto.message_field(1)
 
 
 @dataclass
 class GetPaginatedCollectionInfosRequest(betterproto.Message):
     page_size: int = betterproto.int32_field(1)
     page_cursor: str = betterproto.string_field(2)
     sort_field: "CollectionInfoSortField" = betterproto.enum_field(3)
     sort_direction: "SortDirection" = betterproto.enum_field(4)
     search: str = betterproto.string_field(5)
+    workspace_id: int = betterproto.int32_field(6)
 
 
 @dataclass
 class GetPaginatedCollectionInfosResponse(betterproto.Message):
     collection_infos: List["CollectionInfo"] = betterproto.message_field(1)
     pagination_info: "PaginationInfo" = betterproto.message_field(2)
 
@@ -1138,14 +1159,19 @@
 
 @dataclass
 class GetCollectionResponse(betterproto.Message):
     collection: "Collection" = betterproto.message_field(1)
 
 
 @dataclass
+class GetCollectionsRequest(betterproto.Message):
+    workspace_id: int = betterproto.int32_field(1)
+
+
+@dataclass
 class GetCollectionsResponse(betterproto.Message):
     collections: List["Collection"] = betterproto.message_field(1)
 
 
 @dataclass
 class EditCollectionWrapper(betterproto.Message):
     collection_id: int = betterproto.int32_field(1)
@@ -1155,14 +1181,15 @@
 @dataclass
 class EditCollectionRequest(betterproto.Message):
     collection_name: str = betterproto.string_field(1)
     description: str = betterproto.string_field(2)
     metric_ids: List[int] = betterproto.int32_field(3)
     notification_channels: List["NotificationChannel"] = betterproto.message_field(4)
     muted_until_timestamp: int = betterproto.int32_field(5)
+    workspace_id: int = betterproto.int32_field(6)
 
 
 @dataclass
 class EditCollectionResponse(betterproto.Message):
     collection: "Collection" = betterproto.message_field(1)
     failed_metric_edits: List["FailedMetricEdit"] = betterproto.message_field(2)
 
@@ -1583,14 +1610,15 @@
     timeout: int = betterproto.int32_field(12)
     created_by_id: int = betterproto.int32_field(13)
     created_at: int = betterproto.int64_field(14)
     updated_by_id: int = betterproto.int32_field(15)
     updated_at: int = betterproto.int64_field(16)
     integration_entities_count: int = betterproto.int32_field(17)
     is_favorite: bool = betterproto.bool_field(18)
+    integration_type: "IntegrationType" = betterproto.enum_field(19)
 
 
 @dataclass
 class CreateOrUpdateIntegrationRequest(betterproto.Message):
     name: str = betterproto.string_field(1)
     integration_partner: "IntegrationPartner" = betterproto.enum_field(2)
     api_base_uri: str = betterproto.string_field(3)
@@ -1608,14 +1636,51 @@
     integrations: List["Integration"] = betterproto.message_field(1)
 
 
 @dataclass
 class GetIntegrationEntitiesResponse(betterproto.Message):
     integration_partner: "IntegrationPartner" = betterproto.enum_field(1)
     tableau_workbooks: List["TableauWorkbook"] = betterproto.message_field(2)
+    dbt_projects: List["DbtProject"] = betterproto.message_field(3)
+
+
+@dataclass
+class DbtProject(betterproto.Message):
+    id: int = betterproto.int32_field(1)
+    account_id: int = betterproto.int32_field(2)
+    name: str = betterproto.string_field(3)
+    job_count: int = betterproto.int32_field(4)
+    is_favorite: bool = betterproto.bool_field(5)
+    company_id: int = betterproto.int32_field(6)
+    integration_entity_id: str = betterproto.string_field(7)
+    integration_id: int = betterproto.int32_field(8)
+    workspace_id: int = betterproto.int32_field(9)
+    created_at: int = betterproto.int64_field(10)
+    updated_at: int = betterproto.int64_field(11)
+
+
+@dataclass
+class GetDbtProjectsRequest(betterproto.Message):
+    integration_id: int = betterproto.int32_field(1)
+    page_size: int = betterproto.int32_field(2)
+    page_cursor: str = betterproto.string_field(3)
+    sort_options: List["DbtProjectSortOption"] = betterproto.message_field(4)
+    search: str = betterproto.string_field(5)
+
+
+@dataclass
+class DbtProjectSortOption(betterproto.Message):
+    sort_direction: "SortDirection" = betterproto.enum_field(1)
+    sort_field: "DbtProjectSortField" = betterproto.enum_field(2)
+
+
+@dataclass
+class GetDbtProjectsResponse(betterproto.Message):
+    projects: List["DbtProject"] = betterproto.message_field(1)
+    pagination_info: "PaginationInfo" = betterproto.message_field(2)
 
 
 @dataclass
 class SinglePathParamIntegrationIdRequest(betterproto.Message):
     integration_id: int = betterproto.int32_field(1)
 
 
@@ -1810,14 +1875,19 @@
 
 @dataclass
 class WorkflowCleanupJob(betterproto.Message):
     pass
 
 
 @dataclass
+class RunDashboardJob(betterproto.Message):
+    pass
+
+
+@dataclass
 class JobDefinition(betterproto.Message):
     run_metric_job: "RunMetricJob" = betterproto.message_field(1, group="job")
     generate_suggestions_job: "GenerateSuggestionsJob" = betterproto.message_field(
         3, group="job"
     )
     update_warehouse_catalog_models_job: "UpdateWarehouseCatalogModelsJob" = (
         betterproto.message_field(5, group="job")
@@ -1838,14 +1908,15 @@
     generate_pop_scores_job: "GeneratePopScoresJob" = betterproto.message_field(
         12, group="job"
     )
     update_integration_catalog_job: "UpdateIntegrationCatalogJob" = (
         betterproto.message_field(13, group="job")
     )
     run_delta_job: "RunDeltaJob" = betterproto.message_field(14, group="job")
+    run_dashboard_job: "RunDashboardJob" = betterproto.message_field(15, group="job")
 
 
 @dataclass
 class ScheduleRequest(betterproto.Message):
     job_definition: "JobDefinition" = betterproto.message_field(1)
     cron: str = betterproto.string_field(2, group="schedule")
     interval_seconds: int = betterproto.int32_field(3, group="schedule")
@@ -3409,14 +3480,16 @@
     target_table: "IdAndDisplayName" = betterproto.message_field(9)
     target_warehouse_type: "WarehouseType" = betterproto.enum_field(10)
     target_schema: "IdAndDisplayName" = betterproto.message_field(11)
     target_source: "IdAndDisplayName" = betterproto.message_field(12)
     total_group_count: int = betterproto.int32_field(13)
     failed_group_count: int = betterproto.int32_field(14)
     alerting_group_count: int = betterproto.int32_field(15)
+    is_target_table_deleted: bool = betterproto.bool_field(16)
+    last_run_at_epoch_seconds: int = betterproto.int64_field(17)
 
 
 @dataclass
 class ComparisonColumnInfo(betterproto.Message):
     source_column: "IdAndDisplayName" = betterproto.message_field(1)
     target_column: "IdAndDisplayName" = betterproto.message_field(2)
     metrics: List["MetricType"] = betterproto.message_field(3)
@@ -3442,14 +3515,15 @@
 
 @dataclass
 class Workspace(betterproto.Message):
     id: int = betterproto.int32_field(1)
     name: str = betterproto.string_field(2)
     is_default: bool = betterproto.bool_field(3)
     sources: List["Source"] = betterproto.message_field(4)
+    roles: List["RoleV2"] = betterproto.message_field(5)
 
 
 @dataclass
 class WorkspaceListResponse(betterproto.Message):
     workspaces: List["Workspace"] = betterproto.message_field(1)
 
 
@@ -3539,27 +3613,95 @@
 
 
 @dataclass
 class Group(betterproto.Message):
     id: int = betterproto.int32_field(1)
     name: str = betterproto.string_field(2)
     users: List["IdAndDisplayName"] = betterproto.message_field(3)
+    roles: List["RoleV2"] = betterproto.message_field(4)
 
 
 @dataclass
 class GroupListResponse(betterproto.Message):
     groups: List["Group"] = betterproto.message_field(1)
 
 
 @dataclass
 class CreateOrUpdateGroupRequest(betterproto.Message):
     name: str = betterproto.string_field(1)
 
 
 @dataclass
+class BulkChangeGroupUsersRequest(betterproto.Message):
+    user_ids: List[int] = betterproto.int32_field(1)
+    group_ids: List[int] = betterproto.int32_field(2)
+    operation: "GroupUserOperation" = betterproto.enum_field(3)
+
+
+@dataclass
+class GroupUserPair(betterproto.Message):
+    user_id: int = betterproto.int32_field(1)
+    group_id: int = betterproto.int32_field(2)
+
+
+@dataclass
+class FailedGroupUserUpdate(betterproto.Message):
+    user_id: int = betterproto.int32_field(1)
+    group_id: int = betterproto.int32_field(2)
+    reason: str = betterproto.string_field(3)
+
+
+@dataclass
+class BulkChangeGroupUsersResponse(betterproto.Message):
+    successful_ids: List["GroupUserPair"] = betterproto.message_field(1)
+    failed_updates: List["FailedGroupUserUpdate"] = betterproto.message_field(2)
+
+
+@dataclass
+class RoleV2(betterproto.Message):
+    id: int = betterproto.int32_field(1)
+    workspace_id: int = betterproto.int32_field(2)
+    name: str = betterproto.string_field(3)
+
+
+@dataclass
+class RoleV2ListResponse(betterproto.Message):
+    roles: List["RoleV2"] = betterproto.message_field(1)
+
+
+@dataclass
+class BulkChangeGroupRolesRequest(betterproto.Message):
+    role_ids: List[int] = betterproto.int32_field(1)
+    group_id: int = betterproto.int32_field(2)
+    operation: "RoleOperation" = betterproto.enum_field(3)
+
+
+@dataclass
+class BulkDeleteUsersRequest(betterproto.Message):
+    user_ids: List[int] = betterproto.int32_field(1)
+
+
+@dataclass
+class SetBigQueryRegionRequestWrapper(betterproto.Message):
+    schema_id: int = betterproto.int32_field(1)
+    body: "SetBigQueryRegionRequest" = betterproto.message_field(2)
+
+
+@dataclass
+class SetBigQueryRegionRequest(betterproto.Message):
+    region: str = betterproto.string_field(1)
+
+
+@dataclass
+class GetBigQueryRegionResponse(betterproto.Message):
+    region: str = betterproto.string_field(1)
+    manually_set: bool = betterproto.bool_field(2)
+
+
+@dataclass
 class Empty(betterproto.Message):
     pass
 
 
 @dataclass
 class DimensionRun(betterproto.Message):
     dim_name: str = betterproto.string_field(1)
@@ -4413,24 +4555,26 @@
         self,
         *,
         collection_name: str = "",
         description: str = "",
         metric_ids: List[int] = [],
         notification_channels: List["NotificationChannel"] = [],
         muted_until_timestamp: int = 0,
+        workspace_id: int = 0,
     ) -> CreateCollectionResponse:
         """Create collection"""
 
         request = EditCollectionRequest()
         request.collection_name = collection_name
         request.description = description
         request.metric_ids = metric_ids
         if notification_channels is not None:
             request.notification_channels = notification_channels
         request.muted_until_timestamp = muted_until_timestamp
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.CollectionService/CreateCollection",
             request,
             CreateCollectionResponse,
         )
 
@@ -4446,18 +4590,19 @@
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.CollectionService/EditCollection",
             request,
             EditCollectionResponse,
         )
 
-    async def get_collections(self) -> GetCollectionsResponse:
+    async def get_collections(self, *, workspace_id: int = 0) -> GetCollectionsResponse:
         """Get all collections"""
 
-        request = Empty()
+        request = GetCollectionsRequest()
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.CollectionService/GetCollections",
             request,
             GetCollectionsResponse,
         )
 
@@ -4495,23 +4640,26 @@
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.CollectionService/GetCollectionInfo",
             request,
             GetCollectionInfoResponse,
         )
 
-    async def get_collection_infos(self) -> GetCollectionInfoResponse:
+    async def get_collection_infos(
+        self, *, workspace_id: int = 0
+    ) -> GetAllCollectionInfosResponse:
         """Get all collection information"""
 
-        request = Empty()
+        request = GetAllCollectionInfosRequest()
+        request.workspace_id = workspace_id
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.CollectionService/GetCollectionInfos",
             request,
-            GetCollectionInfoResponse,
+            GetAllCollectionInfosResponse,
         )
 
 
 class TableServiceStub(betterproto.ServiceStub):
     """Tables"""
 
     async def get_profile_for_table(
@@ -4835,14 +4983,77 @@
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.SchemaService/GetSchemas",
             request,
             GetSchemaListResponse,
         )
 
+    async def set_big_query_region(
+        self, *, schema_id: int = 0, body: Optional["SetBigQueryRegionRequest"] = None
+    ) -> Empty:
+        """
+        Set the region for a BigQuery schema (called dataset in BigQuery)
+        """
+
+        request = SetBigQueryRegionRequestWrapper()
+        request.schema_id = schema_id
+        if body is not None:
+            request.body = body
+
+        return await self._unary_unary(
+            "/com.bigeye.models.generated.SchemaService/SetBigQueryRegion",
+            request,
+            Empty,
+        )
+
+    async def fake_api1(
+        self, *, schema_id: int = 0, body: Optional["SetBigQueryRegionRequest"] = None
+    ) -> Empty:
+        request = SetBigQueryRegionRequestWrapper()
+        request.schema_id = schema_id
+        if body is not None:
+            request.body = body
+
+        return await self._unary_unary(
+            "/com.bigeye.models.generated.SchemaService/FakeApi1",
+            request,
+            Empty,
+        )
+
+    async def get_big_query_region(
+        self, *, schema_id: int = 0
+    ) -> GetBigQueryRegionResponse:
+        """
+        Get the region for a BigQuery schema (called dataset in BigQuery)
+        """
+
+        request = SinglePathParamSchemaIdRequest()
+        request.schema_id = schema_id
+
+        return await self._unary_unary(
+            "/com.bigeye.models.generated.SchemaService/GetBigQueryRegion",
+            request,
+            GetBigQueryRegionResponse,
+        )
+
+    async def delete_big_query_region_override(self, *, schema_id: int = 0) -> Empty:
+        """
+        Remove the manual override of a region for a BigQuery schema (called
+        dataset in BigQuery)
+        """
+
+        request = SinglePathParamSchemaIdRequest()
+        request.schema_id = schema_id
+
+        return await self._unary_unary(
+            "/com.bigeye.models.generated.SchemaService/DeleteBigQueryRegionOverride",
+            request,
+            Empty,
+        )
+
 
 class ColumnServiceStub(betterproto.ServiceStub):
     """Columns"""
 
     async def get_specified_columns(
         self, *, table_id: int = 0, column_ids: List[int] = []
     ) -> ColumnSearchResponse:
```

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/generated/google/api.py` & `bigeye_sdk-0.4.55/bigeye_sdk/generated/google/api.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/model/big_config.py` & `bigeye_sdk-0.4.55/bigeye_sdk/model/big_config.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/model/collection_models.py` & `bigeye_sdk-0.4.55/bigeye_sdk/model/collection_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/model/dbt_schema.py` & `bigeye_sdk-0.4.55/bigeye_sdk/model/dbt_schema.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/model/delta_facade.py` & `bigeye_sdk-0.4.55/bigeye_sdk/model/delta_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/model/metric_facade.py` & `bigeye_sdk-0.4.55/bigeye_sdk/model/metric_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/model/protobuf_enum_facade.py` & `bigeye_sdk-0.4.55/bigeye_sdk/model/protobuf_enum_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/model/protobuf_message_facade.py` & `bigeye_sdk-0.4.55/bigeye_sdk/model/protobuf_message_facade.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,14 +27,104 @@
 from bigeye_sdk.model.base_datawatch_facade import DatawatchFacade
 from bigeye_sdk.model.protobuf_enum_facade import SimplePredefinedMetricName, SimpleTimeIntervalType, \
     SimpleAutothresholdSensitivity, SimpleLookbackType, SimpleAggregationType
 from bigeye_sdk.serializable import PydanticSubtypeSerializable
 
 log = get_logger(__file__)
 
+freshness_metrics = [
+    SimplePredefinedMetricName.HOURS_SINCE_LAST_LOAD,
+    SimplePredefinedMetricName.HOURS_SINCE_MAX_DATE,
+    SimplePredefinedMetricName.HOURS_SINCE_MAX_TIMESTAMP,
+    SimplePredefinedMetricName.FRESHNESS
+]
+
+volume_metrics = [
+    SimplePredefinedMetricName.VOLUME,
+    SimplePredefinedMetricName.ROWS_INSERTED,
+    SimplePredefinedMetricName.COUNT_ROWS
+]
+
+completeness_metrics = [
+    SimplePredefinedMetricName.PERCENT_NULL,
+    SimplePredefinedMetricName.COUNT_NULL,
+    SimplePredefinedMetricName.PERCENT_NOT_NULL,
+    SimplePredefinedMetricName.COUNT_NOT_NULL,
+    SimplePredefinedMetricName.PERCENT_EMPTY_STRING,
+    SimplePredefinedMetricName.COUNT_EMPTY_STRING,
+    SimplePredefinedMetricName.PERCENT_NAN,
+    SimplePredefinedMetricName.COUNT_NAN
+]
+
+uniqueness_metrics = [
+    SimplePredefinedMetricName.COUNT_DISTINCT,
+    SimplePredefinedMetricName.COUNT_DUPLICATES
+]
+
+distribution_metrics = [
+    SimplePredefinedMetricName.MAX,
+    SimplePredefinedMetricName.MIN,
+    SimplePredefinedMetricName.AVERAGE,
+    SimplePredefinedMetricName.VARIANCE,
+    SimplePredefinedMetricName.MEDIAN,
+    SimplePredefinedMetricName.SUM,
+    SimplePredefinedMetricName.SKEW,
+    SimplePredefinedMetricName.KURTOSIS,
+    SimplePredefinedMetricName.GEOMETRIC_MEAN,
+    SimplePredefinedMetricName.HARMONIC_MEAN,
+    SimplePredefinedMetricName.COUNT_FALSE,
+    SimplePredefinedMetricName.PERCENT_FALSE,
+    SimplePredefinedMetricName.COUNT_TRUE,
+    SimplePredefinedMetricName.PERCENT_TRUE
+]
+
+validity_metrics = [
+    SimplePredefinedMetricName.STRING_LENGTH_MAX,
+    SimplePredefinedMetricName.STRING_LENGTH_MIN,
+    SimplePredefinedMetricName.STRING_LENGTH_AVERAGE,
+    SimplePredefinedMetricName.PERCENT_UUID,
+    SimplePredefinedMetricName.COUNT_UUID,
+    SimplePredefinedMetricName.COUNT_CUSIP,
+    SimplePredefinedMetricName.PERCENT_CUSIP,
+    SimplePredefinedMetricName.COUNT_SEDOL,
+    SimplePredefinedMetricName.PERCENT_SEDOL,
+    SimplePredefinedMetricName.COUNT_ISIN,
+    SimplePredefinedMetricName.PERCENT_ISIN,
+    SimplePredefinedMetricName.COUNT_LEI,
+    SimplePredefinedMetricName.PERCENT_LEI,
+    SimplePredefinedMetricName.COUNT_FIGI,
+    SimplePredefinedMetricName.PERCENT_FIGI,
+    SimplePredefinedMetricName.COUNT_PERM_ID,
+    SimplePredefinedMetricName.PERCENT_PERM_ID,
+    SimplePredefinedMetricName.COUNT_NAN,
+    SimplePredefinedMetricName.PERCENT_NAN,
+    SimplePredefinedMetricName.COUNT_LONGITUDE,
+    SimplePredefinedMetricName.PERCENT_LONGITUDE,
+    SimplePredefinedMetricName.COUNT_LATITUDE,
+    SimplePredefinedMetricName.PERCENT_LATITUDE,
+    SimplePredefinedMetricName.COUNT_NOT_IN_FUTURE,
+    SimplePredefinedMetricName.PERCENT_NOT_IN_FUTURE,
+    SimplePredefinedMetricName.COUNT_DATE_NOT_IN_FUTURE,
+    SimplePredefinedMetricName.PERCENT_DATE_NOT_IN_FUTURE,
+    SimplePredefinedMetricName.COUNT_SSN,
+    SimplePredefinedMetricName.PERCENT_SSN,
+    SimplePredefinedMetricName.COUNT_EMAIL,
+    SimplePredefinedMetricName.PERCENT_EMAIL,
+    SimplePredefinedMetricName.COUNT_USA_PHONE,
+    SimplePredefinedMetricName.PERCENT_USA_PHONE,
+    SimplePredefinedMetricName.COUNT_USA_ZIP_CODE,
+    SimplePredefinedMetricName.PERCENT_USA_ZIP_CODE,
+    SimplePredefinedMetricName.PERCENT_UUID,
+    SimplePredefinedMetricName.COUNT_TIMESTAMP_STRING,
+    SimplePredefinedMetricName.PERCENT_TIMESTAMP_STRING,
+    SimplePredefinedMetricName.COUNT_USA_STATE_CODE,
+    SimplePredefinedMetricName.PERCENT_USA_STATE_CODE,
+    SimplePredefinedMetricName.PERCENT_VALUE_IN_LIST
+]
+
 
 def get_type_from_dict(obj: betterproto.Message) -> str:
     """A patch for beterproto.which_one_of not working on objects serialized from_dict.   I have reported the bug to
     the maintainers of better proto.  TODO remove when bug is fixed."""
     return list(obj.to_dict(casing=betterproto.Casing.SNAKE).keys())[0]
 
 
@@ -46,18 +136,62 @@
         freshness_metric_names = [SimplePredefinedMetricName.HOURS_SINCE_LAST_LOAD,
                                   SimplePredefinedMetricName.HOURS_SINCE_MAX_DATE,
                                   SimplePredefinedMetricName.HOURS_SINCE_MAX_TIMESTAMP,
                                   SimplePredefinedMetricName.FRESHNESS]
         return [SimplePredefinedMetric(type="PREDEFINED", predefined_metric=i) for i in freshness_metric_names]
 
     @classmethod
+    def get_volume_metric_types(cls) -> List[SimplePredefinedMetric]:
+        return cls.__get_simple_predefined_metrics(metric_names=volume_metrics)
+
+    @classmethod
+    def get_completeness_metric_types(cls) -> List[SimplePredefinedMetric]:
+        return cls.__get_simple_predefined_metrics(metric_names=completeness_metrics)
+
+    @classmethod
+    def get_uniqueness_metric_types(cls) -> List[SimplePredefinedMetric]:
+        return cls.__get_simple_predefined_metrics(metric_names=uniqueness_metrics)
+
+    @classmethod
+    def get_distribution_metric_types(cls) -> List[SimplePredefinedMetric]:
+        return cls.__get_simple_predefined_metrics(metric_names=distribution_metrics)
+
+    @classmethod
+    def get_validity_metric_types(cls) -> List[SimplePredefinedMetric]:
+        return cls.__get_simple_predefined_metrics(metric_names=validity_metrics)
+
+    @classmethod
+    def __get_simple_predefined_metrics(cls, metric_names: List[SimplePredefinedMetricName]):
+        return [SimplePredefinedMetric(type="PREDEFINED", predefined_metric=i) for i in metric_names]
+
+    @classmethod
     def is_freshness_metric(cls, predefined_metric):
         return predefined_metric in cls.get_freshness_metric_types()
 
     @classmethod
+    def is_volume_metric(cls, predefined_metric):
+        return predefined_metric in cls.get_volume_metric_types()
+
+    @classmethod
+    def is_completeness_metric(cls, predefined_metric):
+        return predefined_metric in cls.get_completeness_metric_types()
+
+    @classmethod
+    def is_uniqueness_metric(cls, predefined_metric):
+        return predefined_metric in cls.get_uniqueness_metric_types()
+
+    @classmethod
+    def is_distribution_metric(cls, predefined_metric):
+        return predefined_metric in cls.get_distribution_metric_types()
+
+    @classmethod
+    def is_validity_metric(cls, predefined_metric):
+        return predefined_metric in cls.get_validity_metric_types()
+
+    @classmethod
     def is_freshness_volume(cls, predefined_metric):
         return predefined_metric in [
             SimplePredefinedMetric(type="PREDEFINED", predefined_metric=SimplePredefinedMetricName.FRESHNESS),
             SimplePredefinedMetric(type="PREDEFINED", predefined_metric=SimplePredefinedMetricName.VOLUME)
         ]
 
     @classmethod
@@ -1001,15 +1135,14 @@
                 builder.lookback_type = SimpleLookbackType.DATA_TIME.to_datawatch_object()
 
             builder.grain_seconds = self.lookback.bucket_size.to_seconds()
 
         if SimpleMetricType.is_freshness_volume(self.metric_type):
             builder.grain_seconds = BucketSize.HOUR.to_seconds()
 
-
         builder.muted_until_epoch_seconds = self.muted_until_epoch_seconds
 
         if self.collection_ids:
             builder.collection_ids = self.collection_ids
         if self.metric_schedule:
             builder.metric_schedule = self.metric_schedule.to_datawatch_object()
```

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/model/sla_models.py` & `bigeye_sdk-0.4.55/bigeye_sdk/model/sla_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/bigeye_sdk/serializable.py` & `bigeye_sdk-0.4.55/bigeye_sdk/serializable.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.54/pyproject.toml` & `bigeye_sdk-0.4.55/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [tool.poetry]
 name = "bigeye-sdk"
-version = "0.4.54"
+version = "0.4.55"
 description = "Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically."
 license = "Proprietary"
 authors = ["Bigeye <support@bigeye.com>"]
 readme = "README.md"
 homepage = "https://docs.bigeye.com/docs"
 
 [[tool.poetry.source]]
 name = "staging"
 url = "https://bigeye-021451147547.d.codeartifact.us-west-2.amazonaws.com/pypi/pypi-store/"
-secondary = true
+priority = "supplemental"
 
 [tool.poetry.dependencies]
 # Should comply with https://raw.githubusercontent.com/apache/airflow/constraints-2.4.3/constraints-3.10.txt
 # for compatibility with Airflow
-python = "^3.7.2"
+python = "^3.9.0"
 requests = '2.28.1' # frozen for aws and airflow integration
 betterproto = {extras = ["compiler"], version = "^1.2.5"}
-fuzzywuzzy = '^0.18.0'
 PyYAML = '6.0' # frozen for aws and airflow integration
-python-Levenshtein = '^0.12.2'
+rapidfuzz = '^3.1.1'
 lz4 = '^4.0.1'
 keyring = '23.11.0' # frozen for aws and airflow integration
 pycryptodomex = "3.15.0" # frozen for aws and airflow integration .
 pydantic = '^1.9.2'
 pydantic-yaml = '^0.8.0'
 setuptools = '^59.6.0'
 grpclib = '^0.4.2'
@@ -113,11 +112,11 @@
         help = "Run all tests"
         shell = """
         cd ../../tests
         PYTHONPATH=.:../bigeye-cli:../bigeye-aws:$PYTHONPATH pytest
         """
 
 [build-system]
-requires = ["poetry-core>=1.3.1"]
+requires = ["poetry-core>=1.5.1"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bigeye_sdk-0.4.54/PKG-INFO` & `bigeye_sdk-0.4.55/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: bigeye-sdk
-Version: 0.4.54
+Version: 0.4.55
 Summary: Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically.
 Home-page: https://docs.bigeye.com/docs
 License: Proprietary
 Author: Bigeye
 Author-email: support@bigeye.com
-Requires-Python: >=3.7.2,<4.0.0
+Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyGithub (==1.57)
 Requires-Dist: PyYAML (==6.0)
 Requires-Dist: betterproto[compiler] (>=1.2.5,<2.0.0)
 Requires-Dist: boto3 (==1.26.7)
 Requires-Dist: botocore (==1.29.7)
-Requires-Dist: fuzzywuzzy (>=0.18.0,<0.19.0)
 Requires-Dist: grpclib (>=0.4.2,<0.5.0)
 Requires-Dist: keyring (==23.11.0)
 Requires-Dist: lz4 (>=4.0.1,<5.0.0)
 Requires-Dist: pycryptodomex (==3.15.0)
 Requires-Dist: pydantic (>=1.9.2,<2.0.0)
 Requires-Dist: pydantic-yaml (>=0.8.0,<0.9.0)
-Requires-Dist: python-Levenshtein (>=0.12.2,<0.13.0)
+Requires-Dist: rapidfuzz (>=3.1.1,<4.0.0)
 Requires-Dist: requests (==2.28.1)
 Requires-Dist: setuptools (>=59.6.0,<60.0.0)
 Requires-Dist: smart-open (>=6.1.0,<7.0.0)
 Requires-Dist: types-PyYAML (>=6.0.11,<7.0.0)
 Description-Content-Type: text/markdown
 
 # Bigeye SDK
```

