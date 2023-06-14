# Comparing `tmp/google-api-core-2.8.2.tar.gz` & `tmp/google-api-core-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-api-core-2.8.2.tar", last modified: Wed Jun 15 16:07:39 2022, max compression
+gzip compressed data, was "google-api-core-2.9.0.tar", last modified: Fri Sep  2 00:46:16 2022, max compression
```

## Comparing `google-api-core-2.8.2.tar` & `google-api-core-2.9.0.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-15 16:07:39.365488 google-api-core-2.8.2/
--rw-rw-r--   0 root         (0)     1003    11358 2022-06-15 16:04:45.000000 google-api-core-2.8.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-06-15 16:04:45.000000 google-api-core-2.8.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     1767 2022-06-15 16:07:39.365488 google-api-core-2.8.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003      844 2022-06-15 16:04:45.000000 google-api-core-2.8.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-15 16:07:39.349488 google-api-core-2.8.2/google/
--rw-rw-r--   0 root         (0)     1003      850 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-15 16:07:39.353488 google-api-core-2.8.2/google/api_core/
--rw-rw-r--   0 root         (0)     1003      781 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/__init__.py
--rw-rw-r--   0 root         (0)     1003    27313 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/bidi.py
--rw-rw-r--   0 root         (0)     1003     3745 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/client_info.py
--rw-rw-r--   0 root         (0)     1003     4960 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/client_options.py
--rw-rw-r--   0 root         (0)     1003     8991 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/datetime_helpers.py
--rw-rw-r--   0 root         (0)     1003    18850 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/exceptions.py
--rw-rw-r--   0 root         (0)     1003     8038 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/extended_operation.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-15 16:07:39.353488 google-api-core-2.8.2/google/api_core/future/
--rw-rw-r--   0 root         (0)     1003      702 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/future/__init__.py
--rw-rw-r--   0 root         (0)     1003     1248 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/future/_helpers.py
--rw-rw-r--   0 root         (0)     1003     5356 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/future/async_future.py
--rw-rw-r--   0 root         (0)     1003     1763 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/future/base.py
--rw-rw-r--   0 root         (0)     1003     6524 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/future/polling.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-15 16:07:39.353488 google-api-core-2.8.2/google/api_core/gapic_v1/
--rw-rw-r--   0 root         (0)     1003      988 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/gapic_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2216 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/gapic_v1/client_info.py
--rw-rw-r--   0 root         (0)     1003     5984 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/gapic_v1/config.py
--rw-rw-r--   0 root         (0)     1003     1728 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/gapic_v1/config_async.py
--rw-rw-r--   0 root         (0)     1003     9621 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/gapic_v1/method.py
--rw-rw-r--   0 root         (0)     1003     1786 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/gapic_v1/method_async.py
--rw-rw-r--   0 root         (0)     1003     1762 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/gapic_v1/routing_header.py
--rw-rw-r--   0 root         (0)     1003      681 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/general_helpers.py
--rw-rw-r--   0 root         (0)     1003    17036 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/grpc_helpers.py
--rw-rw-r--   0 root         (0)     1003     9998 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/grpc_helpers_async.py
--rw-rw-r--   0 root         (0)     1003    13213 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/iam.py
--rw-rw-r--   0 root         (0)     1003    12885 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/operation.py
--rw-rw-r--   0 root         (0)     1003     8012 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/operation_async.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-15 16:07:39.357488 google-api-core-2.8.2/google/api_core/operations_v1/
--rw-rw-r--   0 root         (0)     1003     1126 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/operations_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    23917 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/operations_v1/abstract_operations_client.py
--rw-rw-r--   0 root         (0)     1003    13625 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/operations_v1/operations_async_client.py
--rw-rw-r--   0 root         (0)     1003    14090 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/operations_v1/operations_client.py
--rw-rw-r--   0 root         (0)     1003     2218 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/operations_v1/operations_client_config.py
--rw-rw-r--   0 root         (0)     1003     3143 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/operations_v1/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-15 16:07:39.357488 google-api-core-2.8.2/google/api_core/operations_v1/transports/
--rw-rw-r--   0 root         (0)     1003      994 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/operations_v1/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8313 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/operations_v1/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18401 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/operations_v1/transports/rest.py
--rw-rw-r--   0 root         (0)     1003    20334 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/page_iterator.py
--rw-rw-r--   0 root         (0)     1003    10294 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/page_iterator_async.py
--rw-rw-r--   0 root         (0)     1003    10108 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/path_template.py
--rw-rw-r--   0 root         (0)     1003    12424 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/protobuf_helpers.py
--rw-rw-r--   0 root         (0)     1003       78 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/py.typed
--rw-rw-r--   0 root         (0)     1003     2929 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/rest_helpers.py
--rw-rw-r--   0 root         (0)     1003     4130 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/rest_streaming.py
--rw-rw-r--   0 root         (0)     1003    12786 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/retry.py
--rw-rw-r--   0 root         (0)     1003    10457 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/retry_async.py
--rw-rw-r--   0 root         (0)     1003     7294 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/timeout.py
--rw-rw-r--   0 root         (0)     1003      597 2022-06-15 16:04:45.000000 google-api-core-2.8.2/google/api_core/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-15 16:07:39.357488 google-api-core-2.8.2/google_api_core.egg-info/
--rw-r--r--   0 root         (0)     1003     1767 2022-06-15 16:07:38.000000 google-api-core-2.8.2/google_api_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3368 2022-06-15 16:07:39.000000 google-api-core-2.8.2/google_api_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-06-15 16:07:38.000000 google-api-core-2.8.2/google_api_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        7 2022-06-15 16:07:38.000000 google-api-core-2.8.2/google_api_core.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-06-15 16:07:38.000000 google-api-core-2.8.2/google_api_core.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      184 2022-06-15 16:07:39.000000 google-api-core-2.8.2/google_api_core.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-06-15 16:07:39.000000 google-api-core-2.8.2/google_api_core.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003      145 2022-06-15 16:07:39.365488 google-api-core-2.8.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3009 2022-06-15 16:04:45.000000 google-api-core-2.8.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-15 16:07:39.357488 google-api-core-2.8.2/tests/
--rw-rw-r--   0 root         (0)     1003        0 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-15 16:07:39.357488 google-api-core-2.8.2/tests/asyncio/
--rw-rw-r--   0 root         (0)     1003        0 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/asyncio/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-15 16:07:39.357488 google-api-core-2.8.2/tests/asyncio/future/
--rw-rw-r--   0 root         (0)     1003        0 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/asyncio/future/__init__.py
--rw-rw-r--   0 root         (0)     1003     5580 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/asyncio/future/test_async_future.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-15 16:07:39.357488 google-api-core-2.8.2/tests/asyncio/gapic/
--rw-rw-r--   0 root         (0)     1003     3080 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/asyncio/gapic/test_config_async.py
--rw-rw-r--   0 root         (0)     1003     8342 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/asyncio/gapic/test_method_async.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-15 16:07:39.357488 google-api-core-2.8.2/tests/asyncio/operations_v1/
--rw-rw-r--   0 root         (0)     1003        0 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/asyncio/operations_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4117 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/asyncio/operations_v1/test_operations_async_client.py
--rw-rw-r--   0 root         (0)     1003    20153 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/asyncio/test_grpc_helpers_async.py
--rw-rw-r--   0 root         (0)     1003     6189 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/asyncio/test_operation_async.py
--rw-rw-r--   0 root         (0)     1003     9906 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/asyncio/test_page_iterator_async.py
--rw-rw-r--   0 root         (0)     1003    14220 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/asyncio/test_retry_async.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-15 16:07:39.361488 google-api-core-2.8.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003        0 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-15 16:07:39.361488 google-api-core-2.8.2/tests/unit/future/
--rw-rw-r--   0 root         (0)     1003        0 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/future/__init__.py
--rw-rw-r--   0 root         (0)     1003     1334 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/future/test__helpers.py
--rw-rw-r--   0 root         (0)     1003     6483 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/future/test_polling.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-15 16:07:39.361488 google-api-core-2.8.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      936 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/gapic/test_client_info.py
--rw-rw-r--   0 root         (0)     1003     3067 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/gapic/test_config.py
--rw-rw-r--   0 root         (0)     1003     8066 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/gapic/test_method.py
--rw-rw-r--   0 root         (0)     1003     1358 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/gapic/test_routing_header.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-15 16:07:39.365488 google-api-core-2.8.2/tests/unit/operations_v1/
--rw-rw-r--   0 root         (0)     1003        0 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/operations_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3596 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/operations_v1/test_operations_client.py
--rw-rw-r--   0 root         (0)     1003    35944 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/operations_v1/test_operations_rest_client.py
--rw-rw-r--   0 root         (0)     1003    29001 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/test_bidi.py
--rw-rw-r--   0 root         (0)     1003     2628 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/test_client_info.py
--rw-rw-r--   0 root         (0)     1003     5140 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/test_client_options.py
--rw-rw-r--   0 root         (0)     1003    13260 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/test_datetime_helpers.py
--rw-rw-r--   0 root         (0)     1003    13530 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/test_exceptions.py
--rw-rw-r--   0 root         (0)     1003     5936 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/test_extended_operation.py
--rw-rw-r--   0 root         (0)     1003    27427 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/test_grpc_helpers.py
--rw-rw-r--   0 root         (0)     1003    13497 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/test_iam.py
--rw-rw-r--   0 root         (0)     1003    10422 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/test_operation.py
--rw-rw-r--   0 root         (0)     1003    21911 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/test_page_iterator.py
--rw-rw-r--   0 root         (0)     1003    13557 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/test_path_template.py
--rw-rw-r--   0 root         (0)     1003    17203 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/test_protobuf_helpers.py
--rw-rw-r--   0 root         (0)     1003     2060 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/test_rest_helpers.py
--rw-rw-r--   0 root         (0)     1003     7158 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/test_rest_streaming.py
--rw-rw-r--   0 root         (0)     1003    16091 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/test_retry.py
--rw-rw-r--   0 root         (0)     1003     4548 2022-06-15 16:04:45.000000 google-api-core-2.8.2/tests/unit/test_timeout.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-09-02 00:46:16.508603 google-api-core-2.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-09-02 00:43:33.000000 google-api-core-2.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-09-02 00:43:33.000000 google-api-core-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     1873 2022-09-02 00:46:16.508603 google-api-core-2.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003      949 2022-09-02 00:43:33.000000 google-api-core-2.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-09-02 00:46:16.492594 google-api-core-2.9.0/google/
+-rw-rw-r--   0 root         (0)     1003      850 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-09-02 00:46:16.496596 google-api-core-2.9.0/google/api_core/
+-rw-rw-r--   0 root         (0)     1003      781 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27313 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/bidi.py
+-rw-rw-r--   0 root         (0)     1003     3745 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/client_info.py
+-rw-rw-r--   0 root         (0)     1003     4960 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/client_options.py
+-rw-rw-r--   0 root         (0)     1003     8991 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/datetime_helpers.py
+-rw-rw-r--   0 root         (0)     1003    18850 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/exceptions.py
+-rw-rw-r--   0 root         (0)     1003     8038 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/extended_operation.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-09-02 00:46:16.496596 google-api-core-2.9.0/google/api_core/future/
+-rw-rw-r--   0 root         (0)     1003      702 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/future/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1248 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/future/_helpers.py
+-rw-rw-r--   0 root         (0)     1003     5356 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/future/async_future.py
+-rw-rw-r--   0 root         (0)     1003     1763 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/future/base.py
+-rw-rw-r--   0 root         (0)     1003     6524 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/future/polling.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-09-02 00:46:16.496596 google-api-core-2.9.0/google/api_core/gapic_v1/
+-rw-rw-r--   0 root         (0)     1003      988 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/gapic_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2216 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/gapic_v1/client_info.py
+-rw-rw-r--   0 root         (0)     1003     5984 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/gapic_v1/config.py
+-rw-rw-r--   0 root         (0)     1003     1728 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/gapic_v1/config_async.py
+-rw-rw-r--   0 root         (0)     1003     9621 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/gapic_v1/method.py
+-rw-rw-r--   0 root         (0)     1003     1786 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/gapic_v1/method_async.py
+-rw-rw-r--   0 root         (0)     1003     1762 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/gapic_v1/routing_header.py
+-rw-rw-r--   0 root         (0)     1003      681 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/general_helpers.py
+-rw-rw-r--   0 root         (0)     1003    17930 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/grpc_helpers.py
+-rw-rw-r--   0 root         (0)     1003     9998 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/grpc_helpers_async.py
+-rw-rw-r--   0 root         (0)     1003    13213 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/iam.py
+-rw-rw-r--   0 root         (0)     1003    12885 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/operation.py
+-rw-rw-r--   0 root         (0)     1003     8012 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/operation_async.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-09-02 00:46:16.500599 google-api-core-2.9.0/google/api_core/operations_v1/
+-rw-rw-r--   0 root         (0)     1003     1126 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/operations_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    23917 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/operations_v1/abstract_operations_client.py
+-rw-rw-r--   0 root         (0)     1003    13625 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/operations_v1/operations_async_client.py
+-rw-rw-r--   0 root         (0)     1003    14090 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/operations_v1/operations_client.py
+-rw-rw-r--   0 root         (0)     1003     2218 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/operations_v1/operations_client_config.py
+-rw-rw-r--   0 root         (0)     1003     3143 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/operations_v1/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-09-02 00:46:16.500599 google-api-core-2.9.0/google/api_core/operations_v1/transports/
+-rw-rw-r--   0 root         (0)     1003      994 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/operations_v1/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8313 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/operations_v1/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18401 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/operations_v1/transports/rest.py
+-rw-rw-r--   0 root         (0)     1003    20334 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/page_iterator.py
+-rw-rw-r--   0 root         (0)     1003    10294 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/page_iterator_async.py
+-rw-rw-r--   0 root         (0)     1003    10929 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/path_template.py
+-rw-rw-r--   0 root         (0)     1003    12424 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/protobuf_helpers.py
+-rw-rw-r--   0 root         (0)     1003       78 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/py.typed
+-rw-rw-r--   0 root         (0)     1003     2929 2022-09-02 00:43:34.000000 google-api-core-2.9.0/google/api_core/rest_helpers.py
+-rw-rw-r--   0 root         (0)     1003     4130 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/rest_streaming.py
+-rw-rw-r--   0 root         (0)     1003    12786 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/retry.py
+-rw-rw-r--   0 root         (0)     1003    10457 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/retry_async.py
+-rw-rw-r--   0 root         (0)     1003     7294 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/timeout.py
+-rw-rw-r--   0 root         (0)     1003      597 2022-09-02 00:43:33.000000 google-api-core-2.9.0/google/api_core/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-09-02 00:46:16.500599 google-api-core-2.9.0/google_api_core.egg-info/
+-rw-r--r--   0 root         (0)     1003     1873 2022-09-02 00:46:16.000000 google-api-core-2.9.0/google_api_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3368 2022-09-02 00:46:16.000000 google-api-core-2.9.0/google_api_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-09-02 00:46:16.000000 google-api-core-2.9.0/google_api_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-09-02 00:46:16.000000 google-api-core-2.9.0/google_api_core.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-09-02 00:46:16.000000 google-api-core-2.9.0/google_api_core.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      261 2022-09-02 00:46:16.000000 google-api-core-2.9.0/google_api_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-09-02 00:46:16.000000 google-api-core-2.9.0/google_api_core.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003      145 2022-09-02 00:46:16.508603 google-api-core-2.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3059 2022-09-02 00:43:33.000000 google-api-core-2.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-09-02 00:46:16.500599 google-api-core-2.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003        0 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-09-02 00:46:16.500599 google-api-core-2.9.0/tests/asyncio/
+-rw-rw-r--   0 root         (0)     1003        0 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/asyncio/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-09-02 00:46:16.500599 google-api-core-2.9.0/tests/asyncio/future/
+-rw-rw-r--   0 root         (0)     1003        0 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/asyncio/future/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5580 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/asyncio/future/test_async_future.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-09-02 00:46:16.500599 google-api-core-2.9.0/tests/asyncio/gapic/
+-rw-rw-r--   0 root         (0)     1003     3080 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/asyncio/gapic/test_config_async.py
+-rw-rw-r--   0 root         (0)     1003     8342 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/asyncio/gapic/test_method_async.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-09-02 00:46:16.500599 google-api-core-2.9.0/tests/asyncio/operations_v1/
+-rw-rw-r--   0 root         (0)     1003        0 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/asyncio/operations_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4117 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/asyncio/operations_v1/test_operations_async_client.py
+-rw-rw-r--   0 root         (0)     1003    20153 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/asyncio/test_grpc_helpers_async.py
+-rw-rw-r--   0 root         (0)     1003     6189 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/asyncio/test_operation_async.py
+-rw-rw-r--   0 root         (0)     1003     9906 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/asyncio/test_page_iterator_async.py
+-rw-rw-r--   0 root         (0)     1003    14220 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/asyncio/test_retry_async.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-09-02 00:46:16.504601 google-api-core-2.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003        0 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-09-02 00:46:16.504601 google-api-core-2.9.0/tests/unit/future/
+-rw-rw-r--   0 root         (0)     1003        0 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/future/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1334 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/future/test__helpers.py
+-rw-rw-r--   0 root         (0)     1003     6483 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/future/test_polling.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-09-02 00:46:16.508603 google-api-core-2.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      936 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/gapic/test_client_info.py
+-rw-rw-r--   0 root         (0)     1003     3067 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/gapic/test_config.py
+-rw-rw-r--   0 root         (0)     1003     8066 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/gapic/test_method.py
+-rw-rw-r--   0 root         (0)     1003     1358 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/gapic/test_routing_header.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-09-02 00:46:16.508603 google-api-core-2.9.0/tests/unit/operations_v1/
+-rw-rw-r--   0 root         (0)     1003        0 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/operations_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3596 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/operations_v1/test_operations_client.py
+-rw-rw-r--   0 root         (0)     1003    35944 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/operations_v1/test_operations_rest_client.py
+-rw-rw-r--   0 root         (0)     1003    29001 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/test_bidi.py
+-rw-rw-r--   0 root         (0)     1003     2628 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/test_client_info.py
+-rw-rw-r--   0 root         (0)     1003     5140 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/test_client_options.py
+-rw-rw-r--   0 root         (0)     1003    13260 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/test_datetime_helpers.py
+-rw-rw-r--   0 root         (0)     1003    13530 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/test_exceptions.py
+-rw-rw-r--   0 root         (0)     1003     5936 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/test_extended_operation.py
+-rw-rw-r--   0 root         (0)     1003    29705 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/test_grpc_helpers.py
+-rw-rw-r--   0 root         (0)     1003    13497 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/test_iam.py
+-rw-rw-r--   0 root         (0)     1003    10422 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/test_operation.py
+-rw-rw-r--   0 root         (0)     1003    21911 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/test_page_iterator.py
+-rw-rw-r--   0 root         (0)     1003    22532 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/test_path_template.py
+-rw-rw-r--   0 root         (0)     1003    17203 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/test_protobuf_helpers.py
+-rw-rw-r--   0 root         (0)     1003     2060 2022-09-02 00:43:34.000000 google-api-core-2.9.0/tests/unit/test_rest_helpers.py
+-rw-rw-r--   0 root         (0)     1003     7158 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/test_rest_streaming.py
+-rw-rw-r--   0 root         (0)     1003    16091 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/test_retry.py
+-rw-rw-r--   0 root         (0)     1003     4548 2022-09-02 00:43:33.000000 google-api-core-2.9.0/tests/unit/test_timeout.py
```

### Comparing `google-api-core-2.8.2/LICENSE` & `google-api-core-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/MANIFEST.in` & `google-api-core-2.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/PKG-INFO` & `google-api-core-2.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: google-api-core
-Version: 2.8.2
+Version: 2.9.0
 Summary: Google API client core library
 Home-page: https://github.com/googleapis/python-api-core
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: grpc
+Provides-Extra: grpcgcp
+Provides-Extra: grpcio-gcp
 License-File: LICENSE
 
 Core Library for Google Client Libraries
 ========================================
 
 |pypi| |versions|
 
