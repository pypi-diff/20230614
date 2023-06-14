# Comparing `tmp/ocellus-0.1.80.tar.gz` & `tmp/ocellus-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocellus-0.1.80.tar", last modified: Wed Jun 14 10:42:14 2023, max compression
+gzip compressed data, was "ocellus-0.1.9.tar", last modified: Thu Jun  9 15:30:04 2022, max compression
```

## Comparing `ocellus-0.1.80.tar` & `ocellus-0.1.9.tar`

### file list

```diff
@@ -1,98 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:42:14.085466 ocellus-0.1.80/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 10:42:04.000000 ocellus-0.1.80/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-14 10:42:14.085466 ocellus-0.1.80/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-14 10:42:04.000000 ocellus-0.1.80/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 10:42:14.085466 ocellus-0.1.80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-14 10:42:13.000000 ocellus-0.1.80/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:42:14.077465 ocellus-0.1.80/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:42:14.077465 ocellus-0.1.80/src/ocellus/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:42:14.077465 ocellus-0.1.80/src/ocellus/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:42:14.077465 ocellus-0.1.80/src/ocellus/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/api/v1/ocellus_api_command_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12279 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/api/v1/ocellus_api_command_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    48293 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/api/v1/ocellus_api_module_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/api/v1/ocellus_api_module_config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11380 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/api/v1/ocellus_api_module_data_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/api/v1/ocellus_api_module_data_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    38795 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/api/v1/ocellus_api_module_info_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    32015 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/api/v1/ocellus_api_module_info_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:42:14.077465 ocellus-0.1.80/src/ocellus/google/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:42:14.085466 ocellus-0.1.80/src/ocellus/google/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/annotations_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/annotations_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/backend_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/backend_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/billing_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/billing_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/client_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/client_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/config_change_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/config_change_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/consumer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/consumer_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/context_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/context_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/control_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/control_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/distribution_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/distribution_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/documentation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/documentation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/endpoint_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/endpoint_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/field_behavior_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/field_behavior_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/http_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/http_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/httpbody_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/httpbody_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/label_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/label_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/launch_stage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/launch_stage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/logging_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/logging_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/metric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/metric_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/monitored_resource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/monitored_resource_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/monitoring_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/monitoring_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/quota_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/quota_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/resource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/resource_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/routing_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/routing_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/source_info_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/source_info_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/system_parameter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/system_parameter_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/usage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/google/api/usage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/ocellus_dataflow_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/ocellus_dataflow_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/ocellus_module_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/ocellus_module_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/ocellus_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/ocellus_types_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:42:14.077465 ocellus-0.1.80/src/ocellus/protoc_gen_swagger/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:42:14.085466 ocellus-0.1.80/src/ocellus/protoc_gen_swagger/options/
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/protoc_gen_swagger/options/annotations_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/protoc_gen_swagger/options/annotations_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/protoc_gen_swagger/options/openapiv2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 10:42:04.000000 ocellus-0.1.80/src/ocellus/protoc_gen_swagger/options/openapiv2_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:42:14.077465 ocellus-0.1.80/src/ocellus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-14 10:42:14.000000 ocellus-0.1.80/src/ocellus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-14 10:42:14.000000 ocellus-0.1.80/src/ocellus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 10:42:14.000000 ocellus-0.1.80/src/ocellus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 10:42:14.000000 ocellus-0.1.80/src/ocellus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 10:42:14.000000 ocellus-0.1.80/src/ocellus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.525245 ocellus-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     9669 2022-06-09 15:30:04.525245 ocellus-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7299 2022-06-09 15:29:53.000000 ocellus-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 15:30:04.525245 ocellus-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-06-09 15:30:03.000000 ocellus-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.513245 ocellus-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.517245 ocellus-0.1.9/src/ocellus/
+-rw-r--r--   0 runner    (1001) docker     (121)      551 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.513245 ocellus-0.1.9/src/ocellus/api/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.517245 ocellus-0.1.9/src/ocellus/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19526 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_command_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14141 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_command_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10198 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_module_data_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4793 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_module_data_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38994 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_module_info_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20690 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_module_info_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.513245 ocellus-0.1.9/src/ocellus/google/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.525245 ocellus-0.1.9/src/ocellus/google/api/
+-rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/annotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4219 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2148 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/backend_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/backend_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2325 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/billing_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/billing_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/client_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/client_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2701 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/config_change_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/config_change_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2467 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/consumer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/consumer_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/context_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/context_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1498 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/control_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/control_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6431 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/distribution_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/distribution_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2949 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/documentation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/documentation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1774 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/endpoint_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/endpoint_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2152 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/field_behavior_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/field_behavior_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2997 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/http_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/http_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/httpbody_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/httpbody_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/label_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1585 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/launch_stage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/launch_stage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2406 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/logging_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/logging_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3924 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/metric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/metric_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5204 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/monitored_resource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/monitored_resource_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2515 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/monitoring_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/monitoring_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4510 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/quota_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/quota_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4155 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/resource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/resource_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2521 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/routing_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/routing_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5321 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/source_info_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/source_info_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2879 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/system_parameter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/system_parameter_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/usage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/usage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6285 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/ocellus_dataflow_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4331 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/ocellus_dataflow_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7999 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/ocellus_module_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4753 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/ocellus_module_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23961 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/ocellus_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/ocellus_types_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.513245 ocellus-0.1.9/src/ocellus/protoc_gen_swagger/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.525245 ocellus-0.1.9/src/ocellus/protoc_gen_swagger/options/
+-rw-r--r--   0 runner    (1001) docker     (121)     2955 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/protoc_gen_swagger/options/annotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/protoc_gen_swagger/options/annotations_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24954 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/protoc_gen_swagger/options/openapiv2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/protoc_gen_swagger/options/openapiv2_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.517245 ocellus-0.1.9/src/ocellus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9669 2022-06-09 15:30:04.000000 ocellus-0.1.9/src/ocellus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3534 2022-06-09 15:30:04.000000 ocellus-0.1.9/src/ocellus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 15:30:04.000000 ocellus-0.1.9/src/ocellus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-06-09 15:30:04.000000 ocellus-0.1.9/src/ocellus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-09 15:30:04.000000 ocellus-0.1.9/src/ocellus.egg-info/top_level.txt
```

### Comparing `ocellus-0.1.80/setup.py` & `ocellus-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(CWD, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="ocellus",
-    version="0.1.80",
+    version="0.1.9",
     description="Ocellus API Python Client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://docs.ocellus.io/",
     author="Byte Motion AB",
     author_email="python@bytemotion.se",
     license="MIT",
```

### Comparing `ocellus-0.1.80/src/ocellus/api/v1/ocellus_api_command_service_pb2_grpc.py` & `ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_command_service_pb2_grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,19 @@
                 response_deserializer=api_dot_v1_dot_ocellus__api__command__service__pb2.GetLoadCommandResponse.FromString,
                 )
         self.GetPauseCommand = channel.unary_unary(
                 '/ocellus.api.v1.command.OcellusCommandService/GetPauseCommand',
                 request_serializer=api_dot_v1_dot_ocellus__api__command__service__pb2.GetPauseCommandRequest.SerializeToString,
                 response_deserializer=api_dot_v1_dot_ocellus__api__command__service__pb2.GetPauseCommandResponse.FromString,
                 )
