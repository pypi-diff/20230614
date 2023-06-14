# Comparing `tmp/giskard-2.0.0b7.tar.gz` & `tmp/giskard-2.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giskard-2.0.0b7.tar", last modified: Tue Jun 13 12:29:40 2023, max compression
+gzip compressed data, was "giskard-2.0.0b8.tar", last modified: Wed Jun 14 18:52:33 2023, max compression
```

## Comparing `giskard-2.0.0b7.tar` & `giskard-2.0.0b8.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.360038 giskard-2.0.0b7/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-13 12:29:40.360178 giskard-2.0.0b7/PKG-INFO
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     8643 2023-06-12 14:14:57.000000 giskard-2.0.0b7/README.md
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.300116 giskard-2.0.0b7/giskard/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1836 2023-06-12 16:43:55.000000 giskard-2.0.0b7/giskard/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      704 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/cli.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3388 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/cli_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.303788 giskard-2.0.0b7/giskard/client/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/client/dtos.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11444 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/client/giskard_client.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2136 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/client/io_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3620 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/client/project.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      673 2023-06-06 13:35:03.000000 giskard-2.0.0b7/giskard/client/python_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.304799 giskard-2.0.0b7/giskard/commands/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    16407 2023-06-13 10:37:18.000000 giskard-2.0.0b7/giskard/commands/cli_server.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7604 2023-06-13 10:46:54.000000 giskard-2.0.0b7/giskard/commands/cli_worker.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.306163 giskard-2.0.0b7/giskard/core/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/core/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11799 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/core/core.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6466 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/core/dataset_validation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      890 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/core/errors.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13215 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/core/model_validation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15807 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/core/suite.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      574 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/core/validation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.306341 giskard-2.0.0b7/giskard/datasets/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2711 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/datasets/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.306515 giskard-2.0.0b7/giskard/datasets/base/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26225 2023-06-12 16:43:48.000000 giskard-2.0.0b7/giskard/datasets/base/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.308000 giskard-2.0.0b7/giskard/datasets/metadata/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      206 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/datasets/metadata/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3431 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/datasets/metadata/indexing.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      788 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/datasets/metadata/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1851 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/datasets/metadata/text_metadata_provider.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.308469 giskard-2.0.0b7/giskard/demo/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3059 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/demo/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    60302 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/demo/titanic.csv
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.309093 giskard-2.0.0b7/giskard/ml_worker/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b7/giskard/ml_worker/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.310097 giskard-2.0.0b7/giskard/ml_worker/bridge/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1406 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/ml_worker/bridge/data_encryptor.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       42 2023-04-12 00:50:05.000000 giskard-2.0.0b7/giskard/ml_worker/bridge/error.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9252 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/bridge/ml_worker_bridge.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       62 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/ml_worker/bridge/service_messages.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.310688 giskard-2.0.0b7/giskard/ml_worker/core/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1012 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/core/log_listener.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5858 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/core/savable.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.312751 giskard-2.0.0b7/giskard/ml_worker/exceptions/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      375 2023-04-12 00:50:05.000000 giskard-2.0.0b7/giskard/ml_worker/exceptions/IllegalArgumentError.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b7/giskard/ml_worker/exceptions/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      114 2023-04-12 00:50:05.000000 giskard-2.0.0b7/giskard/ml_worker/exceptions/giskard_exception.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.314684 giskard-2.0.0b7/giskard/ml_worker/generated/
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    51492 2023-06-13 12:29:40.000000 giskard-2.0.0b7/giskard/ml_worker/generated/ml_worker_pb2.py
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    21397 2023-06-13 12:29:40.000000 giskard-2.0.0b7/giskard/ml_worker/generated/ml_worker_pb2_grpc.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3226 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/ml_worker.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.314933 giskard-2.0.0b7/giskard/ml_worker/server/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b7/giskard/ml_worker/server/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26425 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/server/ml_worker_service.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.316847 giskard-2.0.0b7/giskard/ml_worker/testing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-05-25 10:01:00.000000 giskard-2.0.0b7/giskard/ml_worker/testing/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.317676 giskard-2.0.0b7/giskard/ml_worker/testing/functions/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      170 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/functions/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3927 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/functions/slicing.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6602 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/functions/transformation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.319193 giskard-2.0.0b7/giskard/ml_worker/testing/registry/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/ml_worker/testing/registry/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1799 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/registry/decorators.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2317 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/registry/decorators_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4703 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/registry/giskard_test.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3943 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/registry/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6374 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/registry/slicing_function.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5439 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/registry/transformation_function.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1783 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/registry/udf_repository.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4675 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/ml_worker/testing/stat_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2649 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/test_result.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2036 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.320178 giskard-2.0.0b7/giskard/ml_worker/utils/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b7/giskard/ml_worker/utils/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      137 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/ml_worker/utils/file_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2297 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/ml_worker/utils/logging.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1952 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/utils/network.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2514 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/utils/request_interceptor.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.321052 giskard-2.0.0b7/giskard/models/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15755 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/models/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2207 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/models/_precooked.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.321262 giskard-2.0.0b7/giskard/models/automodel/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9234 2023-06-12 16:43:52.000000 giskard-2.0.0b7/giskard/models/automodel/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.321613 giskard-2.0.0b7/giskard/models/base/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    34331 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/models/base/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.322415 giskard-2.0.0b7/giskard/models/cache/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      803 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/models/cache/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2706 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/models/cache/cache.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.322608 giskard-2.0.0b7/giskard/models/catboost/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      698 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/models/catboost/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.322955 giskard-2.0.0b7/giskard/models/function/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1202 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/models/function/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.323120 giskard-2.0.0b7/giskard/models/huggingface/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5872 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/models/huggingface/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.323338 giskard-2.0.0b7/giskard/models/langchain/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2619 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/models/langchain/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6342 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/models/model_explanation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.323533 giskard-2.0.0b7/giskard/models/pytorch/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7205 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/models/pytorch/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.323760 giskard-2.0.0b7/giskard/models/sklearn/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4321 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/models/sklearn/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.323995 giskard-2.0.0b7/giskard/models/tensorflow/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1656 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/models/tensorflow/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      844 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/models/utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      528 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/path_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.325545 giskard-2.0.0b7/giskard/scanner/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1595 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.326352 giskard-2.0.0b7/giskard/scanner/calibration/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3475 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/calibration/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3894 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/calibration/overconfidence_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3708 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/calibration/underconfidence_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.326781 giskard-2.0.0b7/giskard/scanner/common/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2568 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/common/examples.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4788 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/common/loss_based_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.326971 giskard-2.0.0b7/giskard/scanner/data_leakage/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2702 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/data_leakage/data_leakage_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      617 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/scanner/decorators.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1396 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/issues.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.327331 giskard-2.0.0b7/giskard/scanner/llm/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5929 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/llm/toxicity_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      627 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/llm/utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       84 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/logger.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.328429 giskard-2.0.0b7/giskard/scanner/performance/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      159 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/scanner/performance/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4218 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/performance/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4638 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/performance/metrics.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6651 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/performance/performance_bias_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      941 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/scanner/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3882 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/scanner/result.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.331893 giskard-2.0.0b7/giskard/scanner/robustness/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6379 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/robustness/base_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)   455659 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/scanner/robustness/entity_swap.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      953 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/scanner/robustness/ethical_bias_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3322 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/robustness/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19432 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/robustness/nationalities.json
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1006 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/scanner/robustness/text_perturbation_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11955 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/scanner/robustness/text_transformations.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7997 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/scanner.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.334034 giskard-2.0.0b7/giskard/scanner/stochasticity/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2237 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/stochasticity/stochasticity_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.335814 giskard-2.0.0b7/giskard/scanner/templates/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      767 2023-06-12 14:14:57.000000 giskard-2.0.0b7/giskard/scanner/templates/_code_snippet.html
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.337559 giskard-2.0.0b7/giskard/scanner/templates/_issues/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1475 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues/data_leakage.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1653 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues/default.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1501 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues/llm_toxicity.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2155 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues/overconfidence.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2128 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues/performance.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2020 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues/robustness.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1468 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues/stochasticity.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2144 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues/underconfidence.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1261 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues_table.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6806 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_main_content.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2862 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_tab_header.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      214 2023-06-12 11:29:06.000000 giskard-2.0.0b7/giskard/scanner/templates/base.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      555 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/scan_results.html
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.338397 giskard-2.0.0b7/giskard/scanner/templates/static/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19904 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/scanner/templates/static/external.js
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    65083 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/scanner/templates/static/internal.js
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    12690 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/static/style.css
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.338826 giskard-2.0.0b7/giskard/scanner/visualization/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/scanner/visualization/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      820 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/visualization/custom_jinja.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      902 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/settings.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.341185 giskard-2.0.0b7/giskard/slicing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       82 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/slicing/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      707 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/slicing/base.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1300 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/slicing/bruteforce_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      615 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/slicing/category_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3174 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/slicing/multiscale_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1868 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/slicing/opt_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10534 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/slicing/slice.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15389 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/slicing/stop_words.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7652 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/slicing/text_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3460 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/slicing/tree_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1311 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/slicing/utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.341441 giskard-2.0.0b7/giskard/testing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2085 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/testing/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.342521 giskard-2.0.0b7/giskard/testing/tests/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/testing/tests/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    33167 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/testing/tests/drift.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    30208 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/testing/tests/metamorphic.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    25823 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/testing/tests/performance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10370 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/testing/tests/statistic.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.344126 giskard-2.0.0b7/giskard/utils/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      385 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/utils/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7144 2023-06-13 11:00:17.000000 giskard-2.0.0b7/giskard/utils/analytics_collector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      293 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/utils/display.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4919 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/utils/environment_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.301257 giskard-2.0.0b7/giskard.egg-info/
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-13 12:29:40.000000 giskard-2.0.0b7/giskard.egg-info/PKG-INFO
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     6171 2023-06-13 12:29:40.000000 giskard-2.0.0b7/giskard.egg-info/SOURCES.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        1 2023-06-13 12:29:40.000000 giskard-2.0.0b7/giskard.egg-info/dependency_links.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       44 2023-06-13 12:29:40.000000 giskard-2.0.0b7/giskard.egg-info/entry_points.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)      602 2023-06-13 12:29:40.000000 giskard-2.0.0b7/giskard.egg-info/requires.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       27 2023-06-13 12:29:40.000000 giskard-2.0.0b7/giskard.egg-info/top_level.txt
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7425 2023-06-13 11:07:01.000000 giskard-2.0.0b7/pyproject.toml
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       93 2023-06-13 12:29:40.360501 giskard-2.0.0b7/setup.cfg
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2281 2023-06-07 15:34:18.000000 giskard-2.0.0b7/setup.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.359800 giskard-2.0.0b7/tests/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1513 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_custom_model.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15828 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_data_drift.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6395 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_data_processing_pipeline.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4533 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_dataset.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      199 2023-04-12 00:50:05.000000 giskard-2.0.0b7/tests/test_logging.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11293 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_metamorphic_direction.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10279 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_metamorphic_invariance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2409 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_model.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2148 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_model_auto_inference.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2526 2023-06-07 15:34:18.000000 giskard-2.0.0b7/tests/test_model_explanation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3791 2023-06-07 15:34:18.000000 giskard-2.0.0b7/tests/test_model_postprocess.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14080 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_performance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4572 2023-06-12 16:46:51.000000 giskard-2.0.0b7/tests/test_programmatic.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4283 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_project_uploads.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4554 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_statistical.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4570 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_upload.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      450 2023-06-12 11:29:06.000000 giskard-2.0.0b7/tests/test_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.256336 giskard-2.0.0b8/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-14 18:52:33.256489 giskard-2.0.0b8/PKG-INFO
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     8643 2023-06-14 09:16:20.000000 giskard-2.0.0b8/README.md
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.132049 giskard-2.0.0b8/giskard/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1836 2023-06-13 13:04:39.000000 giskard-2.0.0b8/giskard/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      704 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/cli.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3388 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/cli_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.142868 giskard-2.0.0b8/giskard/client/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/client/dtos.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11481 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/client/giskard_client.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2136 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/client/io_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3602 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/client/project.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      673 2023-06-06 13:35:03.000000 giskard-2.0.0b8/giskard/client/python_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.144067 giskard-2.0.0b8/giskard/commands/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    16407 2023-06-13 13:05:12.000000 giskard-2.0.0b8/giskard/commands/cli_server.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7604 2023-06-13 13:04:39.000000 giskard-2.0.0b8/giskard/commands/cli_worker.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.147039 giskard-2.0.0b8/giskard/core/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/core/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11813 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/core/core.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6466 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/core/dataset_validation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      886 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/core/errors.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13213 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/core/model_validation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    16026 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/core/suite.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      560 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/core/validation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.147301 giskard-2.0.0b8/giskard/datasets/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2691 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/datasets/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.147634 giskard-2.0.0b8/giskard/datasets/base/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26225 2023-06-12 16:43:48.000000 giskard-2.0.0b8/giskard/datasets/base/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.150320 giskard-2.0.0b8/giskard/datasets/metadata/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      206 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/datasets/metadata/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3431 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/datasets/metadata/indexing.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      788 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/datasets/metadata/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1851 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/datasets/metadata/text_metadata_provider.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.152361 giskard-2.0.0b8/giskard/demo/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2922 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/demo/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    60302 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/demo/titanic.csv
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.156144 giskard-2.0.0b8/giskard/ml_worker/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b8/giskard/ml_worker/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.159135 giskard-2.0.0b8/giskard/ml_worker/bridge/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1406 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/ml_worker/bridge/data_encryptor.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       42 2023-04-12 00:50:05.000000 giskard-2.0.0b8/giskard/ml_worker/bridge/error.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9252 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/bridge/ml_worker_bridge.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       62 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/ml_worker/bridge/service_messages.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.161230 giskard-2.0.0b8/giskard/ml_worker/core/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1012 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/core/log_listener.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5857 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/core/savable.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.162223 giskard-2.0.0b8/giskard/ml_worker/exceptions/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      375 2023-04-12 00:50:05.000000 giskard-2.0.0b8/giskard/ml_worker/exceptions/IllegalArgumentError.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b8/giskard/ml_worker/exceptions/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      114 2023-04-12 00:50:05.000000 giskard-2.0.0b8/giskard/ml_worker/exceptions/giskard_exception.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.168126 giskard-2.0.0b8/giskard/ml_worker/generated/
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    51492 2023-06-14 18:52:33.000000 giskard-2.0.0b8/giskard/ml_worker/generated/ml_worker_pb2.py
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    21397 2023-06-14 18:52:33.000000 giskard-2.0.0b8/giskard/ml_worker/generated/ml_worker_pb2_grpc.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3222 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/ml_worker.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.169046 giskard-2.0.0b8/giskard/ml_worker/server/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b8/giskard/ml_worker/server/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26239 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/server/ml_worker_service.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.177369 giskard-2.0.0b8/giskard/ml_worker/testing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-05-25 10:01:00.000000 giskard-2.0.0b8/giskard/ml_worker/testing/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.178635 giskard-2.0.0b8/giskard/ml_worker/testing/functions/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      160 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/functions/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3919 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/functions/slicing.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6585 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/functions/transformation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.193982 giskard-2.0.0b8/giskard/ml_worker/testing/registry/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/ml_worker/testing/registry/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1800 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/registry/decorators.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2356 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/registry/decorators_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4703 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/registry/giskard_test.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3943 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/registry/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6454 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/registry/slicing_function.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5376 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/registry/transformation_function.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1796 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/registry/udf_repository.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4675 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/ml_worker/testing/stat_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2634 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/test_result.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2036 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.200281 giskard-2.0.0b8/giskard/ml_worker/utils/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b8/giskard/ml_worker/utils/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      137 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/ml_worker/utils/file_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2297 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/ml_worker/utils/logging.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1951 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/utils/network.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2502 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/utils/request_interceptor.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.202368 giskard-2.0.0b8/giskard/models/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15755 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/models/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2191 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/models/_precooked.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.204402 giskard-2.0.0b8/giskard/models/automodel/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9234 2023-06-13 13:04:39.000000 giskard-2.0.0b8/giskard/models/automodel/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.207871 giskard-2.0.0b8/giskard/models/base/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    34331 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/models/base/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.208632 giskard-2.0.0b8/giskard/models/cache/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      803 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/models/cache/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2706 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/models/cache/cache.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.208903 giskard-2.0.0b8/giskard/models/catboost/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      698 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/models/catboost/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.209192 giskard-2.0.0b8/giskard/models/function/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1202 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/models/function/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.209482 giskard-2.0.0b8/giskard/models/huggingface/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5872 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/models/huggingface/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.209772 giskard-2.0.0b8/giskard/models/langchain/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2643 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/models/langchain/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6343 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/models/model_explanation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.210061 giskard-2.0.0b8/giskard/models/pytorch/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7205 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/models/pytorch/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.210305 giskard-2.0.0b8/giskard/models/sklearn/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4321 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/models/sklearn/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.211218 giskard-2.0.0b8/giskard/models/tensorflow/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1618 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/models/tensorflow/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      845 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/models/utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      528 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/path_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.220153 giskard-2.0.0b8/giskard/scanner/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1595 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.222996 giskard-2.0.0b8/giskard/scanner/calibration/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3475 2023-06-14 17:21:01.000000 giskard-2.0.0b8/giskard/scanner/calibration/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3894 2023-06-14 17:21:01.000000 giskard-2.0.0b8/giskard/scanner/calibration/overconfidence_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3708 2023-06-14 17:21:01.000000 giskard-2.0.0b8/giskard/scanner/calibration/underconfidence_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.223721 giskard-2.0.0b8/giskard/scanner/common/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2568 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/common/examples.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4788 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/common/loss_based_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.224017 giskard-2.0.0b8/giskard/scanner/data_leakage/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2702 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/data_leakage/data_leakage_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      617 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/scanner/decorators.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1396 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/issues.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.224459 giskard-2.0.0b8/giskard/scanner/llm/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5929 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/llm/toxicity_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      627 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/llm/utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       84 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/logger.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.226231 giskard-2.0.0b8/giskard/scanner/performance/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      159 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/scanner/performance/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4218 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/performance/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4638 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/performance/metrics.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6651 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/performance/performance_bias_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      941 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/scanner/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3820 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/scanner/result.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.231364 giskard-2.0.0b8/giskard/scanner/robustness/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6379 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/robustness/base_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)   455659 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/scanner/robustness/entity_swap.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      964 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/scanner/robustness/ethical_bias_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3322 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/robustness/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19432 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/robustness/nationalities.json
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1077 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/scanner/robustness/text_perturbation_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11957 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/scanner/robustness/text_transformations.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7997 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/scanner.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.231628 giskard-2.0.0b8/giskard/scanner/stochasticity/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2237 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/stochasticity/stochasticity_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.233559 giskard-2.0.0b8/giskard/scanner/templates/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      767 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_code_snippet.html
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.235744 giskard-2.0.0b8/giskard/scanner/templates/_issues/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1475 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues/data_leakage.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1653 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues/default.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1501 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues/llm_toxicity.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2155 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues/overconfidence.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2128 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues/performance.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2020 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues/robustness.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1468 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues/stochasticity.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2144 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues/underconfidence.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1261 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues_table.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6806 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/templates/_main_content.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2862 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/templates/_tab_header.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      214 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/base.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      555 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/scan_results.html
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.237331 giskard-2.0.0b8/giskard/scanner/templates/static/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19904 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/static/external.js
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    65083 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/static/internal.js
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    12690 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/static/style.css
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.237797 giskard-2.0.0b8/giskard/scanner/visualization/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/scanner/visualization/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      820 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/visualization/custom_jinja.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      902 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/settings.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.242349 giskard-2.0.0b8/giskard/slicing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       82 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/slicing/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      707 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/slicing/base.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1300 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/slicing/bruteforce_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      615 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/slicing/category_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3174 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/slicing/multiscale_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1868 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/slicing/opt_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10349 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/slicing/slice.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11248 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/slicing/stop_words.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7652 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/slicing/text_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3460 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/slicing/tree_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1311 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/slicing/utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.242689 giskard-2.0.0b8/giskard/testing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2085 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/testing/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.245022 giskard-2.0.0b8/giskard/testing/tests/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/testing/tests/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    33165 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/testing/tests/drift.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    30188 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/testing/tests/metamorphic.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    25824 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/testing/tests/performance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10353 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/testing/tests/statistic.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.247262 giskard-2.0.0b8/giskard/utils/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      385 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/utils/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7144 2023-06-13 13:04:55.000000 giskard-2.0.0b8/giskard/utils/analytics_collector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      293 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/utils/display.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4919 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/utils/environment_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.134516 giskard-2.0.0b8/giskard.egg-info/
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-14 18:52:33.000000 giskard-2.0.0b8/giskard.egg-info/PKG-INFO
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     6171 2023-06-14 18:52:33.000000 giskard-2.0.0b8/giskard.egg-info/SOURCES.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        1 2023-06-14 18:52:33.000000 giskard-2.0.0b8/giskard.egg-info/dependency_links.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       44 2023-06-14 18:52:33.000000 giskard-2.0.0b8/giskard.egg-info/entry_points.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)      602 2023-06-14 18:52:33.000000 giskard-2.0.0b8/giskard.egg-info/requires.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       27 2023-06-14 18:52:33.000000 giskard-2.0.0b8/giskard.egg-info/top_level.txt
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7428 2023-06-14 18:23:36.000000 giskard-2.0.0b8/pyproject.toml
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       93 2023-06-14 18:52:33.256888 giskard-2.0.0b8/setup.cfg
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2281 2023-06-14 09:21:06.000000 giskard-2.0.0b8/setup.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.256101 giskard-2.0.0b8/tests/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1453 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_custom_model.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14801 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_data_drift.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6424 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_data_processing_pipeline.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4533 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_dataset.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      199 2023-04-12 00:50:05.000000 giskard-2.0.0b8/tests/test_logging.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9561 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_metamorphic_direction.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9533 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_metamorphic_invariance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2402 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_model.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2185 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_model_auto_inference.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2526 2023-06-07 15:34:18.000000 giskard-2.0.0b8/tests/test_model_explanation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3791 2023-06-07 15:34:18.000000 giskard-2.0.0b8/tests/test_model_postprocess.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14080 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_performance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4573 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_programmatic.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4264 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_project_uploads.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4342 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_statistical.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4687 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_upload.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      450 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_utils.py
```

### Comparing `giskard-2.0.0b7/PKG-INFO` & `giskard-2.0.0b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giskard
-Version: 2.0.0b7
+Version: 2.0.0b8
 Summary: The testing framework dedicated to ML models, from tabular to LLMs
 Author-email: Giskard AI <hello@giskard.ai>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://giskard.ai
 Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues
 Project-URL: Documentation, https://docs.giskard.ai/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: giskard Version: 2.0.0b7 Summary: The testing
+Metadata-Version: 2.1 Name: giskard Version: 2.0.0b8 Summary: The testing
 framework dedicated to ML models, from tabular to LLMs Author-email: Giskard AI
 giskard.ai> License: Apache Software License 2.0 Project-URL: Homepage, https:/
 /giskard.ai Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues Project-
 URL: Documentation, https://docs.giskard.ai/ Project-URL: Discord, https://
 discord.gg/ABvfpbu69R Project-URL: Linkedin, https://www.linkedin.com/company/
 giskard-ai Project-URL: Mastodon, https://fosstodon.org/@Giskard Project-URL:
```

### Comparing `giskard-2.0.0b7/README.md` & `giskard-2.0.0b8/README.md`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/__init__.py` & `giskard-2.0.0b8/giskard/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/cli.py` & `giskard-2.0.0b8/giskard/cli.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/cli_utils.py` & `giskard-2.0.0b8/giskard/cli_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     logger.info(f"Writing logs to {log_path}")
     pid_file = PIDLockFile(create_pid_file_path(is_server, url))
 
     with DaemonContext(pidfile=pid_file, stdout=open(log_path, "w+t")):
         # For some reason requests.utils.should_bypass_proxies that's called inside every request made by requests
         # hangs when the process runs as a daemon. A dirty temporary fix is to disable proxies for daemon mode.
         # True reasons for this to happen to be investigated
-        os.environ['no_proxy'] = '*'
+        os.environ["no_proxy"] = "*"
 
         workdir = settings.home_dir / "tmp" / f"daemon-run-{os.getpid()}"
         workdir.mkdir(exist_ok=True, parents=True)
         change_working_directory(workdir)
 
         logger.info(f"Daemon PID: {os.getpid()}")
         asyncio.get_event_loop().run_until_complete(MLWorker(is_server, url, api_key).start())
```

### Comparing `giskard-2.0.0b7/giskard/client/giskard_client.py` & `giskard-2.0.0b8/giskard/client/giskard_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,20 +153,23 @@
         res = self._session.get(f"project/{project_key}/datasets/{uuid}").json()
         return DatasetMeta(
             name=res["name"],
             target=res["target"],
             column_types=res["columnTypes"],
             column_dtypes=res["columnDtypes"],
             number_of_rows=res["numberOfRows"],
-            category_features=res["categoryFeatures"]
+            category_features=res["categoryFeatures"],
         )
 
     def save_model_meta(self, project_key: str, model_id: UUID, meta: ModelMeta, python_version: str, size: int):
-        class_label_dtype = None if (not meta.classification_labels or not len(meta.classification_labels)) else type(
-            meta.classification_labels[0]).__name__
+        class_label_dtype = (
+            None
+            if (not meta.classification_labels or not len(meta.classification_labels))
+            else type(meta.classification_labels[0]).__name__
+        )
 
         self._session.post(
             f"project/{project_key}/models",
             json={
                 "languageVersion": python_version,
                 "language": "PYTHON",
                 "modelType": meta.model_type.name.upper(),
@@ -254,15 +257,15 @@
                 "name": meta.name,
                 "target": meta.target,
                 "columnTypes": meta.column_types,
                 "columnDtypes": meta.column_dtypes,
                 "originalSizeBytes": original_size_bytes,
                 "compressedSizeBytes": compressed_size_bytes,
                 "numberOfRows": meta.number_of_rows,
-                "categoryFeatures": meta.category_features
+                "categoryFeatures": meta.category_features,
             },
         )
         analytics.track(
             "Upload Dataset",
             {
                 "project": anonymize(project_key),
                 "id": anonymize(dataset_id),
@@ -275,15 +278,15 @@
             },
         )
 
         print(f"Dataset successfully uploaded to project key '{project_key}' with ID = {dataset_id}")
 
     def save_meta(self, endpoint: str, meta: SMT) -> SMT:
         json = self._session.put(endpoint, json=meta.to_json()).json()
-        return meta if json is None or 'uuid' not in json else meta.from_json(json)
+        return meta if json is None or "uuid" not in json else meta.from_json(json)
 
     def load_meta(self, endpoint: str, meta_class: SMT) -> TestFunctionMeta:
         return meta_class.from_json(self._session.get(endpoint).json())
 
     def get_server_info(self):
         return self._session.get("settings/ml-worker-connect").json()
```

### Comparing `giskard-2.0.0b7/giskard/client/io_utils.py` & `giskard-2.0.0b8/giskard/client/io_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/client/project.py` & `giskard-2.0.0b8/giskard/client/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from requests_toolbelt.sessions import BaseUrlSession
 
 from giskard.utils.analytics_collector import anonymize, analytics
 
 
 class Project:
-    def __init__(
-            self, session: BaseUrlSession, project_key: str, project_id: int
-    ) -> None:
+    def __init__(self, session: BaseUrlSession, project_key: str, project_id: int) -> None:
         self.project_key = project_key
         self._session = session
         self.url = self._session.base_url.replace("/api/v2/", "")
         self.project_id = project_id
 
     def _update_test_suite_params(self, actual_ds_id, reference_ds_id, model_id, test_id=None, test_suite_id=None):
         assert test_id is not None or test_suite_id is not None, "Either test_id or test_suite_id should be specified"
```

### Comparing `giskard-2.0.0b7/giskard/client/python_utils.py` & `giskard-2.0.0b8/giskard/client/python_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/commands/cli_server.py` & `giskard-2.0.0b8/giskard/commands/cli_server.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/commands/cli_worker.py` & `giskard-2.0.0b8/giskard/commands/cli_worker.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/core/core.py` & `giskard-2.0.0b8/giskard/core/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import re
 import typing
 from abc import ABC
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
+
 try:
     from types import NoneType
 except ImportError:
     # types.NoneType is only available from python >=3.10
     NoneType = type(None)
 from typing import Optional, Dict, List, Union, Literal, TypeVar, Callable, Type, Any
 
@@ -30,14 +31,15 @@
     path_parts.append(func.__name__)
     return ".".join(path_parts)
 
 
 def create_test_function_id(func):
     try:
         from giskard.ml_worker.testing.registry.registry import plugins_root
+
         # is_relative_to is only available from python 3.9
         is_relative = Path(inspect.getfile(func)).relative_to(plugins_root)
     except ValueError:
         is_relative = False
     if is_relative:
         full_name = _get_plugin_method_full_name(func)
     else:
@@ -66,17 +68,15 @@
 class SavableMeta:
     uuid: Optional[str]
 
     def __init__(self, uuid: Optional[str] = None):
         self.uuid = uuid
 
     def to_json(self):
-        return {
-            "uuid": self.uuid
-        }
+        return {"uuid": self.uuid}
 
     @classmethod
     def from_json(cls, json):
         obj = cls()
         obj.init_from_json(json)
         return obj
 
@@ -123,20 +123,22 @@
     module_doc: str
     tags: List[str]
     version: Optional[int]
     full_name: str
     type: str
     args: Dict[str, FunctionArgument]
 
-    def __init__(self,
-                 callable_obj: Union[Callable, Type] = None,
-                 name: Optional[str] = None,
-                 tags: List[str] = None,
-                 version: Optional[int] = None,
-                 type: str = None):
+    def __init__(
+        self,
+        callable_obj: Union[Callable, Type] = None,
+        name: Optional[str] = None,
+        tags: List[str] = None,
+        version: Optional[int] = None,
+        type: str = None,
+    ):
         self.version = version
         self.type = type
         self.name = name
         self.tags = tags
         self.code = None
         self.display_name = None
         self.module = None
@@ -165,20 +167,19 @@
             parameters = self.extract_parameters(callable_obj)
 
             self.args = {
                 parameter.name: FunctionArgument(
                     name=parameter.name,
                     type=extract_optional(parameter.annotation).__qualname__,
                     optional=parameter.default != inspect.Parameter.empty,
-                    default=None if parameter.default == inspect.Parameter.empty
-                    else parameter.default,
-                    argOrder=idx
+                    default=None if parameter.default == inspect.Parameter.empty else parameter.default,
+                    argOrder=idx,
                 )
                 for idx, parameter in enumerate(parameters.values())
-                if name != 'self'
+                if name != "self"
             }
 
     def extract_parameters(self, callable_obj):
         if inspect.isclass(callable_obj):
             parameters = list(inspect.signature(callable_obj.__init__).parameters.values())[1:]
         else:
             parameters = list(inspect.signature(callable_obj).parameters.values())
@@ -229,37 +230,46 @@
             "args": [
                 {
                     "name": arg.name,
                     "type": arg.type,
                     "default": arg.default,
                     "optional": arg.optional,
                     "argOrder": arg.argOrder,
-                } for arg in self.args.values()] if self.args else None
+                }
+                for arg in self.args.values()
+            ]
+            if self.args
+            else None,
         }
 
     def init_from_json(self, json: Dict[str, Any]):
         super().init_from_json(json)
         self.name = json["name"]
         self.display_name = json["displayName"]
         self.module = json["module"]
         self.doc = json["doc"]
         self.module_doc = json["moduleDoc"]
         self.code = json["code"]
         self.tags = json["tags"]
         self.version = json["version"]
         self.type = json["type"]
-        self.args = {
-            arg["name"]: FunctionArgument(
-                name=arg["name"],
-                type=arg["type"],
-                default=arg["defaultValue"],
-                optional=arg["optional"],
-                argOrder=arg["argOrder"]
-            ) for arg in json["args"]
-        } if json["args"] else None
+        self.args = (
+            {
+                arg["name"]: FunctionArgument(
+                    name=arg["name"],
+                    type=arg["type"],
+                    default=arg["defaultValue"],
+                    optional=arg["optional"],
+                    argOrder=arg["argOrder"],
+                )
+                for arg in json["args"]
+            }
+            if json["args"]
+            else None
+        )
 
 
 def __repr__(self) -> str:
     return f"CallableMeta: {self.module}.{self.name}"
 
 
 class TestFunctionMeta(CallableMeta):
@@ -276,23 +286,25 @@
 
 class DatasetProcessFunctionMeta(CallableMeta):
     cell_level: bool
     column_type: Optional[str]
     process_type: DatasetProcessFunctionType
     clauses: Optional[List[Dict[str, Any]]]
 
-    def __init__(self,
-                 callable_obj: Union[Callable, Type] = None,
-                 name: Optional[str] = None,
-                 tags: List[str] = None,
-                 version: Optional[int] = None,
-                 type: str = None,
-                 process_type: DatasetProcessFunctionType = DatasetProcessFunctionType.CODE,
-                 cell_level: bool = False,
-                 clauses: Optional[List[Dict[str, Any]]] = None):
+    def __init__(
+        self,
+        callable_obj: Union[Callable, Type] = None,
+        name: Optional[str] = None,
+        tags: List[str] = None,
+        version: Optional[int] = None,
+        type: str = None,
+        process_type: DatasetProcessFunctionType = DatasetProcessFunctionType.CODE,
+        cell_level: bool = False,
+        clauses: Optional[List[Dict[str, Any]]] = None,
+    ):
         super(DatasetProcessFunctionMeta, self).__init__(callable_obj, name, tags, version, type)
         self.cell_level = cell_level
         self.process_type = process_type
         self.clauses = clauses
 
         if cell_level:
             if inspect.isclass(callable_obj):
@@ -308,69 +320,71 @@
 
         return {p.name: p for p in parameters}
 
     def to_json(self):
         json = super().to_json()
         return {
             **json,
-            'cellLevel': self.cell_level,
-            'columnType': self.column_type,
-            'processType': self.process_type.value,
-            'clauses': self.clauses
+            "cellLevel": self.cell_level,
+            "columnType": self.column_type,
+            "processType": self.process_type.value,
+            "clauses": self.clauses,
         }
 
     def init_from_json(self, json: Dict[str, Any]):
         super().init_from_json(json)
         self.cell_level = json["cellLevel"]
         self.column_type = json["columnType"]
         self.process_type = DatasetProcessFunctionType[json["processType"]]
         self.clauses = json["clauses"]
 
 
-DT = TypeVar('DT')
-SMT = TypeVar('SMT', bound=SavableMeta)
+DT = TypeVar("DT")
+SMT = TypeVar("SMT", bound=SavableMeta)
 
 
 def unknown_annotations_to_kwargs(parameters: List[inspect.Parameter]) -> List[inspect.Parameter]:
     from giskard.models.base import BaseModel
     from giskard.datasets.base import Dataset
     from giskard.ml_worker.testing.registry.slicing_function import SlicingFunction
     from giskard.ml_worker.testing.registry.transformation_function import TransformationFunction
 
     allowed_types = [str, bool, int, float, BaseModel, Dataset, SlicingFunction, TransformationFunction]
     allowed_types = allowed_types + list(map(lambda x: Optional[x], allowed_types))
 
-    has_kwargs = any([param for param in parameters if
-                      not any([param.annotation == allowed_type for allowed_type in allowed_types])])
-
-    parameters = [param for param in parameters if
-                  any([param.annotation == allowed_type for allowed_type in allowed_types])]
+    has_kwargs = any(
+        [param for param in parameters if not any([param.annotation == allowed_type for allowed_type in allowed_types])]
+    )
+
+    parameters = [
+        param for param in parameters if any([param.annotation == allowed_type for allowed_type in allowed_types])
+    ]
 
     if has_kwargs:
-        parameters.append(inspect.Parameter(name='kwargs', kind=4, annotation=Kwargs))
+        parameters.append(inspect.Parameter(name="kwargs", kind=4, annotation=Kwargs))
 
     return parameters
 
 
 def extract_optional(field):
     if typing.get_origin(field) is Union and NoneType in typing.get_args(field):
         return Union[tuple([arg for arg in typing.get_args(field) if arg is not None and arg is not NoneType])]
     else:
         return field
 
 
 class ComparisonType(Enum):
-    IS = 'IS'
-    IS_NOT = 'IS_NOT'
-    CONTAINS = 'CONTAINS'
-    DOES_NOT_CONTAINS = 'DOES_NOT_CONTAINS'
-    STARTS_WITH = 'STARTS_WITH'
-    ENDS_WITH = 'ENDS_WITH'
-    IS_EMPTY = 'IS_EMPTY'
-    IS_NOT_EMPTY = 'IS_NOT_EMPTY'
+    IS = "IS"
+    IS_NOT = "IS_NOT"
+    CONTAINS = "CONTAINS"
+    DOES_NOT_CONTAINS = "DOES_NOT_CONTAINS"
+    STARTS_WITH = "STARTS_WITH"
+    ENDS_WITH = "ENDS_WITH"
+    IS_EMPTY = "IS_EMPTY"
+    IS_NOT_EMPTY = "IS_NOT_EMPTY"
 
 
 @dataclass
 class ComparisonClauseDTO:
     columnName: str
     comparisonType: ComparisonType
     columnDtype: str
```

### Comparing `giskard-2.0.0b7/giskard/core/dataset_validation.py` & `giskard-2.0.0b8/giskard/core/dataset_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     Args:
     df (pandas.DataFrame): The DataFrame to be checked for hashability.
 
     Raises:
     TypeError: If any column containing object types in the input DataFrame is not hashable.
     """
-    df_objects = df.select_dtypes(include='object')
+    df_objects = df.select_dtypes(include="object")
     non_hashable_cols = []
     for col in df_objects.columns:
         if not isinstance(df[col].iat[0], Hashable):
             non_hashable_cols.append(col)
 
     if non_hashable_cols:
         raise TypeError(
```

### Comparing `giskard-2.0.0b7/giskard/core/errors.py` & `giskard-2.0.0b8/giskard/core/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,12 +8,14 @@
     def __init__(self, flavor: str = None, functionality: str = None, msg: str = None) -> None:
         self.msg = msg
         if not self.msg:
             self.flavor = flavor or self.flavor
             self.functionality = functionality or self.functionality
             assert self.flavor, "Either giskard package flavor or custom error message should be provided"
 
-            self.msg = f"It seems that you are using Giskard {self.functionality or self.flavor} functionality " \
-                       f"but you are " \
-                       f"missing some required package. Please install Giskard " \
-                       f"with {self.functionality or self.flavor} support " \
-                       f"with `pip install giskard[{self.flavor}]`."
+            self.msg = (
+                f"It seems that you are using Giskard {self.functionality or self.flavor} functionality "
+                f"but you are "
+                f"missing some required package. Please install Giskard "
+                f"with {self.functionality or self.flavor} support "
+                f"with `pip install giskard[{self.flavor}]`."
+            )
```

### Comparing `giskard-2.0.0b7/giskard/core/model_validation.py` & `giskard-2.0.0b8/giskard/core/model_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,28 +131,28 @@
         with tempfile.TemporaryDirectory(prefix="giskard-model-") as f:
             model.save(f)
 
             with open(f + "/giskard-model-meta.yaml") as yaml_f:
                 saved_meta = yaml.load(yaml_f, Loader=yaml.Loader)
 
             meta = ModelMeta(
-                name=saved_meta['name'],
-                model_type=SupportedModelTypes[saved_meta['model_type']],
-                feature_names=saved_meta['feature_names'],
-                classification_labels=saved_meta['classification_labels'],
-                classification_threshold=saved_meta['threshold'],
-                loader_module=saved_meta['loader_module'],
-                loader_class=saved_meta['loader_class'],
+                name=saved_meta["name"],
+                model_type=SupportedModelTypes[saved_meta["model_type"]],
+                feature_names=saved_meta["feature_names"],
+                classification_labels=saved_meta["classification_labels"],
+                classification_threshold=saved_meta["threshold"],
+                loader_module=saved_meta["loader_module"],
+                loader_class=saved_meta["loader_class"],
             )
 
             clazz = BaseModel.determine_model_class(meta, f)
 
             constructor_params = meta.__dict__
-            del constructor_params['loader_module']
-            del constructor_params['loader_class']
+            del constructor_params["loader_module"]
+            del constructor_params["loader_class"]
 
             loaded_model = clazz.load(f, **constructor_params)
 
             return loaded_model
 
     except Exception as e:
         raise ValueError("Failed to validate model saving and loading from local disk") from e
@@ -239,15 +239,15 @@
 ):
     if target_values is not None:
         to_append = " of the model: " + model_name if model_name else ""
         target_values = list(target_values)
         if not set(target_values).issubset(set(classification_labels)):
             invalid_target_values = set(target_values) - set(classification_labels)
             raise ValueError(
-                f"Values {invalid_target_values} in \"{target_name}\" column are not declared in "
+                f'Values {invalid_target_values} in "{target_name}" column are not declared in '
                 f"classification_labels parameter {classification_labels}" + to_append
             )
 
 
 @configured_validate_arguments
 def validate_prediction_output(ds: Dataset, model_type: ModelType, prediction):
     assert len(ds.df) == len(prediction), (
```

### Comparing `giskard-2.0.0b7/giskard/core/suite.py` & `giskard-2.0.0b8/giskard/core/suite.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,26 +23,32 @@
     """
     Represents the result of a test suite, derived from the tuple class.
 
     Methods:
         _repr_html_(): Returns an HTML representation of all the tests result contained in the test suite.
 
     """
+
     def _repr_html_(self):
         passed = self[0]
-        tests_results = ''.join(
-            [f"<h3>Test: {key}</h3>{(TestResult(passed=value) if type(value) == bool else value)._repr_html_()}" for
-             key, value in self[1]])
+        tests_results = "".join(
+            [
+                f"<h3>Test: {key}</h3>{(TestResult(passed=value) if type(value) == bool else value)._repr_html_()}"
+                for key, value in self[1]
+            ]
+        )
         return """
                <h2><span style="color:{0};">{1}</span> Test suite {2}</h2>
                {3}
-               """.format('green' if passed else 'red',
-                          '\u2713' if passed else '\u00D7',
-                          'succeed' if passed else 'failed',
-                          tests_results)
+               """.format(
+            "green" if passed else "red",
+            "\u2713" if passed else "\u00D7",
+            "succeed" if passed else "failed",
+            tests_results,
+        )
 
 
 class SuiteInput:
     """
     Represents an input parameter for a test suite.
 
     Attributes:
@@ -55,19 +61,20 @@
     Example:
         >>> input_param = SuiteInput("age", int)
         >>> input_param.name
         'age'
         >>> input_param.type
         <class 'int'>
     """
+
     type: Any
     name: str
 
     def __init__(self, name: str, ptype: Any) -> None:
-        assert ptype in suite_input_types, f'Type should be one of those: {suite_input_types}'
+        assert ptype in suite_input_types, f"Type should be one of those: {suite_input_types}"
         self.name = name
         self.type = ptype
 
 
 class DatasetInput(SuiteInput):
     """
     Represents a dataset input parameter for a test suite.
@@ -83,14 +90,15 @@
         >>> dataset_input.name
         'data'
         >>> dataset_input.type
         <class 'Dataset'>
         >>> dataset_input.target
         'label'
     """
+
     target: Optional[str] = None
 
     def __init__(self, name: str, target: Optional[str] = None) -> None:
         super().__init__(name, Dataset)
         self.target = target
 
 
@@ -107,14 +115,15 @@
     Example:
         >>> model_input = ModelInput("model", model_type="SKLearnModel")
         >>> model_input.name
         'model'
         >>> model_input.model_type
         'SKLearnModel'
     """
+
     model_type: Optional[str] = None
 
     def __init__(self, name: str, model_type: Optional[str] = None) -> None:
         super().__init__(name, BaseModel)
         self.model_type = model_type
 
 
@@ -144,19 +153,23 @@
             p.upload(client, project_key)
         uploaded_uuids.append(str(p.id))
         return TestInputDTO(name=pname, value=str(p.id), type=ptype)
     elif issubclass(type(p), Artifact):
         if str(p.meta.uuid) not in uploaded_uuids:
             p.upload(client)
         uploaded_uuids.append(str(p.meta.uuid))
-        return TestInputDTO(name=pname, value=str(p.meta.uuid), type=ptype,
-                            params=[
-                                build_test_input_dto(client, value, pname, p.meta.args[pname].type, project_key,
-                                                     uploaded_uuids) for pname, value in
-                                p.params.items()])
+        return TestInputDTO(
+            name=pname,
+            value=str(p.meta.uuid),
+            type=ptype,
+            params=[
+                build_test_input_dto(client, value, pname, p.meta.args[pname].type, project_key, uploaded_uuids)
+                for pname, value in p.params.items()
+            ],
+        )
     elif isinstance(p, SuiteInput):
         return TestInputDTO(name=pname, value=p.name, is_alias=True, type=ptype)
     else:
         return TestInputDTO(name=pname, value=str(p), type=ptype)
 
 
 class Suite:
@@ -259,24 +272,29 @@
     def to_dto(self, client: GiskardClient, project_key: str):
         suite_tests: List[SuiteTestDTO] = list()
 
         # Avoid to upload the same artifacts several times
         uploaded_uuids: List[str] = []
 
         for t in self.tests:
-            suite_tests.append(SuiteTestDTO(
-                testUuid=t.giskard_test.upload(client),
-                functionInputs={
-                    pname: build_test_input_dto(client, p, pname, t.giskard_test.meta.args[pname].type, project_key,
-                                                uploaded_uuids) for pname, p in t.provided_inputs.items()}
-            ))
+            suite_tests.append(
+                SuiteTestDTO(
+                    testUuid=t.giskard_test.upload(client),
+                    functionInputs={
+                        pname: build_test_input_dto(
+                            client, p, pname, t.giskard_test.meta.args[pname].type, project_key, uploaded_uuids
+                        )
+                        for pname, p in t.provided_inputs.items()
+                    },
+                )
+            )
 
         return TestSuiteDTO(name=self.name, project_key=project_key, tests=suite_tests)
 
-    def add_test(self, test_fn: Test, test_name: Optional[Union[int, str]] = None, **params) -> 'Suite':
+    def add_test(self, test_fn: Test, test_name: Optional[Union[int, str]] = None, **params) -> "Suite":
         """
         Add a test to the suite.
 
         Args:
             test_fn (Test): A test method that will be executed or an instance of a GiskardTest class.
             test_name (Optional[Union[int, str]], optional): A unique identifier used to track the test result.
                 If None, the identifier will be generated based on the module and name of the test method.
@@ -288,16 +306,16 @@
             Suite: The current instance of the test suite to allow chained calls.
 
         """
         if isinstance(test_fn, GiskardTestMethod):
             params = {k: v for k, v in test_fn.params.items() if v is not None}
         elif isinstance(test_fn, GiskardTest):
             params = {
-                k: test_fn.__dict__[k] for k, v
-                in inspect.signature(test_fn.__init__).parameters.items()
+                k: test_fn.__dict__[k]
+                for k, v in inspect.signature(test_fn.__init__).parameters.items()
                 if test_fn.__dict__[k] is not None
             }
         else:
             test_fn = GiskardTestMethod(test_fn)
 
         if test_name is None:
             test_name = test_fn.meta.name if test_fn.meta.display_name is None else test_fn.meta.display_name
@@ -318,57 +336,69 @@
             for p in available_params:
                 if p.default == inspect.Signature.empty:
                     if p.name not in test_partial.provided_inputs:
                         res[p.name] = p.annotation
                     elif isinstance(test_partial.provided_inputs[p.name], SuiteInput):
                         if test_partial.provided_inputs[p.name].type != p.annotation:
                             raise ValueError(
-                                f'Test {test_partial.giskard_test.func.__name__} requires {p.name} input to '
-                                f'be {p.annotation.__name__} '
-                                f'but {test_partial.provided_inputs[p.name].type.__name__} was provided')
+                                f"Test {test_partial.giskard_test.func.__name__} requires {p.name} input to "
+                                f"be {p.annotation.__name__} "
+                                f"but {test_partial.provided_inputs[p.name].type.__name__} was provided"
+                            )
                         res[test_partial.provided_inputs[p.name].name] = p.annotation
         return res
 
     def generate_tests(self, inputs: List[SuiteInput]):
-        giskard_tests = [test for test in tests_registry.get_all().values()
-                         if contains_tag(test, 'giskard') and not self._contains_test(test)]
+        giskard_tests = [
+            test
+            for test in tests_registry.get_all().values()
+            if contains_tag(test, "giskard") and not self._contains_test(test)
+        ]
 
         for test in giskard_tests:
             self._add_test_if_suitable(test, inputs)
 
         return self
 
     def _add_test_if_suitable(self, test_func: TestFunctionMeta, inputs: List[SuiteInput]):
         required_args = [arg for arg in test_func.args.values() if arg.default is None]
-        input_dict: Dict[str, SuiteInput] = {
-            i.name: i
-            for i in inputs
-        }
+        input_dict: Dict[str, SuiteInput] = {i.name: i for i in inputs}
 
-        if any([arg for arg in required_args if
-                arg.name not in input_dict or arg.type != input_dict[arg.name].type.__name__]):
+        if any(
+            [
+                arg
+                for arg in required_args
+                if arg.name not in input_dict or arg.type != input_dict[arg.name].type.__name__
+            ]
+        ):
             # Test is not added if an input  without default value is not specified
             # or if an input does not match the required type
             return
 
         suite_args = {}
 
         for arg in [arg for arg in test_func.args.values() if arg.default is not None and arg.name not in input_dict]:
             # Set default value if not provided
             suite_args[arg.name] = arg.default
 
-        models = [modelInput for modelInput in input_dict.values() if
-                  isinstance(modelInput, ModelInput)
-                  and modelInput.model_type is not None and modelInput.model_type != ""]
+        models = [
+            modelInput
+            for modelInput in input_dict.values()
+            if isinstance(modelInput, ModelInput) and modelInput.model_type is not None and modelInput.model_type != ""
+        ]
         if any(models) and not contains_tag(test_func, next(iter(models)).model_type):
             return
 
-        if contains_tag(test_func, 'ground_truth') \
-                and any([dataset for dataset in input_dict.values()
-                         if isinstance(dataset, DatasetInput) and dataset.target is None and dataset.target != ""]):
+        if contains_tag(test_func, "ground_truth") and any(
+            [
+                dataset
+                for dataset in input_dict.values()
+                if isinstance(dataset, DatasetInput) and dataset.target is None and dataset.target != ""
+            ]
+        ):
             return
 
         self.add_test(GiskardTest.load(test_func.uuid, None, None).get_builder()(**suite_args))
 
     def _contains_test(self, test: TestFunctionMeta):
         return any(t.giskard_test == test for t in self.tests)
 
@@ -377,8 +407,8 @@
     return any([t for t in func.tags if t.upper() == tag.upper()])
 
 
 def format_test_result(result: Union[bool, TestResult]) -> str:
     if isinstance(result, TestResult):
         return f"{{{'passed' if result.passed else 'failed'}, metric={result.metric}}}"
     else:
-        return 'passed' if result else 'failed'
+        return "passed" if result else "failed"
```

### Comparing `giskard-2.0.0b7/giskard/core/validation.py` & `giskard-2.0.0b8/giskard/core/validation.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,12 @@
 
 
 def configured_validate_arguments(func):
     """
     Decorator to enforce a function args to be compatible with their type hints.
     :return: A wrapper function decorated by pydantic validate_arguments configured to allow arbitrary types check.
     """
-    return functools.wraps(func)(
-        validate_arguments(config=dict(arbitrary_types_allowed=True))(func)
-    )
+    return functools.wraps(func)(validate_arguments(config=dict(arbitrary_types_allowed=True))(func))
 
 
 def validate_is_pandasdataframe(df):
     assert isinstance(df, pd.DataFrame), "Dataset provided is not a pandas dataframe"
```

### Comparing `giskard-2.0.0b7/giskard/datasets/__init__.py` & `giskard-2.0.0b8/giskard/datasets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 low_stat_threshold = 100
 
 logger = logging.getLogger(__name__)
 
 
 @configured_validate_arguments
 def wrap_dataset(
-        df: pd.DataFrame,
-        name: Optional[str] = None,
-        target: Optional[str] = None,
-        cat_columns: Optional[List[str]] = None,
-        column_types: Optional[Dict[str, str]] = None,
+    df: pd.DataFrame,
+    name: Optional[str] = None,
+    target: Optional[str] = None,
+    cat_columns: Optional[List[str]] = None,
+    column_types: Optional[Dict[str, str]] = None,
 ):
     """
     A function that wraps a Pandas DataFrame into a Giskard Dataset object, with optional validation of input arguments.
 
     Args:
         df (pd.DataFrame):
             A Pandas dataframe that contains some data examples that might interest you to inspect (test set, train set,
```

### Comparing `giskard-2.0.0b7/giskard/datasets/base/__init__.py` & `giskard-2.0.0b8/giskard/datasets/base/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/datasets/metadata/indexing.py` & `giskard-2.0.0b8/giskard/datasets/metadata/indexing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/datasets/metadata/registry.py` & `giskard-2.0.0b8/giskard/datasets/metadata/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/datasets/metadata/text_metadata_provider.py` & `giskard-2.0.0b8/giskard/datasets/metadata/text_metadata_provider.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/demo/__init__.py` & `giskard-2.0.0b8/giskard/demo/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,44 +18,50 @@
     _classification_labels = {0: "no", 1: "yes"}
     df["Survived"] = df["Survived"].apply(lambda x: _classification_labels[x])
     return df
 
 
 def titanic():
     df = titanic_df()
-    cat_cols = ['Pclass', 'Sex', "SibSp", "Parch", "Embarked"]
+    cat_cols = ["Pclass", "Sex", "SibSp", "Parch", "Embarked"]
     num_cols = ["PassengerId", "Age", "Fare"]
     text_cols = ["Name"]
     target = "Survived"
 
     # tfidf the text column
-    text_transformer = Pipeline([('tfidf', TfidfVectorizer(lowercase=False, strip_accents=None))])
+    text_transformer = Pipeline([("tfidf", TfidfVectorizer(lowercase=False, strip_accents=None))])
 
     # transform and scale the numeric columns
-    num_transformer = Pipeline([('imputer', SimpleImputer(strategy='median')), ('scaler', StandardScaler())])
+    num_transformer = Pipeline([("imputer", SimpleImputer(strategy="median")), ("scaler", StandardScaler())])
 
     # one hot encode the categorical values
-    cat_transormer = Pipeline([('imputer', SimpleImputer(strategy='constant', fill_value='missing')),
-                               ('onehot', OneHotEncoder(handle_unknown='ignore',
-                                                        sparse=False))])
+    cat_transormer = Pipeline(
+        [
+            ("imputer", SimpleImputer(strategy="constant", fill_value="missing")),
+            ("onehot", OneHotEncoder(handle_unknown="ignore", sparse=False)),
+        ]
+    )
 
     # Perform preprocessing of the columns with the above pipelines
     preprocessor = ColumnTransformer(
-        transformers=[('text', text_transformer, text_cols[0]),
-                      ('num', num_transformer, num_cols),
-                      ('cat', cat_transormer, cat_cols)])
+        transformers=[
+            ("text", text_transformer, text_cols[0]),
+            ("num", num_transformer, num_cols),
+            ("cat", cat_transormer, cat_cols),
+        ]
+    )
 
     # Pipeline for the model Logistic Regression
-    clf = Pipeline(steps=[('preprocessor', preprocessor),
-                          ('classifier', LogisticRegression())])
+    clf = Pipeline(steps=[("preprocessor", preprocessor), ("classifier", LogisticRegression())])
 
     Y = df[target]
     X = df.drop(target, axis=1)
-    X_train, X_test, Y_train, Y_test = model_selection.train_test_split(X, Y, test_size=0.50, random_state=30,
-                                                                        stratify=Y)
+    X_train, X_test, Y_train, Y_test = model_selection.train_test_split(
+        X, Y, test_size=0.50, random_state=30, stratify=Y
+    )
 
     clf.fit(X_train, Y_train)
 
     test_data = pd.concat([X_test, Y_test], axis=1)
 
     return clf, test_data
 
@@ -66,16 +72,15 @@
     def preprocessor(df):
         return clf[0].transform(df)
 
     return preprocessor, clf[1]
 
 
 def linear_df():
-    df = pd.DataFrame({"x": np.arange(100),
-                       "y": np.arange(100)})
+    df = pd.DataFrame({"x": np.arange(100), "y": np.arange(100)})
     return df
 
 
 def linear():
     df = linear_df()
 
     reg = LinearRegression()
```

### Comparing `giskard-2.0.0b7/giskard/demo/titanic.csv` & `giskard-2.0.0b8/giskard/demo/titanic.csv`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/ml_worker/bridge/data_encryptor.py` & `giskard-2.0.0b8/giskard/ml_worker/bridge/data_encryptor.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/ml_worker/bridge/ml_worker_bridge.py` & `giskard-2.0.0b8/giskard/ml_worker/bridge/ml_worker_bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             logger.debug(f"handle_server_command: Writing {len(message)} bytes: {readable_hex(message)}")
             remote_writer.write(self.encryptor.encrypt(message, additional_data=self.key_id.encode()))
             await remote_writer.drain()
 
             # On Windows, we go over TCP because UDS are not supported yet.
             # Check on gRPC every once in a while for eventual support.
             if sys.platform == "win32":
-                address_parts = self.local_address.split(':')
+                address_parts = self.local_address.split(":")
                 grpc_reader, grpc_writer = await asyncio.open_connection(address_parts[0], address_parts[1])
             # On Linux, we can use Unix Domain Sockets.
             else:
                 grpc_reader, grpc_writer = await asyncio.open_unix_connection(urlparse(self.local_address).path)
 
             readers.add(grpc_reader)
             writers.add(grpc_writer)
```

### Comparing `giskard-2.0.0b7/giskard/ml_worker/core/log_listener.py` & `giskard-2.0.0b8/giskard/ml_worker/core/log_listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import io
 import logging
 import threading
 
-logger_one = logging.getLogger('shrubbery')
+logger_one = logging.getLogger("shrubbery")
 logger_two = logging.getLogger(__name__)
 
 
 class ThreadLogFilter(logging.Filter):
     thread_ident: int
 
     def __init__(self, thread_ident: int):
```

### Comparing `giskard-2.0.0b7/giskard/ml_worker/core/savable.py` & `giskard-2.0.0b8/giskard/ml_worker/core/savable.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     @abstractmethod
     def _save_locally(self, local_dit: Path):
         ...
 
     @classmethod
     @abstractmethod
-    def load(cls, local_dir: Path, uuid: str, meta: SMT) -> 'Artifact':
+    def load(cls, local_dir: Path, uuid: str, meta: SMT) -> "Artifact":
         ...
 
     @classmethod
     def _get_meta_class(cls) -> type(SMT):
         return SavableMeta
 
     @classmethod
@@ -50,24 +50,24 @@
     def _get_meta_endpoint(cls, uuid: str, project_key: Optional[str]) -> str:
         if project_key is None:
             return posixpath.join(cls._get_name(), uuid)
         else:
             return posixpath.join("project", project_key, cls._get_name(), uuid)
 
     def _save_meta_locally(self, local_dir):
-        with open(Path(local_dir) / 'meta.yaml', 'w') as f:
+        with open(Path(local_dir) / "meta.yaml", "w") as f:
             yaml.dump(self.meta, f)
 
     @classmethod
     def _load_meta_locally(cls, local_dir, uuid: str) -> Optional[SMT]:
-        file = Path(local_dir) / 'meta.yaml'
+        file = Path(local_dir) / "meta.yaml"
         if not file.exists():
             return None
 
-        with open(file, 'r') as f:
+        with open(file, "r") as f:
             return cls._get_meta_class(**yaml.load(f, Loader=yaml.FullLoader))
 
     def upload(self, client: GiskardClient, project_key: Optional[str] = None) -> str:
         """
         Uploads the slicing function and its metadata to the Giskard server.
 
         Args:
@@ -89,15 +89,15 @@
 
         client.log_artifacts(local_dir, posixpath.join(project_key or "global", self._get_name(), self.meta.uuid))
         self.meta = client.save_meta(self._get_meta_endpoint(self.meta.uuid, project_key), self.meta)
 
         return self.meta.uuid
 
     @classmethod
-    def download(cls, uuid: str, client: Optional[GiskardClient], project_key: Optional[str]) -> 'Artifact':
+    def download(cls, uuid: str, client: Optional[GiskardClient], project_key: Optional[str]) -> "Artifact":
         """
         Downloads the artifact from the Giskard server or retrieves it from the local cache.
 
         Args:
             uuid (str): The UUID of the artifact to download.
             client (GiskardClient, optional): The Giskard client instance used for communication with the server. If None,
                 the artifact will be retrieved from the local cache if available. Defaults to None.
@@ -130,40 +130,39 @@
             client.load_artifact(local_dir, posixpath.join(project_key or "global", name, uuid))
             data = cls.load(local_dir, uuid, meta)
 
         return data
 
 
 class RegistryArtifact(Artifact[SMT], ABC):
-
     def _save_locally(self, local_dir: Path):
-        with open(Path(local_dir) / 'data.pkl', 'wb') as f:
+        with open(Path(local_dir) / "data.pkl", "wb") as f:
             cloudpickle.dump(self, f, protocol=pickle.DEFAULT_PROTOCOL)
 
     @classmethod
     def _load_meta_locally(cls, local_dir, uuid: str) -> Optional[SMT]:
         meta = tests_registry.get_test(uuid)
 
         if meta is not None:
             return meta
 
         return super()._load_meta_locally(local_dir, uuid)
 
     @classmethod
     def load(cls, local_dir: Path, uuid: str, meta: SMT):
-        _function: Optional['RegistryArtifact']
+        _function: Optional["RegistryArtifact"]
 
         if local_dir.exists():
-            with open(local_dir / 'data.pkl', 'rb') as f:
+            with open(local_dir / "data.pkl", "rb") as f:
                 _function = cloudpickle.load(f)
         else:
             try:
                 func = getattr(sys.modules[meta.module], meta.name)
 
-                if inspect.isclass(func) or hasattr(func, 'meta'):
+                if inspect.isclass(func) or hasattr(func, "meta"):
                     _function = func()
                 else:
                     _function = cls(func)
                     _function.meta = meta
             except Exception:
                 return None
```

### Comparing `giskard-2.0.0b7/giskard/ml_worker/generated/ml_worker_pb2.py` & `giskard-2.0.0b8/giskard/ml_worker/generated/ml_worker_pb2.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/ml_worker/generated/ml_worker_pb2_grpc.py` & `giskard-2.0.0b8/giskard/ml_worker/generated/ml_worker_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/ml_worker/ml_worker.py` & `giskard-2.0.0b8/giskard/ml_worker/ml_worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,16 +35,16 @@
         from giskard.ml_worker.generated.ml_worker_pb2_grpc import add_MLWorkerServicer_to_server
         from giskard.ml_worker.server.ml_worker_service import MLWorkerServiceImpl
         from giskard.ml_worker.utils.network import find_free_port
 
         server = grpc.aio.server(
             interceptors=[MLWorkerRequestInterceptor()],
             options=[
-                ("grpc.max_send_message_length", settings.max_send_message_length_mb * 1024 ** 2),
-                ("grpc.max_receive_message_length", settings.max_receive_message_length_mb * 1024 ** 2),
+                ("grpc.max_send_message_length", settings.max_send_message_length_mb * 1024**2),
+                ("grpc.max_receive_message_length", settings.max_receive_message_length_mb * 1024**2),
             ],
         )
 
         if is_server:
             port = settings.port if settings.port else find_free_port()
             address = f"{settings.host}:{port}"
         else:
```

### Comparing `giskard-2.0.0b7/giskard/ml_worker/server/ml_worker_service.py` & `giskard-2.0.0b8/giskard/ml_worker/server/ml_worker_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,21 +63,17 @@
             doc=test.doc,
             code=test.code,
             moduleDoc=test.module_doc,
             tags=test.tags,
             type=test.type,
             args=[
                 ml_worker_pb2.TestFunctionArgument(
-                    name=a.name,
-                    type=a.type,
-                    optional=a.optional,
-                    default=str(a.default),
-                    argOrder=a.argOrder
-                ) for a
-                in test.args.values()
+                    name=a.name, type=a.type, optional=a.optional, default=str(a.default), argOrder=a.argOrder
+                )
+                for a in test.args.values()
             ],
         )
         for test in tests_registry.get_all().values()
         if test.type == callable_type
     }
 
 
@@ -91,34 +87,31 @@
             doc=test.doc,
             code=test.code,
             moduleDoc=test.module_doc,
             tags=test.tags,
             type=test.type,
             args=[
                 ml_worker_pb2.TestFunctionArgument(
-                    name=a.name,
-                    type=a.type,
-                    optional=a.optional,
-                    default=str(a.default),
-                    argOrder=a.argOrder
-                ) for a
-                in test.args.values()
+                    name=a.name, type=a.type, optional=a.optional, default=str(a.default), argOrder=a.argOrder
+                )
+                for a in test.args.values()
             ],
             cellLevel=test.cell_level,
             columnType=test.column_type,
-            processType=test.process_type.name
+            processType=test.process_type.name,
         )
         for test in tests_registry.get_all().values()
         if test.type == callable_type
     }
 
 
 class MLWorkerServiceImpl(MLWorkerServicer):
-    def __init__(self, ml_worker: MLWorker, client: GiskardClient, address=None, remote=None,
-                 loop=asyncio.get_event_loop()) -> None:
+    def __init__(
+        self, ml_worker: MLWorker, client: GiskardClient, address=None, remote=None, loop=asyncio.get_event_loop()
+    ) -> None:
         super().__init__()
         self.ml_worker = ml_worker
         self.address = address
         self.remote = remote
         self.client = client
         self.loop = loop
 
@@ -186,139 +179,148 @@
             is_remote=self.remote,
         )
 
     def echo(self, request: ml_worker_pb2.EchoMsg, context: grpc.ServicerContext) -> ml_worker_pb2.EchoMsg:
         return request
 
     def runAdHocTest(
-            self, request: ml_worker_pb2.RunAdHocTestRequest, context: grpc.ServicerContext
+        self, request: ml_worker_pb2.RunAdHocTestRequest, context: grpc.ServicerContext
     ) -> ml_worker_pb2.TestResultMessage:
-
         test: GiskardTest = GiskardTest.download(request.testUuid, self.client, None)
 
         arguments = self.parse_function_arguments(request.arguments)
 
         logger.info(f"Executing {test.meta.display_name or f'{test.meta.module}.{test.meta.name}'}")
         test_result = test.get_builder()(**arguments).execute()
 
-        return ml_worker_pb2.TestResultMessage(results=[
-            ml_worker_pb2.NamedSingleTestResult(testUuid=test.meta.uuid,
-                                                result=map_result_to_single_test_result(test_result))
-        ])
+        return ml_worker_pb2.TestResultMessage(
+            results=[
+                ml_worker_pb2.NamedSingleTestResult(
+                    testUuid=test.meta.uuid, result=map_result_to_single_test_result(test_result)
+                )
+            ]
+        )
 
     def datasetProcessing(
-            self, request: ml_worker_pb2.DatasetProcessingRequest, context: grpc.ServicerContext
+        self, request: ml_worker_pb2.DatasetProcessingRequest, context: grpc.ServicerContext
     ) -> ml_worker_pb2.DatasetProcessingResultMessage:
         dataset = Dataset.download(self.client, request.dataset.project_key, request.dataset.id, request.dataset.sample)
 
         for function in request.functions:
             arguments = self.parse_function_arguments(function.arguments)
             if function.HasField("slicingFunction"):
                 dataset.add_slicing_function(
-                    SlicingFunction.download(function.slicingFunction.id, self.client, None)(**arguments))
+                    SlicingFunction.download(function.slicingFunction.id, self.client, None)(**arguments)
+                )
             else:
                 dataset.add_transformation_function(
-                    TransformationFunction.download(function.transformationFunction.id, self.client, None)(**arguments))
+                    TransformationFunction.download(function.transformationFunction.id, self.client, None)(**arguments)
+                )
 
         result = dataset.process()
 
         filtered_rows_idx = dataset.df.index.difference(result.df.index)
-        modified_rows = result.df[dataset.df.iloc[result.df.index].ne(result.df)].dropna(how='all')
+        modified_rows = result.df[dataset.df.iloc[result.df.index].ne(result.df)].dropna(how="all")
 
         return ml_worker_pb2.DatasetProcessingResultMessage(
             datasetId=request.dataset.id,
             totalRows=len(dataset.df.index),
             filteredRows=filtered_rows_idx,
             modifications=[
                 ml_worker_pb2.DatasetRowModificationResult(
                     rowId=row[0],
-                    modifications={key: str(value) for key, value in row[1].items() if
-                                   not type(value) == float or not math.isnan(value)}
+                    modifications={
+                        key: str(value)
+                        for key, value in row[1].items()
+                        if not type(value) == float or not math.isnan(value)
+                    },
                 )
-                for row
-                in modified_rows.iterrows()
-            ]
+                for row in modified_rows.iterrows()
+            ],
         )
 
-    def runTestSuite(self, request: ml_worker_pb2.RunTestSuiteRequest,
-                     context: grpc.ServicerContext) -> ml_worker_pb2.TestSuiteResultMessage:
+    def runTestSuite(
+        self, request: ml_worker_pb2.RunTestSuiteRequest, context: grpc.ServicerContext
+    ) -> ml_worker_pb2.TestSuiteResultMessage:
         log_listener = LogListener()
         try:
-            tests = [{
-                'test': GiskardTest.download(t.testUuid, self.client, None),
-                'arguments': self.parse_function_arguments(t.arguments),
-                'id': t.id
-            } for t in request.tests]
+            tests = [
+                {
+                    "test": GiskardTest.download(t.testUuid, self.client, None),
+                    "arguments": self.parse_function_arguments(t.arguments),
+                    "id": t.id,
+                }
+                for t in request.tests
+            ]
 
             global_arguments = self.parse_function_arguments(request.globalArguments)
 
             test_names = list(
-                map(lambda t: t['test'].meta.display_name or f"{t['test'].meta.module + '.' + t['test'].meta.name}",
-                    tests)
+                map(
+                    lambda t: t["test"].meta.display_name or f"{t['test'].meta.module + '.' + t['test'].meta.name}",
+                    tests,
+                )
             )
             logger.info(f"Executing test suite: {test_names}")
 
             suite = Suite()
             for t in tests:
-                suite.add_test(t['test'].get_builder()(**t['arguments']), t['id'])
+                suite.add_test(t["test"].get_builder()(**t["arguments"]), t["id"])
 
             is_pass, results = suite.run(**global_arguments)
 
             identifier_single_test_results = []
             for identifier, result in results:
                 identifier_single_test_results.append(
                     ml_worker_pb2.IdentifierSingleTestResult(
                         id=identifier, result=map_result_to_single_test_result(result)
                     )
                 )
 
             return ml_worker_pb2.TestSuiteResultMessage(
-                is_error=False,
-                is_pass=is_pass,
-                results=identifier_single_test_results,
-                logs=log_listener.close()
+                is_error=False, is_pass=is_pass, results=identifier_single_test_results, logs=log_listener.close()
             )
 
         except Exception as exc:
             logger.exception("An error occurred during the test suite execution: %s", exc)
             return ml_worker_pb2.TestSuiteResultMessage(
-                is_error=True,
-                is_pass=False,
-                results=[],
-                logs=log_listener.close()
+                is_error=True, is_pass=False, results=[], logs=log_listener.close()
             )
 
     def parse_function_arguments(self, request_arguments):
         arguments = dict()
 
         for arg in request_arguments:
             if arg.none:
                 continue
             if arg.HasField("dataset"):
-                arguments[arg.name] = Dataset.download(self.client, arg.dataset.project_key, arg.dataset.id,
-                                                       arg.dataset.sample)
+                arguments[arg.name] = Dataset.download(
+                    self.client, arg.dataset.project_key, arg.dataset.id, arg.dataset.sample
+                )
             elif arg.HasField("model"):
                 arguments[arg.name] = BaseModel.download(self.client, arg.model.project_key, arg.model.id)
             elif arg.HasField("slicingFunction"):
                 arguments[arg.name] = SlicingFunction.download(arg.slicingFunction.id, self.client, None)(
-                    **self.parse_function_arguments(arg.args))
+                    **self.parse_function_arguments(arg.args)
+                )
             elif arg.HasField("transformationFunction"):
                 arguments[arg.name] = TransformationFunction.download(arg.transformationFunction.id, self.client, None)(
-                    **self.parse_function_arguments(arg.args))
+                    **self.parse_function_arguments(arg.args)
+                )
             elif arg.HasField("float"):
                 arguments[arg.name] = float(arg.float)
             elif arg.HasField("int"):
                 arguments[arg.name] = int(arg.int)
             elif arg.HasField("str"):
                 arguments[arg.name] = str(arg.str)
             elif arg.HasField("bool"):
                 arguments[arg.name] = bool(arg.bool)
             elif arg.HasField("kwargs"):
                 kwargs = dict()
-                exec(arg.kwargs, {'kwargs': kwargs})
+                exec(arg.kwargs, {"kwargs": kwargs})
                 arguments.update(kwargs)
             else:
                 raise IllegalArgumentError("Unknown argument type")
         return arguments
 
     def explain(self, request: ml_worker_pb2.ExplainRequest, context) -> ml_worker_pb2.ExplainResponse:
         model = BaseModel.download(self.client, request.model.project_key, request.model.id)
@@ -354,33 +356,36 @@
             },
             words=list_words,
         )
 
     def runModelForDataFrame(self, request: ml_worker_pb2.RunModelForDataFrameRequest, context):
         model = BaseModel.download(self.client, request.model.project_key, request.model.id)
         df = pd.DataFrame.from_records([r.columns for r in request.dataframe.rows])
-        ds = Dataset(model.prepare_dataframe(df, column_dtypes=request.column_dtypes),
-                     target=None,
-                     column_types=request.column_types)
+        ds = Dataset(
+            model.prepare_dataframe(df, column_dtypes=request.column_dtypes),
+            target=None,
+            column_types=request.column_types,
+        )
         predictions = model.predict(ds)
         if model.is_classification:
             return ml_worker_pb2.RunModelForDataFrameResponse(
                 all_predictions=self.pandas_df_to_proto_df(predictions.all_predictions),
                 prediction=predictions.prediction.astype(str),
             )
         else:
             return ml_worker_pb2.RunModelForDataFrameResponse(
                 prediction=predictions.prediction.astype(str), raw_prediction=predictions.prediction
             )
 
     def runModel(self, request: ml_worker_pb2.RunModelRequest, context) -> ml_worker_pb2.RunModelResponse:
         try:
             model = BaseModel.download(self.client, request.model.project_key, request.model.id)
-            dataset = Dataset.download(self.client, request.dataset.project_key, request.dataset.id,
-                                       sample=request.dataset.sample)
+            dataset = Dataset.download(
+                self.client, request.dataset.project_key, request.dataset.id, sample=request.dataset.sample
+            )
         except ValueError as e:
             if "unsupported pickle protocol" in str(e):
                 raise ValueError(
                     "Unable to unpickle object, "
                     "Make sure that Python version of client code is the same as the Python version in ML Worker."
                     "To change Python version, please refer to https://docs.giskard.ai/start/guides/configuration"
                     f"\nOriginal Error: {e}"
@@ -420,21 +425,23 @@
             else:
                 calculated = pd.concat([preds_serie], axis=1)
 
         with tempfile.TemporaryDirectory(prefix="giskard-") as f:
             dir = Path(f)
             predictions_csv = get_file_name("predictions", "csv", request.dataset.sample)
             results.to_csv(index=False, path_or_buf=dir / predictions_csv)
-            self.ml_worker.tunnel.client.log_artifact(dir / predictions_csv,
-                                                      f"{request.project_key}/models/inspections/{request.inspectionId}")
+            self.ml_worker.tunnel.client.log_artifact(
+                dir / predictions_csv, f"{request.project_key}/models/inspections/{request.inspectionId}"
+            )
 
             calculated_csv = get_file_name("calculated", "csv", request.dataset.sample)
             calculated.to_csv(index=False, path_or_buf=dir / calculated_csv)
-            self.ml_worker.tunnel.client.log_artifact(dir / calculated_csv,
-                                                      f"{request.project_key}/models/inspections/{request.inspectionId}")
+            self.ml_worker.tunnel.client.log_artifact(
+                dir / calculated_csv, f"{request.project_key}/models/inspections/{request.inspectionId}"
+            )
         return google.protobuf.empty_pb2.Empty()
 
     def filterDataset(self, request_iterator, context: grpc.ServicerContext):
         filterfunc = {}
         meta = None
 
         times = []  # This is an array of chunk execution times for performance stats
@@ -483,66 +490,66 @@
                 )
 
         logger.info(f"Filter dataset finished. Avg chunk time: {sum(times) / len(times)}")
         yield ml_worker_pb2.FilterDatasetResponse(code=ml_worker_pb2.StatusCode.Ok)
 
     @staticmethod
     def map_suite_input(i: ml_worker_pb2.SuiteInput):
-        if i.type == 'Model' and i.model_meta is not None:
+        if i.type == "Model" and i.model_meta is not None:
             return ModelInput(i.name, i.model_meta.model_type)
-        elif i.type == 'Dataset' and i.dataset_meta is not None:
+        elif i.type == "Dataset" and i.dataset_meta is not None:
             return DatasetInput(i.name, i.dataset_meta.target)
         else:
             return SuiteInput(i.name, i.type)
 
     def generateTestSuite(
-            self,
-            request: ml_worker_pb2.GenerateTestSuiteRequest,
-            context: grpc.ServicerContext,
+        self,
+        request: ml_worker_pb2.GenerateTestSuiteRequest,
+        context: grpc.ServicerContext,
     ) -> ml_worker_pb2.GenerateTestSuiteResponse:
         inputs = [self.map_suite_input(i) for i in request.inputs]
 
         suite = Suite().generate_tests(inputs).to_dto(self.client, request.project_key)
 
         return ml_worker_pb2.GenerateTestSuiteResponse(
             tests=[
                 ml_worker_pb2.GeneratedTest(
                     test_uuid=test.testUuid,
                     inputs=[
-                        ml_worker_pb2.GeneratedTestInput(
-                            name=i.name,
-                            value=i.value,
-                            is_alias=i.is_alias
-                        )
+                        ml_worker_pb2.GeneratedTestInput(name=i.name, value=i.value, is_alias=i.is_alias)
                         for i in test.functionInputs.values()
-                    ]
+                    ],
                 )
                 for test in suite.tests
             ]
         )
 
-    def stopWorker(self, request: google.protobuf.empty_pb2.Empty,
-                   context: grpc.ServicerContext) -> google.protobuf.empty_pb2.Empty:
-        logger.info('Received request to stop the worker')
+    def stopWorker(
+        self, request: google.protobuf.empty_pb2.Empty, context: grpc.ServicerContext
+    ) -> google.protobuf.empty_pb2.Empty:
+        logger.info("Received request to stop the worker")
         self.loop.create_task(self.ml_worker.stop())
         return google.protobuf.empty_pb2.Empty()
 
-    def getCatalog(self, request: google.protobuf.empty_pb2.Empty,
-                   context: grpc.ServicerContext) -> ml_worker_pb2.CatalogResponse:
+    def getCatalog(
+        self, request: google.protobuf.empty_pb2.Empty, context: grpc.ServicerContext
+    ) -> ml_worker_pb2.CatalogResponse:
         return ml_worker_pb2.CatalogResponse(
-            tests=map_function_meta('TEST'),
-            slices=map_dataset_process_function_meta('SLICE'),
-            transformations=map_dataset_process_function_meta('TRANSFORMATION')
+            tests=map_function_meta("TEST"),
+            slices=map_dataset_process_function_meta("SLICE"),
+            transformations=map_dataset_process_function_meta("TRANSFORMATION"),
         )
 
     @staticmethod
     def pandas_df_to_proto_df(df):
         return ml_worker_pb2.DataFrame(
-            rows=[ml_worker_pb2.DataRow(columns={str(k): v for k, v in r.astype(str).to_dict().items()}) for _, r in
-                  df.iterrows()]
+            rows=[
+                ml_worker_pb2.DataRow(columns={str(k): v for k, v in r.astype(str).to_dict().items()})
+                for _, r in df.iterrows()
+            ]
         )
 
     @staticmethod
     def pandas_series_to_proto_series(self, series):
         return
 
 
@@ -556,15 +563,17 @@
                 ml_worker_pb2.TestMessage(
                     type=ml_worker_pb2.TestMessageType.ERROR
                     if message.type == TestMessageLevel.ERROR
                     else ml_worker_pb2.TestMessageType.INFO,
                     text=message.text,
                 )
                 for message in result.messages
-            ] if result.messages is not None else [],
+            ]
+            if result.messages is not None
+            else [],
             props=result.props,
             metric=result.metric,
             missing_count=result.missing_count,
             missing_percent=result.missing_percent,
             unexpected_count=result.unexpected_count,
             unexpected_percent=result.unexpected_percent,
             unexpected_percent_total=result.unexpected_percent_total,
```

### Comparing `giskard-2.0.0b7/giskard/ml_worker/testing/functions/slicing.py` & `giskard-2.0.0b8/giskard/ml_worker/testing/functions/slicing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List
 
 import pandas as pd
 
 from giskard.ml_worker.testing.registry.slicing_function import slicing_function
 
 
-@slicing_function(name='Short comment', tags=["text"], cell_level=True)
+@slicing_function(name="Short comment", tags=["text"], cell_level=True)
 def short_comment_slicing_fn(text: str, max_words: int = 5) -> bool:
     """
     Filter the rows where the specified 'column_name' contains a short comment, defined as one with at most 'max_words'.
     """
     return not pd.isnull(text) and len(text.split()) <= max_words
 
 
@@ -60,20 +60,20 @@
     Possible emotion are: 'optimism', 'anger', 'sadness', 'joy'
     """
     return _sentiment_analysis(x, column_name, threshold, "cardiffnlp/twitter-roberta-base-emotion", emotion)
 
 
 def _sentiment_analysis(x, column_name, threshold, model, emotion):
     from transformers import pipeline
+
     sentiment_pipeline = pipeline("sentiment-analysis", model=model)
     # Limit text to 512 characters
     sentences = list(map(lambda txt: txt[:512], list(x[column_name])))
-    return x.iloc[list(
-        map(lambda s: s['label'] == emotion and s['score'] >= threshold, sentiment_pipeline(sentences)))]
+    return x.iloc[list(map(lambda s: s["label"] == emotion and s["score"] >= threshold, sentiment_pipeline(sentences)))]
 
 
-@slicing_function(name='Outlier Filter', tags=['number'], cell_level=True)
+@slicing_function(name="Outlier Filter", tags=["number"], cell_level=True)
 def outlier_filter(value: float, lower_bound: float, upper_bound: float) -> bool:
     """
     Filter rows where the specified column values fall outside the specified range.
     """
     return not pd.isnull(value) and (value < lower_bound or value > upper_bound)
```

### Comparing `giskard-2.0.0b7/giskard/ml_worker/testing/functions/transformation.py` & `giskard-2.0.0b8/giskard/ml_worker/testing/functions/transformation.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,47 +5,48 @@
 
 import numpy as np
 import pandas as pd
 
 from giskard.ml_worker.testing.registry.transformation_function import transformation_function
 
 nearbykeys = {
-    'a': ['q', 'w', 's', 'x', 'z'],
-    'b': ['v', 'g', 'h', 'n'],
-    'c': ['x', 'd', 'f', 'v'],
-    'd': ['s', 'e', 'r', 'f', 'c', 'x'],
-    'e': ['w', 's', 'd', 'r'],
-    'f': ['d', 'r', 't', 'g', 'v', 'c'],
-    'g': ['f', 't', 'y', 'h', 'b', 'v'],
-    'h': ['g', 'y', 'u', 'j', 'n', 'b'],
-    'i': ['u', 'j', 'k', 'o'],
-    'j': ['h', 'u', 'i', 'k', 'n', 'm'],
-    'k': ['j', 'i', 'o', 'l', 'm'],
-    'l': ['k', 'o', 'p'],
-    'm': ['n', 'j', 'k', 'l'],
-    'n': ['b', 'h', 'j', 'm'],
-    'o': ['i', 'k', 'l', 'p'],
-    'p': ['o', 'l'],
-    'q': ['w', 'a', 's'],
-    'r': ['e', 'd', 'f', 't'],
-    's': ['w', 'e', 'd', 'x', 'z', 'a'],
-    't': ['r', 'f', 'g', 'y'],
-    'u': ['y', 'h', 'j', 'i'],
-    'v': ['c', 'f', 'g', 'v', 'b'],
-    'w': ['q', 'a', 's', 'e'],
-    'x': ['z', 's', 'd', 'c'],
-    'y': ['t', 'g', 'h', 'u'],
-    'z': ['a', 's', 'x'],
+    "a": ["q", "w", "s", "x", "z"],
+    "b": ["v", "g", "h", "n"],
+    "c": ["x", "d", "f", "v"],
+    "d": ["s", "e", "r", "f", "c", "x"],
+    "e": ["w", "s", "d", "r"],
+    "f": ["d", "r", "t", "g", "v", "c"],
+    "g": ["f", "t", "y", "h", "b", "v"],
+    "h": ["g", "y", "u", "j", "n", "b"],
+    "i": ["u", "j", "k", "o"],
+    "j": ["h", "u", "i", "k", "n", "m"],
+    "k": ["j", "i", "o", "l", "m"],
+    "l": ["k", "o", "p"],
+    "m": ["n", "j", "k", "l"],
+    "n": ["b", "h", "j", "m"],
+    "o": ["i", "k", "l", "p"],
+    "p": ["o", "l"],
+    "q": ["w", "a", "s"],
+    "r": ["e", "d", "f", "t"],
+    "s": ["w", "e", "d", "x", "z", "a"],
+    "t": ["r", "f", "g", "y"],
+    "u": ["y", "h", "j", "i"],
+    "v": ["c", "f", "g", "v", "b"],
+    "w": ["q", "a", "s", "e"],
+    "x": ["z", "s", "d", "c"],
+    "y": ["t", "g", "h", "u"],
+    "z": ["a", "s", "x"],
 }
 
 gruber = re.compile(
-    r"""(?i)\b((?:https?:(?:/{1,3}|[a-z0-9%])|[a-z0-9.\-]+[.](?:com|net|org|edu|gov|mil|aero|asia|biz|cat|coop|info|int|jobs|mobi|museum|name|post|pro|tel|travel|xxx|ac|ad|ae|af|ag|ai|al|am|an|ao|aq|ar|as|at|au|aw|ax|az|ba|bb|bd|be|bf|bg|bh|bi|bj|bm|bn|bo|br|bs|bt|bv|bw|by|bz|ca|cc|cd|cf|cg|ch|ci|ck|cl|cm|cn|co|cr|cs|cu|cv|cx|cy|cz|dd|de|dj|dk|dm|do|dz|ec|ee|eg|eh|er|es|et|eu|fi|fj|fk|fm|fo|fr|ga|gb|gd|ge|gf|gg|gh|gi|gl|gm|gn|gp|gq|gr|gs|gt|gu|gw|gy|hk|hm|hn|hr|ht|hu|id|ie|il|im|in|io|iq|ir|is|it|je|jm|jo|jp|ke|kg|kh|ki|km|kn|kp|kr|kw|ky|kz|la|lb|lc|li|lk|lr|ls|lt|lu|lv|ly|ma|mc|md|me|mg|mh|mk|ml|mm|mn|mo|mp|mq|mr|ms|mt|mu|mv|mw|mx|my|mz|na|nc|ne|nf|ng|ni|nl|no|np|nr|nu|nz|om|pa|pe|pf|pg|ph|pk|pl|pm|pn|pr|ps|pt|pw|py|qa|re|ro|rs|ru|rw|sa|sb|sc|sd|se|sg|sh|si|sj|Ja|sk|sl|sm|sn|so|sr|ss|st|su|sv|sx|sy|sz|tc|td|tf|tg|th|tj|tk|tl|tm|tn|to|tp|tr|tt|tv|tw|tz|ua|ug|uk|us|uy|uz|va|vc|ve|vg|vi|vn|vu|wf|ws|ye|yt|yu|za|zm|zw)/)(?:[^\s()<>{}\[\]]+|\([^\s()]*?\([^\s()]+\)[^\s()]*?\)|\([^\s]+?\))+(?:\([^\s()]*?\([^\s()]+\)[^\s()]*?\)|\([^\s]+?\)|[^\s`!()\[\]{};:'".,<>?«»“”‘’])|(?:(?<!@)[a-z0-9]+(?:[.\-][a-z0-9]+)*[.](?:com|net|org|edu|gov|mil|aero|asia|biz|cat|coop|info|int|jobs|mobi|museum|name|post|pro|tel|travel|xxx|ac|ad|ae|af|ag|ai|al|am|an|ao|aq|ar|as|at|au|aw|ax|az|ba|bb|bd|be|bf|bg|bh|bi|bj|bm|bn|bo|br|bs|bt|bv|bw|by|bz|ca|cc|cd|cf|cg|ch|ci|ck|cl|cm|cn|co|cr|cs|cu|cv|cx|cy|cz|dd|de|dj|dk|dm|do|dz|ec|ee|eg|eh|er|es|et|eu|fi|fj|fk|fm|fo|fr|ga|gb|gd|ge|gf|gg|gh|gi|gl|gm|gn|gp|gq|gr|gs|gt|gu|gw|gy|hk|hm|hn|hr|ht|hu|id|ie|il|im|in|io|iq|ir|is|it|je|jm|jo|jp|ke|kg|kh|ki|km|kn|kp|kr|kw|ky|kz|la|lb|lc|li|lk|lr|ls|lt|lu|lv|ly|ma|mc|md|me|mg|mh|mk|ml|mm|mn|mo|mp|mq|mr|ms|mt|mu|mv|mw|mx|my|mz|na|nc|ne|nf|ng|ni|nl|no|np|nr|nu|nz|om|pa|pe|pf|pg|ph|pk|pl|pm|pn|pr|ps|pt|pw|py|qa|re|ro|rs|ru|rw|sa|sb|sc|sd|se|sg|sh|si|sj|Ja|sk|sl|sm|sn|so|sr|ss|st|su|sv|sx|sy|sz|tc|td|tf|tg|th|tj|tk|tl|tm|tn|to|tp|tr|tt|tv|tw|tz|ua|ug|uk|us|uy|uz|va|vc|ve|vg|vi|vn|vu|wf|ws|ye|yt|yu|za|zm|zw)\b/?(?!@)))""")  # noqa
+    r"""(?i)\b((?:https?:(?:/{1,3}|[a-z0-9%])|[a-z0-9.\-]+[.](?:com|net|org|edu|gov|mil|aero|asia|biz|cat|coop|info|int|jobs|mobi|museum|name|post|pro|tel|travel|xxx|ac|ad|ae|af|ag|ai|al|am|an|ao|aq|ar|as|at|au|aw|ax|az|ba|bb|bd|be|bf|bg|bh|bi|bj|bm|bn|bo|br|bs|bt|bv|bw|by|bz|ca|cc|cd|cf|cg|ch|ci|ck|cl|cm|cn|co|cr|cs|cu|cv|cx|cy|cz|dd|de|dj|dk|dm|do|dz|ec|ee|eg|eh|er|es|et|eu|fi|fj|fk|fm|fo|fr|ga|gb|gd|ge|gf|gg|gh|gi|gl|gm|gn|gp|gq|gr|gs|gt|gu|gw|gy|hk|hm|hn|hr|ht|hu|id|ie|il|im|in|io|iq|ir|is|it|je|jm|jo|jp|ke|kg|kh|ki|km|kn|kp|kr|kw|ky|kz|la|lb|lc|li|lk|lr|ls|lt|lu|lv|ly|ma|mc|md|me|mg|mh|mk|ml|mm|mn|mo|mp|mq|mr|ms|mt|mu|mv|mw|mx|my|mz|na|nc|ne|nf|ng|ni|nl|no|np|nr|nu|nz|om|pa|pe|pf|pg|ph|pk|pl|pm|pn|pr|ps|pt|pw|py|qa|re|ro|rs|ru|rw|sa|sb|sc|sd|se|sg|sh|si|sj|Ja|sk|sl|sm|sn|so|sr|ss|st|su|sv|sx|sy|sz|tc|td|tf|tg|th|tj|tk|tl|tm|tn|to|tp|tr|tt|tv|tw|tz|ua|ug|uk|us|uy|uz|va|vc|ve|vg|vi|vn|vu|wf|ws|ye|yt|yu|za|zm|zw)/)(?:[^\s()<>{}\[\]]+|\([^\s()]*?\([^\s()]+\)[^\s()]*?\)|\([^\s]+?\))+(?:\([^\s()]*?\([^\s()]+\)[^\s()]*?\)|\([^\s]+?\)|[^\s`!()\[\]{};:'".,<>?«»“”‘’])|(?:(?<!@)[a-z0-9]+(?:[.\-][a-z0-9]+)*[.](?:com|net|org|edu|gov|mil|aero|asia|biz|cat|coop|info|int|jobs|mobi|museum|name|post|pro|tel|travel|xxx|ac|ad|ae|af|ag|ai|al|am|an|ao|aq|ar|as|at|au|aw|ax|az|ba|bb|bd|be|bf|bg|bh|bi|bj|bm|bn|bo|br|bs|bt|bv|bw|by|bz|ca|cc|cd|cf|cg|ch|ci|ck|cl|cm|cn|co|cr|cs|cu|cv|cx|cy|cz|dd|de|dj|dk|dm|do|dz|ec|ee|eg|eh|er|es|et|eu|fi|fj|fk|fm|fo|fr|ga|gb|gd|ge|gf|gg|gh|gi|gl|gm|gn|gp|gq|gr|gs|gt|gu|gw|gy|hk|hm|hn|hr|ht|hu|id|ie|il|im|in|io|iq|ir|is|it|je|jm|jo|jp|ke|kg|kh|ki|km|kn|kp|kr|kw|ky|kz|la|lb|lc|li|lk|lr|ls|lt|lu|lv|ly|ma|mc|md|me|mg|mh|mk|ml|mm|mn|mo|mp|mq|mr|ms|mt|mu|mv|mw|mx|my|mz|na|nc|ne|nf|ng|ni|nl|no|np|nr|nu|nz|om|pa|pe|pf|pg|ph|pk|pl|pm|pn|pr|ps|pt|pw|py|qa|re|ro|rs|ru|rw|sa|sb|sc|sd|se|sg|sh|si|sj|Ja|sk|sl|sm|sn|so|sr|ss|st|su|sv|sx|sy|sz|tc|td|tf|tg|th|tj|tk|tl|tm|tn|to|tp|tr|tt|tv|tw|tz|ua|ug|uk|us|uy|uz|va|vc|ve|vg|vi|vn|vu|wf|ws|ye|yt|yu|za|zm|zw)\b/?(?!@)))"""
+)  # noqa
 
 
-@transformation_function(name="Keyboard typo", tags=['text'], cell_level=True)
+@transformation_function(name="Keyboard typo", tags=["text"], cell_level=True)
 def keyboard_typo_transformation(text: str, rate: float = 0.1) -> str:
     """
     Generate a random typo from words of the text of 'column_name'
     Typos are generated through character substitution based on keyboard proximity
     """
     # Split the text into words
     if pd.isnull(text):
@@ -58,58 +59,59 @@
         if random.random() < rate:
             word = words[i]
             if len(word) > 1:
                 j = random.randint(0, len(word) - 1)
                 c = word[j]
                 if c in nearbykeys:
                     replacement = random.choice(nearbykeys[c])
-                    words[i] = word[:j] + replacement + word[j + 1:]
+                    words[i] = word[:j] + replacement + word[j + 1 :]
 
     # Join the words back into a string
-    return ' '.join(words)
+    return " ".join(words)
 
 
-@transformation_function(name="To uppercase", tags=['text'], cell_level=True)
+@transformation_function(name="To uppercase", tags=["text"], cell_level=True)
 def uppercase_transformation(text: str) -> str:
     """
     Transform the text to uppercase
     """
     return np.nan if pd.isnull(text) else text.upper()
 
 
-@transformation_function(name="To lowercase", tags=['text'], cell_level=True)
+@transformation_function(name="To lowercase", tags=["text"], cell_level=True)
 def lowercase_transformation(text: str) -> str:
     """
     Transform the text of the column 'column_name' to lowercase
     """
     return np.nan if pd.isnull(text) else text.lower()
 
 
-@transformation_function(name="Strip punctuation", tags=['text'], cell_level=True)
+@transformation_function(name="Strip punctuation", tags=["text"], cell_level=True)
 def strip_punctuation(text: str) -> str:
     """
     Remove all punctuation symbols (e.g., ., !, ?) from the text of the column 'column_name'
     """
     if pd.isnull(text):
         return text
 
     split_urls_from_text = gruber.split(text)
 
     # The non-URLs are always even-numbered entries in the list and the URLs are odd-numbered.
     for i in range(0, len(split_urls_from_text), 2):
-        split_urls_from_text[i] = split_urls_from_text[i].translate(str.maketrans('', '', string.punctuation))
+        split_urls_from_text[i] = split_urls_from_text[i].translate(str.maketrans("", "", string.punctuation))
 
     stripped_text = "".join(split_urls_from_text)
 
     return stripped_text
 
 
-@transformation_function(name="Change writing style", row_level=False, tags=['text'])
-def change_writing_style(x: pd.DataFrame, index: int, column_name: str, style: str,
-                         OPENAI_API_KEY: str) -> pd.DataFrame:
+@transformation_function(name="Change writing style", row_level=False, tags=["text"])
+def change_writing_style(
+    x: pd.DataFrame, index: int, column_name: str, style: str, OPENAI_API_KEY: str
+) -> pd.DataFrame:
     os.environ["OPENAI_API_KEY"] = OPENAI_API_KEY
     rewrite_prompt_template = """
     As a text rewriting robot, your task is to rewrite a given text using a specified rewriting style. You will receive a prompt with the following format:
     ```
     "TEXT"
     ===
     "REWRITING STYLE"
@@ -128,12 +130,12 @@
     ```
     """
 
     from langchain import PromptTemplate
     from langchain import LLMChain
     from langchain import OpenAI
 
-    rewrite_prompt = PromptTemplate(input_variables=['text', 'style'], template=rewrite_prompt_template)
+    rewrite_prompt = PromptTemplate(input_variables=["text", "style"], template=rewrite_prompt_template)
     chain_rewrite = LLMChain(llm=OpenAI(), prompt=rewrite_prompt)
 
-    x.at[index, column_name] = chain_rewrite.run({'text': x.at[index, column_name], 'style': style})
+    x.at[index, column_name] = chain_rewrite.run({"text": x.at[index, column_name], "style": style})
     return x
```

### Comparing `giskard-2.0.0b7/giskard/ml_worker/testing/registry/decorators.py` & `giskard-2.0.0b8/giskard/ml_worker/testing/registry/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,22 +13,24 @@
     if sys.version_info >= (3, 10):
         import typing as t
     else:
         import typing_extensions as t
     P = t.ParamSpec("P")
     R = TypeVar("R")
 
-    def inner(original: Union[Callable[P, R], Type[GiskardTest]]) \
-            -> Union[Callable[P, GiskardTest], GiskardTest, GiskardTestMethod]:
+    def inner(
+        original: Union[Callable[P, R], Type[GiskardTest]]
+    ) -> Union[Callable[P, GiskardTest], GiskardTest, GiskardTestMethod]:
         """
         Declare output as both Callable and GiskardTest so that there's autocompletion
         for GiskardTest's methods as well as the original wrapped function arguments (for __call__)
         """
         from giskard.ml_worker.testing.registry.registry import tests_registry
-        tests_registry.register(TestFunctionMeta(original, name=name, tags=tags, type='TEST'))
+
+        tests_registry.register(TestFunctionMeta(original, name=name, tags=tags, type="TEST"))
 
         if inspect.isclass(original) and issubclass(original, GiskardTest):
             return original
 
         return _wrap_test_method(original)
 
     if callable(_fn):
```

### Comparing `giskard-2.0.0b7/giskard/ml_worker/testing/registry/decorators_utils.py` & `giskard-2.0.0b8/giskard/ml_worker/testing/registry/decorators_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,63 +4,70 @@
 
 def make_all_optional_or_suite_input(fn: Callable):
     from inspect import signature, Parameter
     from giskard.core.suite import SuiteInput
 
     sig = signature(fn)
     sig = sig.replace(
-        parameters=[Parameter(name=par.name, kind=par.kind,
-                              default=None if par.default == inspect.Signature.empty else par.default,
-                              annotation=Optional[Union[SuiteInput, par.annotation]])
-                    for par in sig.parameters.values()])
+        parameters=[
+            Parameter(
+                name=par.name,
+                kind=par.kind,
+                default=None if par.default == inspect.Signature.empty else par.default,
+                annotation=Optional[Union[SuiteInput, par.annotation]],
+            )
+            for par in sig.parameters.values()
+        ]
+    )
     fn.__signature__ = sig
 
     fn.__annotations__ = {k: Optional[Union[SuiteInput, v]] for k, v in fn.__annotations__.items()}
 
 
 def set_return_type(fn: Callable, return_type: type):
     from inspect import signature
+
     sig = signature(fn)
     sig = sig.replace(return_annotation=return_type)
     fn.__signature__ = sig
 
     annotations = fn.__annotations__.copy()
-    annotations['return'] = return_type
+    annotations["return"] = return_type
     fn.__annotations__ = annotations
 
 
 def validate_arg_type(fn: Callable, pos: int, arg_type: type):
     from inspect import signature
 
     sig = signature(fn)
     if len(sig.parameters) <= pos:
         raise TypeError(f"Required arg {pos} of {fn.__name__} to be {arg_type}, but none was defined")
     elif list(sig.parameters.values())[0].annotation not in [inspect._empty, arg_type]:
         raise TypeError(
-            f"Required arg {pos} of {fn.__name__} to be {arg_type}, but {list(sig.parameters.values())[0].annotation} was defined")
+            f"Required arg {pos} of {fn.__name__} to be {arg_type}, but {list(sig.parameters.values())[0].annotation} was defined"
+        )
 
 
 def drop_arg(fn: Callable, pos: int):
     from inspect import signature
 
     sig = signature(fn)
     if len(sig.parameters) <= pos:
         return
 
-    sig = sig.replace(
-        parameters=[par for idx, par in enumerate(sig.parameters.values()) if idx != pos])
+    sig = sig.replace(parameters=[par for idx, par in enumerate(sig.parameters.values()) if idx != pos])
     fn.__signature__ = sig
 
-    fn.__annotations__ = {k: v for k, v in fn.__annotations__.items() if k in sig.parameters or k == 'return'}
+    fn.__annotations__ = {k: v for k, v in fn.__annotations__.items() if k in sig.parameters or k == "return"}
 
 
 def insert_arg(fn: Callable, pos: int, param: inspect.Parameter):
     from inspect import signature
 
     sig = signature(fn)
     parameters = [par for par in sig.parameters.values()]
     parameters.insert(pos, param)
 
     sig = sig.replace(parameters=parameters)
     fn.__signature__ = sig
 
-    fn.__annotations__ = {k: v for k, v in fn.__annotations__.items() if k in sig.parameters or k == 'return'}
+    fn.__annotations__ = {k: v for k, v in fn.__annotations__.items() if k in sig.parameters or k == "return"}
```

### Comparing `giskard-2.0.0b7/giskard/ml_worker/testing/registry/giskard_test.py` & `giskard-2.0.0b8/giskard/ml_worker/testing/registry/giskard_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,47 +43,47 @@
         :return: A TestResult or a bool containing detailed information of the test execution results
         :rtype: Union[TestResult, bool]
         """
         ...
 
     @classmethod
     def _get_name(cls) -> str:
-        return 'tests'
+        return "tests"
 
     @classmethod
     def _get_meta_class(cls) -> type(SMT):
         return TestFunctionMeta
 
     def _get_uuid(self) -> str:
         return get_object_uuid(type(self))
 
     def _save_locally(self, local_dir: Path):
-        with open(Path(local_dir) / 'data.pkl', 'wb') as f:
+        with open(Path(local_dir) / "data.pkl", "wb") as f:
             cloudpickle.dump(type(self), f, protocol=pickle.DEFAULT_PROTOCOL)
 
     @classmethod
     def _load_meta_locally(cls, local_dir, uuid: str) -> Optional[TestFunctionMeta]:
         meta = tests_registry.get_test(uuid)
 
         if meta is not None:
             return meta
 
         return super()._load_meta_locally(local_dir, uuid)
 
     @classmethod
     def load(cls, local_dir: Path, uuid: str, meta: TestFunctionMeta):
         if local_dir.exists():
-            with open(Path(local_dir) / 'data.pkl', 'rb') as f:
+            with open(Path(local_dir) / "data.pkl", "rb") as f:
                 func = pickle.load(f)
         elif hasattr(sys.modules[meta.module], meta.name):
             func = getattr(sys.modules[meta.module], meta.name)
         else:
             return None
 
-        if inspect.isclass(func) or hasattr(func, 'meta'):
+        if inspect.isclass(func) or hasattr(func, "meta"):
             giskard_test = func()
         elif isinstance(func, GiskardTest):
             giskard_test = func
         else:
             giskard_test = GiskardTestMethod(func)
 
         tests_registry.add_func(meta)
@@ -111,27 +111,27 @@
             # equivalent to adding @test decorator
             from giskard import test
 
             test()(test_fn)
             meta = tests_registry.get_test(test_uuid)
         super(GiskardTest, self).__init__(meta)
 
-    def __call__(self, *args, **kwargs) -> 'GiskardTestMethod':
+    def __call__(self, *args, **kwargs) -> "GiskardTestMethod":
         instance = copy.deepcopy(self)
 
         instance.is_initialized = True
         instance.params = kwargs
 
         for idx, arg in enumerate(args):
             instance.params[next(iter([arg.name for arg in instance.meta.args.values() if arg.argOrder == idx]))] = arg
 
         return instance
 
     def execute(self) -> Result:
-        analytics.track('test:execute', {"test_name": self.meta.full_name})
+        analytics.track("test:execute", {"test_name": self.meta.full_name})
 
         return self.test_fn(**self.params)
 
     def __repr__(self) -> str:
         if not self.is_initialized:
             hint = "Test object hasn't been initialized, call it by providing the inputs"
         else:
@@ -142,9 +142,9 @@
 
         return "\n".join(output)
 
     def get_builder(self):
         return GiskardTestMethod(self.test_fn)
 
     def _save_locally(self, local_dir: Path):
-        with open(Path(local_dir) / 'data.pkl', 'wb') as f:
+        with open(Path(local_dir) / "data.pkl", "wb") as f:
             cloudpickle.dump(self.test_fn, f, protocol=pickle.DEFAULT_PROTOCOL)
```

### Comparing `giskard-2.0.0b7/giskard/ml_worker/testing/registry/registry.py` & `giskard-2.0.0b8/giskard/ml_worker/testing/registry/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 logger = logging.getLogger(__name__)
 plugins_root = find_plugin_location()
 
 
 def get_object_uuid(obj) -> str:
-    if hasattr(obj, 'meta') and hasattr(obj.meta, 'uuid'):
+    if hasattr(obj, "meta") and hasattr(obj.meta, "uuid"):
         return obj.meta.uuid
     obj_hash = hashlib.sha512(cloudpickle.dumps(obj)).hexdigest()
     return str(uuid.uuid5(uuid.NAMESPACE_OID, obj_hash))
 
 
 def load_plugins():
     giskard_tests_module = "giskard.testing.tests"
@@ -102,24 +102,24 @@
 
 
 def new_getfile(object, _old_getfile=inspect.getfile):
     if not inspect.isclass(object):
         return _old_getfile(object)
 
     # Lookup by parent module (as in current inspect)
-    if hasattr(object, '__module__'):
+    if hasattr(object, "__module__"):
         object_ = sys.modules.get(object.__module__)
-        if hasattr(object_, '__file__'):
+        if hasattr(object_, "__file__"):
             return object_.__file__
 
     # If parent module is __main__, lookup by methods (NEW)
     for name, member in inspect.getmembers(object):
-        if inspect.isfunction(member) and object.__qualname__ + '.' + member.__name__ == member.__qualname__:
+        if inspect.isfunction(member) and object.__qualname__ + "." + member.__name__ == member.__qualname__:
             return inspect.getfile(member)
 
-    raise TypeError('Source for {!r} not found'.format(object))
+    raise TypeError("Source for {!r} not found".format(object))
 
 
 # Override getfile to have it working over Jupyter Notebook files
 inspect.getfile = new_getfile
 
 tests_registry = GiskardTestRegistry()
```

### Comparing `giskard-2.0.0b7/giskard/ml_worker/testing/registry/slicing_function.py` & `giskard-2.0.0b8/giskard/ml_worker/testing/registry/slicing_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,49 +4,54 @@
 from typing import Optional, List, Union, Type, Callable, Dict
 
 import pandas as pd
 
 from giskard.core.core import DatasetProcessFunctionMeta, DatasetProcessFunctionType
 from giskard.core.validation import configured_validate_arguments
 from giskard.ml_worker.core.savable import RegistryArtifact
-from giskard.ml_worker.testing.registry.decorators_utils import validate_arg_type, drop_arg, \
-    make_all_optional_or_suite_input, set_return_type
+from giskard.ml_worker.testing.registry.decorators_utils import (
+    validate_arg_type,
+    drop_arg,
+    make_all_optional_or_suite_input,
+    set_return_type,
+)
 from giskard.ml_worker.testing.registry.registry import get_object_uuid, tests_registry
 
 SlicingFunctionType = Callable[..., bool]
 
-default_tags = ['filter']
+default_tags = ["filter"]
 
 
 class SlicingFunction(RegistryArtifact[DatasetProcessFunctionMeta]):
     """
     A slicing function used to subset data.
 
     Attributes:
         func (SlicingFunctionType): The function used to slice the data.
         row_level (bool): Whether the slicing function should operate on rows or columns.
         cell_level (bool): Whether the slicing function should operate at the cell level.
         params (Dict): Additional parameters for the slicing function.
         is_initialized (bool): Indicates if the slicing function has been initialized.
     """
+
     func: SlicingFunctionType
     row_level: bool
     cell_level: bool
     params: Dict
     is_initialized: bool
 
     @classmethod
     def _get_name(cls) -> str:
         """
         Returns the name of the class.
 
         :return: The name of the class.
         :rtype: str
         """
-        return 'slices'
+        return "slices"
 
     def __init__(self, func: Optional[SlicingFunctionType], row_level=True, cell_level=False):
         """
         Initializes a new instance of the SlicingFunction class.
 
         :param func: The function used to slice the data.
         :type func: SlicingFunctionType
@@ -58,19 +63,19 @@
         self.func = func
         self.row_level = row_level
         self.cell_level = cell_level
 
         test_uuid = get_object_uuid(func)
         meta = tests_registry.get_test(test_uuid)
         if meta is None and func is not None:
-            meta = DatasetProcessFunctionMeta(func, tags=default_tags, type='SLICE', cell_level=self.cell_level)
+            meta = DatasetProcessFunctionMeta(func, tags=default_tags, type="SLICE", cell_level=self.cell_level)
             tests_registry.register(meta)
         super().__init__(meta)
 
-    def __call__(self, *args, **kwargs) -> 'SlicingFunction':
+    def __call__(self, *args, **kwargs) -> "SlicingFunction":
         self.is_initialized = True
         self.params = kwargs
 
         for idx, arg in enumerate(args):
             self.params[next(iter([arg.name for arg in self.meta.args.values() if arg.argOrder == idx]))] = arg
 
         return self
@@ -82,16 +87,16 @@
         Args:
             data (Union[pd.Series, pd.DataFrame]): The data to slice.
 
         Returns:
             Union[pd.Series, pd.DataFrame]: The sliced data.
         """
         if self.cell_level:
-            actual_params = {k: v for k, v in self.params.items() if k != 'column_name'}
-            return data.loc[data.apply(lambda row: self.func(row[self.params['column_name']], **actual_params), axis=1)]
+            actual_params = {k: v for k, v in self.params.items() if k != "column_name"}
+            return data.loc[data.apply(lambda row: self.func(row[self.params["column_name"]], **actual_params), axis=1)]
         if self.row_level:
             return data.loc[data.apply(lambda row: self.func(row, **self.params), axis=1)]
         else:
             return self.func(data, **self.params)
 
     @classmethod
     def load(cls, local_dir: Path, uuid: str, meta: DatasetProcessFunctionMeta):
@@ -124,20 +129,25 @@
                       and if False, it will receive the entire dataframe.
     :param cell_level: Whether to apply the slicing function on the cell level. If True, the slicing function
                        will be applied to individual cells instead of rows or the entire dataframe.
     :return: The wrapped function or a new instance of SlicingFunction.
     """
 
     def inner(func: Union[SlicingFunctionType, Type[SlicingFunction]]) -> SlicingFunction:
-
         from giskard.ml_worker.testing.registry.registry import tests_registry
 
         tests_registry.register(
-            DatasetProcessFunctionMeta(func, name=name, tags=default_tags if not tags else (default_tags + tags),
-                                       type='SLICE', cell_level=cell_level))
+            DatasetProcessFunctionMeta(
+                func,
+                name=name,
+                tags=default_tags if not tags else (default_tags + tags),
+                type="SLICE",
+                cell_level=cell_level,
+            )
+        )
         if inspect.isclass(func) and issubclass(func, SlicingFunction):
             return func
 
         return _wrap_slicing_function(func, row_level, cell_level)()
 
     if callable(_fn):
         return functools.wraps(_fn)(inner(_fn))
```

### Comparing `giskard-2.0.0b7/giskard/ml_worker/testing/registry/transformation_function.py` & `giskard-2.0.0b8/giskard/ml_worker/testing/registry/transformation_function.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,41 +13,42 @@
     make_all_optional_or_suite_input,
     set_return_type,
 )
 from giskard.ml_worker.testing.registry.registry import get_object_uuid, tests_registry
 
 TransformationFunctionType = Callable[..., Union[pd.Series, pd.DataFrame]]
 
-default_tags = ['transformation']
+default_tags = ["transformation"]
 
 
 class TransformationFunction(RegistryArtifact[DatasetProcessFunctionMeta]):
     func: TransformationFunctionType = None
     row_level: bool = True
     cell_level: bool = False
     params = {}
     is_initialized = False
 
     @classmethod
     def _get_name(cls) -> str:
-        return 'transformations'
+        return "transformations"
 
     def __init__(self, func: Optional[TransformationFunctionType], row_level=True, cell_level=False):
         self.func = func
         self.row_level = row_level
         self.cell_level = cell_level
 
         test_uuid = get_object_uuid(func)
         meta = tests_registry.get_test(test_uuid)
         if meta is None and func is not None:
-            meta = tests_registry.register(DatasetProcessFunctionMeta(func, tags=default_tags, type='TRANSFORMATION',
-                                                                      cell_level=self.cell_level))
+            meta = tests_registry.register(
+                DatasetProcessFunctionMeta(func, tags=default_tags, type="TRANSFORMATION", cell_level=self.cell_level)
+            )
         super().__init__(meta)
 
-    def __call__(self, *args, **kwargs) -> 'TransformationFunction':
+    def __call__(self, *args, **kwargs) -> "TransformationFunction":
         self.is_initialized = True
         self.params = kwargs
 
         for idx, arg in enumerate(args):
             self.params[next(iter([arg.name for arg in self.meta.args.values() if arg.argOrder == idx]))] = arg
 
         return self
@@ -59,56 +60,65 @@
         Args:
             data (Union[pd.Series, pd.DataFrame]): The data to transform.
 
         Returns:
             Union[pd.Series, pd.DataFrame]: The transformed data.
         """
         if self.cell_level:
-            actual_params = {k: v for k, v in self.params.items() if k != 'column_name'}
+            actual_params = {k: v for k, v in self.params.items() if k != "column_name"}
 
             def apply(row: pd.Series) -> pd.Series:
-                row[self.params['column_name']] = self.func(row[self.params['column_name']], **actual_params)
+                row[self.params["column_name"]] = self.func(row[self.params["column_name"]], **actual_params)
                 return row
 
             return data.apply(apply, axis=1)
         elif self.row_level:
             return data.apply(lambda row: self.func(row, **self.params), axis=1)
         else:
             return self.func(data, **self.params)
 
     @classmethod
     def _get_meta_class(cls):
         return DatasetProcessFunctionMeta
 
 
-def transformation_function(_fn: Union[TransformationFunctionType, Type[TransformationFunction]] = None,
-                            row_level=True,
-                            cell_level=False,
-                            name=None,
-                            tags: Optional[List[str]] = None):
+def transformation_function(
+    _fn: Union[TransformationFunctionType, Type[TransformationFunction]] = None,
+    row_level=True,
+    cell_level=False,
+    name=None,
+    tags: Optional[List[str]] = None,
+):
     """
     Decorator that registers a function as a transformation function and returns a TransformationFunction instance.
     It can be used for transforming datasets in a specific way during testing.
 
     :param _fn: function to decorate. No need to provide this argument, the decorator will automatically take as input the function to decorate.
     :param name: Optional name to use for the function when registering it.
     :param tags: Optional list of tags to use when registering the function.
     :param row_level: Whether to apply the transformation function row-wise (default) or on the full dataframe. If `row_level`
                       is True, the slicing function will receive a row (either a Series or DataFrame),
                       and if False, it will receive the entire dataframe.
     :param cell_level: Whether to apply the transformation function on the cell level. If True, the slicing function
                        will be applied to individual cells instead of rows or the entire dataframe.
     :return: The wrapped function or a new instance of TransformationFunction.
     """
+
     def inner(func: Union[TransformationFunctionType, Type[TransformationFunction]]) -> TransformationFunction:
         from giskard.ml_worker.testing.registry.registry import tests_registry
 
         tests_registry.register(
-            DatasetProcessFunctionMeta(func, name=name, tags=default_tags if not tags else (default_tags + tags),
-                                       type='TRANSFORMATION', cell_level=cell_level))
+            DatasetProcessFunctionMeta(
+                func,
+                name=name,
+                tags=default_tags if not tags else (default_tags + tags),
+                type="TRANSFORMATION",
+                cell_level=cell_level,
+            )
+        )
 
         if inspect.isclass(func) and issubclass(func, TransformationFunction):
             return func
         return _wrap_transformation_function(func, row_level, cell_level)()
 
     if callable(_fn):
         return functools.wraps(_fn)(inner(_fn))
```

### Comparing `giskard-2.0.0b7/giskard/ml_worker/testing/registry/udf_repository.py` & `giskard-2.0.0b8/giskard/ml_worker/testing/registry/udf_repository.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,31 +16,32 @@
     repo: str
     user: str
     pwd: str
 
 
 def load_config() -> GitConfig:
     return GitConfig(
-        repo=os.getenv('GIT_REPOSITORY'),
-        user=os.getenv('GIT_USER'),
-        pwd=os.getenv('GIT_PASSWORD'),
+        repo=os.getenv("GIT_REPOSITORY"),
+        user=os.getenv("GIT_USER"),
+        pwd=os.getenv("GIT_PASSWORD"),
     )
 
 
 def init_udf_repository(udf_enabled: bool = False) -> bool:
     # Experimental feature, disabled by default
     if not udf_enabled:
         return False
 
     try:
         config = load_config()
 
         if config.repo is None:
             logger.warning(
-                "UDF repository is not available because the 'GIT_REPOSITORY' environment variable is not set")
+                "UDF repository is not available because the 'GIT_REPOSITORY' environment variable is not set"
+            )
             return False
 
         if udf_root.exists():
             update_udf_repository()
         else:
             clone_udf_repository(config)
     except Exception as e:
@@ -48,29 +49,29 @@
         return False
     return True
 
 
 def update_udf_repository():
     repo = Repo(udf_root)
 
-    logger.info('Repository already existing, fetching updates')
+    logger.info("Repository already existing, fetching updates")
     origin = repo.remotes.origin
     origin.pull()
 
     repo.close()
 
 
 def clone_udf_repository(config: GitConfig):
-    logger.info(f'cloning repository: {config.repo}')
+    logger.info(f"cloning repository: {config.repo}")
 
     host = config.repo
 
-    protocol = 'http'
-    if not host.startswith('http://'):
-        protocol = 'https'
+    protocol = "http"
+    if not host.startswith("http://"):
+        protocol = "https"
 
     host = f"{protocol}://{config.user}:{config.pwd}@{config.repo.replace('http://', '').replace('https://', '')}"
 
     repo = Repo.clone_from(host, udf_root)
     repo.close()
```

### Comparing `giskard-2.0.0b7/giskard/ml_worker/testing/stat_utils.py` & `giskard-2.0.0b8/giskard/ml_worker/testing/stat_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/ml_worker/testing/test_result.py` & `giskard-2.0.0b8/giskard/ml_worker/testing/test_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 class TestMessage:
     type: TestMessageLevel
     text: str
 
     def _repr_html_(self):
         return """
                <li style="color:{0};">{1}</li>
-               """.format('red' if self.type == TestMessageLevel.ERROR else 'inherit', self.text)
+               """.format(
+            "red" if self.type == TestMessageLevel.ERROR else "inherit", self.text
+        )
 
     def __repr__(self):
         return f" - [{self.type}] {self.text}"
 
 
 @dataclass
 class PartialUnexpectedCounts:
@@ -34,14 +36,15 @@
     """
     Dataclass representing the result of a test
 
     :param passed: A boolean indicating whether the test passed or not
     :param messages: A list of TestMessage objects containing information about the test execution
     :param metric: A float representing the test metric
     """
+
     passed: bool = False
     messages: List[TestMessage] = field(default_factory=list, repr=False)
     props: Dict[str, str] = field(default_factory=dict, repr=False)
     metric: float = 0
     missing_count: int = 0
     missing_percent: float = 0
     unexpected_count: int = 0
@@ -56,21 +59,25 @@
     reference_slices_size: List[int] = field(default_factory=list, repr=False)
 
     def _repr_html_(self):
         return """
                <h4><span style="color:{0};">{1}</span> Test {2}</h4>
                <p>Metric: {3}<p>
                <ul>{4}</ul>
-               """.format('green' if self.passed else 'red',
-                          '✓' if self.passed else '𐄂',
-                          'succeed' if self.passed else 'failed',
-                          'No metric' if self.metric is None else str(round(self.metric, 2)),
-                          ''.join([] if self.messages is None else [m._repr_html_() for m in self.messages]))
+               """.format(
+            "green" if self.passed else "red",
+            "✓" if self.passed else "𐄂",
+            "succeed" if self.passed else "failed",
+            "No metric" if self.metric is None else str(round(self.metric, 2)),
+            "".join([] if self.messages is None else [m._repr_html_() for m in self.messages]),
+        )
 
     def __repr__(self):
         return """
                Test {0}
                Metric: {1}
                {2}
-               """.format('succeed' if self.passed else 'failed',
-                          'No metric' if self.metric is None else str(round(self.metric, 2)),
-                          '\n'.join([] if self.messages is None else [m.__repr__() for m in self.messages]))
+               """.format(
+            "succeed" if self.passed else "failed",
+            "No metric" if self.metric is None else str(round(self.metric, 2)),
+            "\n".join([] if self.messages is None else [m.__repr__() for m in self.messages]),
+        )
```

### Comparing `giskard-2.0.0b7/giskard/ml_worker/testing/utils.py` & `giskard-2.0.0b8/giskard/ml_worker/testing/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,19 @@
     Increasing = 1
     Decreasing = -1
 
 
 def validate_classification_label(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
-        reference_slice = kwargs.get('reference_dataset', None)
-        actual_slice = kwargs.get('dataset', None)
-        model = kwargs.get('model', None)
-        classification_label = kwargs.get('classification_label', None)
-        target = getattr(reference_slice, 'target', getattr(actual_slice, 'target', None))
+        reference_slice = kwargs.get("reference_dataset", None)
+        actual_slice = kwargs.get("dataset", None)
+        model = kwargs.get("model", None)
+        classification_label = kwargs.get("classification_label", None)
+        target = getattr(reference_slice, "target", getattr(actual_slice, "target", None))
 
         # Try to automatically cast `classification_label` to the right type
         if (
             classification_label is not None
             and model is not None
             and isinstance(model.meta.classification_labels[0], numbers.Number)
         ):
@@ -34,15 +34,15 @@
                 pass
 
         # Validate the label
         if target and classification_label and model:
             assert classification_label != target, (
                 'By "classification_label", we refer to one of the values: '
                 f'{model.meta.classification_labels} and not the target: "{target}". '
-                'Please re-assign this argument.'
+                "Please re-assign this argument."
             )
 
         assert (
             model.meta.model_type != SupportedModelTypes.CLASSIFICATION
             or classification_label in model.meta.classification_labels
         ), f'"{classification_label}" is not part of model labels: {model.meta.classification_labels}'
         return func(*args, **kwargs)
```

### Comparing `giskard-2.0.0b7/giskard/ml_worker/utils/logging.py` & `giskard-2.0.0b8/giskard/ml_worker/utils/logging.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/ml_worker/utils/network.py` & `giskard-2.0.0b8/giskard/ml_worker/utils/network.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,39 +22,39 @@
         return s.getsockname()[1]
 
 
 def readable_hex(data):
     if not os.environ.get("GSK_ML_WORKER_LOG_HEX", False):
         return ""
     s = codecs.encode(data, "hex").decode()
-    return " ".join(s[i: i + 2] for i in range(0, len(s), 2))
+    return " ".join(s[i : i + 2] for i in range(0, len(s), 2))
 
 
 def is_pre_release(current_version: str):
     # A very dummy pre-release checker, to be improved
-    return re.match(r'.*[a-z].*', current_version) is not None
+    return re.match(r".*[a-z].*", current_version) is not None
 
 
 @threaded
 def check_latest_giskard_version():
     try:
         current_version = giskard.__version__
         if not is_pre_release(current_version):
             return
-        respose = requests.get('https://pypi.org/pypi/giskard/json').json()
-        releases = respose.get('releases')
+        respose = requests.get("https://pypi.org/pypi/giskard/json").json()
+        releases = respose.get("releases")
         releases_dates = {}
         if current_version not in releases:
             return
         for ver, resources in releases.items():
-            latest_release_date = max(map(lambda r: datetime.datetime.fromisoformat(r['upload_time']), resources))
+            latest_release_date = max(map(lambda r: datetime.datetime.fromisoformat(r["upload_time"]), resources))
             releases_dates[ver] = latest_release_date
         latest_version, latest_release_date = max(releases_dates.items(), key=lambda x: x[1])
 
         if latest_release_date > releases_dates[current_version]:
             warning(
                 "You're using a pre-release version of giskard while a "
                 "new version is available, please install it with: "
-                f"pip install \"giskard=={latest_version}\""
+                f'pip install "giskard=={latest_version}"'
             )
     except BaseException as e:
         logger.exception("Failed to fetch latest giskard version", e)
```

### Comparing `giskard-2.0.0b7/giskard/ml_worker/utils/request_interceptor.py` & `giskard-2.0.0b8/giskard/ml_worker/utils/request_interceptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,17 +34,17 @@
             )
         )
         code, _ = error_code.value
         rich_status = Status(code=code, message=e.__class__.__name__, details=[detail])
         await context.abort_with_status(rpc_status.to_status(rich_status))
 
     async def intercept_service(
-            self,
-            continuation: Callable[[grpc.HandlerCallDetails], Awaitable[grpc.RpcMethodHandler]],
-            handler_call_details: grpc.HandlerCallDetails,
+        self,
+        continuation: Callable[[grpc.HandlerCallDetails], Awaitable[grpc.RpcMethodHandler]],
+        handler_call_details: grpc.HandlerCallDetails,
     ) -> grpc.RpcMethodHandler:
         def _wrapper(behavior):
             @functools.wraps(behavior)
             async def wrapper(request, context: aio.ServicerContext):
                 try:
                     loop = asyncio.get_running_loop()
                     res = await loop.run_in_executor(pool, behavior, request, context)
```

### Comparing `giskard-2.0.0b7/giskard/models/__init__.py` & `giskard-2.0.0b8/giskard/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,22 +107,22 @@
             feature_names=feature_names,
             classification_threshold=classification_threshold,
             classification_labels=classification_labels,
             **kwargs,
         )
     else:
         raise ValueError(
-            'We could not infer your model library. We currently only support functions or models from:'
-            '\n- sklearn'
-            '\n- catboost'
-            '\n- pytorch'
-            '\n- tensorflow'
-            '\n- huggingface'
-            '\n- langchain'
-            '\nWe recommend that you create your own wrapper using our documentation page: https://giskard.readthedocs.io/en/latest/guides/custom-wrapper'
+            "We could not infer your model library. We currently only support functions or models from:"
+            "\n- sklearn"
+            "\n- catboost"
+            "\n- pytorch"
+            "\n- tensorflow"
+            "\n- huggingface"
+            "\n- langchain"
+            "\nWe recommend that you create your own wrapper using our documentation page: https://giskard.readthedocs.io/en/latest/guides/custom-wrapper"
         )
 
 
 @configured_validate_arguments
 def model_from_sklearn(
     model,
     model_type: ModelType,
```

### Comparing `giskard-2.0.0b7/giskard/models/_precooked.py` & `giskard-2.0.0b8/giskard/models/_precooked.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,21 +12,20 @@
     def __init__(
         self,
         data: Dataset,
         predictions: ModelPredictionResults,
         model_type: ModelType,
         feature_names: Optional[Iterable] = None,
         classification_labels: Optional[Iterable] = None,
-            **kwargs,
+        **kwargs,
     ):
         self._data = data
         self._predictions = predictions
         super().__init__(
-            model_type=model_type, feature_names=feature_names, classification_labels=classification_labels,
-            **kwargs
+            model_type=model_type, feature_names=feature_names, classification_labels=classification_labels, **kwargs
         )
 
     @classmethod
     def from_model(cls, model: BaseModel, dataset: Dataset):
         """Creates a PrecookedModel from an existing model and dataset."""
         predictions = model.predict(dataset)
```

### Comparing `giskard-2.0.0b7/giskard/models/automodel/__init__.py` & `giskard-2.0.0b8/giskard/models/automodel/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/models/base/__init__.py` & `giskard-2.0.0b8/giskard/models/base/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/models/cache/__init__.py` & `giskard-2.0.0b8/giskard/models/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/models/cache/cache.py` & `giskard-2.0.0b8/giskard/models/cache/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import numpy as np
 import pandas as pd
 
 from giskard.core.core import SupportedModelTypes
 from giskard.settings import settings
 
-NaN = float('NaN')
+NaN = float("NaN")
 
 CACHE_CSV_FILENAME = "giskard-model-cache.csv"
 
 
 def flatten(xs):
     for x in xs:
         if isinstance(x, Iterable) and not isinstance(x, (str, bytes)):
```

### Comparing `giskard-2.0.0b7/giskard/models/catboost/__init__.py` & `giskard-2.0.0b8/giskard/models/catboost/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/models/function/__init__.py` & `giskard-2.0.0b8/giskard/models/function/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/models/huggingface/__init__.py` & `giskard-2.0.0b8/giskard/models/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/models/langchain/__init__.py` & `giskard-2.0.0b8/giskard/models/langchain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,17 @@
         data_preprocessing_function: Callable[[pd.DataFrame], Any] = None,
         model_postprocessing_function: Callable[[Any], Any] = None,
         feature_names: Optional[Iterable] = None,
         classification_threshold: Optional[float] = 0.5,
         classification_labels: Optional[Iterable] = None,
         **kwargs,
     ) -> None:
-        assert model_type == SupportedModelTypes.TEXT_GENERATION, 'LangchainModel only support text_generation ModelType'
+        assert (
+            model_type == SupportedModelTypes.TEXT_GENERATION
+        ), "LangchainModel only support text_generation ModelType"
 
         super().__init__(
             model=model,
             model_type=model_type,
             name=name,
             data_preprocessing_function=data_preprocessing_function,
             model_postprocessing_function=model_postprocessing_function,
@@ -40,22 +42,22 @@
         mlflow.langchain.save_model(self.model, path=local_path, mlflow_model=mlflow_meta)
 
     @classmethod
     def load_model(cls, local_dir):
         return mlflow.langchain.load_model(local_dir)
 
     def model_predict(self, df):
-        return [self.model.predict(**data) for data in df.to_dict('records')]
+        return [self.model.predict(**data) for data in df.to_dict("records")]
 
     def rewrite_prompt(self, template, input_variables=None, **kwargs):
         from langchain import LLMChain
 
         update = dict(template=template)
         if input_variables is not None:
-            update['input_variables'] = input_variables
+            update["input_variables"] = input_variables
 
         new_prompt = self.model.prompt.copy(update=update)
         chain = LLMChain(llm=self.model.llm, prompt=new_prompt)
 
         model_kwargs = dict(
             model_type=self.meta.model_type,
             data_preprocessing_function=self.data_preprocessing_function,
```

### Comparing `giskard-2.0.0b7/giskard/models/model_explanation.py` & `giskard-2.0.0b8/giskard/models/model_explanation.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 
 
 @timer()
 def explain_text(model: BaseModel, input_df: pd.DataFrame, text_column: str, text_document: str, n_samples: int):
     try:
         import eli5
         from eli5.lime import TextExplainer
+
         text_explainer = TextExplainer(random_state=42, n_samples=n_samples)
         prediction_function = text_explanation_prediction_wrapper(model.predict_df, input_df, text_column)
         text_explain_attempts = 10
         for i in range(text_explain_attempts):
             try:
                 text_explainer.fit(text_document, prediction_function)
                 break
```

### Comparing `giskard-2.0.0b7/giskard/models/pytorch/__init__.py` & `giskard-2.0.0b8/giskard/models/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/models/sklearn/__init__.py` & `giskard-2.0.0b8/giskard/models/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/models/tensorflow/__init__.py` & `giskard-2.0.0b8/giskard/models/tensorflow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,35 +10,35 @@
 
 logger = logging.getLogger(__name__)
 
 
 class TensorFlowModel(MLFlowBasedModel):
     @configured_validate_arguments
     def __init__(
-            self,
-            model,
-            model_type: ModelType,
-            name: Optional[str] = None,
-            data_preprocessing_function: Callable[[pd.DataFrame], Any] = None,
-            model_postprocessing_function: Callable[[Any], Any] = None,
-            feature_names: Optional[Iterable] = None,
-            classification_threshold: Optional[float] = 0.5,
-            classification_labels: Optional[Iterable] = None,
-            **kwargs
+        self,
+        model,
+        model_type: ModelType,
+        name: Optional[str] = None,
+        data_preprocessing_function: Callable[[pd.DataFrame], Any] = None,
+        model_postprocessing_function: Callable[[Any], Any] = None,
+        feature_names: Optional[Iterable] = None,
+        classification_threshold: Optional[float] = 0.5,
+        classification_labels: Optional[Iterable] = None,
+        **kwargs,
     ):
         super().__init__(
             model=model,
             model_type=model_type,
             name=name,
             data_preprocessing_function=data_preprocessing_function,
             model_postprocessing_function=model_postprocessing_function,
             feature_names=feature_names,
             classification_threshold=classification_threshold,
             classification_labels=classification_labels,
-            **kwargs
+            **kwargs,
         )
 
     @classmethod
     def load_model(cls, local_path):
         return mlflow.tensorflow.load_model(local_path)
 
     def save_model(self, local_path, mlflow_meta: mlflow.models.Model):
```

### Comparing `giskard-2.0.0b7/giskard/models/utils.py` & `giskard-2.0.0b8/giskard/models/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 def fix_seed():
     seed = 1337
 
     random.seed(seed)
     np.random.seed(seed)
     try:
         import torch
+
         torch.manual_seed(seed)
     except ImportError:
         pass
 
 
 @lru_cache(None)
 def warn_once(logger, msg: str):
```

### Comparing `giskard-2.0.0b7/giskard/path_utils.py` & `giskard-2.0.0b8/giskard/path_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/__init__.py` & `giskard-2.0.0b8/giskard/scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/calibration/issues.py` & `giskard-2.0.0b8/giskard/scanner/calibration/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/calibration/overconfidence_detector.py` & `giskard-2.0.0b8/giskard/scanner/calibration/overconfidence_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/calibration/underconfidence_detector.py` & `giskard-2.0.0b8/giskard/scanner/calibration/underconfidence_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/common/examples.py` & `giskard-2.0.0b8/giskard/scanner/common/examples.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/common/loss_based_detector.py` & `giskard-2.0.0b8/giskard/scanner/common/loss_based_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/data_leakage/data_leakage_detector.py` & `giskard-2.0.0b8/giskard/scanner/data_leakage/data_leakage_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/decorators.py` & `giskard-2.0.0b8/giskard/scanner/decorators.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/issues.py` & `giskard-2.0.0b8/giskard/scanner/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/llm/toxicity_detector.py` & `giskard-2.0.0b8/giskard/scanner/llm/toxicity_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/llm/utils.py` & `giskard-2.0.0b8/giskard/scanner/llm/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/performance/issues.py` & `giskard-2.0.0b8/giskard/scanner/performance/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/performance/metrics.py` & `giskard-2.0.0b8/giskard/scanner/performance/metrics.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/performance/performance_bias_detector.py` & `giskard-2.0.0b8/giskard/scanner/performance/performance_bias_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/registry.py` & `giskard-2.0.0b8/giskard/scanner/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/result.py` & `giskard-2.0.0b8/giskard/scanner/result.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,20 +57,20 @@
         uid = id(self)
 
         from pathlib import Path
 
         with Path(__file__).parent.joinpath("templates", "static", "external.js").open("r") as f:
             js_lib = f.read()
 
-        return f'''<iframe id="scan-{uid}" srcdoc="{escaped}" style="width: 100%; border: none;" class="gsk-scan"></iframe>
+        return f"""<iframe id="scan-{uid}" srcdoc="{escaped}" style="width: 100%; border: none;" class="gsk-scan"></iframe>
 <script>
 {js_lib}
 (function(){{iFrameResize({{ checkOrigin: false }}, '#scan-{uid}');}})();
 </script>
-'''
+"""
 
     def to_html(self, filename=None):
         html = self._repr_html_()
 
         if not filename:
             return html
 
@@ -115,13 +115,9 @@
                         tests_cnt[name] = 1
                     else:
                         tests_cnt[name] += 1
                 except:  # noqa
                     pass
         analytics.track(
             "scan:generate_test_suite",
-            {
-                "suite_name": anonymize(name),
-                "tests_cnt": len(suite.tests),
-                **tests_cnt
-            },
+            {"suite_name": anonymize(name), "tests_cnt": len(suite.tests), **tests_cnt},
         )
```

### Comparing `giskard-2.0.0b7/giskard/scanner/robustness/base_detector.py` & `giskard-2.0.0b8/giskard/scanner/robustness/base_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/robustness/entity_swap.py` & `giskard-2.0.0b8/giskard/scanner/robustness/entity_swap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,919 +1,919 @@
 gender_switch_en = {
-    'abbess': 'abbot',
-    'able_seaman': 'able_seawoman',
-    'actress': 'actor',
-    'adulteress': 'adulterer',
-    'adventuress': 'adventurer',
-    'aircraftsman': 'aircraftswoman',
-    'aircrewman': 'aircrewwoman',
-    'alderman': 'alderwoman',
-    'altar_boy': 'altar_girl',
-    'ambassadress': 'ambassador',
-    'ancestress': 'ancestor',
-    'ape-man': 'ape-woman',
-    'archduchess': 'archduke',
-    'artilleryman': 'artillerywoman',
-    'assemblyman': 'assemblywoman',
-    'assemblywoman': 'assemblyman',
-    'au_pair_girl': 'au_pair_boy',
-    'aunt': 'uncle',
-    'authoress': 'author',
-    'aviatrix': 'aviator',
-    'b-girl': 'escort',
-    'bachelor': 'bachelorette',
-    'bachelor_girl': 'bachelor',
-    'backroom_boy': 'backroom_girl',
-    'baggageman': 'baggagewoman',
-    'bagman': 'bagwoman',
-    'ball_boy': 'ball_girl',
-    'ballerina': 'ballet dancer',
-    'bandsman': 'bandswoman',
-    'barmaid': 'barman',
-    'baron': 'baroness',
-    'baroness': 'baron',
-    'bat_boy': 'bat_girl',
-    'batman': 'batwoman',
-    'beadsman': 'beadswoman',
-    'beggarman': 'beggarwoman',
-    'beggarwoman': 'beggarman',
-    'bellboy': 'bellgirl',
-    'benefactress': 'benefactor',
-    'best_man': 'best_woman',
-    'big_sister': 'big brother',
-    'black_man': 'black_woman',
-    'black_woman': 'black_man',
-    'blood_brother': 'blood sister',
-    'boatman': 'boatwoman',
-    'bondman': 'bondwoman',
-    'bondsman': 'bondswoman',
-    'bondwoman': 'bondman',
-    'border_patrolman': 'border_patrolwoman',
-    'boy': 'girl',
-    'boyfriend': 'girlfriend',
-    'brahman': 'brahwoman',
-    'brakeman': 'brakewoman',
-    'bride': 'groom',
-    'bridesmaid': 'groomsman',
-    'broth_of_a_boy': 'broth_of_a_girl',
-    'brother': 'sister',
-    'brownie': 'cub scout',
-    'brunet': 'brunette',
-    'bullyboy': 'bullygirl',
-    'busboy': 'busgirl',
-    'bushman': 'bushwoman',
-    'businessman': 'businesswoman',
-    'businesswoman': 'businessman',
-    'cabin_boy': 'cabin_girl',
-    'call_girl': 'call_boy',
-    'cameraman': 'camerawoman',
-    'campfire_girl': 'campfire_boy',
-    'canary': 'singer',
-    'career_girl': 'career_boy',
-    'career_man': 'career_woman',
-    'cattleman': 'cattlewoman',
-    'cavalryman': 'cavalrywoman',
-    'caveman': 'cavewoman',
-    'chairman_of_the_board': 'chairwoman of the board',
-    'chapman': 'chapwoman',
-    'charwoman': 'charman',
-    'check_girl': 'check_boy',
-    'choirboy': 'choirgirl',
-    'chorus_girl': 'chorus_boy',
-    'city_man': 'city_woman',
-    'clansman': 'clanswoman',
-    'clergyman': 'clergywoman',
-    'co-ed': 'student',
-    'coachman': 'coachwoman',
-    'coalman': 'coalwoman',
-    'coastguardsman': 'coastguardswoman',
-    'coiffeur': 'coiffeuse',
-    'coiffeuse': 'coiffeur',
-    'comedienne': 'comedian',
-    'comfort_woman': 'comfort_man',
-    'committeeman': 'committeewoman',
-    'committeewoman': 'committeeman',
-    'company_man': 'company_woman',
-    'concubine': 'consort',
-    'confidante': 'confidant',
-    'confidence_man': 'confidence_woman',
-    'congressman': 'congresswoman',
-    'cornishman': 'cornishwoman',
-    'cornishwoman': 'cornishman',
-    'councilman': 'councilwoman',
-    'councilwoman': 'councilman',
-    'count': 'countess',
-    'countryman': 'countrywoman',
-    'countrywoman': 'countryman',
-    'cover_girl': 'cover_boy',
-    'cowboy': 'cowgirl',
-    'cowgirl': 'cowboy',
-    'craftsman': 'craftswoman',
-    'crewman': 'crewwoman',
-    'crown_prince': 'crown_princess',
-    'crown_princess': 'heir apparent',
-    'czar': 'czarina',
-    'dad': 'mom',
-    'dairymaid': 'dairyman',
-    'dairyman': 'dairywoman',
-    'dalesman': 'daleswoman',
-    'danseur': 'ballerina',
-    'daughter': 'son',
-    'daughter-in-law': 'son-in-law',
-    'dayboy': 'daygirl',
-    'daygirl': 'dayboy',
-    'deacon': 'deaconess',
-    'deaconess': 'deacon',
-    'deliveryman': 'deliverywoman',
-    'dirty_old_man': 'dirty_old_woman',
-    'divorcee': 'divorcee',
-    'doughboy': 'doughgirl',
-    'draftsman': 'draftswoman',
-    'dragoman': 'dragowoman',
-    'drum_majorette': 'baton twirler',
-    'duenna': 'chaperone',
-    'elder_statesman': 'elder_stateswoman',
-    'embroideress': 'embroiderer',
-    'emperor': 'empress',
-    'empress': 'emperor',
-    'enchantress': 'sorcerer',
-    'end_man': 'end_woman',
-    'englishman': 'englishwoman',
-    'englishwoman': 'englishman',
-    'enlisted_man': 'enlisted_woman',
-    'enlisted_woman': 'enlisted_man',
-    'ent_man': 'ent_woman',
-    'everyman': 'everywoman',
-    'ex-boyfriend': 'ex-girlfriend',
-    'ex-husband': 'ex-wife',
-    'ex-wife': 'ex-husband',
-    'executrix': 'executor',
-    'family_man': 'family_woman',
-    'fancy_man': 'fancy_woman',
-    'farm_boy': 'farm_girl',
-    'farm_girl': 'farm_boy',
-    'farmerette': 'farmer',
-    'father': 'mother',
-    'father-in-law': 'mother-in-law',
-    'female': 'male',
-    'female_aristocrat': 'male aristocrat',
-    'female_child': 'male_child',
-    'female_sibling': 'male sibling',
-    'ferryman': 'ferrywoman',
-    'fireman': 'firewoman',
-    'first_baseman': 'first_basewoman',
-    'fisherman': 'fisherwoman',
-    'flibbertigibbet': 'fool',
-    'flower_girl': 'flower_boy',
-    'footman': 'footwoman',
-    'foreman': 'forewoman',
-    'foremother': 'ancestor',
-    'forewoman': 'foreman',
-    'foster-brother': 'foster-sister',
-    'foster-father': 'foster-mother',
-    'foster-mother': 'foster-father',
-    'foster-sister': 'foster-brother',
-    'foundress': 'founder',
-    'four-minute_man': 'four-minute_woman',
-    'freedman': 'freedwoman',
-    'freeman': 'freewoman',
-    'frenchman': 'frenchwoman',
-    'front_man': 'front_woman',
-    'frontiersman': 'frontierswoman',
-    'frontierswoman': 'frontiersman',
-    'fugleman': 'fuglewoman',
-    'g-man': 'g-woman',
-    'gagman': 'gagwoman',
-    'garbage_man': 'garbage_woman',
-    'gasman': 'gaswoman',
-    'gay_man': 'gay_woman',
-    'gentleman': 'lady',
-    'gentlemen': 'ladies',
-    'gibson_girl': 'gibson_boy',
-    'girl': 'boy',
-    'girl_friday': 'assistant',
-    'girlfriend': 'boyfriend',
-    'goddaughter': 'godson',
-    'godfather': 'godmother',
-    'godmother': 'godfather',
-    'godson': 'goddaughter',
-    'good_old_boy': 'good_old_girl',
-    'governess': 'governor',
-    'granddaughter': 'grandson',
-    'grandfather': 'grandmother',
-    'grandson': 'granddaughter',
-    'great_grandson': 'great granddaughter',
-    'great-aunt': 'great-uncle',
-    'great-nephew': 'great-niece',
-    'grocery_boy': 'grocery_girl',
-    'groom': 'bride',
-    'groomsman': 'groomswoman',
-    'groundsman': 'groundswoman',
-    'guardsman': 'guardswoman',
-    'gunman': 'gunwoman',
-    'guy': 'gal',
-    'half_sister': 'half brother',
-    'handyman': 'handywoman',
-    'hangman': 'hangwoman',
-    'hatchet_man': 'hatchet_woman',
-    'he': 'she',
-    'head_linesman': 'head_lineswoman',
-    'headman': 'headwoman',
-    'headmistress': 'headmaster',
-    'headsman': 'headswoman',
-    'heidelberg_man': 'heidelberg_woman',
-    'heiress': 'heir',
-    'helmsman': 'helmswoman',
-    'her': 'his',
-    'heroine': 'hero',
-    'hers': 'his',
-    'herself': 'himself',
-    'him': 'her',
-    'himself': 'herself',
-    'his': 'her',
-    'holdup_man': 'holdup_woman',
-    'homeboy': 'homegirl',
-    'homegirl': 'homeboy',
-    'honest_woman': 'honest_man',
-    'horseman': 'horsewoman',
-    'horsewoman': 'horseman',
-    'hostess': 'host',
-    'huntress': 'hunter',
-    'husband': 'wife',
-    'iceman': 'icewoman',
-    'idolatress': 'idolater',
-    'inamorata': 'inamorato',
-    'infantryman': 'infantrywoman',
-    'instructress': 'instructor',
-    'irishman': 'irishwoman',
-    'irishwoman': 'irishman',
-    'iron_man': 'iron_woman',
-    'jewess': 'jew',
-    'jilt': 'jilt',
-    'john_doe': 'jane doe',
-    'king': 'queen',
-    'kinsman': 'kinswoman',
-    'kinswoman': 'kinsman',
-    'klansman': 'klanswoman',
-    'lackey': 'servant',
-    'ladies': 'gentlemen',
-    'lady': 'lord',
-    'landlady': 'landlord',
-    'lawman': 'lawwoman',
-    'layman': 'laywoman',
-    'leading_man': 'leading_woman',
-    'letterman': 'letterwoman',
-    'lighterman': 'lighterwoman',
-    'lineman': 'linewoman',
-    'linesman': 'lineswoman',
-    'linkboy': 'linkgirl',
-    'little_brother': 'little sister',
-    'little_sister': 'little brother',
-    'liveryman': 'liverywoman',
-    'lobsterman': 'lobsterwoman',
-    'lollipop_lady': 'crossing guard',
-    'longbowman': 'longbowwoman',
-    'lord': 'lady',
-    'lowerclassman': 'lowerclasswoman',
-    'lumberman': 'lumberwoman',
-    "ma'am": 'sir',
-    'madam': 'sir',
-    'madwoman': 'madman',
-    'maid': 'domestic',
-    'mailman': 'mailwoman',
-    'male': 'female',
-    'male_sibling': 'female sibling',
-    'malik': 'malikah',
-    'mamma': 'pappa',
-    'man': 'woman',
-    'manageress': 'manager',
-    'mannequin': 'model',
-    'marksman': 'markswoman',
-    'masseur': 'masseuse',
-    'matriarch': 'patriarch',
-    'matron': 'warden',
-    'matron_of_honor': 'best man',
-    'mayoress': 'mayor',
-    'mediatrix': 'mediator',
-    'medicine_man': 'medicine_woman',
-    'memsahib': 'sahib',
-    'men': 'women',
-    'messenger_boy': 'messenger_girl',
-    'mestizo': 'mestiza',
-    'middle-aged_man': 'middle-aged_woman',
-    'midshipman': 'midshipwoman',
-    'military_policeman': 'military_policewoman',
-    'militiaman': 'militiawoman',
-    'milkman': 'milkwoman',
-    'mill-girl': 'mill-boy',
-    'millionairess': 'millionaire',
-    'milord': 'milady',
-    'minuteman': 'minutewoman',
-    'miracle_man': 'miracle_woman',
-    'miss': 'mr.',
-    'mistress': 'other man',
-    'monk': 'female monk',
-    'mother': 'father',
+    "abbess": "abbot",
+    "able_seaman": "able_seawoman",
+    "actress": "actor",
+    "adulteress": "adulterer",
+    "adventuress": "adventurer",
+    "aircraftsman": "aircraftswoman",
+    "aircrewman": "aircrewwoman",
+    "alderman": "alderwoman",
+    "altar_boy": "altar_girl",
+    "ambassadress": "ambassador",
+    "ancestress": "ancestor",
+    "ape-man": "ape-woman",
+    "archduchess": "archduke",
+    "artilleryman": "artillerywoman",
+    "assemblyman": "assemblywoman",
+    "assemblywoman": "assemblyman",
+    "au_pair_girl": "au_pair_boy",
+    "aunt": "uncle",
+    "authoress": "author",
+    "aviatrix": "aviator",
+    "b-girl": "escort",
+    "bachelor": "bachelorette",
+    "bachelor_girl": "bachelor",
+    "backroom_boy": "backroom_girl",
+    "baggageman": "baggagewoman",
+    "bagman": "bagwoman",
+    "ball_boy": "ball_girl",
+    "ballerina": "ballet dancer",
+    "bandsman": "bandswoman",
+    "barmaid": "barman",
+    "baron": "baroness",
+    "baroness": "baron",
+    "bat_boy": "bat_girl",
+    "batman": "batwoman",
+    "beadsman": "beadswoman",
+    "beggarman": "beggarwoman",
+    "beggarwoman": "beggarman",
+    "bellboy": "bellgirl",
+    "benefactress": "benefactor",
+    "best_man": "best_woman",
+    "big_sister": "big brother",
+    "black_man": "black_woman",
+    "black_woman": "black_man",
+    "blood_brother": "blood sister",
+    "boatman": "boatwoman",
+    "bondman": "bondwoman",
+    "bondsman": "bondswoman",
+    "bondwoman": "bondman",
+    "border_patrolman": "border_patrolwoman",
+    "boy": "girl",
+    "boyfriend": "girlfriend",
+    "brahman": "brahwoman",
+    "brakeman": "brakewoman",
+    "bride": "groom",
+    "bridesmaid": "groomsman",
+    "broth_of_a_boy": "broth_of_a_girl",
+    "brother": "sister",
+    "brownie": "cub scout",
+    "brunet": "brunette",
+    "bullyboy": "bullygirl",
+    "busboy": "busgirl",
+    "bushman": "bushwoman",
+    "businessman": "businesswoman",
+    "businesswoman": "businessman",
+    "cabin_boy": "cabin_girl",
+    "call_girl": "call_boy",
+    "cameraman": "camerawoman",
+    "campfire_girl": "campfire_boy",
+    "canary": "singer",
+    "career_girl": "career_boy",
+    "career_man": "career_woman",
+    "cattleman": "cattlewoman",
+    "cavalryman": "cavalrywoman",
+    "caveman": "cavewoman",
+    "chairman_of_the_board": "chairwoman of the board",
+    "chapman": "chapwoman",
+    "charwoman": "charman",
+    "check_girl": "check_boy",
+    "choirboy": "choirgirl",
+    "chorus_girl": "chorus_boy",
+    "city_man": "city_woman",
+    "clansman": "clanswoman",
+    "clergyman": "clergywoman",
+    "co-ed": "student",
+    "coachman": "coachwoman",
+    "coalman": "coalwoman",
+    "coastguardsman": "coastguardswoman",
+    "coiffeur": "coiffeuse",
+    "coiffeuse": "coiffeur",
+    "comedienne": "comedian",
+    "comfort_woman": "comfort_man",
+    "committeeman": "committeewoman",
+    "committeewoman": "committeeman",
+    "company_man": "company_woman",
+    "concubine": "consort",
+    "confidante": "confidant",
+    "confidence_man": "confidence_woman",
+    "congressman": "congresswoman",
+    "cornishman": "cornishwoman",
+    "cornishwoman": "cornishman",
+    "councilman": "councilwoman",
+    "councilwoman": "councilman",
+    "count": "countess",
+    "countryman": "countrywoman",
+    "countrywoman": "countryman",
+    "cover_girl": "cover_boy",
+    "cowboy": "cowgirl",
+    "cowgirl": "cowboy",
+    "craftsman": "craftswoman",
+    "crewman": "crewwoman",
+    "crown_prince": "crown_princess",
+    "crown_princess": "heir apparent",
+    "czar": "czarina",
+    "dad": "mom",
+    "dairymaid": "dairyman",
+    "dairyman": "dairywoman",
+    "dalesman": "daleswoman",
+    "danseur": "ballerina",
+    "daughter": "son",
+    "daughter-in-law": "son-in-law",
+    "dayboy": "daygirl",
+    "daygirl": "dayboy",
+    "deacon": "deaconess",
+    "deaconess": "deacon",
+    "deliveryman": "deliverywoman",
+    "dirty_old_man": "dirty_old_woman",
+    "divorcee": "divorcee",
+    "doughboy": "doughgirl",
+    "draftsman": "draftswoman",
+    "dragoman": "dragowoman",
+    "drum_majorette": "baton twirler",
+    "duenna": "chaperone",
+    "elder_statesman": "elder_stateswoman",
+    "embroideress": "embroiderer",
+    "emperor": "empress",
+    "empress": "emperor",
+    "enchantress": "sorcerer",
+    "end_man": "end_woman",
+    "englishman": "englishwoman",
+    "englishwoman": "englishman",
+    "enlisted_man": "enlisted_woman",
+    "enlisted_woman": "enlisted_man",
+    "ent_man": "ent_woman",
+    "everyman": "everywoman",
+    "ex-boyfriend": "ex-girlfriend",
+    "ex-husband": "ex-wife",
+    "ex-wife": "ex-husband",
+    "executrix": "executor",
+    "family_man": "family_woman",
+    "fancy_man": "fancy_woman",
+    "farm_boy": "farm_girl",
+    "farm_girl": "farm_boy",
+    "farmerette": "farmer",
+    "father": "mother",
+    "father-in-law": "mother-in-law",
+    "female": "male",
+    "female_aristocrat": "male aristocrat",
+    "female_child": "male_child",
+    "female_sibling": "male sibling",
+    "ferryman": "ferrywoman",
+    "fireman": "firewoman",
+    "first_baseman": "first_basewoman",
+    "fisherman": "fisherwoman",
+    "flibbertigibbet": "fool",
+    "flower_girl": "flower_boy",
+    "footman": "footwoman",
+    "foreman": "forewoman",
+    "foremother": "ancestor",
+    "forewoman": "foreman",
+    "foster-brother": "foster-sister",
+    "foster-father": "foster-mother",
+    "foster-mother": "foster-father",
+    "foster-sister": "foster-brother",
+    "foundress": "founder",
+    "four-minute_man": "four-minute_woman",
+    "freedman": "freedwoman",
+    "freeman": "freewoman",
+    "frenchman": "frenchwoman",
+    "front_man": "front_woman",
+    "frontiersman": "frontierswoman",
+    "frontierswoman": "frontiersman",
+    "fugleman": "fuglewoman",
+    "g-man": "g-woman",
+    "gagman": "gagwoman",
+    "garbage_man": "garbage_woman",
+    "gasman": "gaswoman",
+    "gay_man": "gay_woman",
+    "gentleman": "lady",
+    "gentlemen": "ladies",
+    "gibson_girl": "gibson_boy",
+    "girl": "boy",
+    "girl_friday": "assistant",
+    "girlfriend": "boyfriend",
+    "goddaughter": "godson",
+    "godfather": "godmother",
+    "godmother": "godfather",
+    "godson": "goddaughter",
+    "good_old_boy": "good_old_girl",
+    "governess": "governor",
+    "granddaughter": "grandson",
+    "grandfather": "grandmother",
+    "grandson": "granddaughter",
+    "great_grandson": "great granddaughter",
+    "great-aunt": "great-uncle",
+    "great-nephew": "great-niece",
+    "grocery_boy": "grocery_girl",
+    "groom": "bride",
+    "groomsman": "groomswoman",
+    "groundsman": "groundswoman",
+    "guardsman": "guardswoman",
+    "gunman": "gunwoman",
+    "guy": "gal",
+    "half_sister": "half brother",
+    "handyman": "handywoman",
+    "hangman": "hangwoman",
+    "hatchet_man": "hatchet_woman",
+    "he": "she",
+    "head_linesman": "head_lineswoman",
+    "headman": "headwoman",
+    "headmistress": "headmaster",
+    "headsman": "headswoman",
+    "heidelberg_man": "heidelberg_woman",
+    "heiress": "heir",
+    "helmsman": "helmswoman",
+    "her": "his",
+    "heroine": "hero",
+    "hers": "his",
+    "herself": "himself",
+    "him": "her",
+    "himself": "herself",
+    "his": "her",
+    "holdup_man": "holdup_woman",
+    "homeboy": "homegirl",
+    "homegirl": "homeboy",
+    "honest_woman": "honest_man",
+    "horseman": "horsewoman",
+    "horsewoman": "horseman",
+    "hostess": "host",
+    "huntress": "hunter",
+    "husband": "wife",
+    "iceman": "icewoman",
+    "idolatress": "idolater",
+    "inamorata": "inamorato",
+    "infantryman": "infantrywoman",
+    "instructress": "instructor",
+    "irishman": "irishwoman",
+    "irishwoman": "irishman",
+    "iron_man": "iron_woman",
+    "jewess": "jew",
+    "jilt": "jilt",
+    "john_doe": "jane doe",
+    "king": "queen",
+    "kinsman": "kinswoman",
+    "kinswoman": "kinsman",
+    "klansman": "klanswoman",
+    "lackey": "servant",
+    "ladies": "gentlemen",
+    "lady": "lord",
+    "landlady": "landlord",
+    "lawman": "lawwoman",
+    "layman": "laywoman",
+    "leading_man": "leading_woman",
+    "letterman": "letterwoman",
+    "lighterman": "lighterwoman",
+    "lineman": "linewoman",
+    "linesman": "lineswoman",
+    "linkboy": "linkgirl",
+    "little_brother": "little sister",
+    "little_sister": "little brother",
+    "liveryman": "liverywoman",
+    "lobsterman": "lobsterwoman",
+    "lollipop_lady": "crossing guard",
+    "longbowman": "longbowwoman",
+    "lord": "lady",
+    "lowerclassman": "lowerclasswoman",
+    "lumberman": "lumberwoman",
+    "ma'am": "sir",
+    "madam": "sir",
+    "madwoman": "madman",
+    "maid": "domestic",
+    "mailman": "mailwoman",
+    "male": "female",
+    "male_sibling": "female sibling",
+    "malik": "malikah",
+    "mamma": "pappa",
+    "man": "woman",
+    "manageress": "manager",
+    "mannequin": "model",
+    "marksman": "markswoman",
+    "masseur": "masseuse",
+    "matriarch": "patriarch",
+    "matron": "warden",
+    "matron_of_honor": "best man",
+    "mayoress": "mayor",
+    "mediatrix": "mediator",
+    "medicine_man": "medicine_woman",
+    "memsahib": "sahib",
+    "men": "women",
+    "messenger_boy": "messenger_girl",
+    "mestizo": "mestiza",
+    "middle-aged_man": "middle-aged_woman",
+    "midshipman": "midshipwoman",
+    "military_policeman": "military_policewoman",
+    "militiaman": "militiawoman",
+    "milkman": "milkwoman",
+    "mill-girl": "mill-boy",
+    "millionairess": "millionaire",
+    "milord": "milady",
+    "minuteman": "minutewoman",
+    "miracle_man": "miracle_woman",
+    "miss": "mr.",
+    "mistress": "other man",
+    "monk": "female monk",
+    "mother": "father",
     "mother's_boy": "mother's_girl",
     "mother's_son": "mother's_daughter",
-    'mr.': 'ms.',
-    'mrs.': 'mr.',
-    'ms.': 'mr.',
-    'muffin_man': 'muffin_woman',
-    'murderess': 'murderer',
-    'muscleman': 'musclewoman',
-    'nabob': 'begum',
-    'nanny': 'manny',
-    'nautch_girl': 'nautch_boy',
-    'negotiatress': 'negotiator',
-    'nephew': 'niece',
-    'newswoman': 'newsman',
-    'niece': 'nephew',
-    'night_watchman': 'night_watchwoman',
-    'nun': 'monk',
-    'oarsman': 'oarswoman',
-    'oarswoman': 'oarsman',
-    'office_boy': 'office_girl',
-    'oilman': 'oilwoman',
-    'oklahoman': 'oklahowoman',
-    'old_boy': 'old_girl',
-    'old_man': 'old_woman',
-    'old_woman': 'old_man',
-    'orangeman': 'orangewoman',
-    'organization_man': 'organization_woman',
-    'ottoman': 'ottowoman',
-    'outdoorsman': 'outdoorswoman',
-    'outdoorswoman': 'outdoorsman',
-    'pachuco': 'pachuca',
-    'paperboy': 'papergirl',
-    'parisienne': 'parisian',
-    'party_girl': 'party_boy',
-    'party_man': 'party_woman',
-    'patroness': 'patron',
-    'piltdown_man': 'piltdown_woman',
-    'pitchman': 'pitchwoman',
-    'placeman': 'placewoman',
-    'plainclothesman': 'plainclotheswoman',
-    'plainsman': 'plainswoman',
-    'plowboy': 'plowgirl',
-    'plowman': 'plowwoman',
-    'poetess': 'poet',
-    'point_man': 'point_woman',
-    'point_woman': 'point_man',
-    'pointsman': 'pointswoman',
-    'police_matron': 'policeman',
-    'policeman': 'policewoman',
-    'poseuse': 'poseur',
-    'posseman': 'possewoman',
-    'poster_boy': 'poster_girl',
-    'poster_girl': 'poster_boy',
-    'postmistress': 'postmaster',
-    'potboy': 'potgirl',
-    'poultryman': 'poultrywoman',
-    'priest': 'priestess',
-    'priestess': 'priest',
-    'prima_donna': 'opera star',
-    'princess': 'prince',
-    'procuress': 'pimp',
-    'property_man': 'property_woman',
-    'prophetess': 'prophet',
-    'proprietress': 'proprietor',
-    'protegee': 'protege',
-    'quarryman': 'quarrywoman',
-    'queen': 'king',
-    'raftsman': 'raftswoman',
-    'remittance_man': 'remittance_woman',
-    'renaissance_man': 'renaissance_woman',
-    'repairman': 'repairwoman',
-    'rifleman': 'riflewoman',
-    'right-hand_man': 'right-hand_woman',
-    'ring_girl': 'ring_boy',
-    'roadman': 'roadwoman',
-    'roman': 'rowoman',
-    'roundsman': 'roundswoman',
-    'salesgirl': 'salesboy',
-    'salesman': 'saleswoman',
-    'sandboy': 'sandgirl',
-    'sandwichman': 'sandwichwoman',
-    'schoolboy': 'schoolgirl',
-    'schoolgirl': 'schoolboy',
-    'schoolman': 'schoolwoman',
-    'schoolmarm': 'schoolteacher',
-    'scotswoman': 'scotsman',
-    'sculptress': 'sculptor',
-    'second_baseman': 'second_basewoman',
-    'section_man': 'section_woman',
-    'seductress': 'seducer',
-    'seedsman': 'seedswoman',
-    'selectman': 'selectwoman',
-    'selectwoman': 'selectman',
-    'senhor': 'senhora',
-    'servant_girl': 'servant_boy',
-    'serviceman': 'servicewoman',
-    'shaheed': 'shahida',
-    'she': 'he',
-    'sheepman': 'sheepwoman',
-    'sheik': 'sheikha',
-    'shepherdess': 'shepherd',
-    'shop_boy': 'shop_girl',
-    'shop_girl': 'shop_boy',
-    'showman': 'showwoman',
-    'sidesman': 'sideswoman',
-    'signalman': 'signalwoman',
-    'sir': 'madam',
-    'sister': 'brother',
-    'sister-in-law': 'brother-in-law',
-    'skivvy': 'domestic servant',
-    'small_businessman': 'small_businesswoman',
-    'son': 'daughter',
-    'son-in-law': 'daughter-in-law',
-    'songstress': 'songster',
-    'soprano': 'singer',
-    'sorceress': 'sorcerer',
-    'soundman': 'soundwoman',
-    'spokesman': 'spokeswoman',
-    'spokeswoman': 'spokesman',
-    'sporting_man': 'sporting_woman',
-    'squaw_man': 'squaw_woman',
-    'stableman': 'stablewoman',
-    'statesman': 'stateswoman',
-    'stateswoman': 'statesman',
-    'stepbrother': 'stepsister',
-    'stepfather': 'stepmother',
-    'stepmother': 'stepfather',
-    'stewardess': 'steward',
-    'stockman': 'stockwoman',
-    'straight_man': 'straight_woman',
-    'strongman': 'strongwoman',
-    'swagman': 'swagwoman',
-    'sweater_girl': 'sweater_boy',
-    't-man': 't-woman',
-    'tallyman': 'tallywoman',
-    'taskmistress': 'taskmaster',
-    'testatrix': 'testator',
-    'third_baseman': 'third_basewoman',
-    'timberman': 'timberwoman',
-    'toast_mistress': 'toastmaster',
-    'tomboy': 'tomgirl',
-    'torch_singer': 'torch singer',
-    'townsman': 'townswoman',
-    'trainbandsman': 'trainbandswoman',
-    'trainman': 'trainwoman',
-    'traveling_salesman': 'traveling_saleswoman',
-    'tribesman': 'tribeswoman',
-    'uncle': 'aunt',
-    'undoer': 'trophy husband',
-    'unmarried_woman': 'unmarried_man',
-    'unpleasant_woman': 'unpleasant_man',
-    'usherette': 'usher',
-    'utility_man': 'utility_woman',
-    'uxor': 'vir',
-    'valley_girl': 'valley_boy',
-    'vestryman': 'vestrywoman',
-    'vestrywoman': 'vestryman',
-    'vice_chairman': 'vice_chairwoman',
-    'villainess': 'villain',
-    'viscountess': 'viscount',
-    'visiting_fireman': 'visiting_firewoman',
-    'waitress': 'waiter',
-    'wardress': 'warder',
-    'washerman': 'washerwoman',
-    'washwoman': 'washman',
-    'watchman': 'watchwoman',
-    'water_boy': 'water_girl',
-    'weatherman': 'weatherwoman',
-    'welshman': 'welshwoman',
-    'white_man': 'white_woman',
-    'white_woman': 'white_man',
-    'widow': 'widower',
-    'widower': 'widow',
-    'wife': 'husband',
-    'wild_man': 'wild_woman',
-    'wingman': 'wingwoman',
-    'wireman': 'wirewoman',
-    'wolf_boy': 'wolf_girl',
-    'woman': 'man',
-    'women': 'men',
-    'wonder_boy': 'wonder_girl',
-    'wonder_woman': 'wonder_man',
-    'woodsman': 'woodswoman',
-    'working_girl': 'working_boy',
-    'workman': 'workwoman',
-    'yachtsman': 'yachtswoman',
-    'yardman': 'yardwoman',
-    'yellow_man': 'yellow_woman',
-    'yellow_woman': 'yellow_man',
-    'yeoman': 'yeowoman',
-    'abbot': 'abbess',
-    'able_seawoman': 'able_seaman',
-    'actor': 'actress',
-    'adulterer': 'adulteress',
-    'adventurer': 'adventuress',
-    'aircraftswoman': 'aircraftsman',
-    'aircrewwoman': 'aircrewman',
-    'alderwoman': 'alderman',
-    'altar_girl': 'altar_boy',
-    'ambassador': 'ambassadress',
-    'ancestor': 'foremother',
-    'ape-woman': 'ape-man',
-    'archduke': 'archduchess',
-    'artillerywoman': 'artilleryman',
-    'au_pair_boy': 'au_pair_girl',
-    'author': 'authoress',
-    'aviator': 'aviatrix',
-    'escort': 'b-girl',
-    'bachelorette': 'bachelor',
-    'backroom_girl': 'backroom_boy',
-    'baggagewoman': 'baggageman',
-    'bagwoman': 'bagman',
-    'ball_girl': 'ball_boy',
-    'ballet dancer': 'ballerina',
-    'bandswoman': 'bandsman',
-    'barman': 'barmaid',
-    'bat_girl': 'bat_boy',
-    'batwoman': 'batman',
-    'beadswoman': 'beadsman',
-    'bellgirl': 'bellboy',
-    'benefactor': 'benefactress',
-    'best_woman': 'best_man',
-    'big brother': 'big_sister',
-    'blood sister': 'blood_brother',
-    'boatwoman': 'boatman',
-    'bondswoman': 'bondsman',
-    'border_patrolwoman': 'border_patrolman',
-    'brahwoman': 'brahman',
-    'brakewoman': 'brakeman',
-    'broth_of_a_girl': 'broth_of_a_boy',
-    'cub scout': 'brownie',
-    'brunette': 'brunet',
-    'bullygirl': 'bullyboy',
-    'busgirl': 'busboy',
-    'bushwoman': 'bushman',
-    'cabin_girl': 'cabin_boy',
-    'call_boy': 'call_girl',
-    'camerawoman': 'cameraman',
-    'campfire_boy': 'campfire_girl',
-    'singer': 'soprano',
-    'career_boy': 'career_girl',
-    'career_woman': 'career_man',
-    'cattlewoman': 'cattleman',
-    'cavalrywoman': 'cavalryman',
-    'cavewoman': 'caveman',
-    'chairwoman of the board': 'chairman_of_the_board',
-    'chapwoman': 'chapman',
-    'charman': 'charwoman',
-    'check_boy': 'check_girl',
-    'choirgirl': 'choirboy',
-    'chorus_boy': 'chorus_girl',
-    'city_woman': 'city_man',
-    'clanswoman': 'clansman',
-    'clergywoman': 'clergyman',
-    'student': 'co-ed',
-    'coachwoman': 'coachman',
-    'coalwoman': 'coalman',
-    'coastguardswoman': 'coastguardsman',
-    'comedian': 'comedienne',
-    'comfort_man': 'comfort_woman',
-    'company_woman': 'company_man',
-    'consort': 'concubine',
-    'confidant': 'confidante',
-    'confidence_woman': 'confidence_man',
-    'congresswoman': 'congressman',
-    'countess': 'count',
-    'cover_boy': 'cover_girl',
-    'craftswoman': 'craftsman',
-    'crewwoman': 'crewman',
-    'heir apparent': 'crown_princess',
-    'czarina': 'czar',
-    'mom': 'dad',
-    'dairywoman': 'dairyman',
-    'daleswoman': 'dalesman',
-    'deliverywoman': 'deliveryman',
-    'dirty_old_woman': 'dirty_old_man',
-    'doughgirl': 'doughboy',
-    'draftswoman': 'draftsman',
-    'dragowoman': 'dragoman',
-    'drum major': 'drum_majorette',
-    'baton twirler': 'drum_majorette',
-    'chaperone': 'duenna',
-    'elder_stateswoman': 'elder_statesman',
-    'embroiderer': 'embroideress',
-    'sorcerer': 'sorceress',
-    'end_woman': 'end_man',
-    'ent_woman': 'ent_man',
-    'everywoman': 'everyman',
-    'ex-girlfriend': 'ex-boyfriend',
-    'executor': 'executrix',
-    'family_woman': 'family_man',
-    'fancy_woman': 'fancy_man',
-    'farmer': 'farmerette',
-    'mother-in-law': 'father-in-law',
-    'male aristocrat': 'female_aristocrat',
-    'male_child': 'female_child',
-    'male sibling': 'female_sibling',
-    'ferrywoman': 'ferryman',
-    'firewoman': 'fireman',
-    'first_basewoman': 'first_baseman',
-    'fisherwoman': 'fisherman',
-    'fool': 'flibbertigibbet',
-    'flower_boy': 'flower_girl',
-    'footwoman': 'footman',
-    'founder': 'foundress',
-    'four-minute_woman': 'four-minute_man',
-    'freedwoman': 'freedman',
-    'freewoman': 'freeman',
-    'frenchwoman': 'frenchman',
-    'front_woman': 'front_man',
-    'fuglewoman': 'fugleman',
-    'g-woman': 'g-man',
-    'gagwoman': 'gagman',
-    'garbage_woman': 'garbage_man',
-    'gaswoman': 'gasman',
-    'gay_woman': 'gay_man',
-    'gibson_boy': 'gibson_girl',
-    'assistant': 'girl_friday',
-    'good_old_girl': 'good_old_boy',
-    'governor': 'governess',
-    'grandmother': 'grandfather',
-    'great granddaughter': 'great_grandson',
-    'great-uncle': 'great-aunt',
-    'great-niece': 'great-nephew',
-    'grocery_girl': 'grocery_boy',
-    'groomswoman': 'groomsman',
-    'groundswoman': 'groundsman',
-    'guardswoman': 'guardsman',
-    'gunwoman': 'gunman',
-    'gal': 'guy',
-    'half brother': 'half_sister',
-    'handywoman': 'handyman',
-    'hangwoman': 'hangman',
-    'hatchet_woman': 'hatchet_man',
-    'head_lineswoman': 'head_linesman',
-    'headwoman': 'headman',
-    'headmaster': 'headmistress',
-    'headswoman': 'headsman',
-    'heidelberg_woman': 'heidelberg_man',
-    'heir': 'heiress',
-    'helmswoman': 'helmsman',
-    'hero': 'heroine',
-    'holdup_woman': 'holdup_man',
-    'honest_man': 'honest_woman',
-    'innkeeper': 'hostess',
-    'host': 'hostess',
-    'hunter': 'huntress',
-    'icewoman': 'iceman',
-    'idolater': 'idolatress',
-    'inamorato': 'inamorata',
-    'infantrywoman': 'infantryman',
-    'instructor': 'instructress',
-    'iron_woman': 'iron_man',
-    'jew': 'jewess',
-    'jane doe': 'john_doe',
-    'klanswoman': 'klansman',
-    'servant': 'lackey',
-    'landlord': 'landlady',
-    'lawwoman': 'lawman',
-    'laywoman': 'layman',
-    'leading_woman': 'leading_man',
-    'letterwoman': 'letterman',
-    'lighterwoman': 'lighterman',
-    'linewoman': 'lineman',
-    'lineswoman': 'linesman',
-    'linkgirl': 'linkboy',
-    'little sister': 'little_brother',
-    'little brother': 'little_sister',
-    'liverywoman': 'liveryman',
-    'lobsterwoman': 'lobsterman',
-    'crossing guard': 'lollipop_lady',
-    'longbowwoman': 'longbowman',
-    'lowerclasswoman': 'lowerclassman',
-    'lumberwoman': 'lumberman',
-    'madman': 'madwoman',
-    'domestic': 'maid',
-    'mailwoman': 'mailman',
-    'female sibling': 'male_sibling',
-    'malikah': 'malik',
-    'pappa': 'mamma',
-    'manager': 'manageress',
-    'model': 'mannequin',
-    'markswoman': 'marksman',
-    'masseuse': 'masseur',
-    'patriarch': 'matriarch',
-    'warden': 'matron',
-    'best man': 'matron_of_honor',
-    'mayor': 'mayoress',
-    'mediator': 'mediatrix',
-    'medicine_woman': 'medicine_man',
-    'sahib': 'memsahib',
-    'messenger_girl': 'messenger_boy',
-    'mestiza': 'mestizo',
-    'middle-aged_woman': 'middle-aged_man',
-    'midshipwoman': 'midshipman',
-    'military_policewoman': 'military_policeman',
-    'militiawoman': 'militiaman',
-    'milkwoman': 'milkman',
-    'mill-boy': 'mill-girl',
-    'millionaire': 'millionairess',
-    'milady': 'milord',
-    'minutewoman': 'minuteman',
-    'miracle_woman': 'miracle_man',
-    'other man': 'mistress',
-    'female monk': 'monk',
+    "mr.": "ms.",
+    "mrs.": "mr.",
+    "ms.": "mr.",
+    "muffin_man": "muffin_woman",
+    "murderess": "murderer",
+    "muscleman": "musclewoman",
+    "nabob": "begum",
+    "nanny": "manny",
+    "nautch_girl": "nautch_boy",
+    "negotiatress": "negotiator",
+    "nephew": "niece",
+    "newswoman": "newsman",
+    "niece": "nephew",
+    "night_watchman": "night_watchwoman",
+    "nun": "monk",
+    "oarsman": "oarswoman",
+    "oarswoman": "oarsman",
+    "office_boy": "office_girl",
+    "oilman": "oilwoman",
+    "oklahoman": "oklahowoman",
+    "old_boy": "old_girl",
+    "old_man": "old_woman",
+    "old_woman": "old_man",
+    "orangeman": "orangewoman",
+    "organization_man": "organization_woman",
+    "ottoman": "ottowoman",
+    "outdoorsman": "outdoorswoman",
+    "outdoorswoman": "outdoorsman",
+    "pachuco": "pachuca",
+    "paperboy": "papergirl",
+    "parisienne": "parisian",
+    "party_girl": "party_boy",
+    "party_man": "party_woman",
+    "patroness": "patron",
+    "piltdown_man": "piltdown_woman",
+    "pitchman": "pitchwoman",
+    "placeman": "placewoman",
+    "plainclothesman": "plainclotheswoman",
+    "plainsman": "plainswoman",
+    "plowboy": "plowgirl",
+    "plowman": "plowwoman",
+    "poetess": "poet",
+    "point_man": "point_woman",
+    "point_woman": "point_man",
+    "pointsman": "pointswoman",
+    "police_matron": "policeman",
+    "policeman": "policewoman",
+    "poseuse": "poseur",
+    "posseman": "possewoman",
+    "poster_boy": "poster_girl",
+    "poster_girl": "poster_boy",
+    "postmistress": "postmaster",
+    "potboy": "potgirl",
+    "poultryman": "poultrywoman",
+    "priest": "priestess",
+    "priestess": "priest",
+    "prima_donna": "opera star",
+    "princess": "prince",
+    "procuress": "pimp",
+    "property_man": "property_woman",
+    "prophetess": "prophet",
+    "proprietress": "proprietor",
+    "protegee": "protege",
+    "quarryman": "quarrywoman",
+    "queen": "king",
+    "raftsman": "raftswoman",
+    "remittance_man": "remittance_woman",
+    "renaissance_man": "renaissance_woman",
+    "repairman": "repairwoman",
+    "rifleman": "riflewoman",
+    "right-hand_man": "right-hand_woman",
+    "ring_girl": "ring_boy",
+    "roadman": "roadwoman",
+    "roman": "rowoman",
+    "roundsman": "roundswoman",
+    "salesgirl": "salesboy",
+    "salesman": "saleswoman",
+    "sandboy": "sandgirl",
+    "sandwichman": "sandwichwoman",
+    "schoolboy": "schoolgirl",
+    "schoolgirl": "schoolboy",
+    "schoolman": "schoolwoman",
+    "schoolmarm": "schoolteacher",
+    "scotswoman": "scotsman",
+    "sculptress": "sculptor",
+    "second_baseman": "second_basewoman",
+    "section_man": "section_woman",
+    "seductress": "seducer",
+    "seedsman": "seedswoman",
+    "selectman": "selectwoman",
+    "selectwoman": "selectman",
+    "senhor": "senhora",
+    "servant_girl": "servant_boy",
+    "serviceman": "servicewoman",
+    "shaheed": "shahida",
+    "she": "he",
+    "sheepman": "sheepwoman",
+    "sheik": "sheikha",
+    "shepherdess": "shepherd",
+    "shop_boy": "shop_girl",
+    "shop_girl": "shop_boy",
+    "showman": "showwoman",
+    "sidesman": "sideswoman",
+    "signalman": "signalwoman",
+    "sir": "madam",
+    "sister": "brother",
+    "sister-in-law": "brother-in-law",
+    "skivvy": "domestic servant",
+    "small_businessman": "small_businesswoman",
+    "son": "daughter",
+    "son-in-law": "daughter-in-law",
+    "songstress": "songster",
+    "soprano": "singer",
+    "sorceress": "sorcerer",
+    "soundman": "soundwoman",
+    "spokesman": "spokeswoman",
+    "spokeswoman": "spokesman",
+    "sporting_man": "sporting_woman",
+    "squaw_man": "squaw_woman",
+    "stableman": "stablewoman",
+    "statesman": "stateswoman",
+    "stateswoman": "statesman",
+    "stepbrother": "stepsister",
+    "stepfather": "stepmother",
+    "stepmother": "stepfather",
+    "stewardess": "steward",
+    "stockman": "stockwoman",
+    "straight_man": "straight_woman",
+    "strongman": "strongwoman",
+    "swagman": "swagwoman",
+    "sweater_girl": "sweater_boy",
+    "t-man": "t-woman",
+    "tallyman": "tallywoman",
+    "taskmistress": "taskmaster",
+    "testatrix": "testator",
+    "third_baseman": "third_basewoman",
+    "timberman": "timberwoman",
+    "toast_mistress": "toastmaster",
+    "tomboy": "tomgirl",
+    "torch_singer": "torch singer",
+    "townsman": "townswoman",
+    "trainbandsman": "trainbandswoman",
+    "trainman": "trainwoman",
+    "traveling_salesman": "traveling_saleswoman",
+    "tribesman": "tribeswoman",
+    "uncle": "aunt",
+    "undoer": "trophy husband",
+    "unmarried_woman": "unmarried_man",
+    "unpleasant_woman": "unpleasant_man",
+    "usherette": "usher",
+    "utility_man": "utility_woman",
+    "uxor": "vir",
+    "valley_girl": "valley_boy",
+    "vestryman": "vestrywoman",
+    "vestrywoman": "vestryman",
+    "vice_chairman": "vice_chairwoman",
+    "villainess": "villain",
+    "viscountess": "viscount",
+    "visiting_fireman": "visiting_firewoman",
+    "waitress": "waiter",
+    "wardress": "warder",
+    "washerman": "washerwoman",
+    "washwoman": "washman",
+    "watchman": "watchwoman",
+    "water_boy": "water_girl",
+    "weatherman": "weatherwoman",
+    "welshman": "welshwoman",
+    "white_man": "white_woman",
+    "white_woman": "white_man",
+    "widow": "widower",
+    "widower": "widow",
+    "wife": "husband",
+    "wild_man": "wild_woman",
+    "wingman": "wingwoman",
+    "wireman": "wirewoman",
+    "wolf_boy": "wolf_girl",
+    "woman": "man",
+    "women": "men",
+    "wonder_boy": "wonder_girl",
+    "wonder_woman": "wonder_man",
+    "woodsman": "woodswoman",
+    "working_girl": "working_boy",
+    "workman": "workwoman",
+    "yachtsman": "yachtswoman",
+    "yardman": "yardwoman",
+    "yellow_man": "yellow_woman",
+    "yellow_woman": "yellow_man",
+    "yeoman": "yeowoman",
+    "abbot": "abbess",
+    "able_seawoman": "able_seaman",
+    "actor": "actress",
+    "adulterer": "adulteress",
+    "adventurer": "adventuress",
+    "aircraftswoman": "aircraftsman",
+    "aircrewwoman": "aircrewman",
+    "alderwoman": "alderman",
+    "altar_girl": "altar_boy",
+    "ambassador": "ambassadress",
+    "ancestor": "foremother",
+    "ape-woman": "ape-man",
+    "archduke": "archduchess",
+    "artillerywoman": "artilleryman",
+    "au_pair_boy": "au_pair_girl",
+    "author": "authoress",
+    "aviator": "aviatrix",
+    "escort": "b-girl",
+    "bachelorette": "bachelor",
+    "backroom_girl": "backroom_boy",
+    "baggagewoman": "baggageman",
+    "bagwoman": "bagman",
+    "ball_girl": "ball_boy",
+    "ballet dancer": "ballerina",
+    "bandswoman": "bandsman",
+    "barman": "barmaid",
+    "bat_girl": "bat_boy",
+    "batwoman": "batman",
+    "beadswoman": "beadsman",
+    "bellgirl": "bellboy",
+    "benefactor": "benefactress",
+    "best_woman": "best_man",
+    "big brother": "big_sister",
+    "blood sister": "blood_brother",
+    "boatwoman": "boatman",
+    "bondswoman": "bondsman",
+    "border_patrolwoman": "border_patrolman",
+    "brahwoman": "brahman",
+    "brakewoman": "brakeman",
+    "broth_of_a_girl": "broth_of_a_boy",
+    "cub scout": "brownie",
+    "brunette": "brunet",
+    "bullygirl": "bullyboy",
+    "busgirl": "busboy",
+    "bushwoman": "bushman",
+    "cabin_girl": "cabin_boy",
+    "call_boy": "call_girl",
+    "camerawoman": "cameraman",
+    "campfire_boy": "campfire_girl",
+    "singer": "soprano",
+    "career_boy": "career_girl",
+    "career_woman": "career_man",
+    "cattlewoman": "cattleman",
+    "cavalrywoman": "cavalryman",
+    "cavewoman": "caveman",
+    "chairwoman of the board": "chairman_of_the_board",
+    "chapwoman": "chapman",
+    "charman": "charwoman",
+    "check_boy": "check_girl",
+    "choirgirl": "choirboy",
+    "chorus_boy": "chorus_girl",
+    "city_woman": "city_man",
+    "clanswoman": "clansman",
+    "clergywoman": "clergyman",
+    "student": "co-ed",
+    "coachwoman": "coachman",
+    "coalwoman": "coalman",
+    "coastguardswoman": "coastguardsman",
+    "comedian": "comedienne",
+    "comfort_man": "comfort_woman",
+    "company_woman": "company_man",
+    "consort": "concubine",
+    "confidant": "confidante",
+    "confidence_woman": "confidence_man",
+    "congresswoman": "congressman",
+    "countess": "count",
+    "cover_boy": "cover_girl",
+    "craftswoman": "craftsman",
+    "crewwoman": "crewman",
+    "heir apparent": "crown_princess",
+    "czarina": "czar",
+    "mom": "dad",
+    "dairywoman": "dairyman",
+    "daleswoman": "dalesman",
+    "deliverywoman": "deliveryman",
+    "dirty_old_woman": "dirty_old_man",
+    "doughgirl": "doughboy",
+    "draftswoman": "draftsman",
+    "dragowoman": "dragoman",
+    "drum major": "drum_majorette",
+    "baton twirler": "drum_majorette",
+    "chaperone": "duenna",
+    "elder_stateswoman": "elder_statesman",
+    "embroiderer": "embroideress",
+    "sorcerer": "sorceress",
+    "end_woman": "end_man",
+    "ent_woman": "ent_man",
+    "everywoman": "everyman",
+    "ex-girlfriend": "ex-boyfriend",
+    "executor": "executrix",
+    "family_woman": "family_man",
+    "fancy_woman": "fancy_man",
+    "farmer": "farmerette",
+    "mother-in-law": "father-in-law",
+    "male aristocrat": "female_aristocrat",
+    "male_child": "female_child",
+    "male sibling": "female_sibling",
+    "ferrywoman": "ferryman",
+    "firewoman": "fireman",
+    "first_basewoman": "first_baseman",
+    "fisherwoman": "fisherman",
+    "fool": "flibbertigibbet",
+    "flower_boy": "flower_girl",
+    "footwoman": "footman",
+    "founder": "foundress",
+    "four-minute_woman": "four-minute_man",
+    "freedwoman": "freedman",
+    "freewoman": "freeman",
+    "frenchwoman": "frenchman",
+    "front_woman": "front_man",
+    "fuglewoman": "fugleman",
+    "g-woman": "g-man",
+    "gagwoman": "gagman",
+    "garbage_woman": "garbage_man",
+    "gaswoman": "gasman",
+    "gay_woman": "gay_man",
+    "gibson_boy": "gibson_girl",
+    "assistant": "girl_friday",
+    "good_old_girl": "good_old_boy",
+    "governor": "governess",
+    "grandmother": "grandfather",
+    "great granddaughter": "great_grandson",
+    "great-uncle": "great-aunt",
+    "great-niece": "great-nephew",
+    "grocery_girl": "grocery_boy",
+    "groomswoman": "groomsman",
+    "groundswoman": "groundsman",
+    "guardswoman": "guardsman",
+    "gunwoman": "gunman",
+    "gal": "guy",
+    "half brother": "half_sister",
+    "handywoman": "handyman",
+    "hangwoman": "hangman",
+    "hatchet_woman": "hatchet_man",
+    "head_lineswoman": "head_linesman",
+    "headwoman": "headman",
+    "headmaster": "headmistress",
+    "headswoman": "headsman",
+    "heidelberg_woman": "heidelberg_man",
+    "heir": "heiress",
+    "helmswoman": "helmsman",
+    "hero": "heroine",
+    "holdup_woman": "holdup_man",
+    "honest_man": "honest_woman",
+    "innkeeper": "hostess",
+    "host": "hostess",
+    "hunter": "huntress",
+    "icewoman": "iceman",
+    "idolater": "idolatress",
+    "inamorato": "inamorata",
+    "infantrywoman": "infantryman",
+    "instructor": "instructress",
+    "iron_woman": "iron_man",
+    "jew": "jewess",
+    "jane doe": "john_doe",
+    "klanswoman": "klansman",
+    "servant": "lackey",
+    "landlord": "landlady",
+    "lawwoman": "lawman",
+    "laywoman": "layman",
+    "leading_woman": "leading_man",
+    "letterwoman": "letterman",
+    "lighterwoman": "lighterman",
+    "linewoman": "lineman",
+    "lineswoman": "linesman",
+    "linkgirl": "linkboy",
+    "little sister": "little_brother",
+    "little brother": "little_sister",
+    "liverywoman": "liveryman",
+    "lobsterwoman": "lobsterman",
+    "crossing guard": "lollipop_lady",
+    "longbowwoman": "longbowman",
+    "lowerclasswoman": "lowerclassman",
+    "lumberwoman": "lumberman",
+    "madman": "madwoman",
+    "domestic": "maid",
+    "mailwoman": "mailman",
+    "female sibling": "male_sibling",
+    "malikah": "malik",
+    "pappa": "mamma",
+    "manager": "manageress",
+    "model": "mannequin",
+    "markswoman": "marksman",
+    "masseuse": "masseur",
+    "patriarch": "matriarch",
+    "warden": "matron",
+    "best man": "matron_of_honor",
+    "mayor": "mayoress",
+    "mediator": "mediatrix",
+    "medicine_woman": "medicine_man",
+    "sahib": "memsahib",
+    "messenger_girl": "messenger_boy",
+    "mestiza": "mestizo",
+    "middle-aged_woman": "middle-aged_man",
+    "midshipwoman": "midshipman",
+    "military_policewoman": "military_policeman",
+    "militiawoman": "militiaman",
+    "milkwoman": "milkman",
+    "mill-boy": "mill-girl",
+    "millionaire": "millionairess",
+    "milady": "milord",
+    "minutewoman": "minuteman",
+    "miracle_woman": "miracle_man",
+    "other man": "mistress",
+    "female monk": "monk",
     "mother's_girl": "mother's_boy",
     "mother's_daughter": "mother's_son",
-    'muffin_woman': 'muffin_man',
-    'murderer': 'murderess',
-    'musclewoman': 'muscleman',
-    'begum': 'nabob',
-    'manny': 'nanny',
-    'nautch_boy': 'nautch_girl',
-    'negotiator': 'negotiatress',
-    'newsman': 'newswoman',
-    'night_watchwoman': 'night_watchman',
-    'office_girl': 'office_boy',
-    'oilwoman': 'oilman',
-    'oklahowoman': 'oklahoman',
-    'old_girl': 'old_boy',
-    'orangewoman': 'orangeman',
-    'organization_woman': 'organization_man',
-    'ottowoman': 'ottoman',
-    'pachuca': 'pachuco',
-    'papergirl': 'paperboy',
-    'parisian': 'parisienne',
-    'party_boy': 'party_girl',
-    'party_woman': 'party_man',
-    'patron': 'patroness',
-    'piltdown_woman': 'piltdown_man',
-    'pitchwoman': 'pitchman',
-    'placewoman': 'placeman',
-    'plainclotheswoman': 'plainclothesman',
-    'plainswoman': 'plainsman',
-    'plowgirl': 'plowboy',
-    'plowwoman': 'plowman',
-    'poet': 'poetess',
-    'pointswoman': 'pointsman',
-    'policewoman': 'policeman',
-    'poseur': 'poseuse',
-    'possewoman': 'posseman',
-    'postmaster': 'postmistress',
-    'potgirl': 'potboy',
-    'poultrywoman': 'poultryman',
-    'opera star': 'prima_donna',
-    'prince': 'princess',
-    'pimp': 'procuress',
-    'property_woman': 'property_man',
-    'prophet': 'prophetess',
-    'proprietor': 'proprietress',
-    'protege': 'protegee',
-    'quarrywoman': 'quarryman',
-    'raftswoman': 'raftsman',
-    'remittance_woman': 'remittance_man',
-    'renaissance_woman': 'renaissance_man',
-    'repairwoman': 'repairman',
-    'riflewoman': 'rifleman',
-    'right-hand_woman': 'right-hand_man',
-    'ring_boy': 'ring_girl',
-    'roadwoman': 'roadman',
-    'rowoman': 'roman',
-    'roundswoman': 'roundsman',
-    'salesboy': 'salesgirl',
-    'saleswoman': 'salesman',
-    'sandgirl': 'sandboy',
-    'sandwichwoman': 'sandwichman',
-    'schoolwoman': 'schoolman',
-    'schoolteacher': 'schoolmarm',
-    'scotsman': 'scotswoman',
-    'sculptor': 'sculptress',
-    'second_basewoman': 'second_baseman',
-    'section_woman': 'section_man',
-    'seducer': 'seductress',
-    'seedswoman': 'seedsman',
-    'senhora': 'senhor',
-    'servant_boy': 'servant_girl',
-    'servicewoman': 'serviceman',
-    'shahida': 'shaheed',
-    'sheepwoman': 'sheepman',
-    'sheikha': 'sheik',
-    'shepherd': 'shepherdess',
-    'showwoman': 'showman',
-    'sideswoman': 'sidesman',
-    'signalwoman': 'signalman',
-    'brother-in-law': 'sister-in-law',
-    'domestic servant': 'skivvy',
-    'small_businesswoman': 'small_businessman',
-    'songster': 'songstress',
-    'soundwoman': 'soundman',
-    'sporting_woman': 'sporting_man',
-    'squaw_woman': 'squaw_man',
-    'stablewoman': 'stableman',
-    'stepsister': 'stepbrother',
-    'steward': 'stewardess',
-    'stockwoman': 'stockman',
-    'straight_woman': 'straight_man',
-    'strongwoman': 'strongman',
-    'swagwoman': 'swagman',
-    'sweater_boy': 'sweater_girl',
-    't-woman': 't-man',
-    'tallywoman': 'tallyman',
-    'taskmaster': 'taskmistress',
-    'testator': 'testatrix',
-    'third_basewoman': 'third_baseman',
-    'timberwoman': 'timberman',
-    'toastmaster': 'toast_mistress',
-    'tomgirl': 'tomboy',
-    'torch singer': 'torch_singer',
-    'townswoman': 'townsman',
-    'trainbandswoman': 'trainbandsman',
-    'trainwoman': 'trainman',
-    'traveling_saleswoman': 'traveling_salesman',
-    'tribeswoman': 'tribesman',
-    'trophy husband': 'undoer',
-    'unmarried_man': 'unmarried_woman',
-    'unpleasant_man': 'unpleasant_woman',
-    'usher': 'usherette',
-    'utility_woman': 'utility_man',
-    'vir': 'uxor',
-    'valley_boy': 'valley_girl',
-    'vice_chairwoman': 'vice_chairman',
-    'villain': 'villainess',
-    'viscount': 'viscountess',
-    'visiting_firewoman': 'visiting_fireman',
-    'waiter': 'waitress',
-    'warder': 'wardress',
-    'washerwoman': 'washerman',
-    'washman': 'washwoman',
-    'watchwoman': 'watchman',
-    'water_girl': 'water_boy',
-    'weatherwoman': 'weatherman',
-    'welshwoman': 'welshman',
-    'wild_woman': 'wild_man',
-    'wingwoman': 'wingman',
-    'wirewoman': 'wireman',
-    'wolf_girl': 'wolf_boy',
-    'wonder_girl': 'wonder_boy',
-    'wonder_man': 'wonder_woman',
-    'woodswoman': 'woodsman',
-    'working_boy': 'working_girl',
-    'workwoman': 'workman',
-    'yachtswoman': 'yachtsman',
-    'yardwoman': 'yardman',
-    'yeowoman': 'yeoman',
+    "muffin_woman": "muffin_man",
+    "murderer": "murderess",
+    "musclewoman": "muscleman",
+    "begum": "nabob",
+    "manny": "nanny",
+    "nautch_boy": "nautch_girl",
+    "negotiator": "negotiatress",
+    "newsman": "newswoman",
+    "night_watchwoman": "night_watchman",
+    "office_girl": "office_boy",
+    "oilwoman": "oilman",
+    "oklahowoman": "oklahoman",
+    "old_girl": "old_boy",
+    "orangewoman": "orangeman",
+    "organization_woman": "organization_man",
+    "ottowoman": "ottoman",
+    "pachuca": "pachuco",
+    "papergirl": "paperboy",
+    "parisian": "parisienne",
+    "party_boy": "party_girl",
+    "party_woman": "party_man",
+    "patron": "patroness",
+    "piltdown_woman": "piltdown_man",
+    "pitchwoman": "pitchman",
+    "placewoman": "placeman",
+    "plainclotheswoman": "plainclothesman",
+    "plainswoman": "plainsman",
+    "plowgirl": "plowboy",
+    "plowwoman": "plowman",
+    "poet": "poetess",
+    "pointswoman": "pointsman",
+    "policewoman": "policeman",
+    "poseur": "poseuse",
+    "possewoman": "posseman",
+    "postmaster": "postmistress",
+    "potgirl": "potboy",
+    "poultrywoman": "poultryman",
+    "opera star": "prima_donna",
+    "prince": "princess",
+    "pimp": "procuress",
+    "property_woman": "property_man",
+    "prophet": "prophetess",
+    "proprietor": "proprietress",
+    "protege": "protegee",
+    "quarrywoman": "quarryman",
+    "raftswoman": "raftsman",
+    "remittance_woman": "remittance_man",
+    "renaissance_woman": "renaissance_man",
+    "repairwoman": "repairman",
+    "riflewoman": "rifleman",
+    "right-hand_woman": "right-hand_man",
+    "ring_boy": "ring_girl",
+    "roadwoman": "roadman",
+    "rowoman": "roman",
+    "roundswoman": "roundsman",
+    "salesboy": "salesgirl",
+    "saleswoman": "salesman",
+    "sandgirl": "sandboy",
+    "sandwichwoman": "sandwichman",
+    "schoolwoman": "schoolman",
+    "schoolteacher": "schoolmarm",
+    "scotsman": "scotswoman",
+    "sculptor": "sculptress",
+    "second_basewoman": "second_baseman",
+    "section_woman": "section_man",
+    "seducer": "seductress",
+    "seedswoman": "seedsman",
+    "senhora": "senhor",
+    "servant_boy": "servant_girl",
+    "servicewoman": "serviceman",
+    "shahida": "shaheed",
+    "sheepwoman": "sheepman",
+    "sheikha": "sheik",
+    "shepherd": "shepherdess",
+    "showwoman": "showman",
+    "sideswoman": "sidesman",
+    "signalwoman": "signalman",
+    "brother-in-law": "sister-in-law",
+    "domestic servant": "skivvy",
+    "small_businesswoman": "small_businessman",
+    "songster": "songstress",
+    "soundwoman": "soundman",
+    "sporting_woman": "sporting_man",
+    "squaw_woman": "squaw_man",
+    "stablewoman": "stableman",
+    "stepsister": "stepbrother",
+    "steward": "stewardess",
+    "stockwoman": "stockman",
+    "straight_woman": "straight_man",
+    "strongwoman": "strongman",
+    "swagwoman": "swagman",
+    "sweater_boy": "sweater_girl",
+    "t-woman": "t-man",
+    "tallywoman": "tallyman",
+    "taskmaster": "taskmistress",
+    "testator": "testatrix",
+    "third_basewoman": "third_baseman",
+    "timberwoman": "timberman",
+    "toastmaster": "toast_mistress",
+    "tomgirl": "tomboy",
+    "torch singer": "torch_singer",
+    "townswoman": "townsman",
+    "trainbandswoman": "trainbandsman",
+    "trainwoman": "trainman",
+    "traveling_saleswoman": "traveling_salesman",
+    "tribeswoman": "tribesman",
+    "trophy husband": "undoer",
+    "unmarried_man": "unmarried_woman",
+    "unpleasant_man": "unpleasant_woman",
+    "usher": "usherette",
+    "utility_woman": "utility_man",
+    "vir": "uxor",
+    "valley_boy": "valley_girl",
+    "vice_chairwoman": "vice_chairman",
+    "villain": "villainess",
+    "viscount": "viscountess",
+    "visiting_firewoman": "visiting_fireman",
+    "waiter": "waitress",
+    "warder": "wardress",
+    "washerwoman": "washerman",
+    "washman": "washwoman",
+    "watchwoman": "watchman",
+    "water_girl": "water_boy",
+    "weatherwoman": "weatherman",
+    "welshwoman": "welshman",
+    "wild_woman": "wild_man",
+    "wingwoman": "wingman",
+    "wirewoman": "wireman",
+    "wolf_girl": "wolf_boy",
+    "wonder_girl": "wonder_boy",
+    "wonder_man": "wonder_woman",
+    "woodswoman": "woodsman",
+    "working_boy": "working_girl",
+    "workwoman": "workman",
+    "yachtswoman": "yachtsman",
+    "yardwoman": "yardman",
+    "yeowoman": "yeoman",
 }
 
 # Modifying the religion_dict using the list of religions from the ethnicity_dict
 religion_dict_en = [
-    ['buddhism', 'christianity', 'hinduism', 'islam', 'judaism'],
-    ['siddhartha gautama', 'jesus christ', 'muhammad', 'abraham'],
-    ['buddhist', 'christian', 'hindu', 'muslim', 'jew'],
-    ['allah', 'god'],
-    ['temple', 'church', 'temple', 'mosque', 'synagogue'],
-    ['bodh gaya', "vatican", "kumbh mela", "mecca", "jerusalem"],
+    ["buddhism", "christianity", "hinduism", "islam", "judaism"],
+    ["siddhartha gautama", "jesus christ", "muhammad", "abraham"],
+    ["buddhist", "christian", "hindu", "muslim", "jew"],
+    ["allah", "god"],
+    ["temple", "church", "temple", "mosque", "synagogue"],
+    ["bodh gaya", "vatican", "kumbh mela", "mecca", "jerusalem"],
     ["tripitaka", "bible", "veda", "quran", "talmud"],
-    ['dalai lama', 'pope', "imam", "rabbi"],
+    ["dalai lama", "pope", "imam", "rabbi"],
 ]
 
 religion_dict_fr = [
-    ['bouddhisme', 'christianisme', 'hindouisme', 'islam', 'judaïsme'],
-    ['siddhartha gautama', 'jésus christ', 'muhammad', 'abraham'],
-    ['bouddhiste', 'chrétien', 'hindou', 'musulman', 'juif'],
-    ['dieu', 'allah'],
-    ['temple', 'église', 'temple', 'mosquée', 'synagogue'],
-    ['bodh gaya', "vatican", "kumbh mela", "la mecque", "jérusalem"],
+    ["bouddhisme", "christianisme", "hindouisme", "islam", "judaïsme"],
+    ["siddhartha gautama", "jésus christ", "muhammad", "abraham"],
+    ["bouddhiste", "chrétien", "hindou", "musulman", "juif"],
+    ["dieu", "allah"],
+    ["temple", "église", "temple", "mosquée", "synagogue"],
+    ["bodh gaya", "vatican", "kumbh mela", "la mecque", "jérusalem"],
     ["tripitaka", "bible", "veda", "coran", "talmud"],
-    ['dalai lama', 'pape', "imam", "rabbin"],
+    ["dalai lama", "pape", "imam", "rabbin"],
 ]
 
 
 typos = {
-    'a': ['s', 'z', 'q', 'w', 'x'],
-    'b': ['v', 'n', 'g', 'h'],
-    'c': ['x', 'v', 'f', 'd'],
-    'd': ['s', 'e', 'r', 'f', 'c', 'x'],
-    'e': ['w', 's', 'd', 'r'],
-    'f': ['d', 'r', 't', 'g', 'v', 'c'],
-    'g': ['f', 't', 'y', 'h', 'b', 'v'],
-    'h': ['g', 'y', 'u', 'j', 'n', 'b'],
-    'i': ['u', 'j', 'k', 'o'],
-    'j': ['h', 'u', 'i', 'k', 'm', 'n'],
-    'k': ['j', 'i', 'o', 'l', 'm'],
-    'l': ['k', 'o', 'p'],
-    'm': ['n', 'j', 'k'],
-    'n': ['b', 'h', 'j', 'm'],
-    'o': ['i', 'k', 'l', 'p'],
-    'p': ['o', 'l'],
-    'q': ['a', 'w'],
-    'r': ['e', 'd', 'f', 't'],
-    's': ['a', 'w', 'd', 'x', 'z'],
-    't': ['r', 'f', 'g', 'y'],
-    'u': ['y', 'h', 'j', 'i'],
-    'v': ['c', 'f', 'g', 'b'],
-    'w': ['q', 'a', 's', 'e'],
-    'x': ['z', 's', 'd', 'c'],
-    'y': ['t', 'g', 'h', 'u'],
-    'z': ['a', 's', 'x'],
+    "a": ["s", "z", "q", "w", "x"],
+    "b": ["v", "n", "g", "h"],
+    "c": ["x", "v", "f", "d"],
+    "d": ["s", "e", "r", "f", "c", "x"],
+    "e": ["w", "s", "d", "r"],
+    "f": ["d", "r", "t", "g", "v", "c"],
+    "g": ["f", "t", "y", "h", "b", "v"],
+    "h": ["g", "y", "u", "j", "n", "b"],
+    "i": ["u", "j", "k", "o"],
+    "j": ["h", "u", "i", "k", "m", "n"],
+    "k": ["j", "i", "o", "l", "m"],
+    "l": ["k", "o", "p"],
+    "m": ["n", "j", "k"],
+    "n": ["b", "h", "j", "m"],
+    "o": ["i", "k", "l", "p"],
+    "p": ["o", "l"],
+    "q": ["a", "w"],
+    "r": ["e", "d", "f", "t"],
+    "s": ["a", "w", "d", "x", "z"],
+    "t": ["r", "f", "g", "y"],
+    "u": ["y", "h", "j", "i"],
+    "v": ["c", "f", "g", "b"],
+    "w": ["q", "a", "s", "e"],
+    "x": ["z", "s", "d", "c"],
+    "y": ["t", "g", "h", "u"],
+    "z": ["a", "s", "x"],
 }
 
 gender_switch_fr = {
     "abaissant": "abaissante",
     "abaissante": "abaissant",
     "abaissé": "abaissée",
     "abaissée": "abaissé",
```

### Comparing `giskard-2.0.0b7/giskard/scanner/robustness/ethical_bias_detector.py` & `giskard-2.0.0b8/giskard/scanner/robustness/ethical_bias_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 from .base_detector import BaseTextPerturbationDetector
 from .text_transformations import TextTransformation
 from ...datasets.base import Dataset
 from ...models.base import BaseModel
 from ..decorators import detector
 
 
-@detector(name="ethical_bias", tags=["ethical_bias", "robustness", "nlp", "classification", "regression", "generative", "text_generation", "llm"])
+@detector(
+    name="ethical_bias",
+    tags=["ethical_bias", "robustness", "nlp", "classification", "regression", "generative", "text_generation", "llm"],
+)
 class EthicalBiasDetector(BaseTextPerturbationDetector):
     _issue_cls = EthicalIssue
 
     def _get_default_transformations(self, model: BaseModel, dataset: Dataset) -> Sequence[TextTransformation]:
         from .text_transformations import (
             TextGenderTransformation,
             TextReligionTransformation,
```

### Comparing `giskard-2.0.0b7/giskard/scanner/robustness/issues.py` & `giskard-2.0.0b8/giskard/scanner/robustness/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/robustness/nationalities.json` & `giskard-2.0.0b8/giskard/scanner/robustness/nationalities.json`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/robustness/text_perturbation_detector.py` & `giskard-2.0.0b8/giskard/scanner/robustness/text_perturbation_detector.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,24 @@
 from ...datasets.base import Dataset
 from ...models.base import BaseModel
 from ..decorators import detector
 
 
 @detector(
     name="text_perturbation",
-    tags=["text_perturbation", "robustness", "nlp", "classification", "regression", "generative", "text_generation", "llm"],
+    tags=[
+        "text_perturbation",
+        "robustness",
+        "nlp",
+        "classification",
+        "regression",
+        "generative",
+        "text_generation",
+        "llm",
+    ],
 )
 class TextPerturbationDetector(BaseTextPerturbationDetector):
     def _get_default_transformations(self, model: BaseModel, dataset: Dataset) -> Sequence[TextTransformation]:
         from .text_transformations import (
             TextUppercase,
             TextLowercase,
             TextTitleCase,
```

### Comparing `giskard-2.0.0b7/giskard/scanner/robustness/text_transformations.py` & `giskard-2.0.0b8/giskard/scanner/robustness/text_transformations.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 
 class TextTransformation(TransformationFunction):
     name: str
 
     def __init__(self, column):
         super().__init__(None, row_level=False, cell_level=False)
         self.column = column
-        self.meta = DatasetProcessFunctionMeta(type='TRANSFORMATION')
+        self.meta = DatasetProcessFunctionMeta(type="TRANSFORMATION")
         self.meta.uuid = get_object_uuid(self)
         self.meta.code = self.name
         self.meta.name = self.name
         self.meta.display_name = self.name
         self.meta.tags = ["pickle", "scan"]
-        self.meta.doc = 'Automatically generated transformation function'
+        self.meta.doc = "Automatically generated transformation function"
 
     def execute(self, data: pd.DataFrame) -> pd.DataFrame:
         feature_data = data[self.column].dropna().astype(str)
         data.loc[feature_data.index, self.column] = feature_data.apply(self.make_perturbation)
         return data
 
     def make_perturbation(self, text: str) -> str:
@@ -78,31 +78,31 @@
             new_text.append(self._add_typos(token))
         return " ".join(new_text)
 
     def _add_typos(self, word):
         # Get the token's word and apply a perturbation with probability 0.1
         if random.random() < 0.2 and len(word) > 1:
             # Choose a perturbation type randomly
-            perturbation_type = random.choice(['insert', 'delete', 'replace'])
+            perturbation_type = random.choice(["insert", "delete", "replace"])
             # Apply the perturbation
-            if perturbation_type == 'insert':
+            if perturbation_type == "insert":
                 idx = random.randint(0, len(word))
                 new_char = chr(random.randint(33, 126))
                 word = word[:idx] + new_char + word[idx:]
                 return word
-            elif perturbation_type == 'delete':
+            elif perturbation_type == "delete":
                 idx = random.randint(0, len(word) - 1)
-                word = word[:idx] + word[idx + 1:]
+                word = word[:idx] + word[idx + 1 :]
                 return word
-            elif perturbation_type == 'replace':
+            elif perturbation_type == "replace":
                 j = random.randint(0, len(word) - 1)
                 c = word[j]
                 if c in self._typos:
                     replacement = random.choice(self._typos[c])
-                    text_modified = word[:j] + replacement + word[j + 1:]
+                    text_modified = word[:j] + replacement + word[j + 1 :]
                     return text_modified
         return word
 
 
 class TextPunctuationRemovalTransformation(TextTransformation):
     name = "Punctuation Removal"
 
@@ -116,15 +116,15 @@
         return " ".join(new_text)
 
     def _remove_punc(self, text):
         split_urls_from_text = gruber.split(text)
 
         # The non-URLs are always even-numbered entries in the list and the URLs are odd-numbered.
         for i in range(0, len(split_urls_from_text), 2):
-            split_urls_from_text[i] = split_urls_from_text[i].translate(str.maketrans('', '', self._punctuation))
+            split_urls_from_text[i] = split_urls_from_text[i].translate(str.maketrans("", "", self._punctuation))
 
         stripped_text = "".join(split_urls_from_text)
 
         return stripped_text
 
 
 class TextLanguageBasedTransformation(TextTransformation):
@@ -136,15 +136,15 @@
         self._load_dictionaries()
 
     def _load_dictionaries(self):
         raise NotImplementedError()
 
     def execute(self, dataset: Dataset) -> pd.DataFrame:
         feature_data = dataset.df.loc[:, (self.column,)].dropna().astype(str)
-        meta_dataframe = dataset.column_meta[self.column, "text"].add_suffix('__gsk__meta')
+        meta_dataframe = dataset.column_meta[self.column, "text"].add_suffix("__gsk__meta")
         feature_data = feature_data.join(meta_dataframe)
         dataset.df.loc[feature_data.index, self.column] = feature_data.apply(self.make_perturbation, axis=1)
         return dataset.df
 
     def make_perturbation(self, row):
         raise NotImplementedError()
 
@@ -174,15 +174,15 @@
             return text
 
         replacements = [self._switch(token, language) for token in text.split()]
         replacements = [r for r in replacements if r is not None]
 
         new_text = text
         for original_word, switched_word in replacements:
-            new_text = re.sub(fr"\b{original_word}\b", switched_word, new_text)
+            new_text = re.sub(rf"\b{original_word}\b", switched_word, new_text)
 
         return new_text
 
     def _switch(self, word, language):
         try:
             return (word, self._lang_dictionary[language][word.lower()])
         except KeyError:
@@ -246,15 +246,15 @@
         ent_types = list(itertools.product(["country", "nationality"], ["high-income", "low-income"]))
 
         # Mask entities and prepare replacements
         replacements = []
         for entity_type, income_type in ent_types:
             for n, entity_word in enumerate(nationalities_word_dict[entity_type][income_type]):
                 mask_value = f"__GSK__ENT__{entity_type}__{income_type}__{n}__"
-                text, num_rep = re.subn(fr"\b{entity_word}\b", mask_value, text, flags=re.IGNORECASE)
+                text, num_rep = re.subn(rf"\b{entity_word}\b", mask_value, text, flags=re.IGNORECASE)
                 if num_rep > 0:
                     r_income_type = "low-income" if income_type == "high-income" else "high-income"
                     replacement = random.choice(nationalities_word_dict[entity_type][r_income_type])
                     replacements.append((mask_value, replacement))
 
         # Replace masks
         for mask, replacement in replacements:
```

### Comparing `giskard-2.0.0b7/giskard/scanner/scanner.py` & `giskard-2.0.0b8/giskard/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/stochasticity/stochasticity_detector.py` & `giskard-2.0.0b8/giskard/scanner/stochasticity/stochasticity_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/templates/_code_snippet.html` & `giskard-2.0.0b8/giskard/scanner/templates/_code_snippet.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/templates/_issues/data_leakage.html` & `giskard-2.0.0b8/giskard/scanner/templates/_issues/data_leakage.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/templates/_issues/default.html` & `giskard-2.0.0b8/giskard/scanner/templates/_issues/default.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/templates/_issues/llm_toxicity.html` & `giskard-2.0.0b8/giskard/scanner/templates/_issues/llm_toxicity.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/templates/_issues/overconfidence.html` & `giskard-2.0.0b8/giskard/scanner/templates/_issues/overconfidence.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/templates/_issues/performance.html` & `giskard-2.0.0b8/giskard/scanner/templates/_issues/performance.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/templates/_issues/robustness.html` & `giskard-2.0.0b8/giskard/scanner/templates/_issues/robustness.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/templates/_issues/stochasticity.html` & `giskard-2.0.0b8/giskard/scanner/templates/_issues/stochasticity.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/templates/_issues/underconfidence.html` & `giskard-2.0.0b8/giskard/scanner/templates/_issues/underconfidence.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/templates/_issues_table.html` & `giskard-2.0.0b8/giskard/scanner/templates/_issues_table.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/templates/_main_content.html` & `giskard-2.0.0b8/giskard/scanner/templates/_main_content.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/templates/_tab_header.html` & `giskard-2.0.0b8/giskard/scanner/templates/_tab_header.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/templates/scan_results.html` & `giskard-2.0.0b8/giskard/scanner/templates/scan_results.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/templates/static/external.js` & `giskard-2.0.0b8/giskard/scanner/templates/static/external.js`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/templates/static/internal.js` & `giskard-2.0.0b8/giskard/scanner/templates/static/internal.js`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/templates/static/style.css` & `giskard-2.0.0b8/giskard/scanner/templates/static/style.css`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/scanner/visualization/custom_jinja.py` & `giskard-2.0.0b8/giskard/scanner/visualization/custom_jinja.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/settings.py` & `giskard-2.0.0b8/giskard/settings.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/slicing/base.py` & `giskard-2.0.0b8/giskard/slicing/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/slicing/bruteforce_slicer.py` & `giskard-2.0.0b8/giskard/slicing/bruteforce_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/slicing/category_slicer.py` & `giskard-2.0.0b8/giskard/slicing/category_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/slicing/multiscale_slicer.py` & `giskard-2.0.0b8/giskard/slicing/multiscale_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/slicing/opt_slicer.py` & `giskard-2.0.0b8/giskard/slicing/opt_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/slicing/slice.py` & `giskard-2.0.0b8/giskard/slicing/slice.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 
 def escape(value) -> str:
     return str(value) if type(value) is not str else "%s" % value
 
 
 class Clause(ABC):
-
     @abstractmethod
     def mask(self, df: pd.DataFrame) -> pd.Series:
         ...
 
     def __repr__(self) -> str:
         return f"<Clause {str(self)}>"
 
@@ -54,17 +53,17 @@
         return f"`{self.column}` {'does not contain' if self.is_not else 'contains'} \"{self.value}\""
 
     def mask(self, df: pd.DataFrame) -> pd.Series:
         return df[self.column].str.contains(rf"\b{re.escape(self.value)}\b", case=False).ne(self.is_not)
 
     def to_clause(self):
         return {
-            'columnName': self.column,
-            'comparisonType': 'DOES_NOT_CONTAINS' if self.is_not else 'CONTAINS',
-            'value': self.value
+            "columnName": self.column,
+            "comparisonType": "DOES_NOT_CONTAINS" if self.is_not else "CONTAINS",
+            "value": self.value,
         }
 
 
 class IsNa(Clause):
     def __init__(self, column, is_not: bool = False):
         self.column = column
         self.is_not = is_not
@@ -76,62 +75,54 @@
         return df[self.column].isna().ne(self.is_not)
 
     def init_code(self):
         return f"{self.__class__.__module__}.{self.__class__.__name__}({repr(self.column)}, is_not={repr(self.is_not)})"
 
     def to_clause(self):
         return {
-            'columnName': self.column,
-            'comparisonType': 'IS_NOT_EMPTY' if self.is_not else 'IS_EMPTY',
-            'value': None
+            "columnName": self.column,
+            "comparisonType": "IS_NOT_EMPTY" if self.is_not else "IS_EMPTY",
+            "value": None,
         }
 
 
 class StartsWith(Clause):
     def __init__(self, column, value):
         self.column = column
         self.value = value
 
     def __str__(self) -> str:
-        return f"`{self.column}` starts with \"{self.value}\""
+        return f'`{self.column}` starts with "{self.value}"'
 
     def mask(self, df: pd.DataFrame) -> pd.Series:
         return df[self.column].str.lower().str.startswith(self.value.lower())
 
     def init_code(self):
         return f"{self.__class__.__module__}.{self.__class__.__name__}({repr(self.column)}, {repr(self.value)})"
 
     def to_clause(self):
-        return {
-            'columnName': self.column,
-            'comparisonType': 'STARTS_WITH',
-            'value': self.value
-        }
+        return {"columnName": self.column, "comparisonType": "STARTS_WITH", "value": self.value}
 
 
 class EndsWith(Clause):
     def __init__(self, column, value):
         self.column = column
         self.value = value
 
     def __str__(self) -> str:
-        return f"`{self.column}` ends with \"{self.value}\""
+        return f'`{self.column}` ends with "{self.value}"'
 
     def mask(self, df: pd.DataFrame) -> pd.Series:
         return df[self.column].str.lower().str.endswith(self.value.lower())
 
     def init_code(self):
         return f"{self.__class__.__module__}.{self.__class__.__name__}({repr(self.column)}, {repr(self.value)})"
 
     def to_clause(self):
-        return {
-            'columnName': self.column,
-            'comparisonType': 'ENDS_WITH',
-            'value': self.value
-        }
+        return {"columnName": self.column, "comparisonType": "ENDS_WITH", "value": self.value}
 
 
 class GreaterThan(ComparisonClause):
     def __init__(self, column, value, equal=False):
         super().__init__(column, value)
         self.equal = equal
         self._operator = operator.ge if equal else operator.gt
@@ -141,17 +132,17 @@
         return f"`{self.column}` {operator} {_pretty_str(self.value)}"
 
     def init_code(self):
         return f"{self.__class__.__module__}.{self.__class__.__name__}({repr(self.column)}, {repr(self.value)}, equal={repr(self.equal)})"
 
     def to_clause(self):
         return {
-            'columnName': self.column,
-            'comparisonType': 'GREATER_THAN_EQUALS' if self.equal else "GREATER_THAN",
-            'value': self.value
+            "columnName": self.column,
+            "comparisonType": "GREATER_THAN_EQUALS" if self.equal else "GREATER_THAN",
+            "value": self.value,
         }
 
 
 class LowerThan(ComparisonClause):
     def __init__(self, column, value, equal=False):
         super().__init__(column, value)
         self.equal = equal
@@ -162,73 +153,65 @@
         return f"`{self.column}` {operator} {_pretty_str(self.value)}"
 
     def init_code(self):
         return f"{self.__class__.__module__}.{self.__class__.__name__}({repr(self.column)}, {repr(self.value)}, equal={repr(self.equal)})"
 
     def to_clause(self):
         return {
-            'columnName': self.column,
-            'comparisonType': 'LOWER_THAN_EQUALS' if self.equal else "LOWER_THAN",
-            'value': self.value
+            "columnName": self.column,
+            "comparisonType": "LOWER_THAN_EQUALS" if self.equal else "LOWER_THAN",
+            "value": self.value,
         }
 
 
 class EqualTo(ComparisonClause):
     _operator = operator.eq
 
     def __str__(self) -> str:
         return f"`{self.column}` == {_pretty_str(self.value)}"
 
     def to_clause(self):
-        return {
-            'columnName': self.column,
-            'comparisonType': 'IS',
-            'value': self.value
-        }
+        return {"columnName": self.column, "comparisonType": "IS", "value": self.value}
 
 
 class NotEqualTo(ComparisonClause):
     _operator = operator.ne
 
     def __str__(self) -> str:
         return f"`{self.column}` != {_pretty_str(self.value)}"
 
     def to_clause(self):
-        return {
-            'columnName': self.column,
-            'comparisonType': 'IS_NOT',
-            'value': self.value
-        }
+        return {"columnName": self.column, "comparisonType": "IS_NOT", "value": self.value}
 
 
 def generate_clause(clause: Dict[str, str]) -> Clause:
-    if clause['comparisonType'] == 'IS':
-        return EqualTo(clause['columnName'], clause['value'])
-    elif clause['comparisonType'] == 'IS_NOT':
-        return NotEqualTo(clause['columnName'], clause['value'])
-    elif clause['comparisonType'] == 'CONTAINS':
-        return ContainsWord(clause['columnName'], clause['value'], is_not=False)
-    elif clause['comparisonType'] == 'DOES_NOT_CONTAINS':
-        return ContainsWord(clause['columnName'], clause['value'], is_not=True)
-    elif clause['comparisonType'] == 'STARTS_WITH':
-        return StartsWith(clause['columnName'], clause['value'])
-    elif clause['comparisonType'] == 'ENDS_WITH':
-        return EndsWith(clause['columnName'], clause['value'])
-    elif clause['comparisonType'] == 'GREATER_THAN_EQUALS':
-        return GreaterThan(clause['columnName'], clause['value'], equal=True)
-    elif clause['comparisonType'] == 'GREATER_THAN':
-        return GreaterThan(clause['columnName'], clause['value'])
-    elif clause['comparisonType'] == 'LOWER_THAN_EQUALS':
-        return LowerThan(clause['columnName'], clause['value'], equal=True)
-    elif clause['comparisonType'] == 'LOWER_THAN':
-        return LowerThan(clause['columnName'], clause['value'])
-    elif clause['comparisonType'] == 'IS_EMPTY':
-        return IsNa(clause['columnName'], is_not=False)
-    elif clause['comparisonType'] == 'IS_NOT_EMPTY':
-        return IsNa(clause['columnName'], is_not=True)
+    if clause["comparisonType"] == "IS":
+        return EqualTo(clause["columnName"], clause["value"])
+    elif clause["comparisonType"] == "IS_NOT":
+        return NotEqualTo(clause["columnName"], clause["value"])
+    elif clause["comparisonType"] == "CONTAINS":
+        return ContainsWord(clause["columnName"], clause["value"], is_not=False)
+    elif clause["comparisonType"] == "DOES_NOT_CONTAINS":
+        return ContainsWord(clause["columnName"], clause["value"], is_not=True)
+    elif clause["comparisonType"] == "STARTS_WITH":
+        return StartsWith(clause["columnName"], clause["value"])
+    elif clause["comparisonType"] == "ENDS_WITH":
+        return EndsWith(clause["columnName"], clause["value"])
+    elif clause["comparisonType"] == "GREATER_THAN_EQUALS":
+        return GreaterThan(clause["columnName"], clause["value"], equal=True)
+    elif clause["comparisonType"] == "GREATER_THAN":
+        return GreaterThan(clause["columnName"], clause["value"])
+    elif clause["comparisonType"] == "LOWER_THAN_EQUALS":
+        return LowerThan(clause["columnName"], clause["value"], equal=True)
+    elif clause["comparisonType"] == "LOWER_THAN":
+        return LowerThan(clause["columnName"], clause["value"])
+    elif clause["comparisonType"] == "IS_EMPTY":
+        return IsNa(clause["columnName"], is_not=False)
+    elif clause["comparisonType"] == "IS_NOT_EMPTY":
+        return IsNa(clause["columnName"], is_not=True)
     else:
         raise TypeError(f"The comparison clause of type {clause['comparisonType']} does not exist")
 
 
 class Query:
     clauses: defaultdict
 
@@ -304,22 +287,22 @@
 
 class QueryBasedSliceFunction(SlicingFunction):
     query: Query
 
     def __init__(self, query: Query):
         super().__init__(None, row_level=False, cell_level=False)
         self.query = query
-        self.meta = DatasetProcessFunctionMeta(type='SLICE', process_type=DatasetProcessFunctionType.CLAUSES)
+        self.meta = DatasetProcessFunctionMeta(type="SLICE", process_type=DatasetProcessFunctionType.CLAUSES)
         self.meta.uuid = get_object_uuid(query)
         self.meta.clauses = self.query.to_clauses()
         self.meta.code = ""
         self.meta.name = str(self)
         self.meta.display_name = str(self)
         self.meta.tags = ["pickle", "scan"]
-        self.meta.doc = 'Automatically generated slicing function'
+        self.meta.doc = "Automatically generated slicing function"
 
     def execute(self, data: pd.DataFrame):
         return self.query.run(data)
 
     def __str__(self):
         return str(self.query)
```

### Comparing `giskard-2.0.0b7/giskard/slicing/text_slicer.py` & `giskard-2.0.0b8/giskard/slicing/text_slicer.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,21 +180,21 @@
     needs_dataset = True
 
     def __init__(self, query: Query, feature: str, provider: str):
         super().__init__(None, row_level=False, cell_level=False)
         self.query = query
         self.feature = feature
         self.provider = provider
-        self.meta = DatasetProcessFunctionMeta(type='SLICE')
+        self.meta = DatasetProcessFunctionMeta(type="SLICE")
         self.meta.uuid = get_object_uuid(query)
         self.meta.code = str(self)
         self.meta.name = str(self)
         self.meta.display_name = str(self)
         self.meta.tags = ["pickle", "scan"]
-        self.meta.doc = 'Automatically generated slicing function'
+        self.meta.doc = "Automatically generated slicing function"
 
     def execute(self, dataset: Dataset) -> pd.DataFrame:
         metadata = dataset.column_meta[self.feature, self.provider]
         mask = self.query.mask(metadata)
 
         return dataset.df[mask]
```

### Comparing `giskard-2.0.0b7/giskard/slicing/tree_slicer.py` & `giskard-2.0.0b8/giskard/slicing/tree_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/slicing/utils.py` & `giskard-2.0.0b8/giskard/slicing/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/testing/__init__.py` & `giskard-2.0.0b8/giskard/testing/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 __all__ = [
-    'test_drift_psi',
-    'test_drift_chi_square',
-    'test_drift_ks',
-    'test_drift_earth_movers_distance',
-    'test_drift_prediction_psi',
-    'test_drift_prediction_chi_square',
-    'test_drift_prediction_ks',
-    'test_drift_prediction_earth_movers_distance',
-    'test_right_label',
-    'test_output_in_range',
-    'test_disparate_impact',
-    'test_mae',
-    'test_rmse',
-    'test_recall',
-    'test_auc',
-    'test_accuracy',
-    'test_precision',
-    'test_f1',
-    'test_r2',
-    'test_diff_recall',
-    'test_diff_accuracy',
-    'test_diff_precision',
-    'test_diff_rmse',
-    'test_diff_f1',
-    'test_metamorphic_invariance',
-    'test_metamorphic_increasing',
-    'test_metamorphic_decreasing',
-    'test_metamorphic_decreasing_t_test',
-    'test_metamorphic_increasing_t_test',
-    'test_metamorphic_invariance_t_test',
-    'test_metamorphic_increasing_wilcoxon',
-    'test_metamorphic_decreasing_wilcoxon',
-    'test_metamorphic_invariance_wilcoxon',
+    "test_drift_psi",
+    "test_drift_chi_square",
+    "test_drift_ks",
+    "test_drift_earth_movers_distance",
+    "test_drift_prediction_psi",
+    "test_drift_prediction_chi_square",
+    "test_drift_prediction_ks",
+    "test_drift_prediction_earth_movers_distance",
+    "test_right_label",
+    "test_output_in_range",
+    "test_disparate_impact",
+    "test_mae",
+    "test_rmse",
+    "test_recall",
+    "test_auc",
+    "test_accuracy",
+    "test_precision",
+    "test_f1",
+    "test_r2",
+    "test_diff_recall",
+    "test_diff_accuracy",
+    "test_diff_precision",
+    "test_diff_rmse",
+    "test_diff_f1",
+    "test_metamorphic_invariance",
+    "test_metamorphic_increasing",
+    "test_metamorphic_decreasing",
+    "test_metamorphic_decreasing_t_test",
+    "test_metamorphic_increasing_t_test",
+    "test_metamorphic_invariance_t_test",
+    "test_metamorphic_increasing_wilcoxon",
+    "test_metamorphic_decreasing_wilcoxon",
+    "test_metamorphic_invariance_wilcoxon",
 ]
 
 from giskard.testing.tests.drift import (
     test_drift_psi,
     test_drift_chi_square,
     test_drift_ks,
     test_drift_earth_movers_distance,
```

### Comparing `giskard-2.0.0b7/giskard/testing/tests/drift.py` & `giskard-2.0.0b8/giskard/testing/tests/drift.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
     _validate_feature_type(reference_ds, column_name, feature_type)
     actual_series = actual_ds.df[column_name]
     reference_series = reference_ds.df[column_name]
     _validate_series_notempty(actual_series, reference_series)
     return actual_series, reference_series
 
 
-@test(name='Categorical drift (PSI)')
+@test(name="Categorical drift (PSI)")
 def test_drift_psi(
     actual_dataset: Dataset,
     reference_dataset: Dataset,
     column_name: str,
     slicing_function: Optional[SlicingFunction] = None,
     threshold: float = 0.2,
     max_categories: int = 20,
@@ -236,15 +236,15 @@
         reference_slices_size=[len(reference_series)],
         passed=passed,
         metric=total_psi,
         messages=messages,
     )
 
 
-@test(name='Categorical drift (Chi-squared)')
+@test(name="Categorical drift (Chi-squared)")
 def test_drift_chi_square(
     actual_dataset: Dataset,
     reference_dataset: Dataset,
     column_name: str,
     slicing_function: Optional[SlicingFunction] = None,
     threshold: float = 0.05,
     max_categories: int = 20,
@@ -309,15 +309,15 @@
         reference_slices_size=[len(reference_series)],
         passed=passed,
         metric=p_value,
         messages=messages,
     )
 
 
-@test(name='Numerical drift (Kolmogorov-Smirnov)')
+@test(name="Numerical drift (Kolmogorov-Smirnov)")
 def test_drift_ks(
     actual_dataset: Dataset,
     reference_dataset: Dataset,
     column_name: str,
     slicing_function: Optional[SlicingFunction] = None,
     threshold: float = 0.05,
 ) -> TestResult:
@@ -371,15 +371,15 @@
         reference_slices_size=[len(reference_series)],
         passed=passed,
         metric=result.pvalue,
         messages=messages,
     )
 
 
-@test(name='Numerical drift (Earth mover\'s distance)')
+@test(name="Numerical drift (Earth mover's distance)")
 def test_drift_earth_movers_distance(
     actual_dataset: Dataset,
     reference_dataset: Dataset,
     column_name: str,
     slicing_function: Optional[SlicingFunction] = None,
     threshold: float = 0.2,
 ) -> TestResult:
@@ -440,15 +440,15 @@
         reference_slices_size=[len(reference_series)],
         passed=True if threshold is None else passed,
         metric=metric,
         messages=messages,
     )
 
 
-@test(name='Label drift (PSI)')
+@test(name="Label drift (PSI)")
 def test_drift_prediction_psi(
     model: BaseModel,
     actual_dataset: Dataset,
     reference_dataset: Dataset,
     slicing_function: Optional[SlicingFunction] = None,
     max_categories: int = 10,
     threshold: float = 0.2,
@@ -543,15 +543,15 @@
                 type=TestMessageLevel.ERROR,
                 text=f"The {test_data} is drifting for the following modalities: {','.join(filtered_modalities)}",
             )
         ]
     return messages
 
 
-@test(name='Label drift (Chi-squared)')
+@test(name="Label drift (Chi-squared)")
 def test_drift_prediction_chi_square(
     model: BaseModel,
     actual_dataset: Dataset,
     reference_dataset: Dataset,
     slicing_function: Optional[SlicingFunction] = None,
     max_categories: int = 10,
     threshold: float = 0.05,
@@ -633,15 +633,15 @@
     chi_square, p_value, output_data = _calculate_chi_square(actual_series, reference_series, max_categories)
     passed = bool(p_value > threshold)
     main_drifting_modalities_bool = output_data["Chi_square"] > chi_square_contribution_percent * chi_square
     messages = _generate_message_modalities(main_drifting_modalities_bool, output_data, test_data)
     return messages, p_value, passed
 
 
-@test(name='Classification Probability drift (Kolmogorov-Smirnov)', tags=['classification'])
+@test(name="Classification Probability drift (Kolmogorov-Smirnov)", tags=["classification"])
 @validate_classification_label
 def test_drift_prediction_ks(
     model: BaseModel,
     actual_dataset: Dataset,
     reference_dataset: Dataset,
     slicing_function: Optional[SlicingFunction] = None,
     classification_label: Optional[str] = None,
@@ -730,15 +730,15 @@
                 text=f"The {data_type} is drifting (p-value is equal to {np.round(result.pvalue, 9)} "
                 f"and is below the test risk level {threshold}) ",
             )
         ]
     return messages
 
 
-@test(name='Classification Probability drift (Earth mover\'s distance)', tags=['classification'])
+@test(name="Classification Probability drift (Earth mover's distance)", tags=["classification"])
 @validate_classification_label
 def test_drift_prediction_earth_movers_distance(
     model: BaseModel,
     actual_dataset: Dataset,
     reference_dataset: Dataset,
     slicing_function: Optional[SlicingFunction] = None,
     classification_label: Optional[str] = None,
```

### Comparing `giskard-2.0.0b7/giskard/testing/tests/metamorphic.py` & `giskard-2.0.0b8/giskard/testing/tests/metamorphic.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 
 def _prediction_ratio(prediction, perturbed_prediction):
     return abs(perturbed_prediction - prediction) / prediction if prediction != 0 else abs(perturbed_prediction)
 
 
 @timer("Perturb and predict data")
 def _perturb_and_predict(
-        model: BaseModel,
-        ds: Dataset,
-        transformation_function: TransformationFunction,
-        output_proba=True,
-        classification_label=None,
+    model: BaseModel,
+    ds: Dataset,
+    transformation_function: TransformationFunction,
+    output_proba=True,
+    classification_label=None,
 ):
     fix_seed()
 
     results_df = pd.DataFrame(
         {
             "prediction": _predict_numeric_result(model, ds, output_proba, classification_label),
         },
```

### Comparing `giskard-2.0.0b7/giskard/testing/tests/performance.py` & `giskard-2.0.0b8/giskard/testing/tests/performance.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         actual_slices_size=[len(actual_dataset)],
         reference_slices_size=[len(reference_dataset)],
         metric=rel_change,
         passed=np_type_to_native(passed),
     )
 
 
-@test(name='AUC', tags=['performance', 'classification', 'ground_truth'])
+@test(name="AUC", tags=["performance", "classification", "ground_truth"])
 def test_auc(
     model: BaseModel, dataset: Dataset, slicing_function: Optional[SlicingFunction] = None, threshold: float = 1.0
 ):
     """
     Test if the model AUC performance is higher than a threshold for a given slice
 
     Example : The test is passed when the AUC for females is higher than 0.7
@@ -150,25 +150,25 @@
 
     _verify_target_availability(dataset)
     if len(model.meta.classification_labels) == 2:
         metric = roc_auc_score(dataset.df[dataset.target], model.predict(dataset).raw[:, 1])
     else:
         predictions = model.predict(dataset).all_predictions
         non_declared_categories = set(predictions.columns) - set(dataset.df[dataset.target].unique())
-        assert not len(
-            non_declared_categories
-        ), f'Predicted classes don\'t exist in the dataset "{dataset.target}" column: {non_declared_categories}. ' \
-           'ROC AUC score is not defined in that case.'
+        assert not len(non_declared_categories), (
+            f'Predicted classes don\'t exist in the dataset "{dataset.target}" column: {non_declared_categories}. '
+            "ROC AUC score is not defined in that case."
+        )
 
         metric = roc_auc_score(dataset.df[dataset.target], predictions, multi_class="ovo")
 
     return TestResult(actual_slices_size=[len(dataset)], metric=metric, passed=bool(metric >= threshold))
 
 
-@test(name='F1', tags=['performance', 'classification', 'ground_truth'])
+@test(name="F1", tags=["performance", "classification", "ground_truth"])
 def test_f1(
     model: BaseModel, dataset: Dataset, slicing_function: Optional[SlicingFunction] = None, threshold: float = 1.0
 ):
     """
     Test if the model F1 score is higher than a defined threshold for a given slice
 
     Example: The test is passed when F1 score for females is higher than 0.7
@@ -195,15 +195,15 @@
     """
     if slicing_function:
         dataset = dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=dataset, dataset_name="dataset", test_name="test_f1")
     return _test_classification_score(f1_score, model, dataset, threshold)
 
 
-@test(name='Accuracy', tags=['performance', 'classification', 'ground_truth'])
+@test(name="Accuracy", tags=["performance", "classification", "ground_truth"])
 def test_accuracy(
     model: BaseModel, dataset: Dataset, slicing_function: Optional[SlicingFunction] = None, threshold: float = 1.0
 ):
     """
     Test if the model Accuracy is higher than a threshold for a given slice
 
     Example: The test is passed when the Accuracy for females is higher than 0.7
@@ -229,15 +229,15 @@
     """
     if slicing_function:
         dataset = dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=dataset, dataset_name="dataset", test_name="test_accuracy")
     return _test_accuracy_score(dataset, model, threshold)
 
 
-@test(name='Precision', tags=['performance', 'classification', 'ground_truth'])
+@test(name="Precision", tags=["performance", "classification", "ground_truth"])
 def test_precision(
     model: BaseModel, dataset: Dataset, slicing_function: Optional[SlicingFunction] = None, threshold: float = 1.0
 ):
     """
     Test if the model Precision is higher than a threshold for a given slice
 
     Example: The test is passed when the Precision for females is higher than 0.7
@@ -262,15 +262,15 @@
     """
     if slicing_function:
         dataset = dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=dataset, dataset_name="dataset", test_name="test_precision")
     return _test_classification_score(precision_score, model, dataset, threshold)
 
 
-@test(name='Recall', tags=['performance', 'classification', 'ground_truth'])
+@test(name="Recall", tags=["performance", "classification", "ground_truth"])
 def test_recall(
     model: BaseModel, dataset: Dataset, slicing_function: Optional[SlicingFunction] = None, threshold: float = 1.0
 ):
     """
     Test if the model Recall is higher than a threshold for a given slice
 
     Example: The test is passed when the Recall for females is higher than 0.7
@@ -295,15 +295,15 @@
     """
     if slicing_function:
         dataset = dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=dataset, dataset_name="dataset", test_name="test_recall")
     return _test_classification_score(recall_score, model, dataset, threshold)
 
 
-@test(name='RMSE', tags=['performance', 'regression', 'ground_truth'])
+@test(name="RMSE", tags=["performance", "regression", "ground_truth"])
 def test_rmse(
     model: BaseModel, dataset: Dataset, slicing_function: Optional[SlicingFunction] = None, threshold: float = 1.0
 ):
     """
     Test if the model RMSE is lower than a threshold
 
     Example: The test is passed when the RMSE is lower than 10
@@ -328,15 +328,15 @@
     """
     if slicing_function:
         dataset = dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=dataset, dataset_name="dataset", test_name="test_rmse")
     return _test_regression_score(_get_rmse, model, dataset, threshold)
 
 
-@test(name='MSE', tags=['performance', 'regression', 'ground_truth'])
+@test(name="MSE", tags=["performance", "regression", "ground_truth"])
 def test_mse(
     model: BaseModel, dataset: Dataset, slicing_function: Optional[SlicingFunction] = None, threshold: float = 1.0
 ):
     """
     Test if the model mean squared error (MSE) is lower than a threshold.
 
     Example: The test is passed when the MSE is lower than 10.
@@ -361,15 +361,15 @@
     """
     if slicing_function:
         dataset = dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=dataset, dataset_name="dataset", test_name="test_mse")
     return _test_regression_score(_get_mse, model, dataset, threshold)
 
 
-@test(name='MAE', tags=['performance', 'regression', 'ground_truth'])
+@test(name="MAE", tags=["performance", "regression", "ground_truth"])
 def test_mae(
     model: BaseModel, dataset: Dataset, slicing_function: Optional[SlicingFunction] = None, threshold: float = 1.0
 ):
     """
     Test if the model Mean Absolute Error is lower than a threshold
 
     Example: The test is passed when the MAE is lower than 10
@@ -397,15 +397,15 @@
     """
     if slicing_function:
         dataset = dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=dataset, dataset_name="dataset", test_name="test_mae")
     return _test_regression_score(mean_absolute_error, model, dataset, threshold)
 
 
-@test(name='R2', tags=['performance', 'regression', 'ground_truth'])
+@test(name="R2", tags=["performance", "regression", "ground_truth"])
 def test_r2(
     model: BaseModel, dataset: Dataset, slicing_function: Optional[SlicingFunction] = None, threshold: float = 1.0
 ):
     """
     Test if the model R-Squared is higher than a threshold
 
     Example: The test is passed when the R-Squared is higher than 0.7
@@ -431,15 +431,15 @@
     """
     if slicing_function:
         dataset = dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=dataset, dataset_name="dataset", test_name="test_r2")
     return _test_regression_score(r2_score, model, dataset, threshold, r2=True)
 
 
-@test(name='Accuracy difference', tags=['performance', 'classification', 'ground_truth'])
+@test(name="Accuracy difference", tags=["performance", "classification", "ground_truth"])
 def test_diff_accuracy(
     model: BaseModel,
     actual_dataset: Dataset,
     reference_dataset: Dataset,
     slicing_function: Optional[SlicingFunction] = None,
     threshold: float = 0.1,
     direction: Direction = Direction.Invariant,
@@ -489,15 +489,15 @@
         reference_dataset,
         threshold=threshold,
         direction=direction,
         test_name="Accuracy",
     )
 
 
-@test(name='F1 difference', tags=['performance', 'classification', 'ground_truth'])
+@test(name="F1 difference", tags=["performance", "classification", "ground_truth"])
 def test_diff_f1(
     model: BaseModel,
     actual_dataset: Dataset,
     reference_dataset: Dataset,
     slicing_function: Optional[SlicingFunction] = None,
     threshold: float = 0.1,
     direction: Direction = Direction.Invariant,
@@ -547,15 +547,15 @@
         reference_dataset,
         threshold=threshold,
         direction=direction,
         test_name="F1 Score",
     )
 
 
-@test(name='Precision difference', tags=['performance', 'classification', 'ground_truth'])
+@test(name="Precision difference", tags=["performance", "classification", "ground_truth"])
 def test_diff_precision(
     model: BaseModel,
     actual_dataset: Dataset,
     reference_dataset: Dataset,
     slicing_function: Optional[SlicingFunction] = None,
     threshold: float = 0.1,
     direction: Direction = Direction.Invariant,
@@ -604,15 +604,15 @@
         reference_dataset,
         threshold=threshold,
         direction=direction,
         test_name="Precision",
     )
 
 
-@test(name='Recall difference', tags=['performance', 'classification', 'ground_truth'])
+@test(name="Recall difference", tags=["performance", "classification", "ground_truth"])
 def test_diff_recall(
     model: BaseModel,
     actual_dataset: Dataset,
     reference_dataset: Dataset,
     slicing_function: Optional[SlicingFunction] = None,
     threshold: float = 0.1,
     direction: Direction = Direction.Invariant,
@@ -661,15 +661,15 @@
         reference_dataset,
         threshold=threshold,
         direction=direction,
         test_name="Recall",
     )
 
 
-@test(name='RMSE difference', tags=['performance', 'regression', 'ground_truth'])
+@test(name="RMSE difference", tags=["performance", "regression", "ground_truth"])
 def test_diff_rmse(
     model: BaseModel,
     actual_dataset: Dataset,
     reference_dataset: Dataset,
     slicing_function: Optional[SlicingFunction] = None,
     threshold: float = 0.1,
     direction: Direction = Direction.Invariant,
```

### Comparing `giskard-2.0.0b7/giskard/testing/tests/statistic.py` & `giskard-2.0.0b8/giskard/testing/tests/statistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,21 @@
 from giskard.ml_worker.testing.registry.slicing_function import SlicingFunction
 from giskard.models.base import BaseModel
 from giskard.ml_worker.testing.utils import check_slice_not_empty
 
 
 @test(name="Right Label", tags=["heuristic", "classification"])
 @validate_classification_label
-def test_right_label(model: BaseModel, dataset: Dataset, classification_label: str,
-                     slicing_function: Optional[SlicingFunction] = None, threshold: float = 0.5) -> TestResult:
+def test_right_label(
+    model: BaseModel,
+    dataset: Dataset,
+    classification_label: str,
+    slicing_function: Optional[SlicingFunction] = None,
+    threshold: float = 0.5,
+) -> TestResult:
     """
     Summary: Test if the model returns the right classification label for a slice
 
     Description: The test is passed when the percentage of rows returning the right
     classification label is higher than the threshold in a given slice
 
     Example: For a credit scoring model, the test is passed when more than 50%
@@ -60,17 +65,23 @@
         metric=passed_ratio,
         passed=bool(passed_ratio > threshold),
     )
 
 
 @test(name="Output in range", tags=["heuristic", "classification", "regression"])
 @validate_classification_label
-def test_output_in_range(model: BaseModel, dataset: Dataset, slicing_function: Optional[SlicingFunction] = None,
-                         classification_label: Optional[str] = None, min_range: float = 0.3, max_range: float = 0.7,
-                         threshold: float = 0.5) -> TestResult:
+def test_output_in_range(
+    model: BaseModel,
+    dataset: Dataset,
+    slicing_function: Optional[SlicingFunction] = None,
+    classification_label: Optional[str] = None,
+    min_range: float = 0.3,
+    max_range: float = 0.7,
+    threshold: float = 0.5,
+) -> TestResult:
     """
     Summary: Test if the model output belongs to the right range for a slice
 
     Description: - The test is passed when the ratio of rows in the right range inside the
     slice is higher than the threshold.
 
     For classification: Test if the predicted probability for a given classification label
```

### Comparing `giskard-2.0.0b7/giskard/utils/analytics_collector.py` & `giskard-2.0.0b8/giskard/utils/analytics_collector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard/utils/environment_detector.py` & `giskard-2.0.0b8/giskard/utils/environment_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard.egg-info/PKG-INFO` & `giskard-2.0.0b8/giskard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giskard
-Version: 2.0.0b7
+Version: 2.0.0b8
 Summary: The testing framework dedicated to ML models, from tabular to LLMs
 Author-email: Giskard AI <hello@giskard.ai>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://giskard.ai
 Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues
 Project-URL: Documentation, https://docs.giskard.ai/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: giskard Version: 2.0.0b7 Summary: The testing
+Metadata-Version: 2.1 Name: giskard Version: 2.0.0b8 Summary: The testing
 framework dedicated to ML models, from tabular to LLMs Author-email: Giskard AI
 giskard.ai> License: Apache Software License 2.0 Project-URL: Homepage, https:/
 /giskard.ai Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues Project-
 URL: Documentation, https://docs.giskard.ai/ Project-URL: Discord, https://
 discord.gg/ABvfpbu69R Project-URL: Linkedin, https://www.linkedin.com/company/
 giskard-ai Project-URL: Mastodon, https://fosstodon.org/@Giskard Project-URL:
```

### Comparing `giskard-2.0.0b7/giskard.egg-info/SOURCES.txt` & `giskard-2.0.0b8/giskard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/giskard.egg-info/requires.txt` & `giskard-2.0.0b8/giskard.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/pyproject.toml` & `giskard-2.0.0b8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 test-fast.env = { GSK_DISABLE_ANALYTICS = "True"}
 lint = "ruff giskard tests"
 doc = "python -m sphinx_autobuild docs docs/_build/html"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "typing-extensions>=4.5.0",
-    "black>=23.3.0",
+    "black[d]>=23.3.0",
     "bandit>=1.7.4",
     "darglint>=1.8.1",
     "jupyter>=1.0.0",
     "jupyterlab>=3.4.2",
     "pre-commit>=2.19.0",
     "pydocstyle>=6.1.1",
     "pylint>=2.13.9",
@@ -104,15 +104,15 @@
 "Twitter" = "https://twitter.com/giskard_ai"
 
 
 [project]
 name = "giskard"
 readme = "README.md"
 license = { text = "Apache Software License 2.0" }
-version = "2.0.0b7"
+version = "2.0.0b8"
 description = "The testing framework dedicated to ML models, from tabular to LLMs"
 authors = [
     { name = "Giskard AI", email = "hello@giskard.ai" },
 ]
 keywords = [
     "Artificial Intelligence",
     "Machine Learning",
```

### Comparing `giskard-2.0.0b7/setup.py` & `giskard-2.0.0b8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,77 +4,73 @@
 import pkg_resources
 from setuptools import setup, Command
 from setuptools.command.build_py import build_py
 
 
 class GrpcTool(Command):
     user_options = []
-    out_path = 'giskard/ml_worker/generated'
+    out_path = "giskard/ml_worker/generated"
 
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
 
     @staticmethod
     def fix_paths(path):
         for dirpath, dirs, files in os.walk(path):
             for filename in files:
                 print(f"Generated file: {dirpath}/{filename}")
-                if not filename.endswith('.py'):
+                if not filename.endswith(".py"):
                     continue
                 fname = os.path.join(dirpath, filename)
                 with open(fname) as rfile:
                     content = rfile.read()
                     content = re.sub(
-                        '^import ([^\\. ]*?_pb2)', f'import giskard.ml_worker.generated.\g<1>',
-                        content, flags=re.MULTILINE)
-                    with open(fname, 'w') as wfile:
+                        "^import ([^\\. ]*?_pb2)",
+                        "import giskard.ml_worker.generated.\g<1>",
+                        content,
+                        flags=re.MULTILINE,
+                    )
+                    with open(fname, "w") as wfile:
                         wfile.write(content)
-                    print(f'Fixed {fname}')
+                    print(f"Fixed {fname}")
 
     def run(self):
         print("Running grpc_tools.protoc")
         import grpc_tools.protoc
 
         os.makedirs(self.out_path, exist_ok=True)
-        proto_path = '../common/proto'
-        proto_include = pkg_resources.resource_filename('grpc_tools', '_proto')
+        proto_path = "../common/proto"
+        proto_include = pkg_resources.resource_filename("grpc_tools", "_proto")
 
         cmd = [
-            'grpc_tools.protoc',
-            f'-I{proto_include}',
-            f'-I{proto_path}',
-            f'--python_out={self.out_path}',
-            f'--grpc_python_out={self.out_path}'
+            "grpc_tools.protoc",
+            f"-I{proto_include}",
+            f"-I{proto_path}",
+            f"--python_out={self.out_path}",
+            f"--grpc_python_out={self.out_path}",
         ]
         try:
             import importlib
-            importlib.import_module('mypy_protobuf')
-            cmd += [
-                f'--mypy_out={self.out_path}',
-                f'--mypy_grpc_out={self.out_path}'
-            ]
+
+            importlib.import_module("mypy_protobuf")
+            cmd += [f"--mypy_out={self.out_path}", f"--mypy_grpc_out={self.out_path}"]
         except Exception:
             print("mypy-protobuf isn't installed or 'import mypy_protobuf' didn't work")
-        cmd.append(f'ml-worker.proto')
+        cmd.append("ml-worker.proto")
         print(f"Running: {' '.join(cmd)}")
         grpc_tools.protoc.main(cmd)
 
         self.fix_paths(self.out_path)
 
 
 class BuildPyCommand(build_py):
-
     def finalize_options(self) -> None:
         super().finalize_options()
-        self.run_command('grpc')
+        self.run_command("grpc")
 
 
 setup(
-    cmdclass={
-        "build_py": BuildPyCommand,
-        "grpc": GrpcTool
-    },
-
+    cmdclass={"build_py": BuildPyCommand, "grpc": GrpcTool},
 )
```

### Comparing `giskard-2.0.0b7/tests/test_custom_model.py` & `giskard-2.0.0b8/tests/test_custom_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from giskard.models.base import MODEL_CLASS_PKL, WrapperModel, BaseModel
 from giskard.models.sklearn import SKLearnModel
 from tests.utils import MockedClient
 
 
 def test_custom_model(linear_regression_diabetes: BaseModel):
     with MockedClient() as (client, mr):
+
         class MyModel(WrapperModel):
             @classmethod
             def load_model(cls, local_dir):
                 pass
 
             def save_model(self, local_path: Union[str, Path]) -> None:
                 pass
@@ -24,17 +25,14 @@
             def save(self, local_path: Union[str, Path]) -> None:
                 super().save(local_path)
 
             should_save_model_class = True
 
         def has_model_class_been_sent():
             artifact_url_prefix = "http://giskard-host:12345/api/v2/artifacts/pk/models/[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/"
-            return (
-                    len([i for i in mr.request_history if
-                         re.match(artifact_url_prefix + MODEL_CLASS_PKL, i.url)]) > 0
-            )
+            return len([i for i in mr.request_history if re.match(artifact_url_prefix + MODEL_CLASS_PKL, i.url)]) > 0
 
         SKLearnModel(linear_regression_diabetes.model, model_type=SupportedModelTypes.REGRESSION).upload(client, "pk")
         assert not has_model_class_been_sent()
 
         MyModel(model=linear_regression_diabetes.model, model_type=SupportedModelTypes.REGRESSION).upload(client, "pk")
         assert has_model_class_been_sent()
```

### Comparing `giskard-2.0.0b7/tests/test_data_drift.py` & `giskard-2.0.0b8/tests/test_data_drift.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,17 @@
     [("german_credit_data", 0.05, 0.0, "personal_status"), ("enron_data", 2, 1.19, "Week_day")],
 )
 def test_drift_data_psi(data, threshold, expected_metric, column_name, request):
     data = request.getfixturevalue(data)
     results = drift.test_drift_psi(
         actual_dataset=data.slice(SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)),
         reference_dataset=data.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
-        column_name=column_name, threshold=threshold).execute()
+        column_name=column_name,
+        threshold=threshold,
+    ).execute()
 
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
     "data,threshold,expected_metric,column_name,max_categories",
@@ -28,31 +30,35 @@
     ],
 )
 def test_drift_data_psi_max_categories(data, threshold, expected_metric, column_name, max_categories, request):
     data = request.getfixturevalue(data)
     results = drift.test_drift_psi(
         actual_dataset=data.slice(SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)),
         reference_dataset=data.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
-        column_name=column_name, threshold=threshold,
-        max_categories=max_categories).execute()
+        column_name=column_name,
+        threshold=threshold,
+        max_categories=max_categories,
+    ).execute()
 
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
     "data,threshold,expected_metric,column_name",
     [("german_credit_data", 0.05, 0.76, "personal_status"), ("enron_data", 0, 0, "Week_day")],
 )
 def test_drift_data_chi_square(data, threshold, expected_metric, column_name, request):
     data = request.getfixturevalue(data)
     results = drift.test_drift_chi_square(
         actual_dataset=data.slice(SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)),
         reference_dataset=data.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
-        column_name=column_name, threshold=threshold).execute()
+        column_name=column_name,
+        threshold=threshold,
+    ).execute()
 
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
     "data,threshold,expected_metric,column_name,max_categories",
@@ -62,16 +68,18 @@
     ],
 )
 def test_drift_data_chi_square_max_categories(data, threshold, expected_metric, column_name, max_categories, request):
     data = request.getfixturevalue(data)
     results = drift.test_drift_chi_square(
         actual_dataset=data.slice(SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)),
         reference_dataset=data.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
-        column_name=column_name, threshold=threshold,
-        max_categories=max_categories).execute()
+        column_name=column_name,
+        threshold=threshold,
+        max_categories=max_categories,
+    ).execute()
 
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
     "data,threshold,expected_metric,column_name",
@@ -79,15 +87,16 @@
 )
 def test_drift_data_ks(data, threshold, expected_metric, column_name, request):
     data = request.getfixturevalue(data)
     results = drift.test_drift_ks(
         actual_dataset=data.slice(SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)),
         reference_dataset=data.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
         column_name=column_name,
-        threshold=threshold).execute()
+        threshold=threshold,
+    ).execute()
 
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
     "data,threshold,expected_metric,column_name",
@@ -97,46 +106,52 @@
     data = request.getfixturevalue(data)
     data.df.replace({1169: np.nan}, inplace=True)
 
     results = drift.test_drift_ks(
         actual_dataset=data.slice(SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)),
         reference_dataset=data.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
         column_name=column_name,
-        threshold=threshold).execute()
+        threshold=threshold,
+    ).execute()
 
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
     "data,threshold,expected_metric,column_name",
     [("german_credit_data", 0.05, 0.0, "duration_in_month")],
 )
 def test_drift_data_ks_unique_values(data, threshold, expected_metric, column_name, request):
     data = request.getfixturevalue(data)
-    results = drift.test_drift_ks(actual_dataset=data.slice(
-        SlicingFunction(lambda df: df[df["duration_in_month"].isin([6, 48])], row_level=False)),
-        reference_dataset=data.slice(
-            SlicingFunction(lambda df: df[df["duration_in_month"] == 6], row_level=False)),
-        column_name=column_name, threshold=threshold).execute()
+    results = drift.test_drift_ks(
+        actual_dataset=data.slice(
+            SlicingFunction(lambda df: df[df["duration_in_month"].isin([6, 48])], row_level=False)
+        ),
+        reference_dataset=data.slice(SlicingFunction(lambda df: df[df["duration_in_month"] == 6], row_level=False)),
+        column_name=column_name,
+        threshold=threshold,
+    ).execute()
 
     assert round(results.metric, 2) == expected_metric
     assert not results.passed
 
 
 @pytest.mark.parametrize(
     "data,threshold,expected_metric,column_name",
     [("german_credit_data", 1, 0.01, "credit_amount"), ("enron_data", 1, 0.16, "Hour")],
 )
 def test_drift_data_earth_movers_distance(data, threshold, expected_metric, column_name, request):
     data = request.getfixturevalue(data)
     results = drift.test_drift_earth_movers_distance(
         actual_dataset=data.slice(SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)),
         reference_dataset=data.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
-        column_name=column_name, threshold=threshold).execute()
+        column_name=column_name,
+        threshold=threshold,
+    ).execute()
 
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
     "data,model,threshold,expected_metric",
@@ -144,63 +159,75 @@
         ("german_credit_data", "german_credit_model", 1, 0.02),
         ("enron_data", "enron_model", 2, 1.36),
     ],
 )
 def test_drift_prediction_psi(data, model, threshold, expected_metric, request):
     data = request.getfixturevalue(data)
     model = request.getfixturevalue(model)
-    results = drift.test_drift_prediction_psi(model=model, actual_dataset=data.slice(
-        SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)), reference_dataset=data.slice(
-        SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)), threshold=threshold).execute()
+    results = drift.test_drift_prediction_psi(
+        model=model,
+        actual_dataset=data.slice(SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)),
+        reference_dataset=data.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
+        threshold=threshold,
+    ).execute()
 
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
     "data,model,threshold,expected_metric",
     [("german_credit_data", "german_credit_model", 0, 0), ("enron_data", "enron_model", -1, 0)],
 )
 def test_drift_prediction_chi_square(data, model, threshold, expected_metric, request):
     data = request.getfixturevalue(data)
-    results = drift.test_drift_prediction_chi_square(model=request.getfixturevalue(model), actual_dataset=data.slice(
-        SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)), reference_dataset=data.slice(
-        SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)), threshold=threshold).execute()
+    results = drift.test_drift_prediction_chi_square(
+        model=request.getfixturevalue(model),
+        actual_dataset=data.slice(SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)),
+        reference_dataset=data.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
+        threshold=threshold,
+    ).execute()
 
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
     "data,model,threshold,expected_metric",
     [("diabetes_dataset_with_target", "linear_regression_diabetes", 0, 0.69)],
 )
 def test_drift_reg_output_ks(data, model, threshold, expected_metric, request):
     data = request.getfixturevalue(data)
-    results = drift.test_drift_prediction_ks(model=request.getfixturevalue(model), actual_dataset=data.slice(
-        SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)), reference_dataset=data.slice(
-        SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)), threshold=threshold).execute()
+    results = drift.test_drift_prediction_ks(
+        model=request.getfixturevalue(model),
+        actual_dataset=data.slice(SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)),
+        reference_dataset=data.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
+        threshold=threshold,
+    ).execute()
 
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
     "data,model,threshold,expected_metric,classification_label",
     [
         ("german_credit_data", "german_credit_model", 0.05, 0.15, "Default"),
         ("enron_data", "enron_model", 0.05, 0.29, "CALIFORNIA CRISIS"),
     ],
 )
 def test_drift_model_prob_ks(data, model, threshold, expected_metric, classification_label, request):
     data = request.getfixturevalue(data)
-    results = drift.test_drift_prediction_ks(model=request.getfixturevalue(model), actual_dataset=data.slice(
-        SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)), reference_dataset=data.slice(
-        SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)), classification_label=classification_label,
-                                             threshold=threshold).execute()
+    results = drift.test_drift_prediction_ks(
+        model=request.getfixturevalue(model),
+        actual_dataset=data.slice(SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)),
+        reference_dataset=data.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
+        classification_label=classification_label,
+        threshold=threshold,
+    ).execute()
 
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
     "data,model,threshold,expected_metric,classification_label,num_rows",
@@ -209,115 +236,121 @@
         ("enron_data", "enron_model", 0.05, 0.99, "CALIFORNIA CRISIS", 9),
         ("german_credit_data", "german_credit_model", 0.05, 1, "Default", 1),
         ("german_credit_data", "german_credit_model", 0.05, 0.99, "Default", 10),
         ("german_credit_data", "german_credit_model", 0.05, 0.83, "Default", 11),
     ],
 )
 def test_drift_model_prob_ks_small_dataset(
-        data, model, threshold, expected_metric, classification_label, num_rows, request
+    data, model, threshold, expected_metric, classification_label, num_rows, request
 ):
     data = request.getfixturevalue(data)
-    results = drift.test_drift_prediction_ks(model=request.getfixturevalue(model), actual_dataset=data.slice(
-        SlicingFunction(lambda df: df.tail(num_rows), row_level=False)), reference_dataset=data.slice(
-        SlicingFunction(lambda df: df.head(num_rows), row_level=False)), classification_label=classification_label,
-                                             threshold=threshold).execute()
+    results = drift.test_drift_prediction_ks(
+        model=request.getfixturevalue(model),
+        actual_dataset=data.slice(SlicingFunction(lambda df: df.tail(num_rows), row_level=False)),
+        reference_dataset=data.slice(SlicingFunction(lambda df: df.head(num_rows), row_level=False)),
+        classification_label=classification_label,
+        threshold=threshold,
+    ).execute()
 
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
     "data,model,threshold,expected_metric,classification_label",
     [("german_credit_data", "german_credit_model", 0.05, 0.29, "Default")],
 )
 @pytest.mark.skip(reason="#585")
-def test_drift_model_prob_ks_small_unique_dataset(data, model, threshold, expected_metric, classification_label,
-                                                  request):
+def test_drift_model_prob_ks_small_unique_dataset(
+    data, model, threshold, expected_metric, classification_label, request
+):
     data = request.getfixturevalue(data)
-    results = drift.test_drift_prediction_ks(model=request.getfixturevalue(model), actual_dataset=data.slice(
-        SlicingFunction(lambda df: df[df["housing"].isin(["own", "rent"])], row_level=False)),
-                                             reference_dataset=data.slice(
-                                                 SlicingFunction(lambda df: df[df["housing"] == "own"],
-                                                                 row_level=False)),
-                                             classification_label=classification_label, threshold=threshold)
+    results = drift.test_drift_prediction_ks(
+        model=request.getfixturevalue(model),
+        actual_dataset=data.slice(SlicingFunction(lambda df: df[df["housing"].isin(["own", "rent"])], row_level=False)),
+        reference_dataset=data.slice(SlicingFunction(lambda df: df[df["housing"] == "own"], row_level=False)),
+        classification_label=classification_label,
+        threshold=threshold,
+    )
 
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
     "data,model,threshold,expected_metric",
     [("diabetes_dataset_with_target", "linear_regression_diabetes", 0.05, 0.02)],
 )
 def test_drift_reg_output_earth_movers_distance(data, model, threshold, expected_metric, request):
     data = request.getfixturevalue(data)
-    results = drift.test_drift_prediction_earth_movers_distance(model=request.getfixturevalue(model),
-                                                                actual_dataset=data.slice(
-                                                                    SlicingFunction(lambda df: df.tail(len(df) // 2),
-                                                                                    row_level=False)),
-                                                                reference_dataset=data.slice(
-                                                                    SlicingFunction(lambda df: df.head(len(df) // 2),
-                                                                                    row_level=False)),
-                                                                threshold=threshold).execute()
+    results = drift.test_drift_prediction_earth_movers_distance(
+        model=request.getfixturevalue(model),
+        actual_dataset=data.slice(SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)),
+        reference_dataset=data.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
+        threshold=threshold,
+    ).execute()
 
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
     "data,model,threshold,expected_metric,classification_label",
     [
         ("german_credit_data", "german_credit_model", 0.05, 0.03, "Default"),
         ("enron_data", "enron_model", 0.2, 0.12, "CALIFORNIA CRISIS"),
     ],
 )
 def test_drift_model_prob_earth_movers_distance(data, model, threshold, expected_metric, classification_label, request):
     data = request.getfixturevalue(data)
-    results = drift.test_drift_prediction_earth_movers_distance(model=request.getfixturevalue(model),
-                                                                actual_dataset=data.slice(
-                                                                    SlicingFunction(lambda df: df.tail(len(df) // 2),
-                                                                                    row_level=False)),
-                                                                reference_dataset=data.slice(
-                                                                    SlicingFunction(lambda df: df.head(len(df) // 2),
-                                                                                    row_level=False)),
-                                                                classification_label=classification_label,
-                                                                threshold=threshold).execute()
+    results = drift.test_drift_prediction_earth_movers_distance(
+        model=request.getfixturevalue(model),
+        actual_dataset=data.slice(SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)),
+        reference_dataset=data.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
+        classification_label=classification_label,
+        threshold=threshold,
+    ).execute()
 
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 def test_drift_model_prob_ks_exception(german_credit_data, german_credit_model, threshold=0.02):
     with pytest.raises(Exception):
         ds = german_credit_data
-        drift.test_drift_prediction_ks(model=german_credit_model, actual_dataset=ds.slice(
-            SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)), reference_dataset=ds.slice(
-            SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)), classification_label="random_value",
-                                       threshold=threshold).execute()
+        drift.test_drift_prediction_ks(
+            model=german_credit_model,
+            actual_dataset=ds.slice(SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)),
+            reference_dataset=ds.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
+            classification_label="random_value",
+            threshold=threshold,
+        ).execute()
 
 
 @pytest.mark.parametrize(
     "data,threshold,expected_metric,column_name",
     [("german_credit_data", 0.05, 0.76, "credit_amount")],
 )
 def test_drift_data_chi_square_exception(data, threshold, expected_metric, column_name, request):
     with pytest.raises(Exception):
         data = request.getfixturevalue(data)
         drift.test_drift_chi_square(
             actual_dataset=data.slice(SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)),
             reference_dataset=data.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
             column_name=column_name,
-            threshold=threshold).execute()
+            threshold=threshold,
+        ).execute()
 
 
 @pytest.mark.parametrize(
     "data,threshold,expected_metric,column_name",
     [("german_credit_data", 0.05, 0.72, "personal_status")],
 )
 def test_drift_data_ks_exception(data, threshold, expected_metric, column_name, request):
     with pytest.raises(Exception):
         data = request.getfixturevalue(data)
         drift.test_drift_ks(
             actual_dataset=data.slice(SlicingFunction(lambda df: df.tail(len(df) // 2), row_level=False)),
             reference_dataset=data.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
             column_name=column_name,
-            threshold=threshold).execute()
+            threshold=threshold,
+        ).execute()
```

### Comparing `giskard-2.0.0b7/tests/test_data_processing_pipeline.py` & `giskard-2.0.0b8/tests/test_data_processing_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 import pandas as pd
 import pytest
 
 from giskard import slicing_function, Dataset, SlicingFunction
 from giskard.ml_worker.testing.registry.transformation_function import transformation_function
 
 
-@slicing_function(name='slice with parenthesis')
+@slicing_function(name="slice with parenthesis")
 def filter_with_parenthesis(x: pd.Series) -> bool:
     return x.credit_amount > 1000
 
 
-@slicing_function(name='slice cell level', cell_level=True)
+@slicing_function(name="slice cell level", cell_level=True)
 def filter_cell_level(amount: int) -> bool:
     return amount > 1000
 
 
 @slicing_function
 def filter_without_parenthesis(x: pd.Series) -> bool:
     return x.credit_amount > 2000
 
 
-@transformation_function(name='transform with parenthesis')
+@transformation_function(name="transform with parenthesis")
 def transform_with_parenthesis(x: pd.Series) -> pd.Series:
     x.credit_amount = -1
     return x
 
 
 @transformation_function
 def transform_without_parenthesis(x: pd.Series) -> pd.Series:
@@ -60,17 +60,17 @@
     ds = ds.slice(lambda x: x.credit_amount > 2000)
     assert len(ds.df) == 568
 
 
 def test_slicing_cell_level(german_credit_data: Dataset):
     assert len(german_credit_data.df) == 1000
     assert isinstance(filter_with_parenthesis, SlicingFunction), f"{type(filter_with_parenthesis)}"
-    ds = german_credit_data.slice(filter_cell_level, column_name='credit_amount')
+    ds = german_credit_data.slice(filter_cell_level, column_name="credit_amount")
     assert len(ds.df) == 884
-    ds = ds.slice(lambda amount: amount > 2000, cell_level=True, column_name='credit_amount')
+    ds = ds.slice(lambda amount: amount > 2000, cell_level=True, column_name="credit_amount")
     assert len(ds.df) == 568
 
 
 def test_chain(german_credit_data: Dataset):
     assert len(german_credit_data.df) == 1000
     german_credit_data.add_slicing_function(filter_without_parenthesis)
     german_credit_data.add_transformation_function(transform_divide_by_five)
@@ -79,39 +79,45 @@
     ds = german_credit_data.process()
     assert len(ds.df) == 188
 
 
 def test_transform_cell_level(german_credit_data: Dataset):
     assert len(german_credit_data.df) == 1000
 
-    ds = german_credit_data.slice(filter_without_parenthesis) \
-        .transform(column_level_divide(amount=5), column_name='credit_amount') \
+    ds = (
+        german_credit_data.slice(filter_without_parenthesis)
+        .transform(column_level_divide(amount=5), column_name="credit_amount")
         .slice(filter_with_parenthesis)
+    )
 
     assert len(german_credit_data.df) == 1000
     assert len(ds.df) == 188
 
 
 def test_transform_cell_level_parameterized(german_credit_data: Dataset):
     assert len(german_credit_data.df) == 1000
 
-    ds = german_credit_data.slice(filter_without_parenthesis) \
-        .transform(column_level_divide(column_name='credit_amount', amount=5)) \
+    ds = (
+        german_credit_data.slice(filter_without_parenthesis)
+        .transform(column_level_divide(column_name="credit_amount", amount=5))
         .slice(filter_with_parenthesis)
+    )
 
     assert len(german_credit_data.df) == 1000
     assert len(ds.df) == 188
 
 
 def test_transform_cell_level_lambda(german_credit_data: Dataset):
     assert len(german_credit_data.df) == 1000
 
-    ds = german_credit_data.slice(filter_without_parenthesis) \
-        .transform(lambda i: i / 5, cell_level=True, column_name='credit_amount') \
+    ds = (
+        german_credit_data.slice(filter_without_parenthesis)
+        .transform(lambda i: i / 5, cell_level=True, column_name="credit_amount")
         .slice(filter_with_parenthesis)
+    )
 
     assert len(german_credit_data.df) == 1000
     assert len(ds.df) == 188
 
 
 def test_transformation(german_credit_data: Dataset):
     ds = german_credit_data.transform(transform_without_parenthesis)
@@ -130,55 +136,60 @@
     ds = german_credit_data.transform(transform_without_annotation)
     assert np.all(ds.df.credit_amount == -2)
     assert len(german_credit_data.df) == 1000
     assert len(german_credit_data.df.credit_amount.unique()) > 1
 
 
 def test_missing_arg_slicing_function():
-    with pytest.raises(TypeError,
-                       match="Required arg 0 of slice_fn to be <class 'pandas.core.series.Series'>, but none was defined"):
+    with pytest.raises(
+        TypeError, match="Required arg 0 of slice_fn to be <class 'pandas.core.series.Series'>, but none was defined"
+    ):
+
         @slicing_function
         def slice_fn():
             return True
 
 
 def test_wrong_type_slicing_function():
-    with pytest.raises(TypeError,
-                       match="Required arg 0 of slice_fn to be <class 'pandas.core.series.Series'>, but <class 'int'> was defined"):
+    with pytest.raises(
+        TypeError,
+        match="Required arg 0 of slice_fn to be <class 'pandas.core.series.Series'>, but <class 'int'> was defined",
+    ):
+
         @slicing_function
         def slice_fn(row: int):
             return row > 0
 
-        slice_fn('str')
+        slice_fn("str")
 
 
 def test_chain_with_parameters(german_credit_data: Dataset):
-    @slicing_function(name='row greater than')
+    @slicing_function(name="row greater than")
     def filter_greater_than(x: pd.Series, row: str, threshold: int) -> bool:
         return x[row] > threshold
 
     @transformation_function
     def transform_divide_by(x: pd.Series, row: str, divider: int) -> pd.Series:
         x[row] /= divider
         return x
 
     assert len(german_credit_data.df) == 1000
-    german_credit_data.add_slicing_function(filter_greater_than('credit_amount', 2000))
-    german_credit_data.add_transformation_function(transform_divide_by('credit_amount', 5))
-    german_credit_data.add_slicing_function(filter_greater_than('credit_amount', 1000))
+    german_credit_data.add_slicing_function(filter_greater_than("credit_amount", 2000))
+    german_credit_data.add_transformation_function(transform_divide_by("credit_amount", 5))
+    german_credit_data.add_slicing_function(filter_greater_than("credit_amount", 1000))
     assert len(german_credit_data.df) == 1000
     ds = german_credit_data.process()
     assert len(ds.df) == 188
 
 
 def test_transformation_without_type():
     @transformation_function(row_level=True)
     def add_positive_sentence(row):
         row = row.copy()
         row.text += " I love this!"
         return row
 
-    df = pd.DataFrame([{'text': 'testing.'}])
+    df = pd.DataFrame([{"text": "testing."}])
     dataset = Dataset(df, cat_columns=[])
     transformed_dataset = dataset.transform(add_positive_sentence)
 
-    assert transformed_dataset.df.iloc[0].text == 'testing. I love this!'
+    assert transformed_dataset.df.iloc[0].text == "testing. I love this!"
```

### Comparing `giskard-2.0.0b7/tests/test_dataset.py` & `giskard-2.0.0b8/tests/test_dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import pandas as pd
 import numpy as np
 import pytest
 from giskard.datasets.base import Dataset
 
 valid_df = pd.DataFrame(
     {
-        "categorical_column": ['turtle', 'crocodile', 'turtle'],
-        "text_column": ['named Giskard', 'a nile crocodile', 'etc'],
+        "categorical_column": ["turtle", "crocodile", "turtle"],
+        "text_column": ["named Giskard", "a nile crocodile", "etc"],
         "numeric_column": [15.5, 25.9, 2.4],
     }
 )
-valid_df_column_types = {'categorical_column': 'category', 'text_column': 'text', 'numeric_column': 'numeric'}
+valid_df_column_types = {"categorical_column": "category", "text_column": "text", "numeric_column": "numeric"}
 
 nonvalid_df = pd.DataFrame(
     {
-        "categorical_column": [['turtle'], ['crocodile'], ['turtle']],
-        "text_column": [{1: 'named Giskard'}, {2: 'a nile crocodile'}, {3: 'etc'}],
+        "categorical_column": [["turtle"], ["crocodile"], ["turtle"]],
+        "text_column": [{1: "named Giskard"}, {2: "a nile crocodile"}, {3: "etc"}],
         "numeric_column": [(15.5, 1), (25.9, 2), (2.4, 3)],
     }
 )
 
 
 def test_factory():
     my_dataset = Dataset(valid_df)
@@ -31,25 +31,25 @@
     with pytest.warns(
         UserWarning,
         match=r"You did not provide the optional argument 'target'\. 'target' is the column name "
         r"in df corresponding to the actual target variable \(ground truth\)\.",
     ):
         my_dataset = Dataset(valid_df)
     assert my_dataset.column_types == {
-        'categorical_column': 'category',
-        'text_column': 'text',
-        'numeric_column': 'numeric',
+        "categorical_column": "category",
+        "text_column": "text",
+        "numeric_column": "numeric",
     }
 
     # Option 1: column_types is provided
     my_dataset = Dataset(valid_df, column_types=valid_df_column_types)
     assert my_dataset.column_types == valid_df_column_types
 
     # Option 2: cat_columns is provided
-    cat_columns = ['categorical_column']
+    cat_columns = ["categorical_column"]
     my_dataset = Dataset(valid_df, cat_columns=cat_columns)
     assert my_dataset.column_types == valid_df_column_types
 
     # Option 3: infer_column_types is provided
     my_dataset = Dataset(valid_df)
     assert my_dataset.column_types == valid_df_column_types
 
@@ -68,15 +68,15 @@
         TypeError,
         match=r"The following columns in your df: \['categorical_column', 'text_column'\] are not hashable\. "
         r"We currently support only hashable column types such as int, bool, str, tuple and not list or dict\.",
     ):
         Dataset(nonvalid_df, column_types=valid_df_column_types)
 
     # Option 2: cat_columns is provided
-    cat_columns = ['categorical_column']
+    cat_columns = ["categorical_column"]
     with pytest.raises(
         TypeError,
         match=r"The following columns in your df: \['categorical_column', 'text_column'\] are not hashable\. "
         r"We currently support only hashable column types such as int, bool, str, tuple and not list or dict\.",
     ):
         Dataset(nonvalid_df, cat_columns=cat_columns)
 
@@ -93,22 +93,22 @@
     df = pd.DataFrame({"feature": [1, 2, "string", None, np.nan], "target": [0, 0, 1, 1, 0]})
 
     with pytest.raises(TypeError):
         Dataset(df, target="target")
 
 
 def test_inference_priority():
-    column_types = {'categorical_column': 'text'}
-    expected_df_column_types = {'categorical_column': 'text', 'text_column': 'text', 'numeric_column': 'numeric'}
+    column_types = {"categorical_column": "text"}
+    expected_df_column_types = {"categorical_column": "text", "text_column": "text", "numeric_column": "numeric"}
 
     # Case 1: only one column in column_types is provided
     my_dataset = Dataset(valid_df, column_types=column_types)
     assert my_dataset.column_types == expected_df_column_types
 
     # Case 2: one column in column_types is provided, one in cat_columns
-    my_dataset = Dataset(valid_df, column_types=column_types, cat_columns=['categorical_column'])
+    my_dataset = Dataset(valid_df, column_types=column_types, cat_columns=["categorical_column"])
     assert my_dataset.column_types == valid_df_column_types
 
     # Case 3: an unknown column in column_types is provided
-    column_types = {'unknown_column': 'text'}
-    my_dataset = Dataset(valid_df, column_types=column_types, cat_columns=['categorical_column'])
+    column_types = {"unknown_column": "text"}
+    my_dataset = Dataset(valid_df, column_types=column_types, cat_columns=["categorical_column"])
     assert my_dataset.column_types == valid_df_column_types
```

### Comparing `giskard-2.0.0b7/tests/test_metamorphic_direction.py` & `giskard-2.0.0b8/tests/test_metamorphic_direction.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,61 +8,69 @@
 
 def _test_metamorphic_increasing_regression(ds: Dataset, model, threshold):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         x.bmi = x.bmi + x.bmi * 0.1
         return x
 
-    results = metamorphic.test_metamorphic_increasing(model=model, dataset=ds, transformation_function=perturbation,
-                                                      threshold=threshold).execute()
+    results = metamorphic.test_metamorphic_increasing(
+        model=model, dataset=ds, transformation_function=perturbation, threshold=threshold
+    ).execute()
 
     assert results.actual_slices_size[0] == 442
     assert round(results.metric, 2) == 0.44
     return results.passed
 
 
 def _test_metamorphic_decreasing_regression(ds: Dataset, model, threshold):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         x.age = x.age - x.age * 0.1
         return x
 
-    results = metamorphic.test_metamorphic_decreasing(model=model, dataset=ds, transformation_function=perturbation,
-                                                      threshold=threshold).execute()
+    results = metamorphic.test_metamorphic_decreasing(
+        model=model, dataset=ds, transformation_function=perturbation, threshold=threshold
+    ).execute()
     assert results.actual_slices_size[0] == 442
     assert round(results.metric, 2) == 0.54
     return results.passed
 
 
 def _test_metamorphic_increasing_classification(df, model, threshold):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         x.duration_in_month = x.duration_in_month + x.duration_in_month * 0.5
         return x
 
-    results = metamorphic.test_metamorphic_increasing(model=model, dataset=df, transformation_function=perturbation,
-                                                      threshold=threshold,
-                                                      classification_label=model.meta.classification_labels[
-                                                          0]).execute()
+    results = metamorphic.test_metamorphic_increasing(
+        model=model,
+        dataset=df,
+        transformation_function=perturbation,
+        threshold=threshold,
+        classification_label=model.meta.classification_labels[0],
+    ).execute()
 
     assert results.actual_slices_size[0] == 1000
     assert results.metric == 1
     return results.passed
 
 
 def _test_metamorphic_decreasing_classification(df, model, threshold):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         x.duration_in_month = x.duration_in_month * 0.5
         return x
 
-    results = metamorphic.test_metamorphic_decreasing(model=model, dataset=df, transformation_function=perturbation,
-                                                      threshold=threshold,
-                                                      classification_label=model.meta.classification_labels[
-                                                          0]).execute()
+    results = metamorphic.test_metamorphic_decreasing(
+        model=model,
+        dataset=df,
+        transformation_function=perturbation,
+        threshold=threshold,
+        classification_label=model.meta.classification_labels[0],
+    ).execute()
 
     assert results.actual_slices_size[0] == 1000
     assert results.metric == 1
     return results.passed
 
 
 def test_metamorphic_increasing_classification(german_credit_test_data, german_credit_model):
@@ -81,147 +89,177 @@
 def test_metamorphic_decreasing_regression(diabetes_dataset, linear_regression_diabetes):
     assert _test_metamorphic_decreasing_regression(diabetes_dataset, linear_regression_diabetes, 0.5)
     assert not _test_metamorphic_decreasing_regression(diabetes_dataset, linear_regression_diabetes, 0.6)
 
 
 def test_metamorphic_decreasing_exception(german_credit_test_data, german_credit_model):
     with pytest.raises(Exception):
+
         @transformation_function()
         def perturbation(x: pd.Series) -> pd.Series:
             x.duration_in_month = x.duration_in_month * 0.5
             return x
 
-        metamorphic.test_metamorphic_decreasing(model=german_credit_model, dataset=german_credit_test_data,
-                                                transformation_function=perturbation, threshold=0.5,
-                                                classification_label="random_value").execute()
+        metamorphic.test_metamorphic_decreasing(
+            model=german_credit_model,
+            dataset=german_credit_test_data,
+            transformation_function=perturbation,
+            threshold=0.5,
+            classification_label="random_value",
+        ).execute()
 
 
 def test_metamorphic_increasing_exception(german_credit_test_data, german_credit_model):
     with pytest.raises(Exception):
+
         @transformation_function()
         def perturbation(x: pd.Series) -> pd.Series:
             x.duration_in_month = x.duration_in_month * 0.5
             return x
 
-        metamorphic.test_metamorphic_increasing(model=german_credit_model, dataset=german_credit_test_data,
-                                                transformation_function=perturbation, threshold=0.5,
-                                                classification_label="random_value").execute()
+        metamorphic.test_metamorphic_increasing(
+            model=german_credit_model,
+            dataset=german_credit_test_data,
+            transformation_function=perturbation,
+            threshold=0.5,
+            classification_label="random_value",
+        ).execute()
 
 
 def test_metamorphic_increasing_t_test(german_credit_test_data, german_credit_model):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         x.sex = "female" if x.sex == "male" else "male"
         return x
 
-    results = metamorphic.test_metamorphic_increasing_t_test(model=german_credit_model, dataset=german_credit_test_data,
-                                                             transformation_function=perturbation,
-                                                             critical_quantile=0.05,
-                                                             classification_label="Default").execute()
+    results = metamorphic.test_metamorphic_increasing_t_test(
+        model=german_credit_model,
+        dataset=german_credit_test_data,
+        transformation_function=perturbation,
+        critical_quantile=0.05,
+        classification_label="Default",
+    ).execute()
 
     assert results.actual_slices_size[0] == len(german_credit_test_data)
     assert not results.passed, f"metric = {results.metric}"
 
 
 def test_metamorphic_decreasing_t_test(german_credit_test_data, german_credit_model):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         x.sex = "female" if x.sex == "male" else "male"
         return x
 
-    results = metamorphic.test_metamorphic_decreasing_t_test(model=german_credit_model, dataset=german_credit_test_data,
-                                                             transformation_function=perturbation,
-                                                             critical_quantile=0.05,
-                                                             classification_label="Default").execute()
+    results = metamorphic.test_metamorphic_decreasing_t_test(
+        model=german_credit_model,
+        dataset=german_credit_test_data,
+        transformation_function=perturbation,
+        critical_quantile=0.05,
+        classification_label="Default",
+    ).execute()
 
     assert results.actual_slices_size[0] == len(german_credit_test_data)
     assert results.passed, f"metric = {results.metric}"
 
 
 def test_metamorphic_increasing_wilcoxon(german_credit_test_data, german_credit_model):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         x.sex = "female" if x.sex == "male" else "male"
         return x
 
-    results = metamorphic.test_metamorphic_increasing_wilcoxon(model=german_credit_model,
-                                                               dataset=german_credit_test_data,
-                                                               transformation_function=perturbation,
-                                                               critical_quantile=0.05,
-                                                               classification_label="Default").execute()
+    results = metamorphic.test_metamorphic_increasing_wilcoxon(
+        model=german_credit_model,
+        dataset=german_credit_test_data,
+        transformation_function=perturbation,
+        critical_quantile=0.05,
+        classification_label="Default",
+    ).execute()
 
     assert results.actual_slices_size[0] == len(german_credit_test_data)
     assert not results.passed, f"metric = {results.metric}"
 
 
 def test_metamorphic_decreasing_wilcoxon(german_credit_test_data, german_credit_model):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         x.sex = "female" if x.sex == "male" else "male"
         return x
 
-    results = metamorphic.test_metamorphic_decreasing_wilcoxon(model=german_credit_model,
-                                                               dataset=german_credit_test_data,
-                                                               transformation_function=perturbation,
-                                                               critical_quantile=0.05,
-                                                               classification_label="Default").execute()
+    results = metamorphic.test_metamorphic_decreasing_wilcoxon(
+        model=german_credit_model,
+        dataset=german_credit_test_data,
+        transformation_function=perturbation,
+        critical_quantile=0.05,
+        classification_label="Default",
+    ).execute()
 
     assert results.actual_slices_size[0] == len(german_credit_test_data)
     assert results.passed, f"metric = {results.metric}"
 
 
 def test_metamorphic_increasing_t_test_nopert(german_credit_test_data, german_credit_model):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         return x
 
-    results = metamorphic.test_metamorphic_increasing_t_test(model=german_credit_model, dataset=german_credit_test_data,
-                                                             transformation_function=perturbation,
-                                                             critical_quantile=0.05,
-                                                             classification_label="Default").execute()
+    results = metamorphic.test_metamorphic_increasing_t_test(
+        model=german_credit_model,
+        dataset=german_credit_test_data,
+        transformation_function=perturbation,
+        critical_quantile=0.05,
+        classification_label="Default",
+    ).execute()
 
     assert results.actual_slices_size[0] == len(german_credit_test_data)
     assert not results.passed, f"metric = {results.metric}"
 
 
 def test_metamorphic_decreasing_t_test_nopert(german_credit_test_data, german_credit_model):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         return x
 
-    results = metamorphic.test_metamorphic_decreasing_t_test(model=german_credit_model, dataset=german_credit_test_data,
-                                                             transformation_function=perturbation,
-                                                             critical_quantile=0.05,
-                                                             classification_label="Default").execute()
+    results = metamorphic.test_metamorphic_decreasing_t_test(
+        model=german_credit_model,
+        dataset=german_credit_test_data,
+        transformation_function=perturbation,
+        critical_quantile=0.05,
+        classification_label="Default",
+    ).execute()
 
     assert results.actual_slices_size[0] == len(german_credit_test_data)
     assert not results.passed, f"metric = {results.metric}"
 
 
 def test_metamorphic_increasing_wilcoxon_nopert(german_credit_test_data, german_credit_model):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         return x
 
-    results = metamorphic.test_metamorphic_increasing_wilcoxon(model=german_credit_model,
-                                                               dataset=german_credit_test_data,
-                                                               transformation_function=perturbation,
-                                                               critical_quantile=0.05,
-                                                               classification_label="Default").execute()
+    results = metamorphic.test_metamorphic_increasing_wilcoxon(
+        model=german_credit_model,
+        dataset=german_credit_test_data,
+        transformation_function=perturbation,
+        critical_quantile=0.05,
+        classification_label="Default",
+    ).execute()
 
     assert results.actual_slices_size[0] == len(german_credit_test_data)
     assert not results.passed, f"metric = {results.metric}"
 
 
 def test_metamorphic_decreasing_wilcoxon_nopert(german_credit_test_data, german_credit_model):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         return x
 
-    results = metamorphic.test_metamorphic_decreasing_wilcoxon(model=german_credit_model,
-                                                               dataset=german_credit_test_data,
-                                                               transformation_function=perturbation,
-                                                               critical_quantile=0.05,
-                                                               classification_label="Default").execute()
+    results = metamorphic.test_metamorphic_decreasing_wilcoxon(
+        model=german_credit_model,
+        dataset=german_credit_test_data,
+        transformation_function=perturbation,
+        critical_quantile=0.05,
+        classification_label="Default",
+    ).execute()
 
     assert results.actual_slices_size[0] == len(german_credit_test_data)
     assert not results.passed, f"metric = {results.metric}"
```

### Comparing `giskard-2.0.0b7/tests/test_metamorphic_invariance.py` & `giskard-2.0.0b8/tests/test_metamorphic_invariance.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 
 
 def test_metamorphic_invariance_no_change(german_credit_test_data, german_credit_model):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         return x
 
-    results = metamorphic.test_metamorphic_invariance(model=german_credit_model, dataset=german_credit_test_data,
-                                                      transformation_function=perturbation, threshold=0.1).execute()
+    results = metamorphic.test_metamorphic_invariance(
+        model=german_credit_model, dataset=german_credit_test_data, transformation_function=perturbation, threshold=0.1
+    ).execute()
 
     assert results.actual_slices_size[0] == 1000
     assert results.passed
 
 
 def test_metamorphic_invariance_with_non_linear_index(german_credit_test_data, german_credit_model):
     @transformation_function()
@@ -38,17 +39,20 @@
 
 def _test_metamorphic_invariance_male_female(german_credit_test_data, german_credit_model, threshold):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         x.sex = "female" if x.sex == "male" else "male"
         return x
 
-    results = metamorphic.test_metamorphic_invariance(model=german_credit_model, dataset=german_credit_test_data,
-                                                      transformation_function=perturbation,
-                                                      threshold=threshold).execute()
+    results = metamorphic.test_metamorphic_invariance(
+        model=german_credit_model,
+        dataset=german_credit_test_data,
+        transformation_function=perturbation,
+        threshold=threshold,
+    ).execute()
 
     assert results.actual_slices_size[0] == len(german_credit_test_data)
     assert round(results.metric, 2) == 0.97
     return results.passed
 
 
 def test_metamorphic_invariance_male_female(german_credit_test_data, german_credit_model):
@@ -59,61 +63,66 @@
 def test_metamorphic_invariance_2_perturbations(german_credit_test_data, german_credit_model):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         x.duration_in_month = x.duration_in_month * 2
         x.sex = "female" if x.sex == "male" else "male"
         return x
 
-    results = metamorphic.test_metamorphic_invariance(model=german_credit_model, dataset=german_credit_test_data,
-                                                      transformation_function=perturbation, threshold=0.1).execute()
+    results = metamorphic.test_metamorphic_invariance(
+        model=german_credit_model, dataset=german_credit_test_data, transformation_function=perturbation, threshold=0.1
+    ).execute()
 
     assert results.actual_slices_size[0] == len(german_credit_test_data)
     assert round(results.metric, 2) == 0.86
 
 
 def test_metamorphic_invariance_some_rows(german_credit_test_data, german_credit_model):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         x.sex = "female" if x.sex == "male" else "male"
         return x
 
-    results = metamorphic.test_metamorphic_invariance(model=german_credit_model, dataset=german_credit_test_data,
-                                                      transformation_function=perturbation, threshold=0.1).execute()
+    results = metamorphic.test_metamorphic_invariance(
+        model=german_credit_model, dataset=german_credit_test_data, transformation_function=perturbation, threshold=0.1
+    ).execute()
 
     assert round(results.metric, 2) == 0.97
 
 
 def test_metamorphic_invariance_regression(diabetes_dataset_with_target, linear_regression_diabetes):
     sex_values = list(diabetes_dataset_with_target.df.sex.unique())
     assert len(sex_values) == 2
 
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         x.sex = sex_values[1] if x.sex == sex_values[0] else x.sex
         return x
 
-    results = metamorphic.test_metamorphic_invariance(model=linear_regression_diabetes,
-                                                      dataset=diabetes_dataset_with_target,
-                                                      transformation_function=perturbation, threshold=0.1,
-                                                      output_sensitivity=0.1).execute()
+    results = metamorphic.test_metamorphic_invariance(
+        model=linear_regression_diabetes,
+        dataset=diabetes_dataset_with_target,
+        transformation_function=perturbation,
+        threshold=0.1,
+        output_sensitivity=0.1,
+    ).execute()
 
     assert results.actual_slices_size[0] == len(diabetes_dataset_with_target)
     assert round(results.metric, 2) == 0.11
 
 
 @pytest.mark.parametrize(
     "loc_pop, scale_pop, loc_perturb, scale_perturb, direction, window_size, critical_quantile",
     [
         (0.5, 0.5, 0, 1e-2, Direction.Invariant, 0.2, 0.05),
         (0.5, 0.5, 0.1, 0.1, Direction.Increasing, float("nan"), 0.05),
         (0.5, 0.5, -0.1, 0.1, Direction.Decreasing, float("nan"), 0.05),
     ],
 )
 def test_metamorphic_compare_t_test(
-        loc_pop, scale_pop, loc_perturb, scale_perturb, direction, window_size, critical_quantile
+    loc_pop, scale_pop, loc_perturb, scale_perturb, direction, window_size, critical_quantile
 ):
     population = np.random.normal(loc_pop, scale_pop, size=100)
     perturbation = np.random.normal(loc_perturb, scale_perturb, size=100)
     print(perturbation)
 
     result_inc, p_value_inc = paired_t_test(
         population, population + perturbation, alternative="less", critical_quantile=critical_quantile
@@ -140,15 +149,15 @@
     [
         (0.5, 0.5, 0, 1e-2, Direction.Invariant, 0.2, 0.05),
         (0.5, 0.5, 0.1, 0.1, Direction.Increasing, float("nan"), 0.05),
         (0.5, 0.5, -0.1, 0.1, Direction.Decreasing, float("nan"), 0.05),
     ],
 )
 def test_metamorphic_compare_wilcoxon(
-        loc_pop, scale_pop, loc_perturb, scale_perturb, direction, window_size, critical_quantile
+    loc_pop, scale_pop, loc_perturb, scale_perturb, direction, window_size, critical_quantile
 ):
     population = np.random.normal(loc_pop, scale_pop, size=100)
     perturbation = np.random.normal(loc_perturb, scale_perturb, size=100)
 
     result_inc, p_value_inc = paired_wilcoxon(
         population, population + perturbation, alternative="less", critical_quantile=critical_quantile
     )
@@ -171,55 +180,69 @@
 
 def test_metamorphic_invariance_t_test(german_credit_test_data, german_credit_model):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         x.sex = "female" if x.sex == "male" else "male"
         return x
 
-    results = metamorphic.test_metamorphic_invariance_t_test(model=german_credit_model, dataset=german_credit_test_data,
-                                                             transformation_function=perturbation, window_size=0.2,
-                                                             critical_quantile=0.05).execute()
+    results = metamorphic.test_metamorphic_invariance_t_test(
+        model=german_credit_model,
+        dataset=german_credit_test_data,
+        transformation_function=perturbation,
+        window_size=0.2,
+        critical_quantile=0.05,
+    ).execute()
 
     assert results.actual_slices_size[0] == len(german_credit_test_data)
     assert results.passed, f"metric = {results.metric}"
 
 
 def test_metamorphic_invariance_t_test_nopert(german_credit_test_data, german_credit_model):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         return x
 
-    results = metamorphic.test_metamorphic_invariance_t_test(model=german_credit_model, dataset=german_credit_test_data,
-                                                             transformation_function=perturbation, window_size=0.2,
-                                                             critical_quantile=0.05).execute()
+    results = metamorphic.test_metamorphic_invariance_t_test(
+        model=german_credit_model,
+        dataset=german_credit_test_data,
+        transformation_function=perturbation,
+        window_size=0.2,
+        critical_quantile=0.05,
+    ).execute()
 
     assert results.actual_slices_size[0] == len(german_credit_test_data)
     assert results.passed, f"metric = {results.metric}"
 
 
 def test_metamorphic_invariance_wilcoxon(german_credit_test_data, german_credit_model):
     @transformation_function
     def perturbation(x: pd.Series) -> pd.Series:
         x.sex = "female" if x.sex == "male" else "male"
         return x
 
-    results = metamorphic.test_metamorphic_invariance_wilcoxon(model=german_credit_model,
-                                                               dataset=german_credit_test_data,
-                                                               transformation_function=perturbation, window_size=0.2,
-                                                               critical_quantile=0.05).execute()
+    results = metamorphic.test_metamorphic_invariance_wilcoxon(
+        model=german_credit_model,
+        dataset=german_credit_test_data,
+        transformation_function=perturbation,
+        window_size=0.2,
+        critical_quantile=0.05,
+    ).execute()
 
     assert results.actual_slices_size[0] == len(german_credit_test_data)
     assert results.passed, f"metric = {results.metric}"
 
 
 def test_metamorphic_invariance_wilcoxon_nopert(german_credit_test_data, german_credit_model):
     @transformation_function()
     def perturbation(x: pd.Series) -> pd.Series:
         return x
 
-    results = metamorphic.test_metamorphic_invariance_wilcoxon(model=german_credit_model,
-                                                               dataset=german_credit_test_data,
-                                                               transformation_function=perturbation, window_size=0.2,
-                                                               critical_quantile=0.05).execute()
+    results = metamorphic.test_metamorphic_invariance_wilcoxon(
+        model=german_credit_model,
+        dataset=german_credit_test_data,
+        transformation_function=perturbation,
+        window_size=0.2,
+        critical_quantile=0.05,
+    ).execute()
 
     assert results.actual_slices_size[0] == len(german_credit_test_data)
     assert results.passed, f"metric = {results.metric}"
```

### Comparing `giskard-2.0.0b7/tests/test_model.py` & `giskard-2.0.0b8/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,20 +37,23 @@
 def test_prediction_cache_loaded_model(linear_regression_diabetes, linear_regression_diabetes_raw, diabetes_dataset):
     nb_of_prediction_calls = [0]
 
     def prediction_fn(df):
         nb_of_prediction_calls[0] += 1
         return np.ones(df.shape[0])
 
-    with tempfile.TemporaryDirectory(prefix="cache_dir-") as cache_dir, \
-            tempfile.TemporaryDirectory(prefix="model_dir-") as model_dir:
-        model = Model(prediction_fn,
-                      model_type=SupportedModelTypes.REGRESSION,
-                      feature_names=linear_regression_diabetes.meta.feature_names,
-                      prediction_cache_dir=Path(cache_dir))
+    with tempfile.TemporaryDirectory(prefix="cache_dir-") as cache_dir, tempfile.TemporaryDirectory(
+        prefix="model_dir-"
+    ) as model_dir:
+        model = Model(
+            prediction_fn,
+            model_type=SupportedModelTypes.REGRESSION,
+            feature_names=linear_regression_diabetes.meta.feature_names,
+            prediction_cache_dir=Path(cache_dir),
+        )
 
         predictions = model.predict(diabetes_dataset)
         model.save(model_dir)
 
         loaded_model = Model.load(model_dir, prediction_cache_dir=Path(cache_dir))
         second_predictions = loaded_model.predict(diabetes_dataset)
```

### Comparing `giskard-2.0.0b7/tests/test_model_auto_inference.py` & `giskard-2.0.0b8/tests/test_model_auto_inference.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     my_automodel = Model(**kwargs)
     assert isinstance(my_automodel, CatboostModel)
 
 
 def test_huggingface():
     from giskard.models.huggingface import HuggingFaceModel
     from transformers import BertForSequenceClassification
+
     model_name = "cross-encoder/ms-marco-TinyBERT-L-2"
     my_model = BertForSequenceClassification.from_pretrained(model_name, num_labels=4, ignore_mismatched_sizes=True)
 
     kwargs = {"model": my_model, "model_type": "classification", "classification_labels": [""]}
     my_automodel = Model(**kwargs)
     assert isinstance(my_automodel, HuggingFaceModel)
 
@@ -43,14 +44,17 @@
 
 
 def test_tensorflow():
     import tensorflow as tf
     from tensorflow import keras
     from giskard.models.tensorflow import TensorFlowModel
 
-    my_model = tf.keras.Sequential([
-        keras.layers.Dense(512, activation='relu', input_shape=(784,)),
-        keras.layers.Dropout(0.2),
-        keras.layers.Dense(10, activation='softmax')])
+    my_model = tf.keras.Sequential(
+        [
+            keras.layers.Dense(512, activation="relu", input_shape=(784,)),
+            keras.layers.Dropout(0.2),
+            keras.layers.Dense(10, activation="softmax"),
+        ]
+    )
     kwargs = {"model": my_model, "model_type": "classification", "classification_labels": [""]}
     my_automodel = Model(**kwargs)
     assert isinstance(my_automodel, TensorFlowModel)
```

### Comparing `giskard-2.0.0b7/tests/test_model_explanation.py` & `giskard-2.0.0b8/tests/test_model_explanation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/tests/test_model_postprocess.py` & `giskard-2.0.0b8/tests/test_model_postprocess.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b7/tests/test_performance.py` & `giskard-2.0.0b8/tests/test_performance.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
 @pytest.mark.parametrize(
     "data,model,threshold,expected_metric,actual_slices_size",
     [("german_credit_data", "german_credit_model", 0.5, 0.85, 1000)],
 )
 def test_f1_empty_slice(data, model, threshold, expected_metric, actual_slices_size, request):
     @slicing_function
     def my_slicing_function(row: pd.Series):
-        return row['age'] > 100
+        return row["age"] > 100
 
     with pytest.raises(ValueError, match="The sliced dataset in test_f1 is empty."):
         performance.test_f1(
             dataset=request.getfixturevalue(data),
             model=request.getfixturevalue(model),
             slicing_function=my_slicing_function,
             threshold=threshold,
```

### Comparing `giskard-2.0.0b7/tests/test_programmatic.py` & `giskard-2.0.0b8/tests/test_programmatic.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 def test_save_suite(german_credit_data: Dataset, german_credit_model: BaseModel):
     # with MockedClient() as (client, mr):
     #     Suite().add_test(test_auc(threshold=0.2, dataset=german_credit_data)).add_test(
     #         test_f1(threshold=0.2, dataset=german_credit_data)
     #     ).upload(client, "test_project_key")
     scan(german_credit_model, german_credit_data)
 
+
 # def test_save_suite_real(german_credit_data: Dataset, german_credit_model: BaseModel):
 #     from giskard.client.giskard_client import GiskardClient
 #     client = GiskardClient("http://localhost:9000",
 #                            "")
 #
 #     german_credit_data.upload(client, 'test')
 #     german_credit_model.upload(client, 'test')
```

### Comparing `giskard-2.0.0b7/tests/test_project_uploads.py` & `giskard-2.0.0b8/tests/test_project_uploads.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 @pytest.mark.parametrize("data", [pd.DataFrame(data)])
 def test_verify_is_pandasdataframe_pass(data):
     validate_is_pandasdataframe(data)
 
 
 def test_validate_deterministic_model():
-    data = pd.DataFrame(np.random.rand(5, 1), columns=['0'])
+    data = pd.DataFrame(np.random.rand(5, 1), columns=["0"])
     ones = np.ones(len(data))
     constant_model = SKLearnModel(
         model=DummyClassifier(strategy="constant", constant=1).fit(data, np.ones(len(data))),
         model_type=SupportedModelTypes.CLASSIFICATION,
     )
     ds = Dataset(df=data)
 
@@ -72,40 +72,41 @@
 
 
 def test_validate_column_types(german_credit_data, german_credit_test_data):
     test_ds = german_credit_test_data
     ds = german_credit_data
 
     with pytest.warns(
-            UserWarning,
-            match=r"Feature 'people_under_maintenance' is declared as 'numeric' but has 2 .* Are you sure it is not a 'category' feature?",
+        UserWarning,
+        match=r"Feature 'people_under_maintenance' is declared as 'numeric' but has 2 .* Are you sure it is not a 'category' feature?",
     ):
         validate_column_categorization(test_ds)
 
     test_ds.column_types = {c: test_ds.column_types[c] for c in test_ds.column_types if c != test_ds.target}
     validate_column_categorization(ds)
     original_column_types = ds.column_types
 
     with pytest.raises(ValueError) as e:
         ds.column_types = {c: original_column_types[c] for c in original_column_types if c not in {ds.target, "sex"}}
         validate_column_types(ds)
     assert e.match(
         r"The following keys \['sex'\] are missing from 'column_types'\. "
-        r"Please make sure that the column names in `column_types` covers all the existing columns in your dataset\.")
+        r"Please make sure that the column names in `column_types` covers all the existing columns in your dataset\."
+    )
 
     with pytest.warns(
-            UserWarning,
-            match=r"The provided keys .* in 'column_types' are not part of your.*",
+        UserWarning,
+        match=r"The provided keys .* in 'column_types' are not part of your.*",
     ):
         new_ft = dict(original_column_types)
         new_ft["non-existing-column"] = SupportedColumnTypes.CATEGORY.value
         Dataset(ds.df, target=ds.target, column_types=new_ft)
 
     broken_types = dict(test_ds.column_types)
     broken_types["people_under_maintenance"] = SupportedColumnTypes.CATEGORY.value
     broken_types["sex"] = SupportedColumnTypes.NUMERIC.value
     with pytest.warns(
-            UserWarning,
-            match=r"Feature 'sex' is declared as 'numeric' but has 2 .* Are you sure it is not a 'category' feature?",
+        UserWarning,
+        match=r"Feature 'sex' is declared as 'numeric' but has 2 .* Are you sure it is not a 'category' feature?",
     ):
         test_ds.column_types = broken_types
         validate_column_categorization(test_ds)
```

### Comparing `giskard-2.0.0b7/tests/test_statistical.py` & `giskard-2.0.0b8/tests/test_statistical.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,20 @@
         ("enron_data", "enron_model", 0, 0.1, 0.32, 25),
     ],
 )
 def test_statistical(data, model, threshold, label, expected_metric, actual_slices_size, request):
     data = request.getfixturevalue(data)
     model = request.getfixturevalue(model)
 
-    results = statistical.test_right_label(model=model, dataset=data.slice(
-        SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
-                                           classification_label=model.meta.classification_labels[label],
-                                           threshold=threshold).execute()
+    results = statistical.test_right_label(
+        model=model,
+        dataset=data.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
+        classification_label=model.meta.classification_labels[label],
+        threshold=threshold,
+    ).execute()
 
     assert results.actual_slices_size[0] == actual_slices_size
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
@@ -34,18 +36,20 @@
         ("enron_data", "enron_model", 0, 0.01, 0.1, 10),
     ],
 )
 def test_statistical_filtered(data, model, threshold, label, expected_metric, actual_slices_size, request):
     data = request.getfixturevalue(data)
     model = request.getfixturevalue(model)
 
-    results = statistical.test_right_label(model=model,
-                                           dataset=data.slice(SlicingFunction(lambda df: df.head(10), row_level=False)),
-                                           classification_label=model.meta.classification_labels[label],
-                                           threshold=threshold).execute()
+    results = statistical.test_right_label(
+        model=model,
+        dataset=data.slice(SlicingFunction(lambda df: df.head(10), row_level=False)),
+        classification_label=model.meta.classification_labels[label],
+        threshold=threshold,
+    ).execute()
 
     assert results.actual_slices_size[0] == actual_slices_size
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
@@ -55,43 +59,55 @@
         ("german_credit_data", "german_credit_model", 1, 0.1, 0.34, 500),
         ("enron_data", "enron_model", 0, 0.1, 0.32, 25),
     ],
 )
 def test_output_in_range_model(data, model, threshold, label, expected_metric, actual_slices_size, request):
     data = request.getfixturevalue(data)
     model = request.getfixturevalue(model)
-    results = statistical.test_output_in_range(model=model,
-                                               dataset=data.slice(lambda df: df.head(len(df) // 2), row_level=False),
-                                               classification_label=model.meta.classification_labels[label],
-                                               min_range=0.3, max_range=0.7, threshold=threshold).execute()
+    results = statistical.test_output_in_range(
+        model=model,
+        dataset=data.slice(lambda df: df.head(len(df) // 2), row_level=False),
+        classification_label=model.meta.classification_labels[label],
+        min_range=0.3,
+        max_range=0.7,
+        threshold=threshold,
+    ).execute()
 
     assert results.actual_slices_size[0] == actual_slices_size
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
     "data,model,threshold,expected_metric,actual_slices_size",
     [("diabetes_dataset_with_target", "linear_regression_diabetes", 0.1, 0.28, 221)],
 )
 def test_output_in_range_reg(data, model, threshold, expected_metric, actual_slices_size, request):
     data = request.getfixturevalue(data)
-    results = statistical.test_output_in_range(model=request.getfixturevalue(model), dataset=data.slice(
-        SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)), min_range=100, max_range=150,
-                                               threshold=threshold).execute()
+    results = statistical.test_output_in_range(
+        model=request.getfixturevalue(model),
+        dataset=data.slice(SlicingFunction(lambda df: df.head(len(df) // 2), row_level=False)),
+        min_range=100,
+        max_range=150,
+        threshold=threshold,
+    ).execute()
 
     assert results.actual_slices_size[0] == actual_slices_size
     assert round(results.metric, 2) == expected_metric
     assert results.passed
 
 
 @pytest.mark.parametrize(
     "data,model",
     [("german_credit_data", "german_credit_model")],
 )
 def test_disparate_impact(data, model, request):
     data = request.getfixturevalue(data)
     model = request.getfixturevalue(model)
-    results = statistical.test_disparate_impact(model=model, dataset=data, protected_slicing_function=SlicingFunction(
-        lambda df: df[df.sex == "female"], row_level=False), unprotected_slicing_function=SlicingFunction(
-        lambda df: df[df.sex == "male"], row_level=False), positive_outcome="Not default").execute()
+    results = statistical.test_disparate_impact(
+        model=model,
+        dataset=data,
+        protected_slicing_function=SlicingFunction(lambda df: df[df.sex == "female"], row_level=False),
+        unprotected_slicing_function=SlicingFunction(lambda df: df[df.sex == "male"], row_level=False),
+        positive_outcome="Not default",
+    ).execute()
     assert results.passed, f"DI = {results.metric}"
```

### Comparing `giskard-2.0.0b7/tests/test_upload.py` & `giskard-2.0.0b8/tests/test_upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,27 +18,35 @@
     with MockedClient() as (client, mr):
         saved_id = diabetes_dataset_with_target.upload(client, "test-project")
         match_model_id(saved_id)
         match_url_patterns(mr.request_history, artifact_url_pattern)
         match_url_patterns(mr.request_history, datasets_url_pattern)
 
         with pytest.raises(Exception) as e:
-            Dataset(df=diabetes_dataset.df,
-                    column_types=diabetes_dataset.column_types, target=diabetes_dataset_with_target.target)
+            Dataset(
+                df=diabetes_dataset.df,
+                column_types=diabetes_dataset.column_types,
+                target=diabetes_dataset_with_target.target,
+            )
         assert e.match(
             "Invalid target parameter: 'target' column is not present in the dataset "
-            "with columns: \['age', 'sex', 'bmi', 'bp', 's1', 's2', 's3', 's4', 's5', 's6'\]")  # noqa
+            "with columns: \['age', 'sex', 'bmi', 'bp', 's1', 's2', 's3', 's4', 's5', 's6'\]"
+        )  # noqa
 
         with pytest.raises(Exception) as e:
             diabetes_dataset.column_types = {"test": "test"}
-            Dataset(df=diabetes_dataset.df,
-                    column_types=diabetes_dataset.column_types, target=diabetes_dataset_with_target.target)
+            Dataset(
+                df=diabetes_dataset.df,
+                column_types=diabetes_dataset.column_types,
+                target=diabetes_dataset_with_target.target,
+            )
         assert e.match(
             "Invalid target parameter: 'target' column is not present in the dataset "
-            "with columns: \['age', 'sex', 'bmi', 'bp', 's1', 's2', 's3', 's4', 's5', 's6'\]")  # noqa
+            "with columns: \['age', 'sex', 'bmi', 'bp', 's1', 's2', 's3', 's4', 's5', 's6'\]"
+        )  # noqa
 
 
 def _test_upload_model(model: SKLearnModel, ds: Dataset):
     artifact_url_pattern = re.compile(
         "http://giskard-host:12345/api/v2/artifacts/test-project/models/[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/.*"
     )
     models_url_pattern = re.compile("http://giskard-host:12345/api/v2/project/test-project/models")
@@ -75,15 +83,16 @@
                     model=model.model,
                     model_type=model.meta.model_type,
                     feature_names=model.meta.feature_names,
                     name=model_name,
                     classification_labels=[0, 1],
                 ).upload(client, "test-project", ds)
             assert e.match(
-                "Values .* in .* column are not declared in classification_labels parameter .* of the model: uploaded model")  # noqa
+                "Values .* in .* column are not declared in classification_labels parameter .* of the model: uploaded model"
+            )  # noqa
 
 
 @pytest.mark.parametrize(
     "data,model,",
     [
         ("german_credit_data", "german_credit_model"),
         ("diabetes_dataset", "linear_regression_diabetes"),
```