@@ -37,17 +38,20 @@
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-api_core.svg
    :target: https://pypi.org/project/google-api_core/
 .. _documentation: https://googleapis.dev/python/google-api-core/latest
 
 
 Supported Python Versions
 -------------------------
-Python >= 3.6
+Python >= 3.7
 
 
 Unsupported Python Versions
 ---------------------------
 
-Python == 2.7, Python == 3.5.
+Python == 2.7, Python == 3.5, Python == 3.6.
 
 The last version of this library compatible with Python 2.7 and 3.5 is
 `google-api-core==1.31.1`.
+
+The last version of this library compatible with Python 3.6 is
+`google-api-core==2.8.2`.
```

### Comparing `google-api-core-2.8.2/README.rst` & `google-api-core-2.9.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -12,17 +12,20 @@
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-api_core.svg
    :target: https://pypi.org/project/google-api_core/
 .. _documentation: https://googleapis.dev/python/google-api-core/latest
 
 
 Supported Python Versions
 -------------------------
-Python >= 3.6
+Python >= 3.7
 
 
 Unsupported Python Versions
 ---------------------------
 
-Python == 2.7, Python == 3.5.
+Python == 2.7, Python == 3.5, Python == 3.6.
 
 The last version of this library compatible with Python 2.7 and 3.5 is
 `google-api-core==1.31.1`.