+        self.GetStateCommand = channel.unary_unary(
+                '/ocellus.api.v1.command.OcellusCommandService/GetStateCommand',
+                request_serializer=api_dot_v1_dot_ocellus__api__command__service__pb2.GetStateCommandRequest.SerializeToString,
+                response_deserializer=api_dot_v1_dot_ocellus__api__command__service__pb2.GetStateCommandResponse.FromString,
+                )
 
 
 class OcellusCommandServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def GetCameraCommand(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -82,14 +87,20 @@
 
     def GetPauseCommand(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetStateCommand(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_OcellusCommandServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'GetCameraCommand': grpc.unary_unary_rpc_method_handler(
                     servicer.GetCameraCommand,
                     request_deserializer=api_dot_v1_dot_ocellus__api__command__service__pb2.GetCameraCommandRequest.FromString,
                     response_serializer=api_dot_v1_dot_ocellus__api__command__service__pb2.GetCameraCommandResponse.SerializeToString,
@@ -115,14 +126,19 @@
                     response_serializer=api_dot_v1_dot_ocellus__api__command__service__pb2.GetLoadCommandResponse.SerializeToString,
             ),
             'GetPauseCommand': grpc.unary_unary_rpc_method_handler(
                     servicer.GetPauseCommand,
                     request_deserializer=api_dot_v1_dot_ocellus__api__command__service__pb2.GetPauseCommandRequest.FromString,
                     response_serializer=api_dot_v1_dot_ocellus__api__command__service__pb2.GetPauseCommandResponse.SerializeToString,
             ),
+            'GetStateCommand': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetStateCommand,
+                    request_deserializer=api_dot_v1_dot_ocellus__api__command__service__pb2.GetStateCommandRequest.FromString,
+                    response_serializer=api_dot_v1_dot_ocellus__api__command__service__pb2.GetStateCommandResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'ocellus.api.v1.command.OcellusCommandService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -226,7 +242,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/ocellus.api.v1.command.OcellusCommandService/GetPauseCommand',
             api_dot_v1_dot_ocellus__api__command__service__pb2.GetPauseCommandRequest.SerializeToString,
             api_dot_v1_dot_ocellus__api__command__service__pb2.GetPauseCommandResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetStateCommand(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ocellus.api.v1.command.OcellusCommandService/GetStateCommand',
+            api_dot_v1_dot_ocellus__api__command__service__pb2.GetStateCommandRequest.SerializeToString,
+            api_dot_v1_dot_ocellus__api__command__service__pb2.GetStateCommandResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `ocellus-0.1.80/src/ocellus/api/v1/ocellus_api_module_data_service_pb2.py` & `ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_module_data_service_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,65 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: api/v1/ocellus_api_module_data_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
-from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from protoc_gen_swagger.options import annotations_pb2 as protoc__gen__swagger_dot_options_dot_annotations__pb2
-import ocellus_types_pb2 as ocellus__types__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,api/v1/ocellus_api_module_data_service.proto\x12\x1aocellus.api.v1.module.data\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a google/protobuf/field_mask.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a,protoc-gen-swagger/options/annotations.proto\x1a\x13ocellus_types.proto\"\x92\x03\n\x14GetModuleDataRequest\x12[\n\tmodule_id\x18\x01 \x01(\tBH\x92\x41\x45\x32\x43If provided, only data for the specified module id will be returned\x12\x66\n\x04path\x18\x02 \x01(\tBX\x92\x41U2SIf provided, it will only return the field which matches the path. Case insensitive\x12\xb4\x01\n\x04sort\x18\x03 \x01(\tB\xa5\x01\x92\x41\xa1\x01\x32\x9e\x01If provided, will sort according to query. Example: $.items[*].position.y:asc\nCurrently, only the follow ing supported:\n$.items[*].position.[x|y|z]:[asc|desc]\"\xca\x10\n\x12GetAllDataResponse\x12(\n\x07modules\x18\x01 \x03(\x0b\x32\x17.google.protobuf.Struct:\x89\x10\x92\x41\x85\x10\x32\x82\x10\x12\xff\x0f{\"modules\": [{\"timestamp\": 3194,\"frameId\": 63,\"rgbaImage\": \"/img/rgbaImage\",\"camera\": { \"name\": \"rs1\", \"fov\": 58.165508270263672, \"position\": {\"x\": 0.0052760359831154346,\"y\": 0.058778464794158936,\"z\": -0.00064044661121442914 }, \"quaternion\": {\"w\": -0.74804270267486572,\"x\": -0.02558884397149086,\"y\": -0.66211831569671631,\"z\": 0.037104226648807526 }, \"orientation\": {\"pitch\": 5.0150761604309082,\"yaw\": 82.971817016601562,\"roll\": -1.243896484375 }}},{\"timestamp\": 3200,\"frameId\": 63,\"camera\": { \"name\": \"img\", \"fov\": 53.130104064941406, \"position\": {\"x\": 0,\"y\": 0,\"z\": 0 }, \"quaternion\": {\"w\": 1,\"x\": 0,\"y\": 0,\"z\": 0 }, \"orientation\": {\"pitch\": -0,\"yaw\": 0,\"roll\": 0 }},\"rgbaImage\": \"/img/rgbaImage\",\"items\": []},{\"timestamp\": 2792,\"frameId\": 96,\"camera\": { \"name\": \"rs2\", \"fov\": 58.165508270263672, \"position\": {\"x\": 0.0052760359831154346,\"y\": 0.058778464794158936,\"z\": -0.00064044661121442914 }, \"quaternion\": {\"w\": -0.74804270267486572,\"x\": -0.02558884397149086,\"y\": -0.66211831569671631,\"z\": 0.037104226648807526 }, \"orientation\": {\"pitch\": 5.0150761604309082,\"yaw\": 82.971817016601562,\"roll\": -1.243896484375 }},\"rgbaImage\": \"/img/rgbaImage\"},{\"timestamp\": 2792,\"frameId\": 96,\"items\": [],\"camera\": { \"name\": \"img2\", \"fov\": 53.130104064941406, \"position\": {\"x\": 0,\"y\": 0,\"z\": 0 }, \"quaternion\": {\"w\": 1,\"x\": 0,\"y\": 0,\"z\": 0 }, \"orientation\": {\"pitch\": -0,\"yaw\": 0,\"roll\": 0 }},\"rgbaImage\": \"/img/rgbaImage\"},{\"timestamp\": 3201,\"frameId\": 63,\"items\": [ {\"id\": 0,\"name\": \"blob1\",\"weight\": 0,\"confidence\": 1,\"color\": \"#0000FF\",\"dimension\": { \"width\": 0.044311594218015671, \"height\": 0.15963709354400635, \"depth\": 0.044311594218015671},\"position\": { \"x\": 0.28055679798126221, \"y\": 0.023770391941070557, \"z\": 0.038520518690347672},\"quaternion\": { \"w\": -0.018691437318921089, \"x\": 0.74761569499969482, \"y\": -0.044893074780702591, \"z\": -0.66234886646270752},\"orientation\": { \"pitch\": -5.01507568359375, \"yaw\": -97.0281982421875, \"roll\": -177.56260681152344},\"extremePoints\": {},\"pathPoints\": {},\"parentCamera\": \"rs1\" }],\"rgbaImage\": \"/img/rgbaImage\"}]}\"c\n\x1eGetModuleOutputDataRequestV1_1\x12\x11\n\tmodule_id\x18\x01 \x01(\t\x12.\n\nfield_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"\x80\x02\n\x1fGetModuleOutputDataResponseV1_1\x12Y\n\x07modules\x18\x01 \x03(\x0b\x32H.ocellus.api.v1.module.data.GetModuleOutputDataResponseV1_1.ModuleOutput\x1a\x81\x01\n\x0cModuleOutput\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x66rame_id\x18\x02 \x01(\x05\x12\x13\n\x0bpipeline_id\x18\x03 \x01(\x05\x12\x1b\n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\r.ocellus.Data2\xd0\x05\n\x18OcellusModuleDataService\x12\xb8\x01\n\rGetModuleData\x12\x30.ocellus.api.v1.module.data.GetModuleDataRequest\x1a\x17.google.protobuf.Struct\"\\\x88\x02\x01\x92\x41\x1d\x1a\x1bUse GetModuleOutputDataV1_1\x82\xd3\xe4\x93\x02\x33\x12\x13/api/v1/{module_id}Z\x1c\x12\x1a/api/v1/{module_id}/{path}\x12\xa2\x01\n\nGetAllData\x12\x30.ocellus.api.v1.module.data.GetModuleDataRequest\x1a..ocellus.api.v1.module.data.GetAllDataResponse\"2\x88\x02\x01\x92\x41\x1d\x1a\x1bUse GetModuleOutputDataV1_1\x82\xd3\xe4\x93\x02\t\x12\x07/api/v1\x12\xad\x02\n\x17GetModuleOutputDataV1_1\x12:.ocellus.api.v1.module.data.GetModuleOutputDataRequestV1_1\x1a;.ocellus.api.v1.module.data.GetModuleOutputDataResponseV1_1\"\x98\x01\x92\x41k\x1aiReturns all module data, if module_id is provided, only data for the specified module id will be returned\x82\xd3\xe4\x93\x02$\x12\t/api/v1_1Z\x17\x12\x15/api/v1_1/{module_id}\x1a$\x92\x41!\x12\x1fServes data produced by modulesB\x81\x01\n\x1e\x63om.ocellus.api.v1.module.dataB\x18OcellusModuleDataServiceP\x01Z\x1egithub.com/byte-motion/ocellus\xa2\x02\x05OAPMD\xaa\x02\x1aOcellus.Api.V1.Module.Datab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,api/v1/ocellus_api_module_data_service.proto\x12\x1aocellus.api.v1.module.data\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a,protoc-gen-swagger/options/annotations.proto\"\x91\x03\n\x14GetModuleDataRequest\x12Z\n\x08moduleId\x18\x01 \x01(\tBH\x92\x41\x45\x32\x43If provided, only data for the specified module id will be returned\x12\x66\n\x04path\x18\x02 \x01(\tBX\x92\x41U2SIf provided, it will only return the field which matches the path. Case insensitive\x12\xb4\x01\n\x04sort\x18\x03 \x01(\tB\xa5\x01\x92\x41\xa1\x01\x32\x9e\x01If provided, will sort according to query. Example: $.items[*].position.y:asc\nCurrently, only the follow ing supported:\n$.items[*].position.[x|y|z]:[asc|desc]\"\xca\x10\n\x12GetAllDataResponse\x12(\n\x07modules\x18\x01 \x03(\x0b\x32\x17.google.protobuf.Struct:\x89\x10\x92\x41\x85\x10\x32\x82\x10\x12\xff\x0f{\"modules\": [{\"timestamp\": 3194,\"frameId\": 63,\"rgbaImage\": \"/img/rgbaImage\",\"camera\": { \"name\": \"rs1\", \"fov\": 58.165508270263672, \"position\": {\"x\": 0.0052760359831154346,\"y\": 0.058778464794158936,\"z\": -0.00064044661121442914 }, \"quaternion\": {\"w\": -0.74804270267486572,\"x\": -0.02558884397149086,\"y\": -0.66211831569671631,\"z\": 0.037104226648807526 }, \"orientation\": {\"pitch\": 5.0150761604309082,\"yaw\": 82.971817016601562,\"roll\": -1.243896484375 }}},{\"timestamp\": 3200,\"frameId\": 63,\"camera\": { \"name\": \"img\", \"fov\": 53.130104064941406, \"position\": {\"x\": 0,\"y\": 0,\"z\": 0 }, \"quaternion\": {\"w\": 1,\"x\": 0,\"y\": 0,\"z\": 0 }, \"orientation\": {\"pitch\": -0,\"yaw\": 0,\"roll\": 0 }},\"rgbaImage\": \"/img/rgbaImage\",\"items\": []},{\"timestamp\": 2792,\"frameId\": 96,\"camera\": { \"name\": \"rs2\", \"fov\": 58.165508270263672, \"position\": {\"x\": 0.0052760359831154346,\"y\": 0.058778464794158936,\"z\": -0.00064044661121442914 }, \"quaternion\": {\"w\": -0.74804270267486572,\"x\": -0.02558884397149086,\"y\": -0.66211831569671631,\"z\": 0.037104226648807526 }, \"orientation\": {\"pitch\": 5.0150761604309082,\"yaw\": 82.971817016601562,\"roll\": -1.243896484375 }},\"rgbaImage\": \"/img/rgbaImage\"},{\"timestamp\": 2792,\"frameId\": 96,\"items\": [],\"camera\": { \"name\": \"img2\", \"fov\": 53.130104064941406, \"position\": {\"x\": 0,\"y\": 0,\"z\": 0 }, \"quaternion\": {\"w\": 1,\"x\": 0,\"y\": 0,\"z\": 0 }, \"orientation\": {\"pitch\": -0,\"yaw\": 0,\"roll\": 0 }},\"rgbaImage\": \"/img/rgbaImage\"},{\"timestamp\": 3201,\"frameId\": 63,\"items\": [ {\"id\": 0,\"name\": \"blob1\",\"weight\": 0,\"confidence\": 1,\"color\": \"#0000FF\",\"dimension\": { \"width\": 0.044311594218015671, \"height\": 0.15963709354400635, \"depth\": 0.044311594218015671},\"position\": { \"x\": 0.28055679798126221, \"y\": 0.023770391941070557, \"z\": 0.038520518690347672},\"quaternion\": { \"w\": -0.018691437318921089, \"x\": 0.74761569499969482, \"y\": -0.044893074780702591, \"z\": -0.66234886646270752},\"orientation\": { \"pitch\": -5.01507568359375, \"yaw\": -97.0281982421875, \"roll\": -177.56260681152344},\"extremePoints\": {},\"pathPoints\": {},\"parentCamera\": \"rs1\" }],\"rgbaImage\": \"/img/rgbaImage\"}]}2\xb5\x03\n\x18OcellusModuleDataService\x12\xc3\x01\n\rGetModuleData\x12\x30.ocellus.api.v1.module.data.GetModuleDataRequest\x1a\x17.google.protobuf.Struct\"g\x92\x41-\x1a+Querys the data for the specified module id\x82\xd3\xe4\x93\x02\x31\x12\x12/api/v1/{moduleId}Z\x1b\x12\x19/api/v1/{moduleId}/{path}\x12\xac\x01\n\nGetAllData\x12\x30.ocellus.api.v1.module.data.GetModuleDataRequest\x1a..ocellus.api.v1.module.data.GetAllDataResponse\"<\x92\x41*\x1a(Returns all data produced by all modules\x82\xd3\xe4\x93\x02\t\x12\x07/api/v1\x1a$\x92\x41!\x12\x1fServes data produced by modulesB\x81\x01\n\x1e\x63om.ocellus.api.v1.module.dataB\x18OcellusModuleDataServiceP\x01Z\x1egithub.com/byte-motion/ocellus\xa2\x02\x05OAPMD\xaa\x02\x1aOcellus.Api.V1.Module.Datab\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api.v1.ocellus_api_module_data_service_pb2', globals())
+
+
+_GETMODULEDATAREQUEST = DESCRIPTOR.message_types_by_name['GetModuleDataRequest']
+_GETALLDATARESPONSE = DESCRIPTOR.message_types_by_name['GetAllDataResponse']
+GetModuleDataRequest = _reflection.GeneratedProtocolMessageType('GetModuleDataRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETMODULEDATAREQUEST,
+  '__module__' : 'api.v1.ocellus_api_module_data_service_pb2'
+  # @@protoc_insertion_point(class_scope:ocellus.api.v1.module.data.GetModuleDataRequest)
+  })
+_sym_db.RegisterMessage(GetModuleDataRequest)
+
+GetAllDataResponse = _reflection.GeneratedProtocolMessageType('GetAllDataResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETALLDATARESPONSE,
+  '__module__' : 'api.v1.ocellus_api_module_data_service_pb2'
+  # @@protoc_insertion_point(class_scope:ocellus.api.v1.module.data.GetAllDataResponse)
+  })
+_sym_db.RegisterMessage(GetAllDataResponse)
+
+_OCELLUSMODULEDATASERVICE = DESCRIPTOR.services_by_name['OcellusModuleDataService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036com.ocellus.api.v1.module.dataB\030OcellusModuleDataServiceP\001Z\036github.com/byte-motion/ocellus\242\002\005OAPMD\252\002\032Ocellus.Api.V1.Module.Data'
-  _GETMODULEDATAREQUEST.fields_by_name['module_id']._options = None
-  _GETMODULEDATAREQUEST.fields_by_name['module_id']._serialized_options = b'\222AE2CIf provided, only data for the specified module id will be returned'
+  _GETMODULEDATAREQUEST.fields_by_name['moduleId']._options = None
+  _GETMODULEDATAREQUEST.fields_by_name['moduleId']._serialized_options = b'\222AE2CIf provided, only data for the specified module id will be returned'
   _GETMODULEDATAREQUEST.fields_by_name['path']._options = None
   _GETMODULEDATAREQUEST.fields_by_name['path']._serialized_options = b'\222AU2SIf provided, it will only return the field which matches the path. Case insensitive'
   _GETMODULEDATAREQUEST.fields_by_name['sort']._options = None
   _GETMODULEDATAREQUEST.fields_by_name['sort']._serialized_options = b'\222A\241\0012\236\001If provided, will sort according to query. Example: $.items[*].position.y:asc\nCurrently, only the follow ing supported:\n$.items[*].position.[x|y|z]:[asc|desc]'
   _GETALLDATARESPONSE._options = None
   _GETALLDATARESPONSE._serialized_options = b'\222A\205\0202\202\020\022\377\017{\"modules\": [{\"timestamp\": 3194,\"frameId\": 63,\"rgbaImage\": \"/img/rgbaImage\",\"camera\": { \"name\": \"rs1\", \"fov\": 58.165508270263672, \"position\": {\"x\": 0.0052760359831154346,\"y\": 0.058778464794158936,\"z\": -0.00064044661121442914 }, \"quaternion\": {\"w\": -0.74804270267486572,\"x\": -0.02558884397149086,\"y\": -0.66211831569671631,\"z\": 0.037104226648807526 }, \"orientation\": {\"pitch\": 5.0150761604309082,\"yaw\": 82.971817016601562,\"roll\": -1.243896484375 }}},{\"timestamp\": 3200,\"frameId\": 63,\"camera\": { \"name\": \"img\", \"fov\": 53.130104064941406, \"position\": {\"x\": 0,\"y\": 0,\"z\": 0 }, \"quaternion\": {\"w\": 1,\"x\": 0,\"y\": 0,\"z\": 0 }, \"orientation\": {\"pitch\": -0,\"yaw\": 0,\"roll\": 0 }},\"rgbaImage\": \"/img/rgbaImage\",\"items\": []},{\"timestamp\": 2792,\"frameId\": 96,\"camera\": { \"name\": \"rs2\", \"fov\": 58.165508270263672, \"position\": {\"x\": 0.0052760359831154346,\"y\": 0.058778464794158936,\"z\": -0.00064044661121442914 }, \"quaternion\": {\"w\": -0.74804270267486572,\"x\": -0.02558884397149086,\"y\": -0.66211831569671631,\"z\": 0.037104226648807526 }, \"orientation\": {\"pitch\": 5.0150761604309082,\"yaw\": 82.971817016601562,\"roll\": -1.243896484375 }},\"rgbaImage\": \"/img/rgbaImage\"},{\"timestamp\": 2792,\"frameId\": 96,\"items\": [],\"camera\": { \"name\": \"img2\", \"fov\": 53.130104064941406, \"position\": {\"x\": 0,\"y\": 0,\"z\": 0 }, \"quaternion\": {\"w\": 1,\"x\": 0,\"y\": 0,\"z\": 0 }, \"orientation\": {\"pitch\": -0,\"yaw\": 0,\"roll\": 0 }},\"rgbaImage\": \"/img/rgbaImage\"},{\"timestamp\": 3201,\"frameId\": 63,\"items\": [ {\"id\": 0,\"name\": \"blob1\",\"weight\": 0,\"confidence\": 1,\"color\": \"#0000FF\",\"dimension\": { \"width\": 0.044311594218015671, \"height\": 0.15963709354400635, \"depth\": 0.044311594218015671},\"position\": { \"x\": 0.28055679798126221, \"y\": 0.023770391941070557, \"z\": 0.038520518690347672},\"quaternion\": { \"w\": -0.018691437318921089, \"x\": 0.74761569499969482, \"y\": -0.044893074780702591, \"z\": -0.66234886646270752},\"orientation\": { \"pitch\": -5.01507568359375, \"yaw\": -97.0281982421875, \"roll\": -177.56260681152344},\"extremePoints\": {},\"pathPoints\": {},\"parentCamera\": \"rs1\" }],\"rgbaImage\": \"/img/rgbaImage\"}]}'
   _OCELLUSMODULEDATASERVICE._options = None
   _OCELLUSMODULEDATASERVICE._serialized_options = b'\222A!\022\037Serves data produced by modules'
   _OCELLUSMODULEDATASERVICE.methods_by_name['GetModuleData']._options = None
-  _OCELLUSMODULEDATASERVICE.methods_by_name['GetModuleData']._serialized_options = b'\210\002\001\222A\035\032\033Use GetModuleOutputDataV1_1\202\323\344\223\0023\022\023/api/v1/{module_id}Z\034\022\032/api/v1/{module_id}/{path}'
+  _OCELLUSMODULEDATASERVICE.methods_by_name['GetModuleData']._serialized_options = b'\222A-\032+Querys the data for the specified module id\202\323\344\223\0021\022\022/api/v1/{moduleId}Z\033\022\031/api/v1/{moduleId}/{path}'
   _OCELLUSMODULEDATASERVICE.methods_by_name['GetAllData']._options = None
-  _OCELLUSMODULEDATASERVICE.methods_by_name['GetAllData']._serialized_options = b'\210\002\001\222A\035\032\033Use GetModuleOutputDataV1_1\202\323\344\223\002\t\022\007/api/v1'
-  _OCELLUSMODULEDATASERVICE.methods_by_name['GetModuleOutputDataV1_1']._options = None
-  _OCELLUSMODULEDATASERVICE.methods_by_name['GetModuleOutputDataV1_1']._serialized_options = b'\222Ak\032iReturns all module data, if module_id is provided, only data for the specified module id will be returned\202\323\344\223\002$\022\t/api/v1_1Z\027\022\025/api/v1_1/{module_id}'
-  _GETMODULEDATAREQUEST._serialized_start=271
-  _GETMODULEDATAREQUEST._serialized_end=673
-  _GETALLDATARESPONSE._serialized_start=676
-  _GETALLDATARESPONSE._serialized_end=2798
-  _GETMODULEOUTPUTDATAREQUESTV1_1._serialized_start=2800
-  _GETMODULEOUTPUTDATAREQUESTV1_1._serialized_end=2899
-  _GETMODULEOUTPUTDATARESPONSEV1_1._serialized_start=2902
-  _GETMODULEOUTPUTDATARESPONSEV1_1._serialized_end=3158
-  _GETMODULEOUTPUTDATARESPONSEV1_1_MODULEOUTPUT._serialized_start=3029
-  _GETMODULEOUTPUTDATARESPONSEV1_1_MODULEOUTPUT._serialized_end=3158
-  _OCELLUSMODULEDATASERVICE._serialized_start=3161
-  _OCELLUSMODULEDATASERVICE._serialized_end=3881
+  _OCELLUSMODULEDATASERVICE.methods_by_name['GetAllData']._serialized_options = b'\222A*\032(Returns all data produced by all modules\202\323\344\223\002\t\022\007/api/v1'
+  _GETMODULEDATAREQUEST._serialized_start=183
+  _GETMODULEDATAREQUEST._serialized_end=584
+  _GETALLDATARESPONSE._serialized_start=587
+  _GETALLDATARESPONSE._serialized_end=2709
+  _OCELLUSMODULEDATASERVICE._serialized_start=2712
+  _OCELLUSMODULEDATASERVICE._serialized_end=3149
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ocellus-0.1.80/src/ocellus/api/v1/ocellus_api_module_data_service_pb2_grpc.py` & `ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_module_data_service_pb2_grpc.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,19 +21,14 @@
                 response_deserializer=google_dot_protobuf_dot_struct__pb2.Struct.FromString,
                 )
         self.GetAllData = channel.unary_unary(
                 '/ocellus.api.v1.module.data.OcellusModuleDataService/GetAllData',
                 request_serializer=api_dot_v1_dot_ocellus__api__module__data__service__pb2.GetModuleDataRequest.SerializeToString,
                 response_deserializer=api_dot_v1_dot_ocellus__api__module__data__service__pb2.GetAllDataResponse.FromString,
                 )
-        self.GetModuleOutputDataV1_1 = channel.unary_unary(
-                '/ocellus.api.v1.module.data.OcellusModuleDataService/GetModuleOutputDataV1_1',
-                request_serializer=api_dot_v1_dot_ocellus__api__module__data__service__pb2.GetModuleOutputDataRequestV1_1.SerializeToString,
-                response_deserializer=api_dot_v1_dot_ocellus__api__module__data__service__pb2.GetModuleOutputDataResponseV1_1.FromString,
-                )
 
 
 class OcellusModuleDataServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def GetModuleData(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -43,38 +38,27 @@
 
     def GetAllData(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetModuleOutputDataV1_1(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
 
 def add_OcellusModuleDataServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'GetModuleData': grpc.unary_unary_rpc_method_handler(
                     servicer.GetModuleData,
                     request_deserializer=api_dot_v1_dot_ocellus__api__module__data__service__pb2.GetModuleDataRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_struct__pb2.Struct.SerializeToString,
             ),
             'GetAllData': grpc.unary_unary_rpc_method_handler(
                     servicer.GetAllData,
                     request_deserializer=api_dot_v1_dot_ocellus__api__module__data__service__pb2.GetModuleDataRequest.FromString,
                     response_serializer=api_dot_v1_dot_ocellus__api__module__data__service__pb2.GetAllDataResponse.SerializeToString,
             ),
-            'GetModuleOutputDataV1_1': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetModuleOutputDataV1_1,
-                    request_deserializer=api_dot_v1_dot_ocellus__api__module__data__service__pb2.GetModuleOutputDataRequestV1_1.FromString,
-                    response_serializer=api_dot_v1_dot_ocellus__api__module__data__service__pb2.GetModuleOutputDataResponseV1_1.SerializeToString,
-            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'ocellus.api.v1.module.data.OcellusModuleDataService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -110,24 +94,7 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/ocellus.api.v1.module.data.OcellusModuleDataService/GetAllData',
             api_dot_v1_dot_ocellus__api__module__data__service__pb2.GetModuleDataRequest.SerializeToString,
             api_dot_v1_dot_ocellus__api__module__data__service__pb2.GetAllDataResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetModuleOutputDataV1_1(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ocellus.api.v1.module.data.OcellusModuleDataService/GetModuleOutputDataV1_1',
-            api_dot_v1_dot_ocellus__api__module__data__service__pb2.GetModuleOutputDataRequestV1_1.SerializeToString,
-            api_dot_v1_dot_ocellus__api__module__data__service__pb2.GetModuleOutputDataResponseV1_1.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `ocellus-0.1.80/src/ocellus/api/v1/ocellus_api_module_info_service_pb2.py` & `ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_module_info_service_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,104 +1,166 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: api/v1/ocellus_api_module_info_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
-from api.v1 import ocellus_api_module_config_pb2 as api_dot_v1_dot_ocellus__api__module__config__pb2
 import ocellus_module_service_pb2 as ocellus__module__service__pb2
 import ocellus_types_pb2 as ocellus__types__pb2
 from protoc_gen_swagger.options import annotations_pb2 as protoc__gen__swagger_dot_options_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,api/v1/ocellus_api_module_info_service.proto\x12\x1aocellus.api.v1.module.info\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a&api/v1/ocellus_api_module_config.proto\x1a\x1cocellus_module_service.proto\x1a\x13ocellus_types.proto\x1a,protoc-gen-swagger/options/annotations.proto\"V\n\x11GetModulesRequest\x12\x11\n\tmodule_id\x18\x01 \x01(\t\x12.\n\nfield_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"\xebO\n\x12GetModulesResponse\x12(\n\x07modules\x18\x01 \x03(\x0b\x32\x17.google.protobuf.Struct:\xaaO\x92\x41\xa6O2\xa3O\x12\xa0O{\"modules\": [{\"inputParameters\": [],\"outputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"\" }],\"id\": \"rs1\",\"active\": true,\"render\": true,\"ordinal\": 0,\"pipeline\": 0,\"type\": \"RealSense\",\"moduleState\": 1,\"stateText\": \"\",\"rsCamera\": { \"processingBlocks\": {  \"alignEnabled\": true,  \"alignTo\": 2,  \"decimationFilterEnabled\": true,  \"streamFilter\": 1,  \"formatFilter\": 1,  \"filterMagnitude\": 8,  \"thresholdFilterEnabled\": false,  \"thresholdMaxDistance\": 1.5,  \"thresholdMinDistance\": 0,  \"disparityMode02\": 0,  \"spatialFilterEnabled\": false,  \"spatialMagnitude\": 1,  \"spatialSmoothAlpha\": 0.72000002861022949,  \"spatialSmoothDelta\": 9,  \"holeFillingMode\": 0,  \"temporalFilterEnabled\": false,  \"temporalSmoothAlpha\": 0.079999998211860657,  \"temporalSmoothDelta\": 100,  \"temporalPersistance\": 6,  \"holeFillingFilterEnabled\": false,  \"holesFill\": 2,  \"colorizerEnabled\": true,  \"visualPreset\": 0,  \"colorScheme\": 5,  \"histogramEqualization\": true,  \"colorizerMinDistance\": 0,  \"colorizerMaxDistance\": 6,  \"pointCloudEnabled\": true,  \"occlusionRemoval\": 2,  \"textureStream\": 1,  \"textureFormat\": 5 }, \"cameraInfo\": {  \"name\": \"\",  \"serialNumber\": \"\",  \"firmwareVersion\": \"\",  \"recommendedFirmwareVersion\": \"\",  \"physicalPort\": \"\",  \"debugOpCode\": \"\",  \"advancedMode\": \"\",  \"productId\": \"\",  \"cameraLocked\": \"\",  \"usbTypeDescriptor\": \"\" }, \"depthResolution\": {  \"width\": 0,  \"height\": 0 }, \"colorResolution\": {  \"width\": 0,  \"height\": 0 }, \"depthFps\": 2, \"colorFps\": 2, \"serialNumber\": \"\", \"mode\": 1, \"playbackFile\": \"/home/kcarlson/Documents/test/longredtape.bag\", \"availableFps\": [  6,  15,  30,  60 ], \"availableDepthResolutions\": [  {   \"devicePrefix\": \"D\",   \"resolutions\": [    {     \"width\": 424,     \"height\": 240    },    {     \"width\": 640,     \"height\": 360    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 848,     \"height\": 100    },    {     \"width\": 848,     \"height\": 480    },    {     \"width\": 1280,     \"height\": 720    }   ]  },  {   \"devicePrefix\": \"L\",   \"resolutions\": [    {     \"width\": 240,     \"height\": 640    },    {     \"width\": 384,     \"height\": 1024    },    {     \"width\": 480,     \"height\": 640    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 768,     \"height\": 1024    },    {     \"width\": 1024,     \"height\": 768    }   ]  } ], \"availableColorResolutions\": [  {   \"devicePrefix\": \"D\",   \"resolutions\": [    {     \"width\": 424,     \"height\": 240    },    {     \"width\": 640,     \"height\": 360    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 848,     \"height\": 480    },    {     \"width\": 960,     \"height\": 540    },    {     \"width\": 1280,     \"height\": 720    }   ]  },  {   \"devicePrefix\": \"L\",   \"resolutions\": [    {     \"width\": 1280,     \"height\": 720    },    {     \"width\": 1920,     \"height\": 1080    }   ]  } ]},\"position\": { \"x\": 0.0052760359831154346, \"y\": 0.058778461068868637, \"z\": -0.00064044661121442914},\"orientation\": { \"x\": 5.0150761604309082, \"y\": 82.971817016601562, \"z\": 358.756103515625},\"showPointcloud\": false,\"depthImage\": false,\"imu\": false,\"errors\": []},{\"inputParameters\": [],\"outputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"\" }, {  \"name\": \"ITEMS\",  \"dataType\": 3,  \"key\": \"\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"\" }],\"id\": \"img\",\"active\": true,\"render\": true,\"ordinal\": 1,\"pipeline\": 0,\"type\": \"ImageSource\",\"moduleState\": 0,\"stateText\": \"\",\"flipImage\": false,\"undistort\": false,\"contourThickness\": 1,\"path\": \"/home/kcarlson/Documents/test/slideshow\",\"displayTimeSeconds\": 5,\"intrinsicsConfigName\": \"\",\"position\": { \"x\": 0, \"y\": 0, \"z\": 0},\"orientation\": { \"x\": 0, \"y\": 0, \"z\": 0},\"itemProducerOptions\": { \"graphicType\": 0, \"showPointCloud\": false, \"surface2PolygonMeshOpts\": {  \"searchRadius\": 0.02500000037252903,  \"mu\": 2.5,  \"maximumNearestNeighbors\": 100,  \"maximumSurfaceAngle\": 45,  \"minimumAngle\": 10,  \"maximumAngle\": 120,  \"normalConsistency\": false,  \"consistentVertexOrdering\": true,  \"kSearch\": 20 }},\"errors\": []},{\"inputParameters\": [],\"outputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"\" }],\"id\": \"rs2\",\"active\": true,\"render\": true,\"ordinal\": 2,\"pipeline\": 1,\"type\": \"RealSense\",\"moduleState\": 1,\"stateText\": \"\",\"rsCamera\": { \"processingBlocks\": {  \"alignEnabled\": true,  \"alignTo\": 2,  \"decimationFilterEnabled\": true,  \"streamFilter\": 1,  \"formatFilter\": 1,  \"filterMagnitude\": 8,  \"thresholdFilterEnabled\": false,  \"thresholdMaxDistance\": 1.5,  \"thresholdMinDistance\": 0,  \"disparityMode02\": 0,  \"spatialFilterEnabled\": false,  \"spatialMagnitude\": 1,  \"spatialSmoothAlpha\": 0.72000002861022949,  \"spatialSmoothDelta\": 9,  \"holeFillingMode\": 0,  \"temporalFilterEnabled\": false,  \"temporalSmoothAlpha\": 0.079999998211860657,  \"temporalSmoothDelta\": 100,  \"temporalPersistance\": 6,  \"holeFillingFilterEnabled\": false,  \"holesFill\": 2,  \"colorizerEnabled\": true,  \"visualPreset\": 0,  \"colorScheme\": 5,  \"histogramEqualization\": true,  \"colorizerMinDistance\": 0,  \"colorizerMaxDistance\": 6,  \"pointCloudEnabled\": true,  \"occlusionRemoval\": 2,  \"textureStream\": 1,  \"textureFormat\": 5 }, \"cameraInfo\": {  \"name\": \"\",  \"serialNumber\": \"\",  \"firmwareVersion\": \"\",  \"recommendedFirmwareVersion\": \"\",  \"physicalPort\": \"\",  \"debugOpCode\": \"\",  \"advancedMode\": \"\",  \"productId\": \"\",  \"cameraLocked\": \"\",  \"usbTypeDescriptor\": \"\" }, \"depthResolution\": {  \"width\": 0,  \"height\": 0 }, \"colorResolution\": {  \"width\": 0,  \"height\": 0 }, \"depthFps\": 2, \"colorFps\": 2, \"serialNumber\": \"\", \"mode\": 1, \"playbackFile\": \"/home/kcarlson/Documents/test/longredtape.bag\", \"availableFps\": [  6,  15,  30,  60 ], \"availableDepthResolutions\": [  {   \"devicePrefix\": \"D\",   \"resolutions\": [    {     \"width\": 424,     \"height\": 240    },    {     \"width\": 640,     \"height\": 360    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 848,     \"height\": 100    },    {     \"width\": 848,     \"height\": 480    },    {     \"width\": 1280,     \"height\": 720    }   ]  },  {   \"devicePrefix\": \"L\",   \"resolutions\": [    {     \"width\": 240,     \"height\": 640    },    {     \"width\": 384,     \"height\": 1024    },    {     \"width\": 480,     \"height\": 640    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 768,     \"height\": 1024    },    {     \"width\": 1024,     \"height\": 768    }   ]  } ], \"availableColorResolutions\": [  {   \"devicePrefix\": \"D\",   \"resolutions\": [    {     \"width\": 424,     \"height\": 240    },    {     \"width\": 640,     \"height\": 360    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 848,     \"height\": 480    },    {     \"width\": 960,     \"height\": 540    },    {     \"width\": 1280,     \"height\": 720    }   ]  },  {   \"devicePrefix\": \"L\",   \"resolutions\": [    {     \"width\": 1280,     \"height\": 720    },    {     \"width\": 1920,     \"height\": 1080    }   ]  } ]},\"position\": { \"x\": 0.0052760359831154346, \"y\": 0.058778461068868637, \"z\": -0.00064044661121442914},\"orientation\": { \"x\": 5.0150761604309082, \"y\": 82.971817016601562, \"z\": 358.756103515625},\"showPointcloud\": false,\"depthImage\": false,\"imu\": false,\"errors\": []},{\"inputParameters\": [],\"outputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"\" }, {  \"name\": \"ITEMS\",  \"dataType\": 3,  \"key\": \"\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"\" }],\"id\": \"img2\",\"active\": true,\"render\": true,\"ordinal\": 3,\"pipeline\": 1,\"type\": \"ImageSource\",\"moduleState\": 0,\"stateText\": \"\",\"flipImage\": false,\"undistort\": false,\"contourThickness\": 1,\"path\": \"/home/kcarlson/Documents/test/slideshow\",\"displayTimeSeconds\": 5,\"intrinsicsConfigName\": \"\",\"position\": { \"x\": 0, \"y\": 0, \"z\": 0},\"orientation\": { \"x\": 0, \"y\": 0, \"z\": 0},\"itemProducerOptions\": { \"graphicType\": 0, \"showPointCloud\": false, \"surface2PolygonMeshOpts\": {  \"searchRadius\": 0.02500000037252903,  \"mu\": 2.5,  \"maximumNearestNeighbors\": 100,  \"maximumSurfaceAngle\": 45,  \"minimumAngle\": 10,  \"maximumAngle\": 120,  \"normalConsistency\": false,  \"consistentVertexOrdering\": true,  \"kSearch\": 20 }},\"errors\": []},{\"inputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"rs1/RGBA_IMAGE\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"rs1/POINTCLOUD\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"rs1/CAMERA\" }],\"outputParameters\": [ {  \"name\": \"CONTOURS\",  \"dataType\": 2,  \"key\": \"\" }, {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"ITEMS\",  \"dataType\": 3,  \"key\": \"\" }, {  \"name\": \"BLOB_COUNT\",  \"dataType\": 7,  \"key\": \"\" }],\"id\": \"blob1\",\"active\": true,\"render\": true,\"ordinal\": 4,\"pipeline\": 0,\"type\": \"Blob\",\"moduleState\": 0,\"stateText\": \"\",\"value0UpperBound\": 255,\"value0LowerBound\": 0,\"value1UpperBound\": 186,\"value1LowerBound\": 162,\"value2UpperBound\": 178,\"value2LowerBound\": 154,\"showRect\": false,\"rectColor\": { \"r\": 0, \"g\": 1, \"b\": 1, \"a\": 1},\"contourColor\": { \"r\": 0, \"g\": 0, \"b\": 1, \"a\": 1},\"contourThickness\": 1,\"trackerType\": 0,\"retrievalMode\": 0,\"colorPaletteType\": 0,\"invertMask\": false,\"dilateCount\": 0,\"blurAndReduceEnabled\": true,\"watershedEnabled\": false,\"erodeCount\": 0,\"erodeFirst\": false,\"minWidth\": 0,\"maxWidth\": 1,\"minHeight\": 0,\"maxHeight\": 1,\"kMeansCount\": 0,\"angleAnalysis\": 1,\"regionOfInterest\": { \"x\": 0, \"y\": 0, \"width\": 0, \"height\": 0},\"inferenceOnRoiImage\": false,\"extremePointsAnalysis\": 0,\"extremePointsDistanceFromCenterPointPercent\": 1,\"extremePointsFixedDistance\": 0,\"showRejected\": false,\"showRoi\": true,\"pointCloudFilters\": { \"holeFillingEnabled\": false, \"holeFillingResolution\": 1, \"holeFillingPasses\": 1},\"itemProducerOptions\": { \"graphicType\": 0, \"showPointCloud\": false, \"surface2PolygonMeshOpts\": {  \"searchRadius\": 0.02500000037252903,  \"mu\": 2.5,  \"maximumNearestNeighbors\": 100,  \"maximumSurfaceAngle\": 45,  \"minimumAngle\": 10,  \"maximumAngle\": 120,  \"normalConsistency\": false,  \"consistentVertexOrdering\": true,  \"kSearch\": 20 }},\"errors\": []}]}\"f\n\x13\x43reateModuleRequest\x12(\n\x07modules\x18\x01 \x03(\x0b\x32\x17.google.protobuf.Struct\x12%\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x15.ocellus.GlobalConfig\"O\n\x16GetModulesResponseV1_1\x12\x35\n\x07modules\x18\x01 \x03(\x0b\x32$.ocellus.api.v1.module.config.Module\"w\n\x17\x43reateModuleRequestV1_1\x12\x35\n\x07modules\x18\x01 \x03(\x0b\x32$.ocellus.api.v1.module.config.Module\x12%\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x15.ocellus.GlobalConfig\"\xa0\x02\n\x12PatchModuleRequest\x12\x11\n\tmodule_id\x18\x01 \x01(\t\x12L\n\noperations\x18\x02 \x03(\x0b\x32\x38.ocellus.api.v1.module.info.PatchModuleRequest.Operation\x1a\x34\n\tOperation\x12\n\n\x02op\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t:s\x92\x41p*#\n\nJSON Patch\x12\x15http://jsonpatch.com/2I\x12G{ \"operations\": [{ \"op\": \"replace\", \"path\": \"/baz\", \"value\": \"boo\" }] }\"\x92\x02\n\x16PatchModuleRequestV1_1\x12\x11\n\tmodule_id\x18\x01 \x01(\t\x12\x34\n\x06module\x18\x02 \x01(\x0b\x32$.ocellus.api.v1.module.config.Module\x12.\n\nfield_mask\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.FieldMask:\x7f\x92\x41|2z\x12x{ \"module\": { \"real_sense\": { \"playback_file\": \"/data/playback_file.bag\" } }, \"field_mask\": \"real_sense.playback_file\" }\"O\n\x13\x44\x65leteModuleRequest\x12\x38\n\tmodule_id\x18\x01 \x01(\tB%\x92\x41\"2\x14The module to delete\xd2\x01\tmodule_id\"\'\n\x18UpdateModuleOrderRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"x\n\x17ModuleApiHandlerRequest\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x12\n\npath_param\x18\x03 \x01(\t\x12%\n\x04\x62ody\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xe7\x01\n\x18GetRemoteModulesResponse\x12V\n\x07modules\x18\x01 \x03(\x0b\x32\x45.ocellus.api.v1.module.info.GetRemoteModulesResponse.RemoteModuleInfo\x1as\n\x10RemoteModuleInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1f\n\x06inputs\x18\x02 \x03(\x0b\x32\x0f.ocellus.IOData\x12 \n\x07outputs\x18\x03 \x03(\x0b\x32\x0f.ocellus.IOData\x12\x0e\n\x06states\x18\x04 \x03(\t2\x87\x1a\n\x18OcellusModuleInfoService\x12\x94\x01\n\rReloadModules\x12\x16.google.protobuf.Empty\x1a..ocellus.api.v1.module.info.GetModulesResponse\";\x88\x02\x01\x92\x41\x17\x1a\x15Use ReloadModulesV1_1\x82\xd3\xe4\x93\x02\x18\x1a\x16/api/v1/modules/reload\x12\x9b\x01\n\x13UpdateModulesConfig\x12\x15.ocellus.GlobalConfig\x1a\x16.google.protobuf.Empty\"U\x92\x41\x34\x1a\x32Updates the global configuration, does not persist\x82\xd3\xe4\x93\x02\x18\x1a\x16/api/v1/modules/config\x12\x90\x01\n\x10GetModulesConfig\x12\x16.google.protobuf.Empty\x1a\x15.ocellus.GlobalConfig\"M\x92\x41,\x1a*Retreives the current global configuration\x82\xd3\xe4\x93\x02\x18\x12\x16/api/v1/modules/config\x12\xbb\x01\n\nGetModules\x12-.ocellus.api.v1.module.info.GetModulesRequest\x1a..ocellus.api.v1.module.info.GetModulesResponse\"N\x88\x02\x01\x92\x41\x14\x1a\x12Use GetModulesV1_1\x82\xd3\xe4\x93\x02.\x12\x1a/api/v1/module/{module_id}Z\x10\x12\x0e/api/v1/module\x12\xa3\x01\n\x0c\x43reateModule\x12/.ocellus.api.v1.module.info.CreateModuleRequest\x1a..ocellus.api.v1.module.info.GetModulesResponse\"2\x88\x02\x01\x92\x41\x16\x1a\x14Use CreateModuleV1_1\x82\xd3\xe4\x93\x02\x10\"\x0e/api/v1/module\x12t\n\x0cUpdateModule\x12\x17.google.protobuf.Struct\x1a\x17.google.protobuf.Struct\"2\x88\x02\x01\x92\x41\x16\x1a\x14Use UpdateModuleV1_1\x82\xd3\xe4\x93\x02\x10\x1a\x0e/api/v1/module\x12\x98\x01\n\x0bPatchModule\x12..ocellus.api.v1.module.info.PatchModuleRequest\x1a\x17.google.protobuf.Struct\"@\x88\x02\x01\x92\x41\x15\x1a\x13Use PatchModuleV1_1\x82\xd3\xe4\x93\x02\x1f\x32\x1a/api/v1/module/{module_id}:\x01*\x12\xf1\x01\n\x0eGetModulesV1_1\x12-.ocellus.api.v1.module.info.GetModulesRequest\x1a\x32.ocellus.api.v1.module.info.GetModulesResponseV1_1\"|\x92\x41\x41\x1a?Returns all or the specified module\'s configuration information\x82\xd3\xe4\x93\x02\x32\x12\x1c/api/v1_1/module/{module_id}Z\x12\x12\x10/api/v1_1/module\x12\xc0\x01\n\x10\x43reateModuleV1_1\x12\x33.ocellus.api.v1.module.info.CreateModuleRequestV1_1\x1a\x32.ocellus.api.v1.module.info.GetModulesResponseV1_1\"C\x92\x41(\x1a&Creates a new module, does not persist\x82\xd3\xe4\x93\x02\x12\"\x10/api/v1_1/module\x12\xc6\x01\n\x10UpdateModuleV1_1\x12\x33.ocellus.api.v1.module.info.CreateModuleRequestV1_1\x1a\x32.ocellus.api.v1.module.info.GetModulesResponseV1_1\"I\x92\x41.\x1a,Updates an existing module, does not persist\x82\xd3\xe4\x93\x02\x12\x1a\x10/api/v1_1/module\x12\xa2\x01\n\x0fPatchModuleV1_1\x12\x32.ocellus.api.v1.module.info.PatchModuleRequestV1_1\x1a\x32.ocellus.api.v1.module.info.GetModulesResponseV1_1\"\'\x82\xd3\xe4\x93\x02!2\x1c/api/v1_1/module/{module_id}:\x01*\x12\xba\x01\n\x11ReloadModulesV1_1\x12\x16.google.protobuf.Empty\x1a\x32.ocellus.api.v1.module.info.GetModulesResponseV1_1\"Y\x92\x41\x36\x1a\x34Will reload all modules from the configuration file.\x82\xd3\xe4\x93\x02\x1a\x1a\x18/api/v1_1/modules/reload\x12\xcc\x01\n\x0c\x44\x65leteModule\x12/.ocellus.api.v1.module.info.DeleteModuleRequest\x1a\x16.google.protobuf.Empty\"s\x92\x41<\x1a:Deletes a specific or all loaded modules, does not persist\x82\xd3\xe4\x93\x02.*\x1a/api/v1/module/{module_id}Z\x10*\x0e/api/v1/module\x12\xb8\x01\n\x11UpdateModuleOrder\x12\x34.ocellus.api.v1.module.info.UpdateModuleOrderRequest\x1a\x16.google.protobuf.Empty\"U\x92\x41\x36\x1a\x34\x43hanges the module execution order, does not persist\x82\xd3\xe4\x93\x02\x16\x1a\x14/api/v1/order/module\x12\xca\x02\n\x10ModuleApiHandler\x12\x33.ocellus.api.v1.module.info.ModuleApiHandlerRequest\x1a\x17.google.protobuf.Struct\"\xe7\x01\x92\x41\x17\x1a\x15Module specific APIs.\x82\xd3\xe4\x93\x02\xc6\x01\x12./api/{version}/module/{module_id}/{path_param}Z0*./api/{version}/module/{module_id}/{path_param}Z0\"./api/{version}/module/{module_id}/{path_param}Z0\x1a./api/{version}/module/{module_id}/{path_param}\x12\xed\x01\n\x10GetRemoteModules\x12\x16.google.protobuf.Empty\x1a\x34.ocellus.api.v1.module.info.GetRemoteModulesResponse\"\x8a\x01\x92\x41i\x1agReturns all the currently available remote modules connected using the ocellus.OcellusModuleService API\x82\xd3\xe4\x93\x02\x18\x12\x16/api/v1/modules/remote\x12\xa0\x01\n\x12OnModuleInfoUpdate\x12-.ocellus.api.v1.module.info.GetModulesRequest\x1a\x32.ocellus.api.v1.module.info.GetModulesResponseV1_1\"%\x92\x41\"\x1a Subsrcibe to module info updates0\x01\x1a\x62\x92\x41_\x12]Service for interacting with the user configuration, module metadata, and module interactionsB\x81\x01\n\x1e\x63om.ocellus.api.v1.module.infoB\x18OcellusModuleInfoServiceP\x01Z\x1egithub.com/byte-motion/ocellus\xa2\x02\x05OAPMD\xaa\x02\x1aOcellus.Api.V1.Module.Infob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,api/v1/ocellus_api_module_info_service.proto\x12\x1aocellus.api.v1.module.info\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cocellus_module_service.proto\x1a\x13ocellus_types.proto\x1a,protoc-gen-swagger/options/annotations.proto\"%\n\x11GetModulesRequest\x12\x10\n\x08moduleId\x18\x01 \x01(\t\"\xe4O\n\x12GetModulesResponse\x12(\n\x07modules\x18\x01 \x03(\x0b\x32\x17.google.protobuf.Struct:\xa3O\x92\x41\x9fO2\x9cO\x12\x99O{\"modules\": [{\"inputParameters\": [],\"outputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"\" }],\"id\": \"rs1\",\"active\": true,\"render\": true,\"ordinal\": 0,\"pipeline\": 0,\"type\": \"RealSense\",\"moduleState\": 1,\"stateText\": \"\",\"rsCamera\": { \"processingBlocks\": {  \"alignEnabled\": true,  \"alignTo\": 2,  \"decimationFilterEnabled\": true,  \"streamFilter\": 1,  \"formatFilter\": 1,  \"filterMagnitude\": 8,  \"thresholdFilterEnabled\": false,  \"thresholdMaxDistance\": 1.5,  \"thresholdMinDistance\": 0,  \"disparityMode02\": 0,  \"spatialFilterEnabled\": false,  \"spatialMagnitude\": 1,  \"spatialSmoothAlpha\": 0.72000002861022949,  \"spatialSmoothDelta\": 9,  \"holeFillingMode\": 0,  \"temporalFilterEnabled\": false,  \"temporalSmoothAlpha\": 0.079999998211860657,  \"temporalSmoothDelta\": 100,  \"temporalPersistance\": 6,  \"holeFillingFilterEnabled\": false,  \"holesFill\": 2,  \"colorizerEnabled\": true,  \"visualPreset\": 0,  \"colorScheme\": 5,  \"histogramEqualization\": true,  \"colorizerMinDistance\": 0,  \"colorizerMaxDistance\": 6,  \"pointCloudEnabled\": true,  \"occlusionRemoval\": 2,  \"textureStream\": 1,  \"textureFormat\": 5 }, \"cameraInfo\": {  \"name\": \"\",  \"serialNumber\": \"\",  \"firmwareVersion\": \"\",  \"recommendedFirmwareVersion\": \"\",  \"physicalPort\": \"\",  \"debugOpCode\": \"\",  \"advancedMode\": \"\",  \"productId\": \"\",  \"cameraLocked\": \"\",  \"usbTypeDescriptor\": \"\" }, \"depthResolution\": {  \"width\": 0,  \"height\": 0 }, \"colorResolution\": {  \"width\": 0,  \"height\": 0 }, \"depthFps\": 2, \"colorFps\": 2, \"serialNumber\": \"\", \"mode\": 1, \"playbackFile\": \"/home/kcarlson/Documents/test/longredtape.bag\", \"availableFps\": [  6,  15,  30,  60 ], \"availableDepthResolutions\": [  {   \"devicePrefix\": \"D\",   \"resolutions\": [    {     \"width\": 424,     \"height\": 240    },    {     \"width\": 640,     \"height\": 360    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 848,     \"height\": 100    },    {     \"width\": 848,     \"height\": 480    },    {     \"width\": 1280,     \"height\": 720    }   ]  },  {   \"devicePrefix\": \"L\",   \"resolutions\": [    {     \"width\": 240,     \"height\": 640    },    {     \"width\": 384,     \"height\": 1024    },    {     \"width\": 480,     \"height\": 640    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 768,     \"height\": 1024    },    {     \"width\": 1024,     \"height\": 768    }   ]  } ], \"availableColorResolutions\": [  {   \"devicePrefix\": \"D\",   \"resolutions\": [    {     \"width\": 424,     \"height\": 240    },    {     \"width\": 640,     \"height\": 360    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 848,     \"height\": 480    },    {     \"width\": 960,     \"height\": 540    },    {     \"width\": 1280,     \"height\": 720    }   ]  },  {   \"devicePrefix\": \"L\",   \"resolutions\": [    {     \"width\": 1280,     \"height\": 720    },    {     \"width\": 1920,     \"height\": 1080    }   ]  } ]},\"position\": { \"x\": 0.0052760359831154346, \"y\": 0.058778461068868637, \"z\": -0.00064044661121442914},\"orientation\": { \"x\": 5.0150761604309082, \"y\": 82.971817016601562, \"z\": 358.756103515625},\"showPointcloud\": false,\"depthImage\": false,\"imu\": false,\"errors\": []},{\"inputParameters\": [],\"outputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"\" }, {  \"name\": \"ITEMS\",  \"dataType\": 3,  \"key\": \"\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"\" }],\"id\": \"img\",\"active\": true,\"render\": true,\"ordinal\": 1,\"pipeline\": 0,\"type\": \"ImageSource\",\"moduleState\": 0,\"stateText\": \"\",\"flipImage\": false,\"undistort\": false,\"contourThickness\": 1,\"path\": \"/home/kcarlson/Documents/test/slideshow\",\"displayTimeSeconds\": 5,\"intrinsicsConfigName\": \"\",\"position\": { \"x\": 0, \"y\": 0, \"z\": 0},\"orientation\": { \"x\": 0, \"y\": 0, \"z\": 0},\"itemProducerOptions\": { \"graphicType\": 0, \"showPointCloud\": false, \"surface2PolygonMeshOpts\": {  \"searchRadius\": 0.02500000037252903,  \"mu\": 2.5,  \"maximumNearestNeighbors\": 100,  \"maximumSurfaceAngle\": 45,  \"minimumAngle\": 10,  \"maximumAngle\": 120,  \"normalConsistency\": false,  \"consistentVertexOrdering\": true,  \"kSearch\": 20 }},\"errors\": []},{\"inputParameters\": [],\"outputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"\" }],\"id\": \"rs2\",\"active\": true,\"render\": true,\"ordinal\": 2,\"pipeline\": 1,\"type\": \"RealSense\",\"moduleState\": 1,\"stateText\": \"\",\"rsCamera\": { \"processingBlocks\": {  \"alignEnabled\": true,  \"alignTo\": 2,  \"decimationFilterEnabled\": true,  \"streamFilter\": 1,  \"formatFilter\": 1,  \"filterMagnitude\": 8,  \"thresholdFilterEnabled\": false,  \"thresholdMaxDistance\": 1.5,  \"thresholdMinDistance\": 0,  \"disparityMode02\": 0,  \"spatialFilterEnabled\": false,  \"spatialMagnitude\": 1,  \"spatialSmoothAlpha\": 0.72000002861022949,  \"spatialSmoothDelta\": 9,  \"holeFillingMode\": 0,  \"temporalFilterEnabled\": false,  \"temporalSmoothAlpha\": 0.079999998211860657,  \"temporalSmoothDelta\": 100,  \"temporalPersistance\": 6,  \"holeFillingFilterEnabled\": false,  \"holesFill\": 2,  \"colorizerEnabled\": true,  \"visualPreset\": 0,  \"colorScheme\": 5,  \"histogramEqualization\": true,  \"colorizerMinDistance\": 0,  \"colorizerMaxDistance\": 6,  \"pointCloudEnabled\": true,  \"occlusionRemoval\": 2,  \"textureStream\": 1,  \"textureFormat\": 5 }, \"cameraInfo\": {  \"name\": \"\",  \"serialNumber\": \"\",  \"firmwareVersion\": \"\",  \"recommendedFirmwareVersion\": \"\",  \"physicalPort\": \"\",  \"debugOpCode\": \"\",  \"advancedMode\": \"\",  \"productId\": \"\",  \"cameraLocked\": \"\",  \"usbTypeDescriptor\": \"\" }, \"depthResolution\": {  \"width\": 0,  \"height\": 0 }, \"colorResolution\": {  \"width\": 0,  \"height\": 0 }, \"depthFps\": 2, \"colorFps\": 2, \"serialNumber\": \"\", \"mode\": 1, \"playbackFile\": \"/home/kcarlson/Documents/test/longredtape.bag\", \"availableFps\": [  6,  15,  30,  60 ], \"availableDepthResolutions\": [  {   \"devicePrefix\": \"D\",   \"resolutions\": [    {     \"width\": 424,     \"height\": 240    },    {     \"width\": 640,     \"height\": 360    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 848,     \"height\": 100    },    {     \"width\": 848,     \"height\": 480    },    {     \"width\": 1280,     \"height\": 720    }   ]  },  {   \"devicePrefix\": \"L\",   \"resolutions\": [    {     \"width\": 240,     \"height\": 640    },    {     \"width\": 384,     \"height\": 1024    },    {     \"width\": 480,     \"height\": 640    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 768,     \"height\": 1024    },    {     \"width\": 1024,     \"height\": 768    }   ]  } ], \"availableColorResolutions\": [  {   \"devicePrefix\": \"D\",   \"resolutions\": [    {     \"width\": 424,     \"height\": 240    },    {     \"width\": 640,     \"height\": 360    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 848,     \"height\": 480    },    {     \"width\": 960,     \"height\": 540    },    {     \"width\": 1280,     \"height\": 720    }   ]  },  {   \"devicePrefix\": \"L\",   \"resolutions\": [    {     \"width\": 1280,     \"height\": 720    },    {     \"width\": 1920,     \"height\": 1080    }   ]  } ]},\"position\": { \"x\": 0.0052760359831154346, \"y\": 0.058778461068868637, \"z\": -0.00064044661121442914},\"orientation\": { \"x\": 5.0150761604309082, \"y\": 82.971817016601562, \"z\": 358.756103515625},\"showPointcloud\": false,\"depthImage\": false,\"imu\": false,\"errors\": []},{\"inputParameters\": [],\"outputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"\" }, {  \"name\": \"ITEMS\",  \"dataType\": 3,  \"key\": \"\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"\" }],\"id\": \"img2\",\"active\": true,\"render\": true,\"ordinal\": 3,\"pipeline\": 1,\"type\": \"ImageSource\",\"moduleState\": 0,\"stateText\": \"\",\"flipImage\": false,\"undistort\": false,\"contourThickness\": 1,\"path\": \"/home/kcarlson/Documents/test/slideshow\",\"displayTimeSeconds\": 5,\"intrinsicsConfigName\": \"\",\"position\": { \"x\": 0, \"y\": 0, \"z\": 0},\"orientation\": { \"x\": 0, \"y\": 0, \"z\": 0},\"itemProducerOptions\": { \"graphicType\": 0, \"showPointCloud\": false, \"surface2PolygonMeshOpts\": {  \"searchRadius\": 0.02500000037252903,  \"mu\": 2.5,  \"maximumNearestNeighbors\": 100,  \"maximumSurfaceAngle\": 45,  \"minimumAngle\": 10,  \"maximumAngle\": 120,  \"normalConsistency\": false,  \"consistentVertexOrdering\": true,  \"kSearch\": 20 }},\"errors\": []},{\"inputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"rs1/RGBA_IMAGE\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"rs1/POINTCLOUD\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"rs1/CAMERA\" }],\"outputParameters\": [ {  \"name\": \"CONTOURS\",  \"dataType\": 2,  \"key\": \"\" }, {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"ITEMS\",  \"dataType\": 3,  \"key\": \"\" }, {  \"name\": \"BLOB_COUNT\",  \"dataType\": 7,  \"key\": \"\" }],\"id\": \"blob1\",\"active\": true,\"render\": true,\"ordinal\": 4,\"pipeline\": 0,\"type\": \"Blob\",\"moduleState\": 0,\"stateText\": \"\",\"value0UpperBound\": 255,\"value0LowerBound\": 0,\"value1UpperBound\": 186,\"value1LowerBound\": 162,\"value2UpperBound\": 178,\"value2LowerBound\": 154,\"showRect\": false,\"rectColor\": { \"r\": 0, \"g\": 1, \"b\": 1, \"a\": 1},\"contourColor\": { \"r\": 0, \"g\": 0, \"b\": 1, \"a\": 1},\"contourThickness\": 1,\"trackerType\": 0,\"retrievalMode\": 0,\"colorPaletteType\": 0,\"invertMask\": false,\"dilateCount\": 0,\"blurAndReduceEnabled\": true,\"watershedEnabled\": false,\"erodeCount\": 0,\"erodeFirst\": false,\"minWidth\": 0,\"maxWidth\": 1,\"minHeight\": 0,\"maxHeight\": 1,\"kMeansCount\": 0,\"angleAnalysis\": 1,\"regionOfInterest\": { \"x\": 0, \"y\": 0, \"width\": 0, \"height\": 0},\"inferenceOnRoiImage\": false,\"extremePointsAnalysis\": 0,\"extremePointsDistanceFromCenterPoint\": 1,\"extremePointsFixedDistance\": 0,\"showRejected\": false,\"showRoi\": true,\"pointCloudFilters\": { \"holeFillingEnabled\": false, \"holeFillingResolution\": 1, \"holeFillingPasses\": 1},\"itemProducerOptions\": { \"graphicType\": 0, \"showPointCloud\": false, \"surface2PolygonMeshOpts\": {  \"searchRadius\": 0.02500000037252903,  \"mu\": 2.5,  \"maximumNearestNeighbors\": 100,  \"maximumSurfaceAngle\": 45,  \"minimumAngle\": 10,  \"maximumAngle\": 120,  \"normalConsistency\": false,  \"consistentVertexOrdering\": true,  \"kSearch\": 20 }},\"errors\": []}]}\"f\n\x13\x43reateModuleRequest\x12(\n\x07modules\x18\x01 \x03(\x0b\x32\x17.google.protobuf.Struct\x12%\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x15.ocellus.GlobalConfig\"\x9f\x02\n\x12PatchModuleRequest\x12\x10\n\x08moduleId\x18\x01 \x01(\t\x12L\n\noperations\x18\x02 \x03(\x0b\x32\x38.ocellus.api.v1.module.info.PatchModuleRequest.Operation\x1a\x34\n\tOperation\x12\n\n\x02op\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t:s\x92\x41p*#\n\nJSON Patch\x12\x15http://jsonpatch.com/2I\x12G{ \"operations\": [{ \"op\": \"replace\", \"path\": \"/baz\", \"value\": \"boo\" }] }\"M\n\x13\x44\x65leteModuleRequest\x12\x36\n\x08moduleId\x18\x01 \x01(\tB$\x92\x41!2\x14The module to delete\xd2\x01\x08moduleId\"\'\n\x18UpdateModuleOrderRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"v\n\x17ModuleApiHandlerRequest\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x10\n\x08moduleId\x18\x02 \x01(\t\x12\x11\n\tpathParam\x18\x03 \x01(\t\x12%\n\x04\x62ody\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xe7\x01\n\x18GetRemoteModulesResponse\x12V\n\x07modules\x18\x01 \x03(\x0b\x32\x45.ocellus.api.v1.module.info.GetRemoteModulesResponse.RemoteModuleInfo\x1as\n\x10RemoteModuleInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1f\n\x06inputs\x18\x02 \x03(\x0b\x32\x0f.ocellus.IOData\x12 \n\x07outputs\x18\x03 \x03(\x0b\x32\x0f.ocellus.IOData\x12\x0e\n\x06states\x18\x04 \x03(\t2\xfa\x12\n\x18OcellusModuleInfoService\x12\xb0\x01\n\rReloadModules\x12\x16.google.protobuf.Empty\x1a..ocellus.api.v1.module.info.GetModulesResponse\"W\x92\x41\x36\x1a\x34Will reload all modules from the configuration file.\x82\xd3\xe4\x93\x02\x18\x1a\x16/api/v1/modules/reload\x12\x9b\x01\n\x13UpdateModulesConfig\x12\x15.ocellus.GlobalConfig\x1a\x16.google.protobuf.Empty\"U\x92\x41\x34\x1a\x32Updates the global configuration, does not persist\x82\xd3\xe4\x93\x02\x18\x1a\x16/api/v1/modules/config\x12\x90\x01\n\x10GetModulesConfig\x12\x16.google.protobuf.Empty\x1a\x15.ocellus.GlobalConfig\"M\x92\x41,\x1a*Retreives the current global configuration\x82\xd3\xe4\x93\x02\x18\x12\x16/api/v1/modules/config\x12\xe4\x01\n\nGetModules\x12-.ocellus.api.v1.module.info.GetModulesRequest\x1a..ocellus.api.v1.module.info.GetModulesResponse\"w\x92\x41\x41\x1a?Returns all or the specified module\'s configuration information\x82\xd3\xe4\x93\x02-\x12\x19/api/v1/module/{moduleId}Z\x10\x12\x0e/api/v1/module\x12\xb2\x01\n\x0c\x43reateModule\x12/.ocellus.api.v1.module.info.CreateModuleRequest\x1a..ocellus.api.v1.module.info.GetModulesResponse\"A\x92\x41(\x1a&Creates a new module, does not persist\x82\xd3\xe4\x93\x02\x10\"\x0e/api/v1/module\x12\x89\x01\n\x0cUpdateModule\x12\x17.google.protobuf.Struct\x1a\x17.google.protobuf.Struct\"G\x92\x41.\x1a,Updates an existing module, does not persist\x82\xd3\xe4\x93\x02\x10\x1a\x0e/api/v1/module\x12\xaf\x02\n\x0bPatchModule\x12..ocellus.api.v1.module.info.PatchModuleRequest\x1a\x17.google.protobuf.Struct\"\xd6\x01\x92\x41\xae\x01\x1a\xab\x01Updates a specific field of an existing module, does not persist\nReplaces module fields with ops using jsonpatch. Only replace is supported\nReturns the updated module data\x82\xd3\xe4\x93\x02\x1e\x32\x19/api/v1/module/{moduleId}:\x01*\x12\xcb\x01\n\x0c\x44\x65leteModule\x12/.ocellus.api.v1.module.info.DeleteModuleRequest\x1a\x16.google.protobuf.Empty\"r\x92\x41<\x1a:Deletes a specific or all loaded modules, does not persist\x82\xd3\xe4\x93\x02-*\x19/api/v1/module/{moduleId}Z\x10*\x0e/api/v1/module\x12\xb8\x01\n\x11UpdateModuleOrder\x12\x34.ocellus.api.v1.module.info.UpdateModuleOrderRequest\x1a\x16.google.protobuf.Empty\"U\x92\x41\x36\x1a\x34\x43hanges the module execution order, does not persist\x82\xd3\xe4\x93\x02\x16\x1a\x14/api/v1/order/module\x12\xc2\x02\n\x10ModuleApiHandler\x12\x33.ocellus.api.v1.module.info.ModuleApiHandlerRequest\x1a\x17.google.protobuf.Struct\"\xdf\x01\x92\x41\x17\x1a\x15Module specific APIs.\x82\xd3\xe4\x93\x02\xbe\x01\x12,/api/{version}/module/{moduleId}/{pathParam}Z.*,/api/{version}/module/{moduleId}/{pathParam}Z.\",/api/{version}/module/{moduleId}/{pathParam}Z.\x1a,/api/{version}/module/{moduleId}/{pathParam}\x12\xed\x01\n\x10GetRemoteModules\x12\x16.google.protobuf.Empty\x1a\x34.ocellus.api.v1.module.info.GetRemoteModulesResponse\"\x8a\x01\x92\x41i\x1agReturns all the currently available remote modules connected using the ocellus.OcellusModuleService API\x82\xd3\xe4\x93\x02\x18\x12\x16/api/v1/modules/remote\x1a\x62\x92\x41_\x12]Service for interacting with the user configuration, module metadata, and module interactionsB\x81\x01\n\x1e\x63om.ocellus.api.v1.module.infoB\x18OcellusModuleInfoServiceP\x01Z\x1egithub.com/byte-motion/ocellus\xa2\x02\x05OAPMD\xaa\x02\x1aOcellus.Api.V1.Module.Infob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api.v1.ocellus_api_module_info_service_pb2', globals())
+
+
+_GETMODULESREQUEST = DESCRIPTOR.message_types_by_name['GetModulesRequest']
+_GETMODULESRESPONSE = DESCRIPTOR.message_types_by_name['GetModulesResponse']
+_CREATEMODULEREQUEST = DESCRIPTOR.message_types_by_name['CreateModuleRequest']
+_PATCHMODULEREQUEST = DESCRIPTOR.message_types_by_name['PatchModuleRequest']
+_PATCHMODULEREQUEST_OPERATION = _PATCHMODULEREQUEST.nested_types_by_name['Operation']
+_DELETEMODULEREQUEST = DESCRIPTOR.message_types_by_name['DeleteModuleRequest']
+_UPDATEMODULEORDERREQUEST = DESCRIPTOR.message_types_by_name['UpdateModuleOrderRequest']
+_MODULEAPIHANDLERREQUEST = DESCRIPTOR.message_types_by_name['ModuleApiHandlerRequest']
+_GETREMOTEMODULESRESPONSE = DESCRIPTOR.message_types_by_name['GetRemoteModulesResponse']
+_GETREMOTEMODULESRESPONSE_REMOTEMODULEINFO = _GETREMOTEMODULESRESPONSE.nested_types_by_name['RemoteModuleInfo']
+GetModulesRequest = _reflection.GeneratedProtocolMessageType('GetModulesRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETMODULESREQUEST,
+  '__module__' : 'api.v1.ocellus_api_module_info_service_pb2'
+  # @@protoc_insertion_point(class_scope:ocellus.api.v1.module.info.GetModulesRequest)
+  })
+_sym_db.RegisterMessage(GetModulesRequest)
+
+GetModulesResponse = _reflection.GeneratedProtocolMessageType('GetModulesResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETMODULESRESPONSE,
+  '__module__' : 'api.v1.ocellus_api_module_info_service_pb2'
+  # @@protoc_insertion_point(class_scope:ocellus.api.v1.module.info.GetModulesResponse)
+  })
+_sym_db.RegisterMessage(GetModulesResponse)
+
+CreateModuleRequest = _reflection.GeneratedProtocolMessageType('CreateModuleRequest', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEMODULEREQUEST,
+  '__module__' : 'api.v1.ocellus_api_module_info_service_pb2'
+  # @@protoc_insertion_point(class_scope:ocellus.api.v1.module.info.CreateModuleRequest)
+  })
+_sym_db.RegisterMessage(CreateModuleRequest)
+
+PatchModuleRequest = _reflection.GeneratedProtocolMessageType('PatchModuleRequest', (_message.Message,), {
+
+  'Operation' : _reflection.GeneratedProtocolMessageType('Operation', (_message.Message,), {
+    'DESCRIPTOR' : _PATCHMODULEREQUEST_OPERATION,
+    '__module__' : 'api.v1.ocellus_api_module_info_service_pb2'
+    # @@protoc_insertion_point(class_scope:ocellus.api.v1.module.info.PatchModuleRequest.Operation)
+    })
+  ,
+  'DESCRIPTOR' : _PATCHMODULEREQUEST,
+  '__module__' : 'api.v1.ocellus_api_module_info_service_pb2'
+  # @@protoc_insertion_point(class_scope:ocellus.api.v1.module.info.PatchModuleRequest)
+  })
+_sym_db.RegisterMessage(PatchModuleRequest)
+_sym_db.RegisterMessage(PatchModuleRequest.Operation)
+
+DeleteModuleRequest = _reflection.GeneratedProtocolMessageType('DeleteModuleRequest', (_message.Message,), {
+  'DESCRIPTOR' : _DELETEMODULEREQUEST,
+  '__module__' : 'api.v1.ocellus_api_module_info_service_pb2'
+  # @@protoc_insertion_point(class_scope:ocellus.api.v1.module.info.DeleteModuleRequest)
+  })
+_sym_db.RegisterMessage(DeleteModuleRequest)
+
+UpdateModuleOrderRequest = _reflection.GeneratedProtocolMessageType('UpdateModuleOrderRequest', (_message.Message,), {
+  'DESCRIPTOR' : _UPDATEMODULEORDERREQUEST,
+  '__module__' : 'api.v1.ocellus_api_module_info_service_pb2'
+  # @@protoc_insertion_point(class_scope:ocellus.api.v1.module.info.UpdateModuleOrderRequest)
+  })
+_sym_db.RegisterMessage(UpdateModuleOrderRequest)
+
+ModuleApiHandlerRequest = _reflection.GeneratedProtocolMessageType('ModuleApiHandlerRequest', (_message.Message,), {
+  'DESCRIPTOR' : _MODULEAPIHANDLERREQUEST,
+  '__module__' : 'api.v1.ocellus_api_module_info_service_pb2'
+  # @@protoc_insertion_point(class_scope:ocellus.api.v1.module.info.ModuleApiHandlerRequest)
+  })
+_sym_db.RegisterMessage(ModuleApiHandlerRequest)
+
+GetRemoteModulesResponse = _reflection.GeneratedProtocolMessageType('GetRemoteModulesResponse', (_message.Message,), {
+
+  'RemoteModuleInfo' : _reflection.GeneratedProtocolMessageType('RemoteModuleInfo', (_message.Message,), {
+    'DESCRIPTOR' : _GETREMOTEMODULESRESPONSE_REMOTEMODULEINFO,
+    '__module__' : 'api.v1.ocellus_api_module_info_service_pb2'
+    # @@protoc_insertion_point(class_scope:ocellus.api.v1.module.info.GetRemoteModulesResponse.RemoteModuleInfo)
+    })
+  ,
+  'DESCRIPTOR' : _GETREMOTEMODULESRESPONSE,
+  '__module__' : 'api.v1.ocellus_api_module_info_service_pb2'
+  # @@protoc_insertion_point(class_scope:ocellus.api.v1.module.info.GetRemoteModulesResponse)
+  })
+_sym_db.RegisterMessage(GetRemoteModulesResponse)
+_sym_db.RegisterMessage(GetRemoteModulesResponse.RemoteModuleInfo)
+
+_OCELLUSMODULEINFOSERVICE = DESCRIPTOR.services_by_name['OcellusModuleInfoService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036com.ocellus.api.v1.module.infoB\030OcellusModuleInfoServiceP\001Z\036github.com/byte-motion/ocellus\242\002\005OAPMD\252\002\032Ocellus.Api.V1.Module.Info'
   _GETMODULESRESPONSE._options = None
-  _GETMODULESRESPONSE._serialized_options = b'\222A\246O2\243O\022\240O{\"modules\": [{\"inputParameters\": [],\"outputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"\" }],\"id\": \"rs1\",\"active\": true,\"render\": true,\"ordinal\": 0,\"pipeline\": 0,\"type\": \"RealSense\",\"moduleState\": 1,\"stateText\": \"\",\"rsCamera\": { \"processingBlocks\": {  \"alignEnabled\": true,  \"alignTo\": 2,  \"decimationFilterEnabled\": true,  \"streamFilter\": 1,  \"formatFilter\": 1,  \"filterMagnitude\": 8,  \"thresholdFilterEnabled\": false,  \"thresholdMaxDistance\": 1.5,  \"thresholdMinDistance\": 0,  \"disparityMode02\": 0,  \"spatialFilterEnabled\": false,  \"spatialMagnitude\": 1,  \"spatialSmoothAlpha\": 0.72000002861022949,  \"spatialSmoothDelta\": 9,  \"holeFillingMode\": 0,  \"temporalFilterEnabled\": false,  \"temporalSmoothAlpha\": 0.079999998211860657,  \"temporalSmoothDelta\": 100,  \"temporalPersistance\": 6,  \"holeFillingFilterEnabled\": false,  \"holesFill\": 2,  \"colorizerEnabled\": true,  \"visualPreset\": 0,  \"colorScheme\": 5,  \"histogramEqualization\": true,  \"colorizerMinDistance\": 0,  \"colorizerMaxDistance\": 6,  \"pointCloudEnabled\": true,  \"occlusionRemoval\": 2,  \"textureStream\": 1,  \"textureFormat\": 5 }, \"cameraInfo\": {  \"name\": \"\",  \"serialNumber\": \"\",  \"firmwareVersion\": \"\",  \"recommendedFirmwareVersion\": \"\",  \"physicalPort\": \"\",  \"debugOpCode\": \"\",  \"advancedMode\": \"\",  \"productId\": \"\",  \"cameraLocked\": \"\",  \"usbTypeDescriptor\": \"\" }, \"depthResolution\": {  \"width\": 0,  \"height\": 0 }, \"colorResolution\": {  \"width\": 0,  \"height\": 0 }, \"depthFps\": 2, \"colorFps\": 2, \"serialNumber\": \"\", \"mode\": 1, \"playbackFile\": \"/home/kcarlson/Documents/test/longredtape.bag\", \"availableFps\": [  6,  15,  30,  60 ], \"availableDepthResolutions\": [  {   \"devicePrefix\": \"D\",   \"resolutions\": [    {     \"width\": 424,     \"height\": 240    },    {     \"width\": 640,     \"height\": 360    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 848,     \"height\": 100    },    {     \"width\": 848,     \"height\": 480    },    {     \"width\": 1280,     \"height\": 720    }   ]  },  {   \"devicePrefix\": \"L\",   \"resolutions\": [    {     \"width\": 240,     \"height\": 640    },    {     \"width\": 384,     \"height\": 1024    },    {     \"width\": 480,     \"height\": 640    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 768,     \"height\": 1024    },    {     \"width\": 1024,     \"height\": 768    }   ]  } ], \"availableColorResolutions\": [  {   \"devicePrefix\": \"D\",   \"resolutions\": [    {     \"width\": 424,     \"height\": 240    },    {     \"width\": 640,     \"height\": 360    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 848,     \"height\": 480    },    {     \"width\": 960,     \"height\": 540    },    {     \"width\": 1280,     \"height\": 720    }   ]  },  {   \"devicePrefix\": \"L\",   \"resolutions\": [    {     \"width\": 1280,     \"height\": 720    },    {     \"width\": 1920,     \"height\": 1080    }   ]  } ]},\"position\": { \"x\": 0.0052760359831154346, \"y\": 0.058778461068868637, \"z\": -0.00064044661121442914},\"orientation\": { \"x\": 5.0150761604309082, \"y\": 82.971817016601562, \"z\": 358.756103515625},\"showPointcloud\": false,\"depthImage\": false,\"imu\": false,\"errors\": []},{\"inputParameters\": [],\"outputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"\" }, {  \"name\": \"ITEMS\",  \"dataType\": 3,  \"key\": \"\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"\" }],\"id\": \"img\",\"active\": true,\"render\": true,\"ordinal\": 1,\"pipeline\": 0,\"type\": \"ImageSource\",\"moduleState\": 0,\"stateText\": \"\",\"flipImage\": false,\"undistort\": false,\"contourThickness\": 1,\"path\": \"/home/kcarlson/Documents/test/slideshow\",\"displayTimeSeconds\": 5,\"intrinsicsConfigName\": \"\",\"position\": { \"x\": 0, \"y\": 0, \"z\": 0},\"orientation\": { \"x\": 0, \"y\": 0, \"z\": 0},\"itemProducerOptions\": { \"graphicType\": 0, \"showPointCloud\": false, \"surface2PolygonMeshOpts\": {  \"searchRadius\": 0.02500000037252903,  \"mu\": 2.5,  \"maximumNearestNeighbors\": 100,  \"maximumSurfaceAngle\": 45,  \"minimumAngle\": 10,  \"maximumAngle\": 120,  \"normalConsistency\": false,  \"consistentVertexOrdering\": true,  \"kSearch\": 20 }},\"errors\": []},{\"inputParameters\": [],\"outputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"\" }],\"id\": \"rs2\",\"active\": true,\"render\": true,\"ordinal\": 2,\"pipeline\": 1,\"type\": \"RealSense\",\"moduleState\": 1,\"stateText\": \"\",\"rsCamera\": { \"processingBlocks\": {  \"alignEnabled\": true,  \"alignTo\": 2,  \"decimationFilterEnabled\": true,  \"streamFilter\": 1,  \"formatFilter\": 1,  \"filterMagnitude\": 8,  \"thresholdFilterEnabled\": false,  \"thresholdMaxDistance\": 1.5,  \"thresholdMinDistance\": 0,  \"disparityMode02\": 0,  \"spatialFilterEnabled\": false,  \"spatialMagnitude\": 1,  \"spatialSmoothAlpha\": 0.72000002861022949,  \"spatialSmoothDelta\": 9,  \"holeFillingMode\": 0,  \"temporalFilterEnabled\": false,  \"temporalSmoothAlpha\": 0.079999998211860657,  \"temporalSmoothDelta\": 100,  \"temporalPersistance\": 6,  \"holeFillingFilterEnabled\": false,  \"holesFill\": 2,  \"colorizerEnabled\": true,  \"visualPreset\": 0,  \"colorScheme\": 5,  \"histogramEqualization\": true,  \"colorizerMinDistance\": 0,  \"colorizerMaxDistance\": 6,  \"pointCloudEnabled\": true,  \"occlusionRemoval\": 2,  \"textureStream\": 1,  \"textureFormat\": 5 }, \"cameraInfo\": {  \"name\": \"\",  \"serialNumber\": \"\",  \"firmwareVersion\": \"\",  \"recommendedFirmwareVersion\": \"\",  \"physicalPort\": \"\",  \"debugOpCode\": \"\",  \"advancedMode\": \"\",  \"productId\": \"\",  \"cameraLocked\": \"\",  \"usbTypeDescriptor\": \"\" }, \"depthResolution\": {  \"width\": 0,  \"height\": 0 }, \"colorResolution\": {  \"width\": 0,  \"height\": 0 }, \"depthFps\": 2, \"colorFps\": 2, \"serialNumber\": \"\", \"mode\": 1, \"playbackFile\": \"/home/kcarlson/Documents/test/longredtape.bag\", \"availableFps\": [  6,  15,  30,  60 ], \"availableDepthResolutions\": [  {   \"devicePrefix\": \"D\",   \"resolutions\": [    {     \"width\": 424,     \"height\": 240    },    {     \"width\": 640,     \"height\": 360    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 848,     \"height\": 100    },    {     \"width\": 848,     \"height\": 480    },    {     \"width\": 1280,     \"height\": 720    }   ]  },  {   \"devicePrefix\": \"L\",   \"resolutions\": [    {     \"width\": 240,     \"height\": 640    },    {     \"width\": 384,     \"height\": 1024    },    {     \"width\": 480,     \"height\": 640    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 768,     \"height\": 1024    },    {     \"width\": 1024,     \"height\": 768    }   ]  } ], \"availableColorResolutions\": [  {   \"devicePrefix\": \"D\",   \"resolutions\": [    {     \"width\": 424,     \"height\": 240    },    {     \"width\": 640,     \"height\": 360    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 848,     \"height\": 480    },    {     \"width\": 960,     \"height\": 540    },    {     \"width\": 1280,     \"height\": 720    }   ]  },  {   \"devicePrefix\": \"L\",   \"resolutions\": [    {     \"width\": 1280,     \"height\": 720    },    {     \"width\": 1920,     \"height\": 1080    }   ]  } ]},\"position\": { \"x\": 0.0052760359831154346, \"y\": 0.058778461068868637, \"z\": -0.00064044661121442914},\"orientation\": { \"x\": 5.0150761604309082, \"y\": 82.971817016601562, \"z\": 358.756103515625},\"showPointcloud\": false,\"depthImage\": false,\"imu\": false,\"errors\": []},{\"inputParameters\": [],\"outputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"\" }, {  \"name\": \"ITEMS\",  \"dataType\": 3,  \"key\": \"\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"\" }],\"id\": \"img2\",\"active\": true,\"render\": true,\"ordinal\": 3,\"pipeline\": 1,\"type\": \"ImageSource\",\"moduleState\": 0,\"stateText\": \"\",\"flipImage\": false,\"undistort\": false,\"contourThickness\": 1,\"path\": \"/home/kcarlson/Documents/test/slideshow\",\"displayTimeSeconds\": 5,\"intrinsicsConfigName\": \"\",\"position\": { \"x\": 0, \"y\": 0, \"z\": 0},\"orientation\": { \"x\": 0, \"y\": 0, \"z\": 0},\"itemProducerOptions\": { \"graphicType\": 0, \"showPointCloud\": false, \"surface2PolygonMeshOpts\": {  \"searchRadius\": 0.02500000037252903,  \"mu\": 2.5,  \"maximumNearestNeighbors\": 100,  \"maximumSurfaceAngle\": 45,  \"minimumAngle\": 10,  \"maximumAngle\": 120,  \"normalConsistency\": false,  \"consistentVertexOrdering\": true,  \"kSearch\": 20 }},\"errors\": []},{\"inputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"rs1/RGBA_IMAGE\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"rs1/POINTCLOUD\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"rs1/CAMERA\" }],\"outputParameters\": [ {  \"name\": \"CONTOURS\",  \"dataType\": 2,  \"key\": \"\" }, {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"ITEMS\",  \"dataType\": 3,  \"key\": \"\" }, {  \"name\": \"BLOB_COUNT\",  \"dataType\": 7,  \"key\": \"\" }],\"id\": \"blob1\",\"active\": true,\"render\": true,\"ordinal\": 4,\"pipeline\": 0,\"type\": \"Blob\",\"moduleState\": 0,\"stateText\": \"\",\"value0UpperBound\": 255,\"value0LowerBound\": 0,\"value1UpperBound\": 186,\"value1LowerBound\": 162,\"value2UpperBound\": 178,\"value2LowerBound\": 154,\"showRect\": false,\"rectColor\": { \"r\": 0, \"g\": 1, \"b\": 1, \"a\": 1},\"contourColor\": { \"r\": 0, \"g\": 0, \"b\": 1, \"a\": 1},\"contourThickness\": 1,\"trackerType\": 0,\"retrievalMode\": 0,\"colorPaletteType\": 0,\"invertMask\": false,\"dilateCount\": 0,\"blurAndReduceEnabled\": true,\"watershedEnabled\": false,\"erodeCount\": 0,\"erodeFirst\": false,\"minWidth\": 0,\"maxWidth\": 1,\"minHeight\": 0,\"maxHeight\": 1,\"kMeansCount\": 0,\"angleAnalysis\": 1,\"regionOfInterest\": { \"x\": 0, \"y\": 0, \"width\": 0, \"height\": 0},\"inferenceOnRoiImage\": false,\"extremePointsAnalysis\": 0,\"extremePointsDistanceFromCenterPointPercent\": 1,\"extremePointsFixedDistance\": 0,\"showRejected\": false,\"showRoi\": true,\"pointCloudFilters\": { \"holeFillingEnabled\": false, \"holeFillingResolution\": 1, \"holeFillingPasses\": 1},\"itemProducerOptions\": { \"graphicType\": 0, \"showPointCloud\": false, \"surface2PolygonMeshOpts\": {  \"searchRadius\": 0.02500000037252903,  \"mu\": 2.5,  \"maximumNearestNeighbors\": 100,  \"maximumSurfaceAngle\": 45,  \"minimumAngle\": 10,  \"maximumAngle\": 120,  \"normalConsistency\": false,  \"consistentVertexOrdering\": true,  \"kSearch\": 20 }},\"errors\": []}]}'
+  _GETMODULESRESPONSE._serialized_options = b'\222A\237O2\234O\022\231O{\"modules\": [{\"inputParameters\": [],\"outputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"\" }],\"id\": \"rs1\",\"active\": true,\"render\": true,\"ordinal\": 0,\"pipeline\": 0,\"type\": \"RealSense\",\"moduleState\": 1,\"stateText\": \"\",\"rsCamera\": { \"processingBlocks\": {  \"alignEnabled\": true,  \"alignTo\": 2,  \"decimationFilterEnabled\": true,  \"streamFilter\": 1,  \"formatFilter\": 1,  \"filterMagnitude\": 8,  \"thresholdFilterEnabled\": false,  \"thresholdMaxDistance\": 1.5,  \"thresholdMinDistance\": 0,  \"disparityMode02\": 0,  \"spatialFilterEnabled\": false,  \"spatialMagnitude\": 1,  \"spatialSmoothAlpha\": 0.72000002861022949,  \"spatialSmoothDelta\": 9,  \"holeFillingMode\": 0,  \"temporalFilterEnabled\": false,  \"temporalSmoothAlpha\": 0.079999998211860657,  \"temporalSmoothDelta\": 100,  \"temporalPersistance\": 6,  \"holeFillingFilterEnabled\": false,  \"holesFill\": 2,  \"colorizerEnabled\": true,  \"visualPreset\": 0,  \"colorScheme\": 5,  \"histogramEqualization\": true,  \"colorizerMinDistance\": 0,  \"colorizerMaxDistance\": 6,  \"pointCloudEnabled\": true,  \"occlusionRemoval\": 2,  \"textureStream\": 1,  \"textureFormat\": 5 }, \"cameraInfo\": {  \"name\": \"\",  \"serialNumber\": \"\",  \"firmwareVersion\": \"\",  \"recommendedFirmwareVersion\": \"\",  \"physicalPort\": \"\",  \"debugOpCode\": \"\",  \"advancedMode\": \"\",  \"productId\": \"\",  \"cameraLocked\": \"\",  \"usbTypeDescriptor\": \"\" }, \"depthResolution\": {  \"width\": 0,  \"height\": 0 }, \"colorResolution\": {  \"width\": 0,  \"height\": 0 }, \"depthFps\": 2, \"colorFps\": 2, \"serialNumber\": \"\", \"mode\": 1, \"playbackFile\": \"/home/kcarlson/Documents/test/longredtape.bag\", \"availableFps\": [  6,  15,  30,  60 ], \"availableDepthResolutions\": [  {   \"devicePrefix\": \"D\",   \"resolutions\": [    {     \"width\": 424,     \"height\": 240    },    {     \"width\": 640,     \"height\": 360    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 848,     \"height\": 100    },    {     \"width\": 848,     \"height\": 480    },    {     \"width\": 1280,     \"height\": 720    }   ]  },  {   \"devicePrefix\": \"L\",   \"resolutions\": [    {     \"width\": 240,     \"height\": 640    },    {     \"width\": 384,     \"height\": 1024    },    {     \"width\": 480,     \"height\": 640    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 768,     \"height\": 1024    },    {     \"width\": 1024,     \"height\": 768    }   ]  } ], \"availableColorResolutions\": [  {   \"devicePrefix\": \"D\",   \"resolutions\": [    {     \"width\": 424,     \"height\": 240    },    {     \"width\": 640,     \"height\": 360    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 848,     \"height\": 480    },    {     \"width\": 960,     \"height\": 540    },    {     \"width\": 1280,     \"height\": 720    }   ]  },  {   \"devicePrefix\": \"L\",   \"resolutions\": [    {     \"width\": 1280,     \"height\": 720    },    {     \"width\": 1920,     \"height\": 1080    }   ]  } ]},\"position\": { \"x\": 0.0052760359831154346, \"y\": 0.058778461068868637, \"z\": -0.00064044661121442914},\"orientation\": { \"x\": 5.0150761604309082, \"y\": 82.971817016601562, \"z\": 358.756103515625},\"showPointcloud\": false,\"depthImage\": false,\"imu\": false,\"errors\": []},{\"inputParameters\": [],\"outputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"\" }, {  \"name\": \"ITEMS\",  \"dataType\": 3,  \"key\": \"\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"\" }],\"id\": \"img\",\"active\": true,\"render\": true,\"ordinal\": 1,\"pipeline\": 0,\"type\": \"ImageSource\",\"moduleState\": 0,\"stateText\": \"\",\"flipImage\": false,\"undistort\": false,\"contourThickness\": 1,\"path\": \"/home/kcarlson/Documents/test/slideshow\",\"displayTimeSeconds\": 5,\"intrinsicsConfigName\": \"\",\"position\": { \"x\": 0, \"y\": 0, \"z\": 0},\"orientation\": { \"x\": 0, \"y\": 0, \"z\": 0},\"itemProducerOptions\": { \"graphicType\": 0, \"showPointCloud\": false, \"surface2PolygonMeshOpts\": {  \"searchRadius\": 0.02500000037252903,  \"mu\": 2.5,  \"maximumNearestNeighbors\": 100,  \"maximumSurfaceAngle\": 45,  \"minimumAngle\": 10,  \"maximumAngle\": 120,  \"normalConsistency\": false,  \"consistentVertexOrdering\": true,  \"kSearch\": 20 }},\"errors\": []},{\"inputParameters\": [],\"outputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"\" }],\"id\": \"rs2\",\"active\": true,\"render\": true,\"ordinal\": 2,\"pipeline\": 1,\"type\": \"RealSense\",\"moduleState\": 1,\"stateText\": \"\",\"rsCamera\": { \"processingBlocks\": {  \"alignEnabled\": true,  \"alignTo\": 2,  \"decimationFilterEnabled\": true,  \"streamFilter\": 1,  \"formatFilter\": 1,  \"filterMagnitude\": 8,  \"thresholdFilterEnabled\": false,  \"thresholdMaxDistance\": 1.5,  \"thresholdMinDistance\": 0,  \"disparityMode02\": 0,  \"spatialFilterEnabled\": false,  \"spatialMagnitude\": 1,  \"spatialSmoothAlpha\": 0.72000002861022949,  \"spatialSmoothDelta\": 9,  \"holeFillingMode\": 0,  \"temporalFilterEnabled\": false,  \"temporalSmoothAlpha\": 0.079999998211860657,  \"temporalSmoothDelta\": 100,  \"temporalPersistance\": 6,  \"holeFillingFilterEnabled\": false,  \"holesFill\": 2,  \"colorizerEnabled\": true,  \"visualPreset\": 0,  \"colorScheme\": 5,  \"histogramEqualization\": true,  \"colorizerMinDistance\": 0,  \"colorizerMaxDistance\": 6,  \"pointCloudEnabled\": true,  \"occlusionRemoval\": 2,  \"textureStream\": 1,  \"textureFormat\": 5 }, \"cameraInfo\": {  \"name\": \"\",  \"serialNumber\": \"\",  \"firmwareVersion\": \"\",  \"recommendedFirmwareVersion\": \"\",  \"physicalPort\": \"\",  \"debugOpCode\": \"\",  \"advancedMode\": \"\",  \"productId\": \"\",  \"cameraLocked\": \"\",  \"usbTypeDescriptor\": \"\" }, \"depthResolution\": {  \"width\": 0,  \"height\": 0 }, \"colorResolution\": {  \"width\": 0,  \"height\": 0 }, \"depthFps\": 2, \"colorFps\": 2, \"serialNumber\": \"\", \"mode\": 1, \"playbackFile\": \"/home/kcarlson/Documents/test/longredtape.bag\", \"availableFps\": [  6,  15,  30,  60 ], \"availableDepthResolutions\": [  {   \"devicePrefix\": \"D\",   \"resolutions\": [    {     \"width\": 424,     \"height\": 240    },    {     \"width\": 640,     \"height\": 360    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 848,     \"height\": 100    },    {     \"width\": 848,     \"height\": 480    },    {     \"width\": 1280,     \"height\": 720    }   ]  },  {   \"devicePrefix\": \"L\",   \"resolutions\": [    {     \"width\": 240,     \"height\": 640    },    {     \"width\": 384,     \"height\": 1024    },    {     \"width\": 480,     \"height\": 640    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 768,     \"height\": 1024    },    {     \"width\": 1024,     \"height\": 768    }   ]  } ], \"availableColorResolutions\": [  {   \"devicePrefix\": \"D\",   \"resolutions\": [    {     \"width\": 424,     \"height\": 240    },    {     \"width\": 640,     \"height\": 360    },    {     \"width\": 640,     \"height\": 480    },    {     \"width\": 848,     \"height\": 480    },    {     \"width\": 960,     \"height\": 540    },    {     \"width\": 1280,     \"height\": 720    }   ]  },  {   \"devicePrefix\": \"L\",   \"resolutions\": [    {     \"width\": 1280,     \"height\": 720    },    {     \"width\": 1920,     \"height\": 1080    }   ]  } ]},\"position\": { \"x\": 0.0052760359831154346, \"y\": 0.058778461068868637, \"z\": -0.00064044661121442914},\"orientation\": { \"x\": 5.0150761604309082, \"y\": 82.971817016601562, \"z\": 358.756103515625},\"showPointcloud\": false,\"depthImage\": false,\"imu\": false,\"errors\": []},{\"inputParameters\": [],\"outputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"\" }, {  \"name\": \"ITEMS\",  \"dataType\": 3,  \"key\": \"\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"\" }],\"id\": \"img2\",\"active\": true,\"render\": true,\"ordinal\": 3,\"pipeline\": 1,\"type\": \"ImageSource\",\"moduleState\": 0,\"stateText\": \"\",\"flipImage\": false,\"undistort\": false,\"contourThickness\": 1,\"path\": \"/home/kcarlson/Documents/test/slideshow\",\"displayTimeSeconds\": 5,\"intrinsicsConfigName\": \"\",\"position\": { \"x\": 0, \"y\": 0, \"z\": 0},\"orientation\": { \"x\": 0, \"y\": 0, \"z\": 0},\"itemProducerOptions\": { \"graphicType\": 0, \"showPointCloud\": false, \"surface2PolygonMeshOpts\": {  \"searchRadius\": 0.02500000037252903,  \"mu\": 2.5,  \"maximumNearestNeighbors\": 100,  \"maximumSurfaceAngle\": 45,  \"minimumAngle\": 10,  \"maximumAngle\": 120,  \"normalConsistency\": false,  \"consistentVertexOrdering\": true,  \"kSearch\": 20 }},\"errors\": []},{\"inputParameters\": [ {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"rs1/RGBA_IMAGE\" }, {  \"name\": \"POINTCLOUD\",  \"dataType\": 5,  \"key\": \"rs1/POINTCLOUD\" }, {  \"name\": \"CAMERA\",  \"dataType\": 1,  \"key\": \"rs1/CAMERA\" }],\"outputParameters\": [ {  \"name\": \"CONTOURS\",  \"dataType\": 2,  \"key\": \"\" }, {  \"name\": \"RGBA_IMAGE\",  \"dataType\": 4,  \"key\": \"\" }, {  \"name\": \"ITEMS\",  \"dataType\": 3,  \"key\": \"\" }, {  \"name\": \"BLOB_COUNT\",  \"dataType\": 7,  \"key\": \"\" }],\"id\": \"blob1\",\"active\": true,\"render\": true,\"ordinal\": 4,\"pipeline\": 0,\"type\": \"Blob\",\"moduleState\": 0,\"stateText\": \"\",\"value0UpperBound\": 255,\"value0LowerBound\": 0,\"value1UpperBound\": 186,\"value1LowerBound\": 162,\"value2UpperBound\": 178,\"value2LowerBound\": 154,\"showRect\": false,\"rectColor\": { \"r\": 0, \"g\": 1, \"b\": 1, \"a\": 1},\"contourColor\": { \"r\": 0, \"g\": 0, \"b\": 1, \"a\": 1},\"contourThickness\": 1,\"trackerType\": 0,\"retrievalMode\": 0,\"colorPaletteType\": 0,\"invertMask\": false,\"dilateCount\": 0,\"blurAndReduceEnabled\": true,\"watershedEnabled\": false,\"erodeCount\": 0,\"erodeFirst\": false,\"minWidth\": 0,\"maxWidth\": 1,\"minHeight\": 0,\"maxHeight\": 1,\"kMeansCount\": 0,\"angleAnalysis\": 1,\"regionOfInterest\": { \"x\": 0, \"y\": 0, \"width\": 0, \"height\": 0},\"inferenceOnRoiImage\": false,\"extremePointsAnalysis\": 0,\"extremePointsDistanceFromCenterPoint\": 1,\"extremePointsFixedDistance\": 0,\"showRejected\": false,\"showRoi\": true,\"pointCloudFilters\": { \"holeFillingEnabled\": false, \"holeFillingResolution\": 1, \"holeFillingPasses\": 1},\"itemProducerOptions\": { \"graphicType\": 0, \"showPointCloud\": false, \"surface2PolygonMeshOpts\": {  \"searchRadius\": 0.02500000037252903,  \"mu\": 2.5,  \"maximumNearestNeighbors\": 100,  \"maximumSurfaceAngle\": 45,  \"minimumAngle\": 10,  \"maximumAngle\": 120,  \"normalConsistency\": false,  \"consistentVertexOrdering\": true,  \"kSearch\": 20 }},\"errors\": []}]}'
   _PATCHMODULEREQUEST._options = None
   _PATCHMODULEREQUEST._serialized_options = b'\222Ap*#\n\nJSON Patch\022\025http://jsonpatch.com/2I\022G{ \"operations\": [{ \"op\": \"replace\", \"path\": \"/baz\", \"value\": \"boo\" }] }'
-  _PATCHMODULEREQUESTV1_1._options = None
-  _PATCHMODULEREQUESTV1_1._serialized_options = b'\222A|2z\022x{ \"module\": { \"real_sense\": { \"playback_file\": \"/data/playback_file.bag\" } }, \"field_mask\": \"real_sense.playback_file\" }'
-  _DELETEMODULEREQUEST.fields_by_name['module_id']._options = None
-  _DELETEMODULEREQUEST.fields_by_name['module_id']._serialized_options = b'\222A\"2\024The module to delete\322\001\tmodule_id'
+  _DELETEMODULEREQUEST.fields_by_name['moduleId']._options = None
+  _DELETEMODULEREQUEST.fields_by_name['moduleId']._serialized_options = b'\222A!2\024The module to delete\322\001\010moduleId'
   _OCELLUSMODULEINFOSERVICE._options = None
   _OCELLUSMODULEINFOSERVICE._serialized_options = b'\222A_\022]Service for interacting with the user configuration, module metadata, and module interactions'
   _OCELLUSMODULEINFOSERVICE.methods_by_name['ReloadModules']._options = None
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['ReloadModules']._serialized_options = b'\210\002\001\222A\027\032\025Use ReloadModulesV1_1\202\323\344\223\002\030\032\026/api/v1/modules/reload'
+  _OCELLUSMODULEINFOSERVICE.methods_by_name['ReloadModules']._serialized_options = b'\222A6\0324Will reload all modules from the configuration file.\202\323\344\223\002\030\032\026/api/v1/modules/reload'
   _OCELLUSMODULEINFOSERVICE.methods_by_name['UpdateModulesConfig']._options = None
   _OCELLUSMODULEINFOSERVICE.methods_by_name['UpdateModulesConfig']._serialized_options = b'\222A4\0322Updates the global configuration, does not persist\202\323\344\223\002\030\032\026/api/v1/modules/config'
   _OCELLUSMODULEINFOSERVICE.methods_by_name['GetModulesConfig']._options = None
   _OCELLUSMODULEINFOSERVICE.methods_by_name['GetModulesConfig']._serialized_options = b'\222A,\032*Retreives the current global configuration\202\323\344\223\002\030\022\026/api/v1/modules/config'
   _OCELLUSMODULEINFOSERVICE.methods_by_name['GetModules']._options = None
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['GetModules']._serialized_options = b'\210\002\001\222A\024\032\022Use GetModulesV1_1\202\323\344\223\002.\022\032/api/v1/module/{module_id}Z\020\022\016/api/v1/module'
+  _OCELLUSMODULEINFOSERVICE.methods_by_name['GetModules']._serialized_options = b'\222AA\032?Returns all or the specified module\'s configuration information\202\323\344\223\002-\022\031/api/v1/module/{moduleId}Z\020\022\016/api/v1/module'
   _OCELLUSMODULEINFOSERVICE.methods_by_name['CreateModule']._options = None
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['CreateModule']._serialized_options = b'\210\002\001\222A\026\032\024Use CreateModuleV1_1\202\323\344\223\002\020\"\016/api/v1/module'
+  _OCELLUSMODULEINFOSERVICE.methods_by_name['CreateModule']._serialized_options = b'\222A(\032&Creates a new module, does not persist\202\323\344\223\002\020\"\016/api/v1/module'
   _OCELLUSMODULEINFOSERVICE.methods_by_name['UpdateModule']._options = None
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['UpdateModule']._serialized_options = b'\210\002\001\222A\026\032\024Use UpdateModuleV1_1\202\323\344\223\002\020\032\016/api/v1/module'
+  _OCELLUSMODULEINFOSERVICE.methods_by_name['UpdateModule']._serialized_options = b'\222A.\032,Updates an existing module, does not persist\202\323\344\223\002\020\032\016/api/v1/module'
   _OCELLUSMODULEINFOSERVICE.methods_by_name['PatchModule']._options = None
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['PatchModule']._serialized_options = b'\210\002\001\222A\025\032\023Use PatchModuleV1_1\202\323\344\223\002\0372\032/api/v1/module/{module_id}:\001*'
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['GetModulesV1_1']._options = None
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['GetModulesV1_1']._serialized_options = b'\222AA\032?Returns all or the specified module\'s configuration information\202\323\344\223\0022\022\034/api/v1_1/module/{module_id}Z\022\022\020/api/v1_1/module'
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['CreateModuleV1_1']._options = None
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['CreateModuleV1_1']._serialized_options = b'\222A(\032&Creates a new module, does not persist\202\323\344\223\002\022\"\020/api/v1_1/module'
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['UpdateModuleV1_1']._options = None
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['UpdateModuleV1_1']._serialized_options = b'\222A.\032,Updates an existing module, does not persist\202\323\344\223\002\022\032\020/api/v1_1/module'
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['PatchModuleV1_1']._options = None
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['PatchModuleV1_1']._serialized_options = b'\202\323\344\223\002!2\034/api/v1_1/module/{module_id}:\001*'
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['ReloadModulesV1_1']._options = None
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['ReloadModulesV1_1']._serialized_options = b'\222A6\0324Will reload all modules from the configuration file.\202\323\344\223\002\032\032\030/api/v1_1/modules/reload'
+  _OCELLUSMODULEINFOSERVICE.methods_by_name['PatchModule']._serialized_options = b'\222A\256\001\032\253\001Updates a specific field of an existing module, does not persist\nReplaces module fields with ops using jsonpatch. Only replace is supported\nReturns the updated module data\202\323\344\223\002\0362\031/api/v1/module/{moduleId}:\001*'
   _OCELLUSMODULEINFOSERVICE.methods_by_name['DeleteModule']._options = None
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['DeleteModule']._serialized_options = b'\222A<\032:Deletes a specific or all loaded modules, does not persist\202\323\344\223\002.*\032/api/v1/module/{module_id}Z\020*\016/api/v1/module'
+  _OCELLUSMODULEINFOSERVICE.methods_by_name['DeleteModule']._serialized_options = b'\222A<\032:Deletes a specific or all loaded modules, does not persist\202\323\344\223\002-*\031/api/v1/module/{moduleId}Z\020*\016/api/v1/module'
   _OCELLUSMODULEINFOSERVICE.methods_by_name['UpdateModuleOrder']._options = None
   _OCELLUSMODULEINFOSERVICE.methods_by_name['UpdateModuleOrder']._serialized_options = b'\222A6\0324Changes the module execution order, does not persist\202\323\344\223\002\026\032\024/api/v1/order/module'
   _OCELLUSMODULEINFOSERVICE.methods_by_name['ModuleApiHandler']._options = None
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['ModuleApiHandler']._serialized_options = b'\222A\027\032\025Module specific APIs.\202\323\344\223\002\306\001\022./api/{version}/module/{module_id}/{path_param}Z0*./api/{version}/module/{module_id}/{path_param}Z0\"./api/{version}/module/{module_id}/{path_param}Z0\032./api/{version}/module/{module_id}/{path_param}'
+  _OCELLUSMODULEINFOSERVICE.methods_by_name['ModuleApiHandler']._serialized_options = b'\222A\027\032\025Module specific APIs.\202\323\344\223\002\276\001\022,/api/{version}/module/{moduleId}/{pathParam}Z.*,/api/{version}/module/{moduleId}/{pathParam}Z.\",/api/{version}/module/{moduleId}/{pathParam}Z.\032,/api/{version}/module/{moduleId}/{pathParam}'
   _OCELLUSMODULEINFOSERVICE.methods_by_name['GetRemoteModules']._options = None
   _OCELLUSMODULEINFOSERVICE.methods_by_name['GetRemoteModules']._serialized_options = b'\222Ai\032gReturns all the currently available remote modules connected using the ocellus.OcellusModuleService API\202\323\344\223\002\030\022\026/api/v1/modules/remote'
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['OnModuleInfoUpdate']._options = None
-  _OCELLUSMODULEINFOSERVICE.methods_by_name['OnModuleInfoUpdate']._serialized_options = b'\222A\"\032 Subsrcibe to module info updates'
-  _GETMODULESREQUEST._serialized_start=336
-  _GETMODULESREQUEST._serialized_end=422
-  _GETMODULESRESPONSE._serialized_start=425
-  _GETMODULESRESPONSE._serialized_end=10644
-  _CREATEMODULEREQUEST._serialized_start=10646
-  _CREATEMODULEREQUEST._serialized_end=10748
-  _GETMODULESRESPONSEV1_1._serialized_start=10750
-  _GETMODULESRESPONSEV1_1._serialized_end=10829
-  _CREATEMODULEREQUESTV1_1._serialized_start=10831
-  _CREATEMODULEREQUESTV1_1._serialized_end=10950
-  _PATCHMODULEREQUEST._serialized_start=10953
-  _PATCHMODULEREQUEST._serialized_end=11241
-  _PATCHMODULEREQUEST_OPERATION._serialized_start=11072
-  _PATCHMODULEREQUEST_OPERATION._serialized_end=11124
-  _PATCHMODULEREQUESTV1_1._serialized_start=11244
-  _PATCHMODULEREQUESTV1_1._serialized_end=11518
-  _DELETEMODULEREQUEST._serialized_start=11520
-  _DELETEMODULEREQUEST._serialized_end=11599
-  _UPDATEMODULEORDERREQUEST._serialized_start=11601
-  _UPDATEMODULEORDERREQUEST._serialized_end=11640
-  _MODULEAPIHANDLERREQUEST._serialized_start=11642
-  _MODULEAPIHANDLERREQUEST._serialized_end=11762
-  _GETREMOTEMODULESRESPONSE._serialized_start=11765
-  _GETREMOTEMODULESRESPONSE._serialized_end=11996
-  _GETREMOTEMODULESRESPONSE_REMOTEMODULEINFO._serialized_start=11881
-  _GETREMOTEMODULESRESPONSE_REMOTEMODULEINFO._serialized_end=11996
-  _OCELLUSMODULEINFOSERVICE._serialized_start=11999
-  _OCELLUSMODULEINFOSERVICE._serialized_end=15334
+  _GETMODULESREQUEST._serialized_start=262
+  _GETMODULESREQUEST._serialized_end=299
+  _GETMODULESRESPONSE._serialized_start=302
+  _GETMODULESRESPONSE._serialized_end=10514
+  _CREATEMODULEREQUEST._serialized_start=10516
+  _CREATEMODULEREQUEST._serialized_end=10618
+  _PATCHMODULEREQUEST._serialized_start=10621
+  _PATCHMODULEREQUEST._serialized_end=10908
+  _PATCHMODULEREQUEST_OPERATION._serialized_start=10739
+  _PATCHMODULEREQUEST_OPERATION._serialized_end=10791
+  _DELETEMODULEREQUEST._serialized_start=10910
+  _DELETEMODULEREQUEST._serialized_end=10987
+  _UPDATEMODULEORDERREQUEST._serialized_start=10989
+  _UPDATEMODULEORDERREQUEST._serialized_end=11028
+  _MODULEAPIHANDLERREQUEST._serialized_start=11030
+  _MODULEAPIHANDLERREQUEST._serialized_end=11148
+  _GETREMOTEMODULESRESPONSE._serialized_start=11151
+  _GETREMOTEMODULESRESPONSE._serialized_end=11382
+  _GETREMOTEMODULESRESPONSE_REMOTEMODULEINFO._serialized_start=11267
+  _GETREMOTEMODULESRESPONSE_REMOTEMODULEINFO._serialized_end=11382
+  _OCELLUSMODULEINFOSERVICE._serialized_start=11385
+  _OCELLUSMODULEINFOSERVICE._serialized_end=13811
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/annotations_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/annotations_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/api/annotations.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import http_pb2 as google_dot_api_dot_http__pb2
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cgoogle/api/annotations.proto\x12\ngoogle.api\x1a\x15google/api/http.proto\x1a google/protobuf/descriptor.proto:E\n\x04http\x12\x1e.google.protobuf.MethodOptions\x18\xb0\xca\xbc\" \x01(\x0b\x32\x14.google.api.HttpRuleBn\n\x0e\x63om.google.apiB\x10\x41nnotationsProtoP\x01ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\xa2\x02\x04GAPIb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.annotations_pb2', globals())
+
+HTTP_FIELD_NUMBER = 72295728
+http = DESCRIPTOR.extensions_by_name['http']
+
 if _descriptor._USE_C_DESCRIPTORS == False:
   google_dot_protobuf_dot_descriptor__pb2.MethodOptions.RegisterExtension(http)
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\020AnnotationsProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\242\002\004GAPI'
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/auth_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/usage_pb2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: google/api/auth.proto
+# source: google/api/usage.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15google/api/auth.proto\x12\ngoogle.api\x1a\x1cgoogle/api/annotations.proto\"l\n\x0e\x41uthentication\x12-\n\x05rules\x18\x03 \x03(\x0b\x32\x1e.google.api.AuthenticationRule\x12+\n\tproviders\x18\x04 \x03(\x0b\x32\x18.google.api.AuthProvider\"\xa9\x01\n\x12\x41uthenticationRule\x12\x10\n\x08selector\x18\x01 \x01(\t\x12,\n\x05oauth\x18\x02 \x01(\x0b\x32\x1d.google.api.OAuthRequirements\x12 \n\x18\x61llow_without_credential\x18\x05 \x01(\x08\x12\x31\n\x0crequirements\x18\x07 \x03(\x0b\x32\x1b.google.api.AuthRequirement\"j\n\x0c\x41uthProvider\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06issuer\x18\x02 \x01(\t\x12\x10\n\x08jwks_uri\x18\x03 \x01(\t\x12\x11\n\taudiences\x18\x04 \x01(\t\x12\x19\n\x11\x61uthorization_url\x18\x05 \x01(\t\"-\n\x11OAuthRequirements\x12\x18\n\x10\x63\x61nonical_scopes\x18\x01 \x01(\t\"9\n\x0f\x41uthRequirement\x12\x13\n\x0bprovider_id\x18\x01 \x01(\t\x12\x11\n\taudiences\x18\x02 \x01(\tBk\n\x0e\x63om.google.apiB\tAuthProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16google/api/usage.proto\x12\ngoogle.api\x1a\x1cgoogle/api/annotations.proto\"j\n\x05Usage\x12\x14\n\x0crequirements\x18\x01 \x03(\t\x12$\n\x05rules\x18\x06 \x03(\x0b\x32\x15.google.api.UsageRule\x12%\n\x1dproducer_notification_channel\x18\x07 \x01(\t\"]\n\tUsageRule\x12\x10\n\x08selector\x18\x01 \x01(\t\x12 \n\x18\x61llow_unregistered_calls\x18\x02 \x01(\x08\x12\x1c\n\x14skip_service_control\x18\x03 \x01(\x08\x42l\n\x0e\x63om.google.apiB\nUsageProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3')
+
+
+
+_USAGE = DESCRIPTOR.message_types_by_name['Usage']
+_USAGERULE = DESCRIPTOR.message_types_by_name['UsageRule']
+Usage = _reflection.GeneratedProtocolMessageType('Usage', (_message.Message,), {
+  'DESCRIPTOR' : _USAGE,
+  '__module__' : 'google.api.usage_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.Usage)
+  })
+_sym_db.RegisterMessage(Usage)
+
+UsageRule = _reflection.GeneratedProtocolMessageType('UsageRule', (_message.Message,), {
+  'DESCRIPTOR' : _USAGERULE,
+  '__module__' : 'google.api.usage_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.UsageRule)
+  })
+_sym_db.RegisterMessage(UsageRule)
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.auth_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\tAuthProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI'
-  _AUTHENTICATION._serialized_start=67
-  _AUTHENTICATION._serialized_end=175
-  _AUTHENTICATIONRULE._serialized_start=178
-  _AUTHENTICATIONRULE._serialized_end=347
-  _AUTHPROVIDER._serialized_start=349
-  _AUTHPROVIDER._serialized_end=455
-  _OAUTHREQUIREMENTS._serialized_start=457
-  _OAUTHREQUIREMENTS._serialized_end=502
-  _AUTHREQUIREMENT._serialized_start=504
-  _AUTHREQUIREMENT._serialized_end=561
+  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\nUsageProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI'
+  _USAGE._serialized_start=68
+  _USAGE._serialized_end=174
+  _USAGERULE._serialized_start=176
+  _USAGERULE._serialized_end=269
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/backend_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/endpoint_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: google/api/backend.proto
+# source: google/api/endpoint.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18google/api/backend.proto\x12\ngoogle.api\"1\n\x07\x42\x61\x63kend\x12&\n\x05rules\x18\x01 \x03(\x0b\x32\x17.google.api.BackendRule\"X\n\x0b\x42\x61\x63kendRule\x12\x10\n\x08selector\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x10\n\x08\x64\x65\x61\x64line\x18\x03 \x01(\x01\x12\x14\n\x0cmin_deadline\x18\x04 \x01(\x01\x42n\n\x0e\x63om.google.apiB\x0c\x42\x61\x63kendProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19google/api/endpoint.proto\x12\ngoogle.api\x1a\x1cgoogle/api/annotations.proto\"_\n\x08\x45ndpoint\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x61liases\x18\x02 \x03(\t\x12\x10\n\x08\x66\x65\x61tures\x18\x04 \x03(\t\x12\x0e\n\x06target\x18\x65 \x01(\t\x12\x12\n\nallow_cors\x18\x05 \x01(\x08\x42o\n\x0e\x63om.google.apiB\rEndpointProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3')
+
+
+
+_ENDPOINT = DESCRIPTOR.message_types_by_name['Endpoint']
+Endpoint = _reflection.GeneratedProtocolMessageType('Endpoint', (_message.Message,), {
+  'DESCRIPTOR' : _ENDPOINT,
+  '__module__' : 'google.api.endpoint_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.Endpoint)
+  })
+_sym_db.RegisterMessage(Endpoint)
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.backend_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\014BackendProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI'
-  _BACKEND._serialized_start=40
-  _BACKEND._serialized_end=89
-  _BACKENDRULE._serialized_start=91
-  _BACKENDRULE._serialized_end=179
+  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\rEndpointProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI'
+  _ENDPOINT._serialized_start=71
+  _ENDPOINT._serialized_end=166
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/billing_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/billing_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,45 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/api/billing.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18google/api/billing.proto\x12\ngoogle.api\x1a\x1cgoogle/api/annotations.proto\"\x93\x01\n\x07\x42illing\x12\x45\n\x15\x63onsumer_destinations\x18\x08 \x03(\x0b\x32&.google.api.Billing.BillingDestination\x1a\x41\n\x12\x42illingDestination\x12\x1a\n\x12monitored_resource\x18\x01 \x01(\t\x12\x0f\n\x07metrics\x18\x02 \x03(\tBn\n\x0e\x63om.google.apiB\x0c\x42illingProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.billing_pb2', globals())
+
+
+_BILLING = DESCRIPTOR.message_types_by_name['Billing']
+_BILLING_BILLINGDESTINATION = _BILLING.nested_types_by_name['BillingDestination']
+Billing = _reflection.GeneratedProtocolMessageType('Billing', (_message.Message,), {
+
+  'BillingDestination' : _reflection.GeneratedProtocolMessageType('BillingDestination', (_message.Message,), {
+    'DESCRIPTOR' : _BILLING_BILLINGDESTINATION,
+    '__module__' : 'google.api.billing_pb2'
+    # @@protoc_insertion_point(class_scope:google.api.Billing.BillingDestination)
+    })
+  ,
+  'DESCRIPTOR' : _BILLING,
+  '__module__' : 'google.api.billing_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.Billing)
+  })
+_sym_db.RegisterMessage(Billing)
+_sym_db.RegisterMessage(Billing.BillingDestination)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\014BillingProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI'
   _BILLING._serialized_start=71
   _BILLING._serialized_end=218
   _BILLING_BILLINGDESTINATION._serialized_start=153
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/client_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/client_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/api/client.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17google/api/client.proto\x12\ngoogle.api\x1a google/protobuf/descriptor.proto:9\n\x10method_signature\x12\x1e.google.protobuf.MethodOptions\x18\x9b\x08 \x03(\t:6\n\x0c\x64\x65\x66\x61ult_host\x12\x1f.google.protobuf.ServiceOptions\x18\x99\x08 \x01(\t:6\n\x0coauth_scopes\x12\x1f.google.protobuf.ServiceOptions\x18\x9a\x08 \x01(\tBi\n\x0e\x63om.google.apiB\x0b\x43lientProtoP\x01ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\xa2\x02\x04GAPIb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.client_pb2', globals())
+
+METHOD_SIGNATURE_FIELD_NUMBER = 1051
+method_signature = DESCRIPTOR.extensions_by_name['method_signature']
+DEFAULT_HOST_FIELD_NUMBER = 1049
+default_host = DESCRIPTOR.extensions_by_name['default_host']
+OAUTH_SCOPES_FIELD_NUMBER = 1050
+oauth_scopes = DESCRIPTOR.extensions_by_name['oauth_scopes']
+
 if _descriptor._USE_C_DESCRIPTORS == False:
   google_dot_protobuf_dot_descriptor__pb2.MethodOptions.RegisterExtension(method_signature)
   google_dot_protobuf_dot_descriptor__pb2.ServiceOptions.RegisterExtension(default_host)
   google_dot_protobuf_dot_descriptor__pb2.ServiceOptions.RegisterExtension(oauth_scopes)
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\013ClientProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\242\002\004GAPI'
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/config_change_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/config_change_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,50 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/api/config_change.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
+from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1egoogle/api/config_change.proto\x12\ngoogle.api\"\x97\x01\n\x0c\x43onfigChange\x12\x0f\n\x07\x65lement\x18\x01 \x01(\t\x12\x11\n\told_value\x18\x02 \x01(\t\x12\x11\n\tnew_value\x18\x03 \x01(\t\x12+\n\x0b\x63hange_type\x18\x04 \x01(\x0e\x32\x16.google.api.ChangeType\x12#\n\x07\x61\x64vices\x18\x05 \x03(\x0b\x32\x12.google.api.Advice\"\x1d\n\x06\x41\x64vice\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t*O\n\nChangeType\x12\x1b\n\x17\x43HANGE_TYPE_UNSPECIFIED\x10\x00\x12\t\n\x05\x41\x44\x44\x45\x44\x10\x01\x12\x0b\n\x07REMOVED\x10\x02\x12\x0c\n\x08MODIFIED\x10\x03\x42q\n\x0e\x63om.google.apiB\x11\x43onfigChangeProtoP\x01ZCgoogle.golang.org/genproto/googleapis/api/configchange;configchange\xa2\x02\x04GAPIb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.config_change_pb2', globals())
+_CHANGETYPE = DESCRIPTOR.enum_types_by_name['ChangeType']
+ChangeType = enum_type_wrapper.EnumTypeWrapper(_CHANGETYPE)
+CHANGE_TYPE_UNSPECIFIED = 0
+ADDED = 1
+REMOVED = 2
+MODIFIED = 3
+
+
+_CONFIGCHANGE = DESCRIPTOR.message_types_by_name['ConfigChange']
+_ADVICE = DESCRIPTOR.message_types_by_name['Advice']
+ConfigChange = _reflection.GeneratedProtocolMessageType('ConfigChange', (_message.Message,), {
+  'DESCRIPTOR' : _CONFIGCHANGE,
+  '__module__' : 'google.api.config_change_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.ConfigChange)
+  })
+_sym_db.RegisterMessage(ConfigChange)
+
+Advice = _reflection.GeneratedProtocolMessageType('Advice', (_message.Message,), {
+  'DESCRIPTOR' : _ADVICE,
+  '__module__' : 'google.api.config_change_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.Advice)
+  })
+_sym_db.RegisterMessage(Advice)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\021ConfigChangeProtoP\001ZCgoogle.golang.org/genproto/googleapis/api/configchange;configchange\242\002\004GAPI'
   _CHANGETYPE._serialized_start=231
   _CHANGETYPE._serialized_end=310
   _CONFIGCHANGE._serialized_start=47
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/consumer_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/label_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: google/api/consumer.proto
+# source: google/api/label.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19google/api/consumer.proto\x12\ngoogle.api\"=\n\x11ProjectProperties\x12(\n\nproperties\x18\x01 \x03(\x0b\x32\x14.google.api.Property\"\xac\x01\n\x08Property\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\x04type\x18\x02 \x01(\x0e\x32!.google.api.Property.PropertyType\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\"L\n\x0cPropertyType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\t\n\x05INT64\x10\x01\x12\x08\n\x04\x42OOL\x10\x02\x12\n\n\x06STRING\x10\x03\x12\n\n\x06\x44OUBLE\x10\x04\x42h\n\x0e\x63om.google.apiB\rConsumerProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfigb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16google/api/label.proto\x12\ngoogle.api\"\x9c\x01\n\x0fLabelDescriptor\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x39\n\nvalue_type\x18\x02 \x01(\x0e\x32%.google.api.LabelDescriptor.ValueType\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\",\n\tValueType\x12\n\n\x06STRING\x10\x00\x12\x08\n\x04\x42OOL\x10\x01\x12\t\n\x05INT64\x10\x02\x42_\n\x0e\x63om.google.apiB\nLabelProtoP\x01Z5google.golang.org/genproto/googleapis/api/label;label\xf8\x01\x01\xa2\x02\x04GAPIb\x06proto3')
+
+
+
+_LABELDESCRIPTOR = DESCRIPTOR.message_types_by_name['LabelDescriptor']
+_LABELDESCRIPTOR_VALUETYPE = _LABELDESCRIPTOR.enum_types_by_name['ValueType']
+LabelDescriptor = _reflection.GeneratedProtocolMessageType('LabelDescriptor', (_message.Message,), {
+  'DESCRIPTOR' : _LABELDESCRIPTOR,
+  '__module__' : 'google.api.label_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.LabelDescriptor)
+  })
+_sym_db.RegisterMessage(LabelDescriptor)
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.consumer_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\rConsumerProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig'
-  _PROJECTPROPERTIES._serialized_start=41
-  _PROJECTPROPERTIES._serialized_end=102
-  _PROPERTY._serialized_start=105
-  _PROPERTY._serialized_end=277
-  _PROPERTY_PROPERTYTYPE._serialized_start=201
-  _PROPERTY_PROPERTYTYPE._serialized_end=277
+  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\nLabelProtoP\001Z5google.golang.org/genproto/googleapis/api/label;label\370\001\001\242\002\004GAPI'
+  _LABELDESCRIPTOR._serialized_start=39
+  _LABELDESCRIPTOR._serialized_end=195
+  _LABELDESCRIPTOR_VALUETYPE._serialized_start=151
+  _LABELDESCRIPTOR_VALUETYPE._serialized_end=195
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/context_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/context_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,43 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/api/context.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18google/api/context.proto\x12\ngoogle.api\"1\n\x07\x43ontext\x12&\n\x05rules\x18\x01 \x03(\x0b\x32\x17.google.api.ContextRule\"D\n\x0b\x43ontextRule\x12\x10\n\x08selector\x18\x01 \x01(\t\x12\x11\n\trequested\x18\x02 \x03(\t\x12\x10\n\x08provided\x18\x03 \x03(\tBn\n\x0e\x63om.google.apiB\x0c\x43ontextProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.context_pb2', globals())
+
+
+_CONTEXT = DESCRIPTOR.message_types_by_name['Context']
+_CONTEXTRULE = DESCRIPTOR.message_types_by_name['ContextRule']
+Context = _reflection.GeneratedProtocolMessageType('Context', (_message.Message,), {
+  'DESCRIPTOR' : _CONTEXT,
+  '__module__' : 'google.api.context_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.Context)
+  })
+_sym_db.RegisterMessage(Context)
+
+ContextRule = _reflection.GeneratedProtocolMessageType('ContextRule', (_message.Message,), {
+  'DESCRIPTOR' : _CONTEXTRULE,
+  '__module__' : 'google.api.context_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.ContextRule)
+  })
+_sym_db.RegisterMessage(ContextRule)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\014ContextProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI'
   _CONTEXT._serialized_start=40
   _CONTEXT._serialized_end=89
   _CONTEXTRULE._serialized_start=91
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/control_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/source_info_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: google/api/control.proto
+# source: google/api/source_info.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18google/api/control.proto\x12\ngoogle.api\"\x1e\n\x07\x43ontrol\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\tBn\n\x0e\x63om.google.apiB\x0c\x43ontrolProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cgoogle/api/source_info.proto\x12\ngoogle.api\x1a\x19google/protobuf/any.proto\"8\n\nSourceInfo\x12*\n\x0csource_files\x18\x01 \x03(\x0b\x32\x14.google.protobuf.AnyBq\n\x0e\x63om.google.apiB\x0fSourceInfoProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3')
+
+
+
+_SOURCEINFO = DESCRIPTOR.message_types_by_name['SourceInfo']
+SourceInfo = _reflection.GeneratedProtocolMessageType('SourceInfo', (_message.Message,), {
+  'DESCRIPTOR' : _SOURCEINFO,
+  '__module__' : 'google.api.source_info_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.SourceInfo)
+  })
+_sym_db.RegisterMessage(SourceInfo)
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.control_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\014ControlProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI'
-  _CONTROL._serialized_start=40
-  _CONTROL._serialized_end=70
+  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\017SourceInfoProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI'
+  _SOURCEINFO._serialized_start=71
+  _SOURCEINFO._serialized_end=127
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/documentation_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/documentation_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,51 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/api/documentation.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1egoogle/api/documentation.proto\x12\ngoogle.api\"\xa1\x01\n\rDocumentation\x12\x0f\n\x07summary\x18\x01 \x01(\t\x12\x1f\n\x05pages\x18\x05 \x03(\x0b\x32\x10.google.api.Page\x12,\n\x05rules\x18\x03 \x03(\x0b\x32\x1d.google.api.DocumentationRule\x12\x1e\n\x16\x64ocumentation_root_url\x18\x04 \x01(\t\x12\x10\n\x08overview\x18\x02 \x01(\t\"[\n\x11\x44ocumentationRule\x12\x10\n\x08selector\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x1f\n\x17\x64\x65precation_description\x18\x03 \x01(\t\"I\n\x04Page\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\x12\"\n\x08subpages\x18\x03 \x03(\x0b\x32\x10.google.api.PageBt\n\x0e\x63om.google.apiB\x12\x44ocumentationProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.documentation_pb2', globals())
+
+
+_DOCUMENTATION = DESCRIPTOR.message_types_by_name['Documentation']
+_DOCUMENTATIONRULE = DESCRIPTOR.message_types_by_name['DocumentationRule']
+_PAGE = DESCRIPTOR.message_types_by_name['Page']
+Documentation = _reflection.GeneratedProtocolMessageType('Documentation', (_message.Message,), {
+  'DESCRIPTOR' : _DOCUMENTATION,
+  '__module__' : 'google.api.documentation_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.Documentation)
+  })
+_sym_db.RegisterMessage(Documentation)
+
+DocumentationRule = _reflection.GeneratedProtocolMessageType('DocumentationRule', (_message.Message,), {
+  'DESCRIPTOR' : _DOCUMENTATIONRULE,
+  '__module__' : 'google.api.documentation_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.DocumentationRule)
+  })
+_sym_db.RegisterMessage(DocumentationRule)
+
+Page = _reflection.GeneratedProtocolMessageType('Page', (_message.Message,), {
+  'DESCRIPTOR' : _PAGE,
+  '__module__' : 'google.api.documentation_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.Page)
+  })
+_sym_db.RegisterMessage(Page)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\022DocumentationProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI'
   _DOCUMENTATION._serialized_start=47
   _DOCUMENTATION._serialized_end=208
   _DOCUMENTATIONRULE._serialized_start=210
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/endpoint_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/httpbody_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: google/api/endpoint.proto
+# source: google/api/httpbody.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19google/api/endpoint.proto\x12\ngoogle.api\x1a\x1cgoogle/api/annotations.proto\"_\n\x08\x45ndpoint\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x61liases\x18\x02 \x03(\t\x12\x10\n\x08\x66\x65\x61tures\x18\x04 \x03(\t\x12\x0e\n\x06target\x18\x65 \x01(\t\x12\x12\n\nallow_cors\x18\x05 \x01(\x08\x42o\n\x0e\x63om.google.apiB\rEndpointProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19google/api/httpbody.proto\x12\ngoogle.api\x1a\x19google/protobuf/any.proto\"X\n\x08HttpBody\x12\x14\n\x0c\x63ontent_type\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12(\n\nextensions\x18\x03 \x03(\x0b\x32\x14.google.protobuf.AnyBe\n\x0e\x63om.google.apiB\rHttpBodyProtoP\x01Z;google.golang.org/genproto/googleapis/api/httpbody;httpbody\xa2\x02\x04GAPIb\x06proto3')
+
+
+
+_HTTPBODY = DESCRIPTOR.message_types_by_name['HttpBody']
+HttpBody = _reflection.GeneratedProtocolMessageType('HttpBody', (_message.Message,), {
+  'DESCRIPTOR' : _HTTPBODY,
+  '__module__' : 'google.api.httpbody_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.HttpBody)
+  })
+_sym_db.RegisterMessage(HttpBody)
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.endpoint_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\rEndpointProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI'
-  _ENDPOINT._serialized_start=71
-  _ENDPOINT._serialized_end=166
+  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\rHttpBodyProtoP\001Z;google.golang.org/genproto/googleapis/api/httpbody;httpbody\242\002\004GAPI'
+  _HTTPBODY._serialized_start=68
+  _HTTPBODY._serialized_end=156
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/field_behavior_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/launch_stage_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: google/api/field_behavior.proto
+# source: google/api/launch_stage.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
+from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fgoogle/api/field_behavior.proto\x12\ngoogle.api\x1a google/protobuf/descriptor.proto*\x8f\x01\n\rFieldBehavior\x12\x1e\n\x1a\x46IELD_BEHAVIOR_UNSPECIFIED\x10\x00\x12\x0c\n\x08OPTIONAL\x10\x01\x12\x0c\n\x08REQUIRED\x10\x02\x12\x0f\n\x0bOUTPUT_ONLY\x10\x03\x12\x0e\n\nINPUT_ONLY\x10\x04\x12\r\n\tIMMUTABLE\x10\x05\x12\x12\n\x0eUNORDERED_LIST\x10\x06:Q\n\x0e\x66ield_behavior\x12\x1d.google.protobuf.FieldOptions\x18\x9c\x08 \x03(\x0e\x32\x19.google.api.FieldBehaviorBp\n\x0e\x63om.google.apiB\x12\x46ieldBehaviorProtoP\x01ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\xa2\x02\x04GAPIb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dgoogle/api/launch_stage.proto\x12\ngoogle.api*j\n\x0bLaunchStage\x12\x1c\n\x18LAUNCH_STAGE_UNSPECIFIED\x10\x00\x12\x10\n\x0c\x45\x41RLY_ACCESS\x10\x01\x12\t\n\x05\x41LPHA\x10\x02\x12\x08\n\x04\x42\x45TA\x10\x03\x12\x06\n\x02GA\x10\x04\x12\x0e\n\nDEPRECATED\x10\x05\x42Z\n\x0e\x63om.google.apiB\x10LaunchStageProtoP\x01Z-google.golang.org/genproto/googleapis/api;api\xa2\x02\x04GAPIb\x06proto3')
+
+_LAUNCHSTAGE = DESCRIPTOR.enum_types_by_name['LaunchStage']
+LaunchStage = enum_type_wrapper.EnumTypeWrapper(_LAUNCHSTAGE)
+LAUNCH_STAGE_UNSPECIFIED = 0
+EARLY_ACCESS = 1
+ALPHA = 2
+BETA = 3
+GA = 4
+DEPRECATED = 5
+
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.field_behavior_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-  google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(field_behavior)
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\022FieldBehaviorProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\242\002\004GAPI'
-  _FIELDBEHAVIOR._serialized_start=82
-  _FIELDBEHAVIOR._serialized_end=225
+  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\020LaunchStageProtoP\001Z-google.golang.org/genproto/googleapis/api;api\242\002\004GAPI'
+  _LAUNCHSTAGE._serialized_start=45
+  _LAUNCHSTAGE._serialized_end=151
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/http_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/field_behavior_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: google/api/http.proto
+# source: google/api/field_behavior.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
+from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15google/api/http.proto\x12\ngoogle.api\"T\n\x04Http\x12#\n\x05rules\x18\x01 \x03(\x0b\x32\x14.google.api.HttpRule\x12\'\n\x1f\x66ully_decode_reserved_expansion\x18\x02 \x01(\x08\"\x81\x02\n\x08HttpRule\x12\x10\n\x08selector\x18\x01 \x01(\t\x12\r\n\x03get\x18\x02 \x01(\tH\x00\x12\r\n\x03put\x18\x03 \x01(\tH\x00\x12\x0e\n\x04post\x18\x04 \x01(\tH\x00\x12\x10\n\x06\x64\x65lete\x18\x05 \x01(\tH\x00\x12\x0f\n\x05patch\x18\x06 \x01(\tH\x00\x12/\n\x06\x63ustom\x18\x08 \x01(\x0b\x32\x1d.google.api.CustomHttpPatternH\x00\x12\x0c\n\x04\x62ody\x18\x07 \x01(\t\x12\x15\n\rresponse_body\x18\x0c \x01(\t\x12\x31\n\x13\x61\x64\x64itional_bindings\x18\x0b \x03(\x0b\x32\x14.google.api.HttpRuleB\t\n\x07pattern\"/\n\x11\x43ustomHttpPattern\x12\x0c\n\x04kind\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\tBj\n\x0e\x63om.google.apiB\tHttpProtoP\x01ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\xf8\x01\x01\xa2\x02\x04GAPIb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fgoogle/api/field_behavior.proto\x12\ngoogle.api\x1a google/protobuf/descriptor.proto*\x8f\x01\n\rFieldBehavior\x12\x1e\n\x1a\x46IELD_BEHAVIOR_UNSPECIFIED\x10\x00\x12\x0c\n\x08OPTIONAL\x10\x01\x12\x0c\n\x08REQUIRED\x10\x02\x12\x0f\n\x0bOUTPUT_ONLY\x10\x03\x12\x0e\n\nINPUT_ONLY\x10\x04\x12\r\n\tIMMUTABLE\x10\x05\x12\x12\n\x0eUNORDERED_LIST\x10\x06:Q\n\x0e\x66ield_behavior\x12\x1d.google.protobuf.FieldOptions\x18\x9c\x08 \x03(\x0e\x32\x19.google.api.FieldBehaviorBp\n\x0e\x63om.google.apiB\x12\x46ieldBehaviorProtoP\x01ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\xa2\x02\x04GAPIb\x06proto3')
+
+_FIELDBEHAVIOR = DESCRIPTOR.enum_types_by_name['FieldBehavior']
+FieldBehavior = enum_type_wrapper.EnumTypeWrapper(_FIELDBEHAVIOR)
+FIELD_BEHAVIOR_UNSPECIFIED = 0
+OPTIONAL = 1
+REQUIRED = 2
+OUTPUT_ONLY = 3
+INPUT_ONLY = 4
+IMMUTABLE = 5
+UNORDERED_LIST = 6
+
+FIELD_BEHAVIOR_FIELD_NUMBER = 1052
+field_behavior = DESCRIPTOR.extensions_by_name['field_behavior']
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.http_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
+  google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(field_behavior)
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\tHttpProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\370\001\001\242\002\004GAPI'
-  _HTTP._serialized_start=37
-  _HTTP._serialized_end=121
-  _HTTPRULE._serialized_start=124
-  _HTTPRULE._serialized_end=381
-  _CUSTOMHTTPPATTERN._serialized_start=383
-  _CUSTOMHTTPPATTERN._serialized_end=430
+  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\022FieldBehaviorProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\242\002\004GAPI'
+  _FIELDBEHAVIOR._serialized_start=82
+  _FIELDBEHAVIOR._serialized_end=225
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/httpbody_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/log_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: google/api/httpbody.proto
+# source: google/api/log.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
+from google.api import label_pb2 as google_dot_api_dot_label__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19google/api/httpbody.proto\x12\ngoogle.api\x1a\x19google/protobuf/any.proto\"X\n\x08HttpBody\x12\x14\n\x0c\x63ontent_type\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12(\n\nextensions\x18\x03 \x03(\x0b\x32\x14.google.protobuf.AnyBe\n\x0e\x63om.google.apiB\rHttpBodyProtoP\x01Z;google.golang.org/genproto/googleapis/api/httpbody;httpbody\xa2\x02\x04GAPIb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14google/api/log.proto\x12\ngoogle.api\x1a\x16google/api/label.proto\"u\n\rLogDescriptor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x06labels\x18\x02 \x03(\x0b\x32\x1b.google.api.LabelDescriptor\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x04 \x01(\tBj\n\x0e\x63om.google.apiB\x08LogProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3')
+
+
+
+_LOGDESCRIPTOR = DESCRIPTOR.message_types_by_name['LogDescriptor']
+LogDescriptor = _reflection.GeneratedProtocolMessageType('LogDescriptor', (_message.Message,), {
+  'DESCRIPTOR' : _LOGDESCRIPTOR,
+  '__module__' : 'google.api.log_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.LogDescriptor)
+  })
+_sym_db.RegisterMessage(LogDescriptor)
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.httpbody_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\rHttpBodyProtoP\001Z;google.golang.org/genproto/googleapis/api/httpbody;httpbody\242\002\004GAPI'
-  _HTTPBODY._serialized_start=68
-  _HTTPBODY._serialized_end=156
+  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\010LogProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI'
+  _LOGDESCRIPTOR._serialized_start=60
+  _LOGDESCRIPTOR._serialized_end=177
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/monitoring_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/monitoring_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,45 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/api/monitoring.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bgoogle/api/monitoring.proto\x12\ngoogle.api\x1a\x1cgoogle/api/annotations.proto\"\xec\x01\n\nMonitoring\x12K\n\x15producer_destinations\x18\x01 \x03(\x0b\x32,.google.api.Monitoring.MonitoringDestination\x12K\n\x15\x63onsumer_destinations\x18\x02 \x03(\x0b\x32,.google.api.Monitoring.MonitoringDestination\x1a\x44\n\x15MonitoringDestination\x12\x1a\n\x12monitored_resource\x18\x01 \x01(\t\x12\x0f\n\x07metrics\x18\x02 \x03(\tBq\n\x0e\x63om.google.apiB\x0fMonitoringProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.monitoring_pb2', globals())
+
+
+_MONITORING = DESCRIPTOR.message_types_by_name['Monitoring']
+_MONITORING_MONITORINGDESTINATION = _MONITORING.nested_types_by_name['MonitoringDestination']
+Monitoring = _reflection.GeneratedProtocolMessageType('Monitoring', (_message.Message,), {
+
+  'MonitoringDestination' : _reflection.GeneratedProtocolMessageType('MonitoringDestination', (_message.Message,), {
+    'DESCRIPTOR' : _MONITORING_MONITORINGDESTINATION,
+    '__module__' : 'google.api.monitoring_pb2'
+    # @@protoc_insertion_point(class_scope:google.api.Monitoring.MonitoringDestination)
+    })
+  ,
+  'DESCRIPTOR' : _MONITORING,
+  '__module__' : 'google.api.monitoring_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.Monitoring)
+  })
+_sym_db.RegisterMessage(Monitoring)
+_sym_db.RegisterMessage(Monitoring.MonitoringDestination)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\017MonitoringProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI'
   _MONITORING._serialized_start=74
   _MONITORING._serialized_end=310
   _MONITORING_MONITORINGDESTINATION._serialized_start=242
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/resource_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/resource_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,52 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/api/resource.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19google/api/resource.proto\x12\ngoogle.api\x1a google/protobuf/descriptor.proto\"\xee\x02\n\x12ResourceDescriptor\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07pattern\x18\x02 \x03(\t\x12\x12\n\nname_field\x18\x03 \x01(\t\x12\x37\n\x07history\x18\x04 \x01(\x0e\x32&.google.api.ResourceDescriptor.History\x12\x0e\n\x06plural\x18\x05 \x01(\t\x12\x10\n\x08singular\x18\x06 \x01(\t\x12\x33\n\x05style\x18\n \x03(\x0e\x32$.google.api.ResourceDescriptor.Style\"[\n\x07History\x12\x17\n\x13HISTORY_UNSPECIFIED\x10\x00\x12\x1d\n\x19ORIGINALLY_SINGLE_PATTERN\x10\x01\x12\x18\n\x14\x46UTURE_MULTI_PATTERN\x10\x02\"8\n\x05Style\x12\x15\n\x11STYLE_UNSPECIFIED\x10\x00\x12\x18\n\x14\x44\x45\x43LARATIVE_FRIENDLY\x10\x01\"5\n\x11ResourceReference\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x12\n\nchild_type\x18\x02 \x01(\t:Y\n\x12resource_reference\x12\x1d.google.protobuf.FieldOptions\x18\x9f\x08 \x01(\x0b\x32\x1d.google.api.ResourceReference:Z\n\x13resource_definition\x12\x1c.google.protobuf.FileOptions\x18\x9d\x08 \x03(\x0b\x32\x1e.google.api.ResourceDescriptor:R\n\x08resource\x12\x1f.google.protobuf.MessageOptions\x18\x9d\x08 \x01(\x0b\x32\x1e.google.api.ResourceDescriptorBn\n\x0e\x63om.google.apiB\rResourceProtoP\x01ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\xf8\x01\x01\xa2\x02\x04GAPIb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.resource_pb2', globals())
+
+RESOURCE_REFERENCE_FIELD_NUMBER = 1055
+resource_reference = DESCRIPTOR.extensions_by_name['resource_reference']
+RESOURCE_DEFINITION_FIELD_NUMBER = 1053
+resource_definition = DESCRIPTOR.extensions_by_name['resource_definition']
+RESOURCE_FIELD_NUMBER = 1053
+resource = DESCRIPTOR.extensions_by_name['resource']
+
+_RESOURCEDESCRIPTOR = DESCRIPTOR.message_types_by_name['ResourceDescriptor']
+_RESOURCEREFERENCE = DESCRIPTOR.message_types_by_name['ResourceReference']
+_RESOURCEDESCRIPTOR_HISTORY = _RESOURCEDESCRIPTOR.enum_types_by_name['History']
+_RESOURCEDESCRIPTOR_STYLE = _RESOURCEDESCRIPTOR.enum_types_by_name['Style']
+ResourceDescriptor = _reflection.GeneratedProtocolMessageType('ResourceDescriptor', (_message.Message,), {
+  'DESCRIPTOR' : _RESOURCEDESCRIPTOR,
+  '__module__' : 'google.api.resource_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.ResourceDescriptor)
+  })
+_sym_db.RegisterMessage(ResourceDescriptor)
+
+ResourceReference = _reflection.GeneratedProtocolMessageType('ResourceReference', (_message.Message,), {
+  'DESCRIPTOR' : _RESOURCEREFERENCE,
+  '__module__' : 'google.api.resource_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.ResourceReference)
+  })
+_sym_db.RegisterMessage(ResourceReference)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
   google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(resource_reference)
   google_dot_protobuf_dot_descriptor__pb2.FileOptions.RegisterExtension(resource_definition)
   google_dot_protobuf_dot_descriptor__pb2.MessageOptions.RegisterExtension(resource)
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\rResourceProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\370\001\001\242\002\004GAPI'
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/routing_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/routing_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,46 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/api/routing.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18google/api/routing.proto\x12\ngoogle.api\x1a google/protobuf/descriptor.proto\"G\n\x0bRoutingRule\x12\x38\n\x12routing_parameters\x18\x02 \x03(\x0b\x32\x1c.google.api.RoutingParameter\"8\n\x10RoutingParameter\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x15\n\rpath_template\x18\x02 \x01(\t:K\n\x07routing\x12\x1e.google.protobuf.MethodOptions\x18\xb1\xca\xbc\" \x01(\x0b\x32\x17.google.api.RoutingRuleBj\n\x0e\x63om.google.apiB\x0cRoutingProtoP\x01ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\xa2\x02\x04GAPIb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.routing_pb2', globals())
+
+ROUTING_FIELD_NUMBER = 72295729
+routing = DESCRIPTOR.extensions_by_name['routing']
+
+_ROUTINGRULE = DESCRIPTOR.message_types_by_name['RoutingRule']
+_ROUTINGPARAMETER = DESCRIPTOR.message_types_by_name['RoutingParameter']
+RoutingRule = _reflection.GeneratedProtocolMessageType('RoutingRule', (_message.Message,), {
+  'DESCRIPTOR' : _ROUTINGRULE,
+  '__module__' : 'google.api.routing_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.RoutingRule)
+  })
+_sym_db.RegisterMessage(RoutingRule)
+
+RoutingParameter = _reflection.GeneratedProtocolMessageType('RoutingParameter', (_message.Message,), {
+  'DESCRIPTOR' : _ROUTINGPARAMETER,
+  '__module__' : 'google.api.routing_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.RoutingParameter)
+  })
+_sym_db.RegisterMessage(RoutingParameter)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
   google_dot_protobuf_dot_descriptor__pb2.MethodOptions.RegisterExtension(routing)
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\014RoutingProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\242\002\004GAPI'
   _ROUTINGRULE._serialized_start=74
   _ROUTINGRULE._serialized_end=145
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/service_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/service_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/api/service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
@@ -32,16 +33,24 @@
 from google.protobuf import api_pb2 as google_dot_protobuf_dot_api__pb2
 from google.protobuf import type_pb2 as google_dot_protobuf_dot_type__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18google/api/service.proto\x12\ngoogle.api\x1a\x1cgoogle/api/annotations.proto\x1a\x15google/api/auth.proto\x1a\x18google/api/backend.proto\x1a\x18google/api/billing.proto\x1a\x18google/api/context.proto\x1a\x18google/api/control.proto\x1a\x1egoogle/api/documentation.proto\x1a\x19google/api/endpoint.proto\x1a\x15google/api/http.proto\x1a\x14google/api/log.proto\x1a\x18google/api/logging.proto\x1a\x17google/api/metric.proto\x1a#google/api/monitored_resource.proto\x1a\x1bgoogle/api/monitoring.proto\x1a\x16google/api/quota.proto\x1a\x1cgoogle/api/source_info.proto\x1a!google/api/system_parameter.proto\x1a\x16google/api/usage.proto\x1a\x19google/protobuf/api.proto\x1a\x1agoogle/protobuf/type.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xdc\x07\n\x07Service\x12\x34\n\x0e\x63onfig_version\x18\x14 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02id\x18! \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x1b\n\x13producer_project_id\x18\x16 \x01(\t\x12\"\n\x04\x61pis\x18\x03 \x03(\x0b\x32\x14.google.protobuf.Api\x12$\n\x05types\x18\x04 \x03(\x0b\x32\x15.google.protobuf.Type\x12$\n\x05\x65nums\x18\x05 \x03(\x0b\x32\x15.google.protobuf.Enum\x12\x30\n\rdocumentation\x18\x06 \x01(\x0b\x32\x19.google.api.Documentation\x12$\n\x07\x62\x61\x63kend\x18\x08 \x01(\x0b\x32\x13.google.api.Backend\x12\x1e\n\x04http\x18\t \x01(\x0b\x32\x10.google.api.Http\x12 \n\x05quota\x18\n \x01(\x0b\x32\x11.google.api.Quota\x12\x32\n\x0e\x61uthentication\x18\x0b \x01(\x0b\x32\x1a.google.api.Authentication\x12$\n\x07\x63ontext\x18\x0c \x01(\x0b\x32\x13.google.api.Context\x12 \n\x05usage\x18\x0f \x01(\x0b\x32\x11.google.api.Usage\x12\'\n\tendpoints\x18\x12 \x03(\x0b\x32\x14.google.api.Endpoint\x12$\n\x07\x63ontrol\x18\x15 \x01(\x0b\x32\x13.google.api.Control\x12\'\n\x04logs\x18\x17 \x03(\x0b\x32\x19.google.api.LogDescriptor\x12-\n\x07metrics\x18\x18 \x03(\x0b\x32\x1c.google.api.MetricDescriptor\x12\x44\n\x13monitored_resources\x18\x19 \x03(\x0b\x32\'.google.api.MonitoredResourceDescriptor\x12$\n\x07\x62illing\x18\x1a \x01(\x0b\x32\x13.google.api.Billing\x12$\n\x07logging\x18\x1b \x01(\x0b\x32\x13.google.api.Logging\x12*\n\nmonitoring\x18\x1c \x01(\x0b\x32\x16.google.api.Monitoring\x12\x37\n\x11system_parameters\x18\x1d \x01(\x0b\x32\x1c.google.api.SystemParameters\x12+\n\x0bsource_info\x18% \x01(\x0b\x32\x16.google.api.SourceInfoJ\x04\x08\x65\x10\x66\x42n\n\x0e\x63om.google.apiB\x0cServiceProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.service_pb2', globals())
+
+
+_SERVICE = DESCRIPTOR.message_types_by_name['Service']
+Service = _reflection.GeneratedProtocolMessageType('Service', (_message.Message,), {
+  'DESCRIPTOR' : _SERVICE,
+  '__module__' : 'google.api.service_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.Service)
+  })
+_sym_db.RegisterMessage(Service)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\014ServiceProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI'
   _SERVICE._serialized_start=619
   _SERVICE._serialized_end=1607
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ocellus-0.1.80/src/ocellus/google/api/system_parameter_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/system_parameter_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,51 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/api/system_parameter.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!google/api/system_parameter.proto\x12\ngoogle.api\"B\n\x10SystemParameters\x12.\n\x05rules\x18\x01 \x03(\x0b\x32\x1f.google.api.SystemParameterRule\"X\n\x13SystemParameterRule\x12\x10\n\x08selector\x18\x01 \x01(\t\x12/\n\nparameters\x18\x02 \x03(\x0b\x32\x1b.google.api.SystemParameter\"Q\n\x0fSystemParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bhttp_header\x18\x02 \x01(\t\x12\x1b\n\x13url_query_parameter\x18\x03 \x01(\tBv\n\x0e\x63om.google.apiB\x14SystemParameterProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.system_parameter_pb2', globals())
+
+
+_SYSTEMPARAMETERS = DESCRIPTOR.message_types_by_name['SystemParameters']
+_SYSTEMPARAMETERRULE = DESCRIPTOR.message_types_by_name['SystemParameterRule']
+_SYSTEMPARAMETER = DESCRIPTOR.message_types_by_name['SystemParameter']
+SystemParameters = _reflection.GeneratedProtocolMessageType('SystemParameters', (_message.Message,), {
+  'DESCRIPTOR' : _SYSTEMPARAMETERS,
+  '__module__' : 'google.api.system_parameter_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.SystemParameters)
+  })
+_sym_db.RegisterMessage(SystemParameters)
+
+SystemParameterRule = _reflection.GeneratedProtocolMessageType('SystemParameterRule', (_message.Message,), {
+  'DESCRIPTOR' : _SYSTEMPARAMETERRULE,
+  '__module__' : 'google.api.system_parameter_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.SystemParameterRule)
+  })
+_sym_db.RegisterMessage(SystemParameterRule)
+
+SystemParameter = _reflection.GeneratedProtocolMessageType('SystemParameter', (_message.Message,), {
+  'DESCRIPTOR' : _SYSTEMPARAMETER,
+  '__module__' : 'google.api.system_parameter_pb2'
+  # @@protoc_insertion_point(class_scope:google.api.SystemParameter)
+  })
+_sym_db.RegisterMessage(SystemParameter)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\024SystemParameterProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI'
   _SYSTEMPARAMETERS._serialized_start=49
   _SYSTEMPARAMETERS._serialized_end=115
   _SYSTEMPARAMETERRULE._serialized_start=117
```

### Comparing `ocellus-0.1.80/src/ocellus/ocellus_dataflow_service_pb2_grpc.py` & `ocellus-0.1.9/src/ocellus/ocellus_dataflow_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.80/src/ocellus/ocellus_module_service_pb2_grpc.py` & `ocellus-0.1.9/src/ocellus/ocellus_module_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.80/src/ocellus/protoc_gen_swagger/options/annotations_pb2.py` & `ocellus-0.1.9/src/ocellus/protoc_gen_swagger/options/annotations_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: protoc-gen-swagger/options/annotations.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 from protoc_gen_swagger.options import openapiv2_pb2 as protoc__gen__swagger_dot_options_dot_openapiv2__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,protoc-gen-swagger/options/annotations.proto\x12\'grpc.gateway.protoc_gen_swagger.options\x1a google/protobuf/descriptor.proto\x1a*protoc-gen-swagger/options/openapiv2.proto:j\n\x11openapiv2_swagger\x12\x1c.google.protobuf.FileOptions\x18\x92\x08 \x01(\x0b\x32\x30.grpc.gateway.protoc_gen_swagger.options.Swagger:p\n\x13openapiv2_operation\x12\x1e.google.protobuf.MethodOptions\x18\x92\x08 \x01(\x0b\x32\x32.grpc.gateway.protoc_gen_swagger.options.Operation:k\n\x10openapiv2_schema\x12\x1f.google.protobuf.MessageOptions\x18\x92\x08 \x01(\x0b\x32/.grpc.gateway.protoc_gen_swagger.options.Schema:e\n\ropenapiv2_tag\x12\x1f.google.protobuf.ServiceOptions\x18\x92\x08 \x01(\x0b\x32,.grpc.gateway.protoc_gen_swagger.options.Tag:l\n\x0fopenapiv2_field\x12\x1d.google.protobuf.FieldOptions\x18\x92\x08 \x01(\x0b\x32\x33.grpc.gateway.protoc_gen_swagger.options.JSONSchemaBCZAgithub.com/grpc-ecosystem/grpc-gateway/protoc-gen-swagger/optionsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protoc_gen_swagger.options.annotations_pb2', globals())
+
+OPENAPIV2_SWAGGER_FIELD_NUMBER = 1042
+openapiv2_swagger = DESCRIPTOR.extensions_by_name['openapiv2_swagger']
+OPENAPIV2_OPERATION_FIELD_NUMBER = 1042
+openapiv2_operation = DESCRIPTOR.extensions_by_name['openapiv2_operation']
+OPENAPIV2_SCHEMA_FIELD_NUMBER = 1042
+openapiv2_schema = DESCRIPTOR.extensions_by_name['openapiv2_schema']
+OPENAPIV2_TAG_FIELD_NUMBER = 1042
+openapiv2_tag = DESCRIPTOR.extensions_by_name['openapiv2_tag']
+OPENAPIV2_FIELD_FIELD_NUMBER = 1042
+openapiv2_field = DESCRIPTOR.extensions_by_name['openapiv2_field']
+
 if _descriptor._USE_C_DESCRIPTORS == False:
   google_dot_protobuf_dot_descriptor__pb2.FileOptions.RegisterExtension(openapiv2_swagger)
   google_dot_protobuf_dot_descriptor__pb2.MethodOptions.RegisterExtension(openapiv2_operation)
   google_dot_protobuf_dot_descriptor__pb2.MessageOptions.RegisterExtension(openapiv2_schema)
   google_dot_protobuf_dot_descriptor__pb2.ServiceOptions.RegisterExtension(openapiv2_tag)
   google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(openapiv2_field)
```

### Comparing `ocellus-0.1.80/src/ocellus.egg-info/SOURCES.txt` & `ocellus-0.1.9/src/ocellus.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 src/ocellus/__init__.py
 src/ocellus/ocellus_dataflow_service_pb2.py
 src/ocellus/ocellus_dataflow_service_pb2_grpc.py
 src/ocellus/ocellus_module_service_pb2.py
 src/ocellus/ocellus_module_service_pb2_grpc.py
@@ -12,16 +11,14 @@
 src/ocellus.egg-info/SOURCES.txt
 src/ocellus.egg-info/dependency_links.txt
 src/ocellus.egg-info/requires.txt
 src/ocellus.egg-info/top_level.txt
 src/ocellus/api/v1/__init__.py
 src/ocellus/api/v1/ocellus_api_command_service_pb2.py
 src/ocellus/api/v1/ocellus_api_command_service_pb2_grpc.py
-src/ocellus/api/v1/ocellus_api_module_config_pb2.py
-src/ocellus/api/v1/ocellus_api_module_config_pb2_grpc.py
 src/ocellus/api/v1/ocellus_api_module_data_service_pb2.py
 src/ocellus/api/v1/ocellus_api_module_data_service_pb2_grpc.py
 src/ocellus/api/v1/ocellus_api_module_info_service_pb2.py
 src/ocellus/api/v1/ocellus_api_module_info_service_pb2_grpc.py
 src/ocellus/google/api/annotations_pb2.py
 src/ocellus/google/api/annotations_pb2_grpc.py
 src/ocellus/google/api/auth_pb2.py
```