+
+The last version of this library compatible with Python 3.6 is
+`google-api-core==2.8.2`.
```

### Comparing `google-api-core-2.8.2/google/__init__.py` & `google-api-core-2.9.0/google/__init__.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/__init__.py` & `google-api-core-2.9.0/google/api_core/__init__.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/bidi.py` & `google-api-core-2.9.0/google/api_core/bidi.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/client_info.py` & `google-api-core-2.9.0/google/api_core/client_info.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/client_options.py` & `google-api-core-2.9.0/google/api_core/client_options.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/datetime_helpers.py` & `google-api-core-2.9.0/google/api_core/datetime_helpers.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/exceptions.py` & `google-api-core-2.9.0/google/api_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/extended_operation.py` & `google-api-core-2.9.0/google/api_core/extended_operation.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/future/__init__.py` & `google-api-core-2.9.0/google/api_core/future/__init__.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/future/_helpers.py` & `google-api-core-2.9.0/google/api_core/future/_helpers.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/future/async_future.py` & `google-api-core-2.9.0/google/api_core/future/async_future.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/future/base.py` & `google-api-core-2.9.0/google/api_core/future/base.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/future/polling.py` & `google-api-core-2.9.0/google/api_core/future/polling.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/gapic_v1/__init__.py` & `google-api-core-2.9.0/google/api_core/gapic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/gapic_v1/client_info.py` & `google-api-core-2.9.0/google/api_core/gapic_v1/client_info.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/gapic_v1/config.py` & `google-api-core-2.9.0/google/api_core/gapic_v1/config.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/gapic_v1/config_async.py` & `google-api-core-2.9.0/google/api_core/gapic_v1/config_async.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/gapic_v1/method.py` & `google-api-core-2.9.0/google/api_core/gapic_v1/method.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/gapic_v1/method_async.py` & `google-api-core-2.9.0/google/api_core/gapic_v1/method_async.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/gapic_v1/routing_header.py` & `google-api-core-2.9.0/google/api_core/gapic_v1/routing_header.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/general_helpers.py` & `google-api-core-2.9.0/google/api_core/general_helpers.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/grpc_helpers.py` & `google-api-core-2.9.0/google/api_core/grpc_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,22 +12,44 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Helpers for :mod:`grpc`."""
 
 import collections
 import functools
+import warnings
 
 import grpc
 
 from google.api_core import exceptions
 import google.auth
 import google.auth.credentials
 import google.auth.transport.grpc
 import google.auth.transport.requests
+import google.protobuf
+
+PROTOBUF_VERSION = google.protobuf.__version__
+
+# The grpcio-gcp package only has support for protobuf < 4
+if PROTOBUF_VERSION[0:2] == "3.":
+    try:
+        import grpc_gcp
+
+        warnings.warn(
+            """Support for grpcio-gcp is deprecated. This feature will be
+            removed from `google-api-core` after January 1, 2024. If you need to
+            continue to use this feature, please pin to a specific version of
+            `google-api-core`.""",
+            DeprecationWarning,
+        )
+        HAS_GRPC_GCP = True
+    except ImportError:
+        HAS_GRPC_GCP = False
+else:
+    HAS_GRPC_GCP = False
 
 
 # The list of gRPC Callable interfaces that return iterators.
 _STREAM_WRAP_CLASSES = (grpc.UnaryStreamMultiCallable, grpc.StreamStreamMultiCallable)
 
 
 def _patch_callable_name(callable_):
@@ -271,15 +293,17 @@
         credentials_file (str): A file with credentials that can be loaded with
             :func:`google.auth.load_credentials_from_file`. This argument is
             mutually exclusive with credentials.
         quota_project_id (str): An optional project to use for billing and quota.
         default_scopes (Sequence[str]): Default scopes passed by a Google client
             library. Use 'scopes' for user-defined scopes.
         default_host (str): The default endpoint. e.g., "pubsub.googleapis.com".
-        kwargs: Additional key-word args passed to :func:`grpc.secure_channel`.
+        kwargs: Additional key-word args passed to
+            :func:`grpc_gcp.secure_channel` or :func:`grpc.secure_channel`.
+            Note: `grpc_gcp` is only supported in environments with protobuf < 4.0.0.
 
     Returns:
         grpc.Channel: The created channel.
 
     Raises:
         google.api_core.DuplicateCredentialArgs: If both a credentials object and credentials_file are passed.
     """
@@ -290,14 +314,16 @@
         default_scopes=default_scopes,
         scopes=scopes,
         ssl_credentials=ssl_credentials,
         quota_project_id=quota_project_id,
         default_host=default_host,
     )
 
+    if HAS_GRPC_GCP:
+        return grpc_gcp.secure_channel(target, composite_credentials, **kwargs)
     return grpc.secure_channel(target, composite_credentials, **kwargs)
 
 
 _MethodCall = collections.namedtuple(
     "_MethodCall", ("request", "timeout", "metadata", "credentials")
 )
```

### Comparing `google-api-core-2.8.2/google/api_core/grpc_helpers_async.py` & `google-api-core-2.9.0/google/api_core/grpc_helpers_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""AsyncIO helpers for :mod:`grpc` supporting 3.6+.
+"""AsyncIO helpers for :mod:`grpc` supporting 3.7+.
 
 Please combine more detailed docstring in grpc_helpers.py to use following
 functions. This module is implementing the same surface with AsyncIO semantics.
 """
 
 import asyncio
 import functools
```

### Comparing `google-api-core-2.8.2/google/api_core/iam.py` & `google-api-core-2.9.0/google/api_core/iam.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/operation.py` & `google-api-core-2.9.0/google/api_core/operation.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/operation_async.py` & `google-api-core-2.9.0/google/api_core/operation_async.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/operations_v1/__init__.py` & `google-api-core-2.9.0/google/api_core/operations_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/operations_v1/abstract_operations_client.py` & `google-api-core-2.9.0/google/api_core/operations_v1/abstract_operations_client.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/operations_v1/operations_async_client.py` & `google-api-core-2.9.0/google/api_core/operations_v1/operations_async_client.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/operations_v1/operations_client.py` & `google-api-core-2.9.0/google/api_core/operations_v1/operations_client.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/operations_v1/operations_client_config.py` & `google-api-core-2.9.0/google/api_core/operations_v1/operations_client_config.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/operations_v1/pagers.py` & `google-api-core-2.9.0/google/api_core/operations_v1/pagers.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/operations_v1/transports/__init__.py` & `google-api-core-2.9.0/google/api_core/operations_v1/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/operations_v1/transports/base.py` & `google-api-core-2.9.0/google/api_core/operations_v1/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/operations_v1/transports/rest.py` & `google-api-core-2.9.0/google/api_core/operations_v1/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/page_iterator.py` & `google-api-core-2.9.0/google/api_core/page_iterator.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/page_iterator_async.py` & `google-api-core-2.9.0/google/api_core/page_iterator_async.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/path_template.py` & `google-api-core-2.9.0/google/api_core/path_template.py`

 * *Files 9% similar despite different names*

```diff
@@ -172,48 +172,58 @@
     return _VARIABLE_RE.sub(_replace_variable_with_pattern, tmpl)
 
 
 def get_field(request, field):
     """Get the value of a field from a given dictionary.
 
     Args:
-        request (dict): A dictionary object.
+        request (dict | Message): A dictionary or a Message object.
         field (str): The key to the request in dot notation.
 
     Returns:
         The value of the field.
     """
     parts = field.split(".")
     value = request
+
     for part in parts:
         if not isinstance(value, dict):
-            return
-        value = value.get(part)
+            value = getattr(value, part, None)
+        else:
+            value = value.get(part)
     if isinstance(value, dict):
         return
     return value
 
 
 def delete_field(request, field):
     """Delete the value of a field from a given dictionary.
 
     Args:
-        request (dict): A dictionary object.
+        request (dict | Message): A dictionary object or a Message.
         field (str): The key to the request in dot notation.
     """
     parts = deque(field.split("."))
     while len(parts) > 1:
-        if not isinstance(request, dict):
-            return
         part = parts.popleft()
-        request = request.get(part)
+        if not isinstance(request, dict):
+            if hasattr(request, part):
+                request = getattr(request, part, None)
+            else:
+                return
+        else:
+            request = request.get(part)
     part = parts.popleft()
     if not isinstance(request, dict):
-        return
-    request.pop(part, None)
+        if hasattr(request, part):
+            request.ClearField(part)
+        else:
+            return
+    else:
+        request.pop(part, None)
 
 
 def validate(tmpl, path):
     """Validate a path against the path template.
 
     .. code-block:: python
 
@@ -233,66 +243,76 @@
     Returns:
         bool: True if the path matches.
     """
     pattern = _generate_pattern_for_template(tmpl) + "$"
     return True if re.match(pattern, path) is not None else False
 
 
-def transcode(http_options, **request_kwargs):
+def transcode(http_options, message=None, **request_kwargs):
     """Transcodes a grpc request pattern into a proper HTTP request following the rules outlined here,
     https://github.com/googleapis/googleapis/blob/master/google/api/http.proto#L44-L312
 
      Args:
          http_options (list(dict)): A list of dicts which consist of these keys,
              'method'    (str): The http method
              'uri'       (str): The path template
              'body'      (str): The body field name (optional)
              (This is a simplified representation of the proto option `google.api.http`)
 
+         message (Message) : A request object (optional)
          request_kwargs (dict) : A dict representing the request object
 
      Returns:
          dict: The transcoded request with these keys,
              'method'        (str)   : The http method
              'uri'           (str)   : The expanded uri
-             'body'          (dict)  : A dict representing the body (optional)
-             'query_params'  (dict)  : A dict mapping query parameter variables and values
+             'body'          (dict | Message)  : A dict or a Message representing the body (optional)
+             'query_params'  (dict | Message)  : A dict or Message mapping query parameter variables and values
 
      Raises:
          ValueError: If the request does not match the given template.
     """
+    transcoded_value = message or request_kwargs
     for http_option in http_options:
         request = {}
 
         # Assign path
         uri_template = http_option["uri"]
         path_fields = [
             match.group("name") for match in _VARIABLE_RE.finditer(uri_template)
         ]
-        path_args = {field: get_field(request_kwargs, field) for field in path_fields}
+        path_args = {field: get_field(transcoded_value, field) for field in path_fields}
         request["uri"] = expand(uri_template, **path_args)
-        # Remove fields used in uri path from request
-        leftovers = copy.deepcopy(request_kwargs)
-        for path_field in path_fields:
-            delete_field(leftovers, path_field)
 
         if not validate(uri_template, request["uri"]) or not all(path_args.values()):
             continue
 
+        # Remove fields used in uri path from request
+        leftovers = copy.deepcopy(transcoded_value)
+        for path_field in path_fields:
+            delete_field(leftovers, path_field)
+
         # Assign body and query params
         body = http_option.get("body")
 
         if body:
             if body == "*":
                 request["body"] = leftovers
-                request["query_params"] = {}
+                if message:
+                    request["query_params"] = message.__class__()
+                else:
+                    request["query_params"] = {}
             else:
                 try:
-                    request["body"] = leftovers.pop(body)
-                except KeyError:
+                    if message:
+                        request["body"] = getattr(leftovers, body)
+                        delete_field(leftovers, body)
+                    else:
+                        request["body"] = leftovers.pop(body)
+                except (KeyError, AttributeError):
                     continue
                 request["query_params"] = leftovers
         else:
             request["query_params"] = leftovers
         request["method"] = http_option["method"]
         return request
```

### Comparing `google-api-core-2.8.2/google/api_core/protobuf_helpers.py` & `google-api-core-2.9.0/google/api_core/protobuf_helpers.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/rest_helpers.py` & `google-api-core-2.9.0/google/api_core/rest_helpers.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/rest_streaming.py` & `google-api-core-2.9.0/google/api_core/rest_streaming.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/retry.py` & `google-api-core-2.9.0/google/api_core/retry.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/retry_async.py` & `google-api-core-2.9.0/google/api_core/retry_async.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/timeout.py` & `google-api-core-2.9.0/google/api_core/timeout.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/google/api_core/version.py` & `google-api-core-2.9.0/google/api_core/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "2.8.2"
+__version__ = "2.9.0"
```

### Comparing `google-api-core-2.8.2/google_api_core.egg-info/PKG-INFO` & `google-api-core-2.9.0/google_api_core.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: google-api-core
-Version: 2.8.2
+Version: 2.9.0
 Summary: Google API client core library
 Home-page: https://github.com/googleapis/python-api-core
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: grpc
+Provides-Extra: grpcgcp
+Provides-Extra: grpcio-gcp
 License-File: LICENSE
 
 Core Library for Google Client Libraries
 ========================================
 
 |pypi| |versions|
 
@@ -37,17 +38,20 @@
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-api_core.svg
    :target: https://pypi.org/project/google-api_core/
 .. _documentation: https://googleapis.dev/python/google-api-core/latest
 
 
 Supported Python Versions
 -------------------------
-Python >= 3.6
+Python >= 3.7
 
 
 Unsupported Python Versions
 ---------------------------
 
-Python == 2.7, Python == 3.5.
+Python == 2.7, Python == 3.5, Python == 3.6.
 
 The last version of this library compatible with Python 2.7 and 3.5 is
 `google-api-core==1.31.1`.
+
+The last version of this library compatible with Python 3.6 is
+`google-api-core==2.8.2`.
```

### Comparing `google-api-core-2.8.2/google_api_core.egg-info/SOURCES.txt` & `google-api-core-2.9.0/google_api_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/setup.py` & `google-api-core-2.9.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,20 +26,22 @@
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
 # 'Development Status :: 5 - Production/Stable'
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     "googleapis-common-protos >= 1.56.2, < 2.0dev",
-    "protobuf >= 3.15.0, <5.0.0dev",
+    "protobuf >= 3.20.1, <5.0.0dev",
     "google-auth >= 1.25.0, < 3.0dev",
     "requests >= 2.18.0, < 3.0.0dev",
 ]
 extras = {
     "grpc": ["grpcio >= 1.33.2, < 2.0dev", "grpcio-status >= 1.33.2, < 2.0dev"],
+    "grpcgcp": "grpcio-gcp >= 0.2.2, < 1.0dev",
+    "grpcio-gcp": "grpcio-gcp >= 0.2.2, < 1.0dev",
 }
 
 
 # Setup boilerplate below this line.
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
@@ -76,24 +78,23 @@
     url="https://github.com/googleapis/python-api-core",
     classifiers=[
         release_status,
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
         "Topic :: Internet",
     ],
     platforms="Posix; MacOS X; Windows",
     packages=packages,
     namespace_packages=namespaces,
     install_requires=dependencies,
     extras_require=extras,
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `google-api-core-2.8.2/tests/asyncio/future/test_async_future.py` & `google-api-core-2.9.0/tests/asyncio/future/test_async_future.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/asyncio/gapic/test_config_async.py` & `google-api-core-2.9.0/tests/asyncio/gapic/test_config_async.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/asyncio/gapic/test_method_async.py` & `google-api-core-2.9.0/tests/asyncio/gapic/test_method_async.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/asyncio/operations_v1/test_operations_async_client.py` & `google-api-core-2.9.0/tests/asyncio/operations_v1/test_operations_async_client.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/asyncio/test_grpc_helpers_async.py` & `google-api-core-2.9.0/tests/asyncio/test_grpc_helpers_async.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/asyncio/test_operation_async.py` & `google-api-core-2.9.0/tests/asyncio/test_operation_async.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/asyncio/test_page_iterator_async.py` & `google-api-core-2.9.0/tests/asyncio/test_page_iterator_async.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/asyncio/test_retry_async.py` & `google-api-core-2.9.0/tests/asyncio/test_retry_async.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/future/test__helpers.py` & `google-api-core-2.9.0/tests/unit/future/test__helpers.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/future/test_polling.py` & `google-api-core-2.9.0/tests/unit/future/test_polling.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/gapic/test_client_info.py` & `google-api-core-2.9.0/tests/unit/gapic/test_client_info.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/gapic/test_config.py` & `google-api-core-2.9.0/tests/unit/gapic/test_config.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/gapic/test_method.py` & `google-api-core-2.9.0/tests/unit/gapic/test_method.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/gapic/test_routing_header.py` & `google-api-core-2.9.0/tests/unit/gapic/test_routing_header.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/operations_v1/test_operations_client.py` & `google-api-core-2.9.0/tests/unit/operations_v1/test_operations_client.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/operations_v1/test_operations_rest_client.py` & `google-api-core-2.9.0/tests/unit/operations_v1/test_operations_rest_client.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/test_bidi.py` & `google-api-core-2.9.0/tests/unit/test_bidi.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/test_client_info.py` & `google-api-core-2.9.0/tests/unit/test_client_info.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/test_client_options.py` & `google-api-core-2.9.0/tests/unit/test_client_options.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/test_datetime_helpers.py` & `google-api-core-2.9.0/tests/unit/test_datetime_helpers.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/test_exceptions.py` & `google-api-core-2.9.0/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/test_extended_operation.py` & `google-api-core-2.9.0/tests/unit/test_extended_operation.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/test_grpc_helpers.py` & `google-api-core-2.9.0/tests/unit/test_grpc_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -361,15 +361,18 @@
 
     channel = grpc_helpers.create_channel(target)
 
     assert channel is grpc_secure_channel.return_value
 
     default.assert_called_once_with(scopes=None, default_scopes=None)
 
-    grpc_secure_channel.assert_called_once_with(target, composite_creds)
+    if grpc_helpers.HAS_GRPC_GCP:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds, None)
+    else:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds)
 
 
 @mock.patch("google.auth.transport.grpc.AuthMetadataPlugin", autospec=True)
 @mock.patch(
     "google.auth.transport.requests.Request",
     autospec=True,
     return_value=mock.sentinel.Request,
@@ -393,15 +396,18 @@
     assert channel is grpc_secure_channel.return_value
 
     default.assert_called_once_with(scopes=None, default_scopes=None)
     auth_metadata_plugin.assert_called_once_with(
         mock.sentinel.credentials, mock.sentinel.Request, default_host=default_host
     )
 
-    grpc_secure_channel.assert_called_once_with(target, composite_creds)
+    if grpc_helpers.HAS_GRPC_GCP:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds, None)
+    else:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds)
 
 
 @mock.patch("grpc.composite_channel_credentials")
 @mock.patch(
     "google.auth.default",
     autospec=True,
     return_value=(mock.sentinel.credentials, mock.sentinel.projet),
@@ -416,15 +422,19 @@
 
     grpc_helpers.create_channel(target, ssl_credentials=ssl_creds)
 
     default.assert_called_once_with(scopes=None, default_scopes=None)
 
     composite_creds_call.assert_called_once_with(ssl_creds, mock.ANY)
     composite_creds = composite_creds_call.return_value
-    grpc_secure_channel.assert_called_once_with(target, composite_creds)
+
+    if grpc_helpers.HAS_GRPC_GCP:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds, None)
+    else:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds)
 
 
 @mock.patch("grpc.composite_channel_credentials")
 @mock.patch(
     "google.auth.default",
     autospec=True,
     return_value=(mock.sentinel.credentials, mock.sentinel.projet),
@@ -438,15 +448,18 @@
 
     channel = grpc_helpers.create_channel(target, scopes=["one", "two"])
 
     assert channel is grpc_secure_channel.return_value
 
     default.assert_called_once_with(scopes=["one", "two"], default_scopes=None)
 
-    grpc_secure_channel.assert_called_once_with(target, composite_creds)
+    if grpc_helpers.HAS_GRPC_GCP:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds, None)
+    else:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds)
 
 
 @mock.patch("grpc.composite_channel_credentials")
 @mock.patch(
     "google.auth.default",
     autospec=True,
     return_value=(mock.sentinel.credentials, mock.sentinel.projet),
@@ -460,15 +473,18 @@
 
     channel = grpc_helpers.create_channel(target, default_scopes=["three", "four"])
 
     assert channel is grpc_secure_channel.return_value
 
     default.assert_called_once_with(scopes=None, default_scopes=["three", "four"])
 
-    grpc_secure_channel.assert_called_once_with(target, composite_creds)
+    if grpc_helpers.HAS_GRPC_GCP:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds, None)
+    else:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds)
 
 
 def test_create_channel_explicit_with_duplicate_credentials():
     target = "example.com:443"
 
     with pytest.raises(exceptions.DuplicateCredentialArgs):
         grpc_helpers.create_channel(
@@ -488,15 +504,19 @@
     channel = grpc_helpers.create_channel(target, credentials=mock.sentinel.credentials)
 
     auth_creds.assert_called_once_with(
         mock.sentinel.credentials, scopes=None, default_scopes=None
     )
 
     assert channel is grpc_secure_channel.return_value
-    grpc_secure_channel.assert_called_once_with(target, composite_creds)
+
+    if grpc_helpers.HAS_GRPC_GCP:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds, None)
+    else:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds)
 
 
 @mock.patch("grpc.composite_channel_credentials")
 @mock.patch("grpc.secure_channel")
 def test_create_channel_explicit_scoped(grpc_secure_channel, composite_creds_call):
     target = "example.com:443"
     scopes = ["1", "2"]
@@ -508,15 +528,19 @@
     channel = grpc_helpers.create_channel(
         target, credentials=credentials, scopes=scopes
     )
 
     credentials.with_scopes.assert_called_once_with(scopes, default_scopes=None)
 
     assert channel is grpc_secure_channel.return_value
-    grpc_secure_channel.assert_called_once_with(target, composite_creds)
+
+    if grpc_helpers.HAS_GRPC_GCP:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds, None)
+    else:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds)
 
 
 @mock.patch("grpc.composite_channel_credentials")
 @mock.patch("grpc.secure_channel")
 def test_create_channel_explicit_default_scopes(
     grpc_secure_channel, composite_creds_call
 ):
@@ -532,15 +556,19 @@
     )
 
     credentials.with_scopes.assert_called_once_with(
         scopes=None, default_scopes=default_scopes
     )
 
     assert channel is grpc_secure_channel.return_value
-    grpc_secure_channel.assert_called_once_with(target, composite_creds)
+
+    if grpc_helpers.HAS_GRPC_GCP:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds, None)
+    else:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds)
 
 
 @mock.patch("grpc.composite_channel_credentials")
 @mock.patch("grpc.secure_channel")
 def test_create_channel_explicit_with_quota_project(
     grpc_secure_channel, composite_creds_call
 ):
@@ -554,15 +582,19 @@
     channel = grpc_helpers.create_channel(
         target, credentials=credentials, quota_project_id="project-foo"
     )
 
     credentials.with_quota_project.assert_called_once_with("project-foo")
 
     assert channel is grpc_secure_channel.return_value
-    grpc_secure_channel.assert_called_once_with(target, composite_creds)
+
+    if grpc_helpers.HAS_GRPC_GCP:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds, None)
+    else:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds)
 
 
 @mock.patch("grpc.composite_channel_credentials")
 @mock.patch("grpc.secure_channel")
 @mock.patch(
     "google.auth.load_credentials_from_file",
     autospec=True,
@@ -579,15 +611,19 @@
     channel = grpc_helpers.create_channel(target, credentials_file=credentials_file)
 
     google.auth.load_credentials_from_file.assert_called_once_with(
         credentials_file, scopes=None, default_scopes=None
     )
 
     assert channel is grpc_secure_channel.return_value
-    grpc_secure_channel.assert_called_once_with(target, composite_creds)
+
+    if grpc_helpers.HAS_GRPC_GCP:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds, None)
+    else:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds)
 
 
 @mock.patch("grpc.composite_channel_credentials")
 @mock.patch("grpc.secure_channel")
 @mock.patch(
     "google.auth.load_credentials_from_file",
     autospec=True,
@@ -607,15 +643,19 @@
     )
 
     google.auth.load_credentials_from_file.assert_called_once_with(
         credentials_file, scopes=scopes, default_scopes=None
     )
 
     assert channel is grpc_secure_channel.return_value
-    grpc_secure_channel.assert_called_once_with(target, composite_creds)
+
+    if grpc_helpers.HAS_GRPC_GCP:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds, None)
+    else:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds)
 
 
 @mock.patch("grpc.composite_channel_credentials")
 @mock.patch("grpc.secure_channel")
 @mock.patch(
     "google.auth.load_credentials_from_file",
     autospec=True,
@@ -635,19 +675,41 @@
     )
 
     load_credentials_from_file.assert_called_once_with(
         credentials_file, scopes=None, default_scopes=default_scopes
     )
 
     assert channel is grpc_secure_channel.return_value
-    grpc_secure_channel.assert_called_once_with(target, composite_creds)
+
+    if grpc_helpers.HAS_GRPC_GCP:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds, None)
+    else:
+        grpc_secure_channel.assert_called_once_with(target, composite_creds)
+
+
+@pytest.mark.skipif(
+    not grpc_helpers.HAS_GRPC_GCP, reason="grpc_gcp module not available"
+)
+@mock.patch("grpc_gcp.secure_channel")
+def test_create_channel_with_grpc_gcp(grpc_gcp_secure_channel):
+    target = "example.com:443"
+    scopes = ["test_scope"]
+
+    credentials = mock.create_autospec(google.auth.credentials.Scoped, instance=True)
+    credentials.requires_scopes = True
+
+    grpc_helpers.create_channel(target, credentials=credentials, scopes=scopes)
+    grpc_gcp_secure_channel.assert_called()
+
+    credentials.with_scopes.assert_called_once_with(scopes, default_scopes=None)
 
 
+@pytest.mark.skipif(grpc_helpers.HAS_GRPC_GCP, reason="grpc_gcp module not available")
 @mock.patch("grpc.secure_channel")
-def test_create_channel(grpc_secure_channel):
+def test_create_channel_without_grpc_gcp(grpc_secure_channel):
     target = "example.com:443"
     scopes = ["test_scope"]
 
     credentials = mock.create_autospec(google.auth.credentials.Scoped, instance=True)
     credentials.requires_scopes = True
 
     grpc_helpers.create_channel(target, credentials=credentials, scopes=scopes)
```

### Comparing `google-api-core-2.8.2/tests/unit/test_iam.py` & `google-api-core-2.9.0/tests/unit/test_iam.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/test_operation.py` & `google-api-core-2.9.0/tests/unit/test_operation.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/test_page_iterator.py` & `google-api-core-2.9.0/tests/unit/test_page_iterator.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/test_protobuf_helpers.py` & `google-api-core-2.9.0/tests/unit/test_protobuf_helpers.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/test_rest_helpers.py` & `google-api-core-2.9.0/tests/unit/test_rest_helpers.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/test_rest_streaming.py` & `google-api-core-2.9.0/tests/unit/test_rest_streaming.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/test_retry.py` & `google-api-core-2.9.0/tests/unit/test_retry.py`

 * *Files identical despite different names*

### Comparing `google-api-core-2.8.2/tests/unit/test_timeout.py` & `google-api-core-2.9.0/tests/unit/test_timeout.py`

 * *Files identical despite different names*

