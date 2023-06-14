# Comparing `tmp/google-cloud-orchestration-airflow-1.8.0.tar.gz` & `tmp/google-cloud-orchestration-airflow-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-orchestration-airflow-1.8.0.tar", last modified: Wed May 31 18:48:37 2023, max compression
+gzip compressed data, was "google-cloud-orchestration-airflow-1.9.0.tar", last modified: Wed Jun 14 14:52:52 2023, max compression
```

## Comparing `google-cloud-orchestration-airflow-1.8.0.tar` & `google-cloud-orchestration-airflow-1.9.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4926 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3968 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.139948 google-cloud-orchestration-airflow-1.8.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.139948 google-cloud-orchestration-airflow-1.8.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.139948 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.139948 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.143948 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service/
--rw-rw-r--   0 root         (0)     1003     3283 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.143948 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/
--rw-rw-r--   0 root         (0)     1003     2825 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4128 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.143948 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.143948 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/
--rw-rw-r--   0 root         (0)     1003      761 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/__init__.py
--rw-rw-r--   0 root         (0)     1003    55879 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/async_client.py
--rw-rw-r--   0 root         (0)     1003    65870 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/client.py
--rw-rw-r--   0 root         (0)     1003     6061 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.143948 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9692 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22079 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22552 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    52792 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.147949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/
--rw-rw-r--   0 root         (0)     1003      765 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/__init__.py
--rw-rw-r--   0 root         (0)     1003    20236 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/async_client.py
--rw-rw-r--   0 root         (0)     1003    28753 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/client.py
--rw-rw-r--   0 root         (0)     1003     6127 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.147949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6890 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14428 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14632 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22147 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.147949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/
--rw-rw-r--   0 root         (0)     1003     2384 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    66667 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/environments.py
--rw-rw-r--   0 root         (0)     1003     4199 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/image_versions.py
--rw-rw-r--   0 root         (0)     1003     4321 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/operations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.147949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/
--rw-rw-r--   0 root         (0)     1003     3148 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4885 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003      103 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.147949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.147949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/
--rw-rw-r--   0 root         (0)     1003      761 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/__init__.py
--rw-rw-r--   0 root         (0)     1003    65214 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/async_client.py
--rw-rw-r--   0 root         (0)     1003    75457 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/client.py
--rw-rw-r--   0 root         (0)     1003     6106 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.151949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10575 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/base.py
--rw-rw-r--   0 root         (0)     1003    24495 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    25040 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    63125 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.151949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/
--rw-rw-r--   0 root         (0)     1003      765 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/__init__.py
--rw-rw-r--   0 root         (0)     1003    20285 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/async_client.py
--rw-rw-r--   0 root         (0)     1003    28802 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/client.py
--rw-rw-r--   0 root         (0)     1003     6172 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.151949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6900 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14438 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14642 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22172 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.151949 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     2702 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    76326 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/environments.py
--rw-rw-r--   0 root         (0)     1003     4210 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/image_versions.py
--rw-rw-r--   0 root         (0)     1003     4201 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/operations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/
--rw-r--r--   0 root         (0)     1003     4926 2023-05-31 18:48:37.000000 google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     5387 2023-05-31 18:48:37.000000 google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-31 18:48:37.000000 google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       82 2023-05-31 18:48:37.000000 google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-31 18:48:37.000000 google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-05-31 18:48:37.000000 google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-05-31 18:48:37.000000 google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3092 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   200608 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1/test_environments.py
--rw-rw-r--   0 root         (0)     1003    98881 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1/test_image_versions.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:37.155950 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   224104 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1beta1/test_environments.py
--rw-rw-r--   0 root         (0)     1003    98916 2023-05-31 18:46:02.000000 google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1beta1/test_image_versions.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.460386 google-cloud-orchestration-airflow-1.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4881 2023-06-14 14:52:52.460386 google-cloud-orchestration-airflow-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3932 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.440384 google-cloud-orchestration-airflow-1.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.440384 google-cloud-orchestration-airflow-1.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.440384 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.440384 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.444384 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service/
+-rw-rw-r--   0 root         (0)     1003     3957 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.444384 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/
+-rw-rw-r--   0 root         (0)     1003     3499 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6156 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.444384 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.444384 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/
+-rw-rw-r--   0 root         (0)     1003      761 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/__init__.py
+-rw-rw-r--   0 root         (0)     1003    72317 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/async_client.py
+-rw-rw-r--   0 root         (0)     1003    83164 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/client.py
+-rw-rw-r--   0 root         (0)     1003     6061 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.448385 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12259 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    28298 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    28895 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    78622 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.448385 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/
+-rw-rw-r--   0 root         (0)     1003      765 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20236 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28753 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/client.py
+-rw-rw-r--   0 root         (0)     1003     6127 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.448385 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6890 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14428 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14632 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22147 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.448385 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3058 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    76532 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/types/environments.py
+-rw-rw-r--   0 root         (0)     1003     4199 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/types/image_versions.py
+-rw-rw-r--   0 root         (0)     1003     4530 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/types/operations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.448385 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     3684 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6913 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003      103 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.452385 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.452385 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/
+-rw-rw-r--   0 root         (0)     1003      761 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/__init__.py
+-rw-rw-r--   0 root         (0)     1003    81777 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/async_client.py
+-rw-rw-r--   0 root         (0)     1003    92876 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/client.py
+-rw-rw-r--   0 root         (0)     1003     6106 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.452385 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13142 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    30739 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    31408 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    88980 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.452385 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/
+-rw-rw-r--   0 root         (0)     1003      765 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20285 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28802 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/client.py
+-rw-rw-r--   0 root         (0)     1003     6172 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.456385 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6900 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14438 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14642 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22172 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.456385 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     3238 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    83347 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/types/environments.py
+-rw-rw-r--   0 root         (0)     1003     4210 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/types/image_versions.py
+-rw-rw-r--   0 root         (0)     1003     4410 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/types/operations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.456385 google-cloud-orchestration-airflow-1.9.0/google_cloud_orchestration_airflow.egg-info/
+-rw-r--r--   0 root         (0)     1003     4881 2023-06-14 14:52:52.000000 google-cloud-orchestration-airflow-1.9.0/google_cloud_orchestration_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     5387 2023-06-14 14:52:52.000000 google-cloud-orchestration-airflow-1.9.0/google_cloud_orchestration_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-14 14:52:52.000000 google-cloud-orchestration-airflow-1.9.0/google_cloud_orchestration_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       82 2023-06-14 14:52:52.000000 google-cloud-orchestration-airflow-1.9.0/google_cloud_orchestration_airflow.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-14 14:52:52.000000 google-cloud-orchestration-airflow-1.9.0/google_cloud_orchestration_airflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-06-14 14:52:52.000000 google-cloud-orchestration-airflow-1.9.0/google_cloud_orchestration_airflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-06-14 14:52:52.000000 google-cloud-orchestration-airflow-1.9.0/google_cloud_orchestration_airflow.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-06-14 14:52:52.460386 google-cloud-orchestration-airflow-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3083 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.456385 google-cloud-orchestration-airflow-1.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.456385 google-cloud-orchestration-airflow-1.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.456385 google-cloud-orchestration-airflow-1.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.456385 google-cloud-orchestration-airflow-1.9.0/tests/unit/gapic/service_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/tests/unit/gapic/service_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   257736 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/tests/unit/gapic/service_v1/test_environments.py
+-rw-rw-r--   0 root         (0)     1003    98881 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/tests/unit/gapic/service_v1/test_image_versions.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-14 14:52:52.460386 google-cloud-orchestration-airflow-1.9.0/tests/unit/gapic/service_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/tests/unit/gapic/service_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   281232 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/tests/unit/gapic/service_v1beta1/test_environments.py
+-rw-rw-r--   0 root         (0)     1003    98916 2023-06-14 14:50:00.000000 google-cloud-orchestration-airflow-1.9.0/tests/unit/gapic/service_v1beta1/test_image_versions.py
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/LICENSE` & `google-cloud-orchestration-airflow-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/MANIFEST.in` & `google-cloud-orchestration-airflow-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/PKG-INFO` & `google-cloud-orchestration-airflow-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-orchestration-airflow
-Version: 1.8.0
+Version: 1.9.0
 Summary: Google Cloud Orchestration Airflow API client library
-Home-page: https://github.com/googleapis/python-orchestration-airflow
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for Cloud Composer API
-====================================
+Python Client for Cloud Composer
+================================
 
 |stable| |pypi| |versions|
 
-`Cloud Composer API`_: is a managed Apache Airflow service that helps you create, schedule, monitor and manage workflows. Cloud Composer automation helps you create Airflow environments quickly and use Airflow-native tools, such as the powerful Airflow web interface and command line tools, so you can focus on your workflows and not your infrastructure.
+`Cloud Composer`_: is a managed Apache Airflow service that helps you create, schedule, monitor and manage workflows. Cloud Composer automation helps you create Airflow environments quickly and use Airflow-native tools, such as the powerful Airflow web interface and command line tools, so you can focus on your workflows and not your infrastructure.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-orchestration-airflow.svg
    :target: https://pypi.org/project/google-cloud-orchestration-airflow/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-orchestration-airflow.svg
    :target: https://pypi.org/project/google-cloud-orchestration-airflow/
-.. _Cloud Composer API: https://cloud.google.com/composer/
+.. _Cloud Composer: https://cloud.google.com/composer/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/composer/latest
 .. _Product Documentation:  https://cloud.google.com/composer/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Composer API.`_
+3. `Enable the Cloud Composer.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Composer API.:  https://cloud.google.com/composer/
+.. _Enable the Cloud Composer.:  https://cloud.google.com/composer/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-orchestration-airflow
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Composer API
+-  Read the `Client Library Documentation`_ for Cloud Composer
    to see other available methods on the client.
--  Read the `Cloud Composer API Product documentation`_ to learn
+-  Read the `Cloud Composer Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Composer API Product documentation:  https://cloud.google.com/composer/
+.. _Cloud Composer Product documentation:  https://cloud.google.com/composer/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/README.rst` & `google-cloud-orchestration-airflow-1.9.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Cloud Composer API
-====================================
+Python Client for Cloud Composer
+================================
 
 |stable| |pypi| |versions|
 
-`Cloud Composer API`_: is a managed Apache Airflow service that helps you create, schedule, monitor and manage workflows. Cloud Composer automation helps you create Airflow environments quickly and use Airflow-native tools, such as the powerful Airflow web interface and command line tools, so you can focus on your workflows and not your infrastructure.
+`Cloud Composer`_: is a managed Apache Airflow service that helps you create, schedule, monitor and manage workflows. Cloud Composer automation helps you create Airflow environments quickly and use Airflow-native tools, such as the powerful Airflow web interface and command line tools, so you can focus on your workflows and not your infrastructure.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-orchestration-airflow.svg
    :target: https://pypi.org/project/google-cloud-orchestration-airflow/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-orchestration-airflow.svg
    :target: https://pypi.org/project/google-cloud-orchestration-airflow/
-.. _Cloud Composer API: https://cloud.google.com/composer/
+.. _Cloud Composer: https://cloud.google.com/composer/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/composer/latest
 .. _Product Documentation:  https://cloud.google.com/composer/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Composer API.`_
+3. `Enable the Cloud Composer.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Composer API.:  https://cloud.google.com/composer/
+.. _Enable the Cloud Composer.:  https://cloud.google.com/composer/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-orchestration-airflow
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Composer API
+-  Read the `Client Library Documentation`_ for Cloud Composer
    to see other available methods on the client.
--  Read the `Cloud Composer API Product documentation`_ to learn
+-  Read the `Cloud Composer Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Composer API Product documentation:  https://cloud.google.com/composer/
+.. _Cloud Composer Product documentation:  https://cloud.google.com/composer/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,101 +9,111 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.orchestration.airflow.service import gapic_version as package_version
+from google.cloud.orchestration.airflow.service_v1 import (
+    gapic_version as package_version,
+)
 
 __version__ = package_version.__version__
 
 
-from google.cloud.orchestration.airflow.service_v1.services.environments.async_client import (
-    EnvironmentsAsyncClient,
-)
-from google.cloud.orchestration.airflow.service_v1.services.environments.client import (
-    EnvironmentsClient,
-)
-from google.cloud.orchestration.airflow.service_v1.services.image_versions.async_client import (
-    ImageVersionsAsyncClient,
-)
-from google.cloud.orchestration.airflow.service_v1.services.image_versions.client import (
-    ImageVersionsClient,
-)
-from google.cloud.orchestration.airflow.service_v1.types.environments import (
+from .services.environments import EnvironmentsAsyncClient, EnvironmentsClient
+from .services.image_versions import ImageVersionsAsyncClient, ImageVersionsClient
+from .types.environments import (
     CheckUpgradeResponse,
     CreateEnvironmentRequest,
     DatabaseConfig,
+    DatabaseFailoverRequest,
+    DatabaseFailoverResponse,
     DeleteEnvironmentRequest,
     EncryptionConfig,
     Environment,
     EnvironmentConfig,
+    ExecuteAirflowCommandRequest,
+    ExecuteAirflowCommandResponse,
+    FetchDatabasePropertiesRequest,
+    FetchDatabasePropertiesResponse,
     GetEnvironmentRequest,
     IPAllocationPolicy,
     ListEnvironmentsRequest,
     ListEnvironmentsResponse,
     LoadSnapshotRequest,
     LoadSnapshotResponse,
     MaintenanceWindow,
     MasterAuthorizedNetworksConfig,
     NetworkingConfig,
     NodeConfig,
+    PollAirflowCommandRequest,
+    PollAirflowCommandResponse,
     PrivateClusterConfig,
     PrivateEnvironmentConfig,
     RecoveryConfig,
     SaveSnapshotRequest,
     SaveSnapshotResponse,
     ScheduledSnapshotsConfig,
     SoftwareConfig,
+    StopAirflowCommandRequest,
+    StopAirflowCommandResponse,
     UpdateEnvironmentRequest,
     WebServerConfig,
     WebServerNetworkAccessControl,
     WorkloadsConfig,
 )
-from google.cloud.orchestration.airflow.service_v1.types.image_versions import (
+from .types.image_versions import (
     ImageVersion,
     ListImageVersionsRequest,
     ListImageVersionsResponse,
 )
-from google.cloud.orchestration.airflow.service_v1.types.operations import (
-    OperationMetadata,
-)
+from .types.operations import OperationMetadata
 
 __all__ = (
-    "EnvironmentsClient",
     "EnvironmentsAsyncClient",
-    "ImageVersionsClient",
     "ImageVersionsAsyncClient",
     "CheckUpgradeResponse",
     "CreateEnvironmentRequest",
     "DatabaseConfig",
+    "DatabaseFailoverRequest",
+    "DatabaseFailoverResponse",
     "DeleteEnvironmentRequest",
     "EncryptionConfig",
     "Environment",
     "EnvironmentConfig",
+    "EnvironmentsClient",
+    "ExecuteAirflowCommandRequest",
+    "ExecuteAirflowCommandResponse",
+    "FetchDatabasePropertiesRequest",
+    "FetchDatabasePropertiesResponse",
     "GetEnvironmentRequest",
     "IPAllocationPolicy",
+    "ImageVersion",
+    "ImageVersionsClient",
     "ListEnvironmentsRequest",
     "ListEnvironmentsResponse",
+    "ListImageVersionsRequest",
+    "ListImageVersionsResponse",
     "LoadSnapshotRequest",
     "LoadSnapshotResponse",
     "MaintenanceWindow",
     "MasterAuthorizedNetworksConfig",
     "NetworkingConfig",
     "NodeConfig",
+    "OperationMetadata",
+    "PollAirflowCommandRequest",
+    "PollAirflowCommandResponse",
     "PrivateClusterConfig",
     "PrivateEnvironmentConfig",
     "RecoveryConfig",
     "SaveSnapshotRequest",
     "SaveSnapshotResponse",
     "ScheduledSnapshotsConfig",
     "SoftwareConfig",
+    "StopAirflowCommandRequest",
+    "StopAirflowCommandResponse",
     "UpdateEnvironmentRequest",
     "WebServerConfig",
     "WebServerNetworkAccessControl",
     "WorkloadsConfig",
-    "ImageVersion",
-    "ListImageVersionsRequest",
-    "ListImageVersionsResponse",
-    "OperationMetadata",
 )
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service/gapic_version.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.0"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/types/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,91 +9,98 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.orchestration.airflow.service_v1 import (
-    gapic_version as package_version,
-)
-
-__version__ = package_version.__version__
-
-
-from .services.environments import EnvironmentsAsyncClient, EnvironmentsClient
-from .services.image_versions import ImageVersionsAsyncClient, ImageVersionsClient
-from .types.environments import (
+from .environments import (
     CheckUpgradeResponse,
     CreateEnvironmentRequest,
     DatabaseConfig,
+    DatabaseFailoverRequest,
+    DatabaseFailoverResponse,
     DeleteEnvironmentRequest,
     EncryptionConfig,
     Environment,
     EnvironmentConfig,
+    ExecuteAirflowCommandRequest,
+    ExecuteAirflowCommandResponse,
+    FetchDatabasePropertiesRequest,
+    FetchDatabasePropertiesResponse,
     GetEnvironmentRequest,
     IPAllocationPolicy,
     ListEnvironmentsRequest,
     ListEnvironmentsResponse,
     LoadSnapshotRequest,
     LoadSnapshotResponse,
     MaintenanceWindow,
     MasterAuthorizedNetworksConfig,
     NetworkingConfig,
     NodeConfig,
+    PollAirflowCommandRequest,
+    PollAirflowCommandResponse,
     PrivateClusterConfig,
     PrivateEnvironmentConfig,
     RecoveryConfig,
     SaveSnapshotRequest,
     SaveSnapshotResponse,
     ScheduledSnapshotsConfig,
     SoftwareConfig,
+    StopAirflowCommandRequest,
+    StopAirflowCommandResponse,
     UpdateEnvironmentRequest,
     WebServerConfig,
     WebServerNetworkAccessControl,
     WorkloadsConfig,
 )
-from .types.image_versions import (
+from .image_versions import (
     ImageVersion,
     ListImageVersionsRequest,
     ListImageVersionsResponse,
 )
-from .types.operations import OperationMetadata
+from .operations import OperationMetadata
 
 __all__ = (
-    "EnvironmentsAsyncClient",
-    "ImageVersionsAsyncClient",
     "CheckUpgradeResponse",
     "CreateEnvironmentRequest",
     "DatabaseConfig",
+    "DatabaseFailoverRequest",
+    "DatabaseFailoverResponse",
     "DeleteEnvironmentRequest",
     "EncryptionConfig",
     "Environment",
     "EnvironmentConfig",
-    "EnvironmentsClient",
+    "ExecuteAirflowCommandRequest",
+    "ExecuteAirflowCommandResponse",
+    "FetchDatabasePropertiesRequest",
+    "FetchDatabasePropertiesResponse",
     "GetEnvironmentRequest",
     "IPAllocationPolicy",
-    "ImageVersion",
-    "ImageVersionsClient",
     "ListEnvironmentsRequest",
     "ListEnvironmentsResponse",
-    "ListImageVersionsRequest",
-    "ListImageVersionsResponse",
     "LoadSnapshotRequest",
     "LoadSnapshotResponse",
     "MaintenanceWindow",
     "MasterAuthorizedNetworksConfig",
     "NetworkingConfig",
     "NodeConfig",
-    "OperationMetadata",
+    "PollAirflowCommandRequest",
+    "PollAirflowCommandResponse",
     "PrivateClusterConfig",
     "PrivateEnvironmentConfig",
     "RecoveryConfig",
     "SaveSnapshotRequest",
     "SaveSnapshotResponse",
     "ScheduledSnapshotsConfig",
     "SoftwareConfig",
+    "StopAirflowCommandRequest",
+    "StopAirflowCommandResponse",
     "UpdateEnvironmentRequest",
     "WebServerConfig",
     "WebServerNetworkAccessControl",
     "WorkloadsConfig",
+    "ImageVersion",
+    "ListImageVersionsRequest",
+    "ListImageVersionsResponse",
+    "OperationMetadata",
 )
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/gapic_version.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.0"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/async_client.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/async_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -990,14 +990,256 @@
             empty_pb2.Empty,
             metadata_type=operations.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
+    async def execute_airflow_command(
+        self,
+        request: Optional[
+            Union[environments.ExecuteAirflowCommandRequest, dict]
+        ] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> environments.ExecuteAirflowCommandResponse:
+        r"""Executes Airflow CLI command.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1
+
+            async def sample_execute_airflow_command():
+                # Create a client
+                client = service_v1.EnvironmentsAsyncClient()
+
+                # Initialize request argument(s)
+                request = service_v1.ExecuteAirflowCommandRequest(
+                )
+
+                # Make the request
+                response = await client.execute_airflow_command(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.orchestration.airflow.service_v1.types.ExecuteAirflowCommandRequest, dict]]):
+                The request object. Execute Airflow Command request.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.orchestration.airflow.service_v1.types.ExecuteAirflowCommandResponse:
+                Response to
+                ExecuteAirflowCommandRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        request = environments.ExecuteAirflowCommandRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.execute_airflow_command,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def stop_airflow_command(
+        self,
+        request: Optional[Union[environments.StopAirflowCommandRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> environments.StopAirflowCommandResponse:
+        r"""Stops Airflow CLI command execution.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1
+
+            async def sample_stop_airflow_command():
+                # Create a client
+                client = service_v1.EnvironmentsAsyncClient()
+
+                # Initialize request argument(s)
+                request = service_v1.StopAirflowCommandRequest(
+                )
+
+                # Make the request
+                response = await client.stop_airflow_command(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.orchestration.airflow.service_v1.types.StopAirflowCommandRequest, dict]]):
+                The request object. Stop Airflow Command request.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.orchestration.airflow.service_v1.types.StopAirflowCommandResponse:
+                Response to
+                StopAirflowCommandRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        request = environments.StopAirflowCommandRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.stop_airflow_command,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def poll_airflow_command(
+        self,
+        request: Optional[Union[environments.PollAirflowCommandRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> environments.PollAirflowCommandResponse:
+        r"""Polls Airflow CLI command execution and fetches logs.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1
+
+            async def sample_poll_airflow_command():
+                # Create a client
+                client = service_v1.EnvironmentsAsyncClient()
+
+                # Initialize request argument(s)
+                request = service_v1.PollAirflowCommandRequest(
+                )
+
+                # Make the request
+                response = await client.poll_airflow_command(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.orchestration.airflow.service_v1.types.PollAirflowCommandRequest, dict]]):
+                The request object. Poll Airflow Command request.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.orchestration.airflow.service_v1.types.PollAirflowCommandResponse:
+                Response to
+                PollAirflowCommandRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        request = environments.PollAirflowCommandRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.poll_airflow_command,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
     async def save_snapshot(
         self,
         request: Optional[Union[environments.SaveSnapshotRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
@@ -1188,14 +1430,196 @@
             environments.LoadSnapshotResponse,
             metadata_type=operations.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
+    async def database_failover(
+        self,
+        request: Optional[Union[environments.DatabaseFailoverRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation_async.AsyncOperation:
+        r"""Triggers database failover (only for highly resilient
+        environments).
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1
+
+            async def sample_database_failover():
+                # Create a client
+                client = service_v1.EnvironmentsAsyncClient()
+
+                # Initialize request argument(s)
+                request = service_v1.DatabaseFailoverRequest(
+                )
+
+                # Make the request
+                operation = client.database_failover(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = (await operation).result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.orchestration.airflow.service_v1.types.DatabaseFailoverRequest, dict]]):
+                The request object. Request to trigger database failover
+                (only for highly resilient
+                environments).
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation_async.AsyncOperation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be
+                :class:`google.cloud.orchestration.airflow.service_v1.types.DatabaseFailoverResponse`
+                Response for DatabaseFailoverRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        request = environments.DatabaseFailoverRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.database_failover,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation_async.from_gapic(
+            response,
+            self._client._transport.operations_client,
+            environments.DatabaseFailoverResponse,
+            metadata_type=operations.OperationMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def fetch_database_properties(
+        self,
+        request: Optional[
+            Union[environments.FetchDatabasePropertiesRequest, dict]
+        ] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> environments.FetchDatabasePropertiesResponse:
+        r"""Fetches database properties.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1
+
+            async def sample_fetch_database_properties():
+                # Create a client
+                client = service_v1.EnvironmentsAsyncClient()
+
+                # Initialize request argument(s)
+                request = service_v1.FetchDatabasePropertiesRequest(
+                    environment="environment_value",
+                )
+
+                # Make the request
+                response = await client.fetch_database_properties(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.orchestration.airflow.service_v1.types.FetchDatabasePropertiesRequest, dict]]):
+                The request object. Request to fetch properties of
+                environment's database.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.orchestration.airflow.service_v1.types.FetchDatabasePropertiesResponse:
+                Response for
+                FetchDatabasePropertiesRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        request = environments.FetchDatabasePropertiesRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.fetch_database_properties,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
     async def list_operations(
         self,
         request: Optional[operations_pb2.ListOperationsRequest] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/client.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1223,14 +1223,259 @@
             empty_pb2.Empty,
             metadata_type=operations.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
+    def execute_airflow_command(
+        self,
+        request: Optional[
+            Union[environments.ExecuteAirflowCommandRequest, dict]
+        ] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> environments.ExecuteAirflowCommandResponse:
+        r"""Executes Airflow CLI command.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1
+
+            def sample_execute_airflow_command():
+                # Create a client
+                client = service_v1.EnvironmentsClient()
+
+                # Initialize request argument(s)
+                request = service_v1.ExecuteAirflowCommandRequest(
+                )
+
+                # Make the request
+                response = client.execute_airflow_command(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.orchestration.airflow.service_v1.types.ExecuteAirflowCommandRequest, dict]):
+                The request object. Execute Airflow Command request.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.orchestration.airflow.service_v1.types.ExecuteAirflowCommandResponse:
+                Response to
+                ExecuteAirflowCommandRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Minor optimization to avoid making a copy if the user passes
+        # in a environments.ExecuteAirflowCommandRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, environments.ExecuteAirflowCommandRequest):
+            request = environments.ExecuteAirflowCommandRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.execute_airflow_command]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def stop_airflow_command(
+        self,
+        request: Optional[Union[environments.StopAirflowCommandRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> environments.StopAirflowCommandResponse:
+        r"""Stops Airflow CLI command execution.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1
+
+            def sample_stop_airflow_command():
+                # Create a client
+                client = service_v1.EnvironmentsClient()
+
+                # Initialize request argument(s)
+                request = service_v1.StopAirflowCommandRequest(
+                )
+
+                # Make the request
+                response = client.stop_airflow_command(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.orchestration.airflow.service_v1.types.StopAirflowCommandRequest, dict]):
+                The request object. Stop Airflow Command request.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.orchestration.airflow.service_v1.types.StopAirflowCommandResponse:
+                Response to
+                StopAirflowCommandRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Minor optimization to avoid making a copy if the user passes
+        # in a environments.StopAirflowCommandRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, environments.StopAirflowCommandRequest):
+            request = environments.StopAirflowCommandRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.stop_airflow_command]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def poll_airflow_command(
+        self,
+        request: Optional[Union[environments.PollAirflowCommandRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> environments.PollAirflowCommandResponse:
+        r"""Polls Airflow CLI command execution and fetches logs.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1
+
+            def sample_poll_airflow_command():
+                # Create a client
+                client = service_v1.EnvironmentsClient()
+
+                # Initialize request argument(s)
+                request = service_v1.PollAirflowCommandRequest(
+                )
+
+                # Make the request
+                response = client.poll_airflow_command(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.orchestration.airflow.service_v1.types.PollAirflowCommandRequest, dict]):
+                The request object. Poll Airflow Command request.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.orchestration.airflow.service_v1.types.PollAirflowCommandResponse:
+                Response to
+                PollAirflowCommandRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Minor optimization to avoid making a copy if the user passes
+        # in a environments.PollAirflowCommandRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, environments.PollAirflowCommandRequest):
+            request = environments.PollAirflowCommandRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.poll_airflow_command]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
     def save_snapshot(
         self,
         request: Optional[Union[environments.SaveSnapshotRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
@@ -1423,14 +1668,200 @@
             environments.LoadSnapshotResponse,
             metadata_type=operations.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
+    def database_failover(
+        self,
+        request: Optional[Union[environments.DatabaseFailoverRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation.Operation:
+        r"""Triggers database failover (only for highly resilient
+        environments).
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1
+
+            def sample_database_failover():
+                # Create a client
+                client = service_v1.EnvironmentsClient()
+
+                # Initialize request argument(s)
+                request = service_v1.DatabaseFailoverRequest(
+                )
+
+                # Make the request
+                operation = client.database_failover(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = operation.result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.orchestration.airflow.service_v1.types.DatabaseFailoverRequest, dict]):
+                The request object. Request to trigger database failover
+                (only for highly resilient
+                environments).
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation.Operation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be
+                :class:`google.cloud.orchestration.airflow.service_v1.types.DatabaseFailoverResponse`
+                Response for DatabaseFailoverRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Minor optimization to avoid making a copy if the user passes
+        # in a environments.DatabaseFailoverRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, environments.DatabaseFailoverRequest):
+            request = environments.DatabaseFailoverRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.database_failover]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation.from_gapic(
+            response,
+            self._transport.operations_client,
+            environments.DatabaseFailoverResponse,
+            metadata_type=operations.OperationMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def fetch_database_properties(
+        self,
+        request: Optional[
+            Union[environments.FetchDatabasePropertiesRequest, dict]
+        ] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> environments.FetchDatabasePropertiesResponse:
+        r"""Fetches database properties.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1
+
+            def sample_fetch_database_properties():
+                # Create a client
+                client = service_v1.EnvironmentsClient()
+
+                # Initialize request argument(s)
+                request = service_v1.FetchDatabasePropertiesRequest(
+                    environment="environment_value",
+                )
+
+                # Make the request
+                response = client.fetch_database_properties(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.orchestration.airflow.service_v1.types.FetchDatabasePropertiesRequest, dict]):
+                The request object. Request to fetch properties of
+                environment's database.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.orchestration.airflow.service_v1.types.FetchDatabasePropertiesResponse:
+                Response for
+                FetchDatabasePropertiesRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Minor optimization to avoid making a copy if the user passes
+        # in a environments.FetchDatabasePropertiesRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, environments.FetchDatabasePropertiesRequest):
+            request = environments.FetchDatabasePropertiesRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[
+            self._transport.fetch_database_properties
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
     def __enter__(self) -> "EnvironmentsClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/pagers.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/base.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,33 +14,33 @@
 # limitations under the License.
 #
 import abc
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Union
 
 import google.api_core
 from google.api_core import exceptions as core_exceptions
-from google.api_core import gapic_v1, operations_v1
+from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
-from google.longrunning import operations_pb2  # type: ignore
+from google.longrunning import operations_pb2
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.orchestration.airflow.service_v1 import (
     gapic_version as package_version,
 )
-from google.cloud.orchestration.airflow.service_v1.types import environments
+from google.cloud.orchestration.airflow.service_v1.types import image_versions
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
-class EnvironmentsTransport(abc.ABC):
-    """Abstract transport class for Environments."""
+class ImageVersionsTransport(abc.ABC):
+    """Abstract transport class for ImageVersions."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "composer.googleapis.com"
 
     def __init__(
         self,
@@ -121,46 +121,16 @@
         if ":" not in host:
             host += ":443"
         self._host = host
 
     def _prep_wrapped_messages(self, client_info):
         # Precompute the wrapped methods.
         self._wrapped_methods = {
-            self.create_environment: gapic_v1.method.wrap_method(
-                self.create_environment,
-                default_timeout=None,
-                client_info=client_info,
-            ),
-            self.get_environment: gapic_v1.method.wrap_method(
-                self.get_environment,
-                default_timeout=None,
-                client_info=client_info,
-            ),
-            self.list_environments: gapic_v1.method.wrap_method(
-                self.list_environments,
-                default_timeout=None,
-                client_info=client_info,
-            ),
-            self.update_environment: gapic_v1.method.wrap_method(
-                self.update_environment,
-                default_timeout=None,
-                client_info=client_info,
-            ),
-            self.delete_environment: gapic_v1.method.wrap_method(
-                self.delete_environment,
-                default_timeout=None,
-                client_info=client_info,
-            ),
-            self.save_snapshot: gapic_v1.method.wrap_method(
-                self.save_snapshot,
-                default_timeout=None,
-                client_info=client_info,
-            ),
-            self.load_snapshot: gapic_v1.method.wrap_method(
-                self.load_snapshot,
+            self.list_image_versions: gapic_v1.method.wrap_method(
+                self.list_image_versions,
                 default_timeout=None,
                 client_info=client_info,
             ),
         }
 
     def close(self):
         """Closes resources associated with the transport.
@@ -168,85 +138,26 @@
         .. warning::
              Only call this method if the transport is NOT shared
              with other clients - this may cause errors in other clients!
         """
         raise NotImplementedError()
 
     @property
-    def operations_client(self):
-        """Return the client designed to process long-running operations."""
-        raise NotImplementedError()
-
-    @property
-    def create_environment(
-        self,
-    ) -> Callable[
-        [environments.CreateEnvironmentRequest],
-        Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
-    ]:
-        raise NotImplementedError()
-
-    @property
-    def get_environment(
-        self,
-    ) -> Callable[
-        [environments.GetEnvironmentRequest],
-        Union[environments.Environment, Awaitable[environments.Environment]],
-    ]:
-        raise NotImplementedError()
-
-    @property
-    def list_environments(
+    def list_image_versions(
         self,
     ) -> Callable[
-        [environments.ListEnvironmentsRequest],
+        [image_versions.ListImageVersionsRequest],
         Union[
-            environments.ListEnvironmentsResponse,
-            Awaitable[environments.ListEnvironmentsResponse],
+            image_versions.ListImageVersionsResponse,
+            Awaitable[image_versions.ListImageVersionsResponse],
         ],
     ]:
         raise NotImplementedError()
 
     @property
-    def update_environment(
-        self,
-    ) -> Callable[
-        [environments.UpdateEnvironmentRequest],
-        Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
-    ]:
-        raise NotImplementedError()
-
-    @property
-    def delete_environment(
-        self,
-    ) -> Callable[
-        [environments.DeleteEnvironmentRequest],
-        Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
-    ]:
-        raise NotImplementedError()
-
-    @property
-    def save_snapshot(
-        self,
-    ) -> Callable[
-        [environments.SaveSnapshotRequest],
-        Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
-    ]:
-        raise NotImplementedError()
-
-    @property
-    def load_snapshot(
-        self,
-    ) -> Callable[
-        [environments.LoadSnapshotRequest],
-        Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
-    ]:
-        raise NotImplementedError()
-
-    @property
     def list_operations(
         self,
     ) -> Callable[
         [operations_pb2.ListOperationsRequest],
         Union[
             operations_pb2.ListOperationsResponse,
             Awaitable[operations_pb2.ListOperationsResponse],
@@ -270,8 +181,8 @@
         raise NotImplementedError()
 
     @property
     def kind(self) -> str:
         raise NotImplementedError()
 
 
-__all__ = ("EnvironmentsTransport",)
+__all__ = ("ImageVersionsTransport",)
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/grpc.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/grpc.py`

 * *Files 16% similar despite different names*

```diff
@@ -373,14 +373,101 @@
                 "/google.cloud.orchestration.airflow.service.v1.Environments/DeleteEnvironment",
                 request_serializer=environments.DeleteEnvironmentRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_environment"]
 
     @property
+    def execute_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.ExecuteAirflowCommandRequest],
+        environments.ExecuteAirflowCommandResponse,
+    ]:
+        r"""Return a callable for the execute airflow command method over gRPC.
+
+        Executes Airflow CLI command.
+
+        Returns:
+            Callable[[~.ExecuteAirflowCommandRequest],
+                    ~.ExecuteAirflowCommandResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "execute_airflow_command" not in self._stubs:
+            self._stubs["execute_airflow_command"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1.Environments/ExecuteAirflowCommand",
+                request_serializer=environments.ExecuteAirflowCommandRequest.serialize,
+                response_deserializer=environments.ExecuteAirflowCommandResponse.deserialize,
+            )
+        return self._stubs["execute_airflow_command"]
+
+    @property
+    def stop_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.StopAirflowCommandRequest],
+        environments.StopAirflowCommandResponse,
+    ]:
+        r"""Return a callable for the stop airflow command method over gRPC.
+
+        Stops Airflow CLI command execution.
+
+        Returns:
+            Callable[[~.StopAirflowCommandRequest],
+                    ~.StopAirflowCommandResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "stop_airflow_command" not in self._stubs:
+            self._stubs["stop_airflow_command"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1.Environments/StopAirflowCommand",
+                request_serializer=environments.StopAirflowCommandRequest.serialize,
+                response_deserializer=environments.StopAirflowCommandResponse.deserialize,
+            )
+        return self._stubs["stop_airflow_command"]
+
+    @property
+    def poll_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.PollAirflowCommandRequest],
+        environments.PollAirflowCommandResponse,
+    ]:
+        r"""Return a callable for the poll airflow command method over gRPC.
+
+        Polls Airflow CLI command execution and fetches logs.
+
+        Returns:
+            Callable[[~.PollAirflowCommandRequest],
+                    ~.PollAirflowCommandResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "poll_airflow_command" not in self._stubs:
+            self._stubs["poll_airflow_command"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1.Environments/PollAirflowCommand",
+                request_serializer=environments.PollAirflowCommandRequest.serialize,
+                response_deserializer=environments.PollAirflowCommandResponse.deserialize,
+            )
+        return self._stubs["poll_airflow_command"]
+
+    @property
     def save_snapshot(
         self,
     ) -> Callable[[environments.SaveSnapshotRequest], operations_pb2.Operation]:
         r"""Return a callable for the save snapshot method over gRPC.
 
         Creates a snapshots of a Cloud Composer environment.
         As a result of this operation, snapshot of environment's
@@ -430,14 +517,70 @@
             self._stubs["load_snapshot"] = self.grpc_channel.unary_unary(
                 "/google.cloud.orchestration.airflow.service.v1.Environments/LoadSnapshot",
                 request_serializer=environments.LoadSnapshotRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["load_snapshot"]
 
+    @property
+    def database_failover(
+        self,
+    ) -> Callable[[environments.DatabaseFailoverRequest], operations_pb2.Operation]:
+        r"""Return a callable for the database failover method over gRPC.
+
+        Triggers database failover (only for highly resilient
+        environments).
+
+        Returns:
+            Callable[[~.DatabaseFailoverRequest],
+                    ~.Operation]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "database_failover" not in self._stubs:
+            self._stubs["database_failover"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1.Environments/DatabaseFailover",
+                request_serializer=environments.DatabaseFailoverRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["database_failover"]
+
+    @property
+    def fetch_database_properties(
+        self,
+    ) -> Callable[
+        [environments.FetchDatabasePropertiesRequest],
+        environments.FetchDatabasePropertiesResponse,
+    ]:
+        r"""Return a callable for the fetch database properties method over gRPC.
+
+        Fetches database properties.
+
+        Returns:
+            Callable[[~.FetchDatabasePropertiesRequest],
+                    ~.FetchDatabasePropertiesResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "fetch_database_properties" not in self._stubs:
+            self._stubs["fetch_database_properties"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1.Environments/FetchDatabaseProperties",
+                request_serializer=environments.FetchDatabasePropertiesRequest.serialize,
+                response_deserializer=environments.FetchDatabasePropertiesResponse.deserialize,
+            )
+        return self._stubs["fetch_database_properties"]
+
     def close(self):
         self.grpc_channel.close()
 
     @property
     def delete_operation(
         self,
     ) -> Callable[[operations_pb2.DeleteOperationRequest], None]:
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/grpc_asyncio.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/grpc_asyncio.py`

 * *Files 17% similar despite different names*

```diff
@@ -387,14 +387,101 @@
                 "/google.cloud.orchestration.airflow.service.v1.Environments/DeleteEnvironment",
                 request_serializer=environments.DeleteEnvironmentRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_environment"]
 
     @property
+    def execute_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.ExecuteAirflowCommandRequest],
+        Awaitable[environments.ExecuteAirflowCommandResponse],
+    ]:
+        r"""Return a callable for the execute airflow command method over gRPC.
+
+        Executes Airflow CLI command.
+
+        Returns:
+            Callable[[~.ExecuteAirflowCommandRequest],
+                    Awaitable[~.ExecuteAirflowCommandResponse]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "execute_airflow_command" not in self._stubs:
+            self._stubs["execute_airflow_command"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1.Environments/ExecuteAirflowCommand",
+                request_serializer=environments.ExecuteAirflowCommandRequest.serialize,
+                response_deserializer=environments.ExecuteAirflowCommandResponse.deserialize,
+            )
+        return self._stubs["execute_airflow_command"]
+
+    @property
+    def stop_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.StopAirflowCommandRequest],
+        Awaitable[environments.StopAirflowCommandResponse],
+    ]:
+        r"""Return a callable for the stop airflow command method over gRPC.
+
+        Stops Airflow CLI command execution.
+
+        Returns:
+            Callable[[~.StopAirflowCommandRequest],
+                    Awaitable[~.StopAirflowCommandResponse]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "stop_airflow_command" not in self._stubs:
+            self._stubs["stop_airflow_command"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1.Environments/StopAirflowCommand",
+                request_serializer=environments.StopAirflowCommandRequest.serialize,
+                response_deserializer=environments.StopAirflowCommandResponse.deserialize,
+            )
+        return self._stubs["stop_airflow_command"]
+
+    @property
+    def poll_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.PollAirflowCommandRequest],
+        Awaitable[environments.PollAirflowCommandResponse],
+    ]:
+        r"""Return a callable for the poll airflow command method over gRPC.
+
+        Polls Airflow CLI command execution and fetches logs.
+
+        Returns:
+            Callable[[~.PollAirflowCommandRequest],
+                    Awaitable[~.PollAirflowCommandResponse]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "poll_airflow_command" not in self._stubs:
+            self._stubs["poll_airflow_command"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1.Environments/PollAirflowCommand",
+                request_serializer=environments.PollAirflowCommandRequest.serialize,
+                response_deserializer=environments.PollAirflowCommandResponse.deserialize,
+            )
+        return self._stubs["poll_airflow_command"]
+
+    @property
     def save_snapshot(
         self,
     ) -> Callable[
         [environments.SaveSnapshotRequest], Awaitable[operations_pb2.Operation]
     ]:
         r"""Return a callable for the save snapshot method over gRPC.
 
@@ -448,14 +535,72 @@
             self._stubs["load_snapshot"] = self.grpc_channel.unary_unary(
                 "/google.cloud.orchestration.airflow.service.v1.Environments/LoadSnapshot",
                 request_serializer=environments.LoadSnapshotRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["load_snapshot"]
 
+    @property
+    def database_failover(
+        self,
+    ) -> Callable[
+        [environments.DatabaseFailoverRequest], Awaitable[operations_pb2.Operation]
+    ]:
+        r"""Return a callable for the database failover method over gRPC.
+
+        Triggers database failover (only for highly resilient
+        environments).
+
+        Returns:
+            Callable[[~.DatabaseFailoverRequest],
+                    Awaitable[~.Operation]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "database_failover" not in self._stubs:
+            self._stubs["database_failover"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1.Environments/DatabaseFailover",
+                request_serializer=environments.DatabaseFailoverRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["database_failover"]
+
+    @property
+    def fetch_database_properties(
+        self,
+    ) -> Callable[
+        [environments.FetchDatabasePropertiesRequest],
+        Awaitable[environments.FetchDatabasePropertiesResponse],
+    ]:
+        r"""Return a callable for the fetch database properties method over gRPC.
+
+        Fetches database properties.
+
+        Returns:
+            Callable[[~.FetchDatabasePropertiesRequest],
+                    Awaitable[~.FetchDatabasePropertiesResponse]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "fetch_database_properties" not in self._stubs:
+            self._stubs["fetch_database_properties"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1.Environments/FetchDatabaseProperties",
+                request_serializer=environments.FetchDatabasePropertiesRequest.serialize,
+                response_deserializer=environments.FetchDatabasePropertiesResponse.deserialize,
+            )
+        return self._stubs["fetch_database_properties"]
+
     def close(self):
         return self.grpc_channel.close()
 
     @property
     def delete_operation(
         self,
     ) -> Callable[[operations_pb2.DeleteOperationRequest], None]:
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/rest.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/environments/transports/rest.py`

 * *Files 16% similar despite different names*

```diff
@@ -76,22 +76,46 @@
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_create_environment(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_database_failover(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_database_failover(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_delete_environment(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_delete_environment(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_execute_airflow_command(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_execute_airflow_command(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
+            def pre_fetch_database_properties(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_fetch_database_properties(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_get_environment(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_get_environment(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -108,22 +132,38 @@
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_load_snapshot(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_poll_airflow_command(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_poll_airflow_command(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_save_snapshot(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_save_snapshot(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_stop_airflow_command(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_stop_airflow_command(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_update_environment(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_update_environment(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -153,14 +193,37 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the Environments server but before
         it is returned to user code.
         """
         return response
 
+    def pre_database_failover(
+        self,
+        request: environments.DatabaseFailoverRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[environments.DatabaseFailoverRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for database_failover
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the Environments server.
+        """
+        return request, metadata
+
+    def post_database_failover(
+        self, response: operations_pb2.Operation
+    ) -> operations_pb2.Operation:
+        """Post-rpc interceptor for database_failover
+
+        Override in a subclass to manipulate the response
+        after it is returned by the Environments server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_delete_environment(
         self,
         request: environments.DeleteEnvironmentRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[environments.DeleteEnvironmentRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for delete_environment
 
@@ -176,14 +239,60 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the Environments server but before
         it is returned to user code.
         """
         return response
 
+    def pre_execute_airflow_command(
+        self,
+        request: environments.ExecuteAirflowCommandRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[environments.ExecuteAirflowCommandRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for execute_airflow_command
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the Environments server.
+        """
+        return request, metadata
+
+    def post_execute_airflow_command(
+        self, response: environments.ExecuteAirflowCommandResponse
+    ) -> environments.ExecuteAirflowCommandResponse:
+        """Post-rpc interceptor for execute_airflow_command
+
+        Override in a subclass to manipulate the response
+        after it is returned by the Environments server but before
+        it is returned to user code.
+        """
+        return response
+
+    def pre_fetch_database_properties(
+        self,
+        request: environments.FetchDatabasePropertiesRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[environments.FetchDatabasePropertiesRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for fetch_database_properties
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the Environments server.
+        """
+        return request, metadata
+
+    def post_fetch_database_properties(
+        self, response: environments.FetchDatabasePropertiesResponse
+    ) -> environments.FetchDatabasePropertiesResponse:
+        """Post-rpc interceptor for fetch_database_properties
+
+        Override in a subclass to manipulate the response
+        after it is returned by the Environments server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_get_environment(
         self,
         request: environments.GetEnvironmentRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[environments.GetEnvironmentRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for get_environment
 
@@ -245,14 +354,37 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the Environments server but before
         it is returned to user code.
         """
         return response
 
+    def pre_poll_airflow_command(
+        self,
+        request: environments.PollAirflowCommandRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[environments.PollAirflowCommandRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for poll_airflow_command
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the Environments server.
+        """
+        return request, metadata
+
+    def post_poll_airflow_command(
+        self, response: environments.PollAirflowCommandResponse
+    ) -> environments.PollAirflowCommandResponse:
+        """Post-rpc interceptor for poll_airflow_command
+
+        Override in a subclass to manipulate the response
+        after it is returned by the Environments server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_save_snapshot(
         self,
         request: environments.SaveSnapshotRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[environments.SaveSnapshotRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for save_snapshot
 
@@ -268,14 +400,37 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the Environments server but before
         it is returned to user code.
         """
         return response
 
+    def pre_stop_airflow_command(
+        self,
+        request: environments.StopAirflowCommandRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[environments.StopAirflowCommandRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for stop_airflow_command
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the Environments server.
+        """
+        return request, metadata
+
+    def post_stop_airflow_command(
+        self, response: environments.StopAirflowCommandResponse
+    ) -> environments.StopAirflowCommandResponse:
+        """Post-rpc interceptor for stop_airflow_command
+
+        Override in a subclass to manipulate the response
+        after it is returned by the Environments server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_update_environment(
         self,
         request: environments.UpdateEnvironmentRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[environments.UpdateEnvironmentRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for update_environment
 
@@ -589,14 +744,103 @@
 
             # Return the response
             resp = operations_pb2.Operation()
             json_format.Parse(response.content, resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_create_environment(resp)
             return resp
 
+    class _DatabaseFailover(EnvironmentsRestStub):
+        def __hash__(self):
+            return hash("DatabaseFailover")
+
+        def __call__(
+            self,
+            request: environments.DatabaseFailoverRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> operations_pb2.Operation:
+            r"""Call the database failover method over HTTP.
+
+            Args:
+                request (~.environments.DatabaseFailoverRequest):
+                    The request object. Request to trigger database failover
+                (only for highly resilient
+                environments).
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.operations_pb2.Operation:
+                    This resource represents a
+                long-running operation that is the
+                result of a network API call.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "post",
+                    "uri": "/v1/{environment=projects/*/locations/*/environments/*}:databaseFailover",
+                    "body": "*",
+                },
+            ]
+            request, metadata = self._interceptor.pre_database_failover(
+                request, metadata
+            )
+            pb_request = environments.DatabaseFailoverRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            # Jsonify the request body
+
+            body = json_format.MessageToJson(
+                transcoded_request["body"],
+                including_default_value_fields=False,
+                use_integers_for_enums=True,
+            )
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = operations_pb2.Operation()
+            json_format.Parse(response.content, resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_database_failover(resp)
+            return resp
+
     class _DeleteEnvironment(EnvironmentsRestStub):
         def __hash__(self):
             return hash("DeleteEnvironment")
 
         def __call__(
             self,
             request: environments.DeleteEnvironmentRequest,
@@ -667,14 +911,193 @@
 
             # Return the response
             resp = operations_pb2.Operation()
             json_format.Parse(response.content, resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_delete_environment(resp)
             return resp
 
+    class _ExecuteAirflowCommand(EnvironmentsRestStub):
+        def __hash__(self):
+            return hash("ExecuteAirflowCommand")
+
+        def __call__(
+            self,
+            request: environments.ExecuteAirflowCommandRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> environments.ExecuteAirflowCommandResponse:
+            r"""Call the execute airflow command method over HTTP.
+
+            Args:
+                request (~.environments.ExecuteAirflowCommandRequest):
+                    The request object. Execute Airflow Command request.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.environments.ExecuteAirflowCommandResponse:
+                    Response to
+                ExecuteAirflowCommandRequest.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "post",
+                    "uri": "/v1/{environment=projects/*/locations/*/environments/*}:executeAirflowCommand",
+                    "body": "*",
+                },
+            ]
+            request, metadata = self._interceptor.pre_execute_airflow_command(
+                request, metadata
+            )
+            pb_request = environments.ExecuteAirflowCommandRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            # Jsonify the request body
+
+            body = json_format.MessageToJson(
+                transcoded_request["body"],
+                including_default_value_fields=False,
+                use_integers_for_enums=True,
+            )
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = environments.ExecuteAirflowCommandResponse()
+            pb_resp = environments.ExecuteAirflowCommandResponse.pb(resp)
+
+            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_execute_airflow_command(resp)
+            return resp
+
+    class _FetchDatabaseProperties(EnvironmentsRestStub):
+        def __hash__(self):
+            return hash("FetchDatabaseProperties")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: environments.FetchDatabasePropertiesRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> environments.FetchDatabasePropertiesResponse:
+            r"""Call the fetch database properties method over HTTP.
+
+            Args:
+                request (~.environments.FetchDatabasePropertiesRequest):
+                    The request object. Request to fetch properties of
+                environment's database.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.environments.FetchDatabasePropertiesResponse:
+                    Response for
+                FetchDatabasePropertiesRequest.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1/{environment=projects/*/locations/*/environments/*}:fetchDatabaseProperties",
+                },
+            ]
+            request, metadata = self._interceptor.pre_fetch_database_properties(
+                request, metadata
+            )
+            pb_request = environments.FetchDatabasePropertiesRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = environments.FetchDatabasePropertiesResponse()
+            pb_resp = environments.FetchDatabasePropertiesResponse.pb(resp)
+
+            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_fetch_database_properties(resp)
+            return resp
+
     class _GetEnvironment(EnvironmentsRestStub):
         def __hash__(self):
             return hash("GetEnvironment")
 
         def __call__(
             self,
             request: environments.GetEnvironmentRequest,
@@ -910,14 +1333,102 @@
 
             # Return the response
             resp = operations_pb2.Operation()
             json_format.Parse(response.content, resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_load_snapshot(resp)
             return resp
 
+    class _PollAirflowCommand(EnvironmentsRestStub):
+        def __hash__(self):
+            return hash("PollAirflowCommand")
+
+        def __call__(
+            self,
+            request: environments.PollAirflowCommandRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> environments.PollAirflowCommandResponse:
+            r"""Call the poll airflow command method over HTTP.
+
+            Args:
+                request (~.environments.PollAirflowCommandRequest):
+                    The request object. Poll Airflow Command request.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.environments.PollAirflowCommandResponse:
+                    Response to
+                PollAirflowCommandRequest.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "post",
+                    "uri": "/v1/{environment=projects/*/locations/*/environments/*}:pollAirflowCommand",
+                    "body": "*",
+                },
+            ]
+            request, metadata = self._interceptor.pre_poll_airflow_command(
+                request, metadata
+            )
+            pb_request = environments.PollAirflowCommandRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            # Jsonify the request body
+
+            body = json_format.MessageToJson(
+                transcoded_request["body"],
+                including_default_value_fields=False,
+                use_integers_for_enums=True,
+            )
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = environments.PollAirflowCommandResponse()
+            pb_resp = environments.PollAirflowCommandResponse.pb(resp)
+
+            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_poll_airflow_command(resp)
+            return resp
+
     class _SaveSnapshot(EnvironmentsRestStub):
         def __hash__(self):
             return hash("SaveSnapshot")
 
         def __call__(
             self,
             request: environments.SaveSnapshotRequest,
@@ -996,14 +1507,102 @@
 
             # Return the response
             resp = operations_pb2.Operation()
             json_format.Parse(response.content, resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_save_snapshot(resp)
             return resp
 
+    class _StopAirflowCommand(EnvironmentsRestStub):
+        def __hash__(self):
+            return hash("StopAirflowCommand")
+
+        def __call__(
+            self,
+            request: environments.StopAirflowCommandRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> environments.StopAirflowCommandResponse:
+            r"""Call the stop airflow command method over HTTP.
+
+            Args:
+                request (~.environments.StopAirflowCommandRequest):
+                    The request object. Stop Airflow Command request.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.environments.StopAirflowCommandResponse:
+                    Response to
+                StopAirflowCommandRequest.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "post",
+                    "uri": "/v1/{environment=projects/*/locations/*/environments/*}:stopAirflowCommand",
+                    "body": "*",
+                },
+            ]
+            request, metadata = self._interceptor.pre_stop_airflow_command(
+                request, metadata
+            )
+            pb_request = environments.StopAirflowCommandRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            # Jsonify the request body
+
+            body = json_format.MessageToJson(
+                transcoded_request["body"],
+                including_default_value_fields=False,
+                use_integers_for_enums=True,
+            )
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = environments.StopAirflowCommandResponse()
+            pb_resp = environments.StopAirflowCommandResponse.pb(resp)
+
+            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_stop_airflow_command(resp)
+            return resp
+
     class _UpdateEnvironment(EnvironmentsRestStub):
         def __hash__(self):
             return hash("UpdateEnvironment")
 
         def __call__(
             self,
             request: environments.UpdateEnvironmentRequest,
@@ -1092,22 +1691,52 @@
         self,
     ) -> Callable[[environments.CreateEnvironmentRequest], operations_pb2.Operation]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._CreateEnvironment(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def database_failover(
+        self,
+    ) -> Callable[[environments.DatabaseFailoverRequest], operations_pb2.Operation]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._DatabaseFailover(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def delete_environment(
         self,
     ) -> Callable[[environments.DeleteEnvironmentRequest], operations_pb2.Operation]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._DeleteEnvironment(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def execute_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.ExecuteAirflowCommandRequest],
+        environments.ExecuteAirflowCommandResponse,
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._ExecuteAirflowCommand(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
+    def fetch_database_properties(
+        self,
+    ) -> Callable[
+        [environments.FetchDatabasePropertiesRequest],
+        environments.FetchDatabasePropertiesResponse,
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._FetchDatabaseProperties(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def get_environment(
         self,
     ) -> Callable[[environments.GetEnvironmentRequest], environments.Environment]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._GetEnvironment(self._session, self._host, self._interceptor)  # type: ignore
 
@@ -1126,22 +1755,44 @@
         self,
     ) -> Callable[[environments.LoadSnapshotRequest], operations_pb2.Operation]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._LoadSnapshot(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def poll_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.PollAirflowCommandRequest],
+        environments.PollAirflowCommandResponse,
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._PollAirflowCommand(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def save_snapshot(
         self,
     ) -> Callable[[environments.SaveSnapshotRequest], operations_pb2.Operation]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._SaveSnapshot(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def stop_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.StopAirflowCommandRequest],
+        environments.StopAirflowCommandResponse,
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._StopAirflowCommand(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def update_environment(
         self,
     ) -> Callable[[environments.UpdateEnvironmentRequest], operations_pb2.Operation]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._UpdateEnvironment(self._session, self._host, self._interceptor)  # type: ignore
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/async_client.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/client.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/pagers.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/base.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.longrunning import operations_pb2
 from google.oauth2 import service_account  # type: ignore
 
-from google.cloud.orchestration.airflow.service_v1 import (
+from google.cloud.orchestration.airflow.service_v1beta1 import (
     gapic_version as package_version,
 )
-from google.cloud.orchestration.airflow.service_v1.types import image_versions
+from google.cloud.orchestration.airflow.service_v1beta1.types import image_versions
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 class ImageVersionsTransport(abc.ABC):
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/grpc.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/grpc_asyncio.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/rest.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/services/image_versions/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,78 +9,117 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from .environments import (
+from google.cloud.orchestration.airflow.service_v1beta1 import (
+    gapic_version as package_version,
+)
+
+__version__ = package_version.__version__
+
+
+from .services.environments import EnvironmentsAsyncClient, EnvironmentsClient
+from .services.image_versions import ImageVersionsAsyncClient, ImageVersionsClient
+from .types.environments import (
+    CheckUpgradeRequest,
     CheckUpgradeResponse,
+    CloudDataLineageIntegration,
     CreateEnvironmentRequest,
     DatabaseConfig,
+    DatabaseFailoverRequest,
+    DatabaseFailoverResponse,
     DeleteEnvironmentRequest,
     EncryptionConfig,
     Environment,
     EnvironmentConfig,
+    ExecuteAirflowCommandRequest,
+    ExecuteAirflowCommandResponse,
+    FetchDatabasePropertiesRequest,
+    FetchDatabasePropertiesResponse,
     GetEnvironmentRequest,
     IPAllocationPolicy,
     ListEnvironmentsRequest,
     ListEnvironmentsResponse,
     LoadSnapshotRequest,
     LoadSnapshotResponse,
     MaintenanceWindow,
     MasterAuthorizedNetworksConfig,
     NetworkingConfig,
     NodeConfig,
+    PollAirflowCommandRequest,
+    PollAirflowCommandResponse,
     PrivateClusterConfig,
     PrivateEnvironmentConfig,
     RecoveryConfig,
+    RestartWebServerRequest,
     SaveSnapshotRequest,
     SaveSnapshotResponse,
     ScheduledSnapshotsConfig,
     SoftwareConfig,
+    StopAirflowCommandRequest,
+    StopAirflowCommandResponse,
     UpdateEnvironmentRequest,
     WebServerConfig,
     WebServerNetworkAccessControl,
     WorkloadsConfig,
 )
-from .image_versions import (
+from .types.image_versions import (
     ImageVersion,
     ListImageVersionsRequest,
     ListImageVersionsResponse,
 )
-from .operations import OperationMetadata
+from .types.operations import OperationMetadata
 
 __all__ = (
+    "EnvironmentsAsyncClient",
+    "ImageVersionsAsyncClient",
+    "CheckUpgradeRequest",
     "CheckUpgradeResponse",
+    "CloudDataLineageIntegration",
     "CreateEnvironmentRequest",
     "DatabaseConfig",
+    "DatabaseFailoverRequest",
+    "DatabaseFailoverResponse",
     "DeleteEnvironmentRequest",
     "EncryptionConfig",
     "Environment",
     "EnvironmentConfig",
+    "EnvironmentsClient",
+    "ExecuteAirflowCommandRequest",
+    "ExecuteAirflowCommandResponse",
+    "FetchDatabasePropertiesRequest",
+    "FetchDatabasePropertiesResponse",
     "GetEnvironmentRequest",
     "IPAllocationPolicy",
+    "ImageVersion",
+    "ImageVersionsClient",
     "ListEnvironmentsRequest",
     "ListEnvironmentsResponse",
+    "ListImageVersionsRequest",
+    "ListImageVersionsResponse",
     "LoadSnapshotRequest",
     "LoadSnapshotResponse",
     "MaintenanceWindow",
     "MasterAuthorizedNetworksConfig",
     "NetworkingConfig",
     "NodeConfig",
+    "OperationMetadata",
+    "PollAirflowCommandRequest",
+    "PollAirflowCommandResponse",
     "PrivateClusterConfig",
     "PrivateEnvironmentConfig",
     "RecoveryConfig",
+    "RestartWebServerRequest",
     "SaveSnapshotRequest",
     "SaveSnapshotResponse",
     "ScheduledSnapshotsConfig",
     "SoftwareConfig",
+    "StopAirflowCommandRequest",
+    "StopAirflowCommandResponse",
     "UpdateEnvironmentRequest",
     "WebServerConfig",
     "WebServerNetworkAccessControl",
     "WorkloadsConfig",
-    "ImageVersion",
-    "ListImageVersionsRequest",
-    "ListImageVersionsResponse",
-    "OperationMetadata",
 )
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/environments.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/types/environments.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,18 +26,28 @@
     manifest={
         "CreateEnvironmentRequest",
         "GetEnvironmentRequest",
         "ListEnvironmentsRequest",
         "ListEnvironmentsResponse",
         "DeleteEnvironmentRequest",
         "UpdateEnvironmentRequest",
+        "ExecuteAirflowCommandRequest",
+        "ExecuteAirflowCommandResponse",
+        "StopAirflowCommandRequest",
+        "StopAirflowCommandResponse",
+        "PollAirflowCommandRequest",
+        "PollAirflowCommandResponse",
         "SaveSnapshotRequest",
         "SaveSnapshotResponse",
         "LoadSnapshotRequest",
         "LoadSnapshotResponse",
+        "DatabaseFailoverRequest",
+        "DatabaseFailoverResponse",
+        "FetchDatabasePropertiesRequest",
+        "FetchDatabasePropertiesResponse",
         "EnvironmentConfig",
         "WebServerNetworkAccessControl",
         "DatabaseConfig",
         "WebServerConfig",
         "EncryptionConfig",
         "MaintenanceWindow",
         "SoftwareConfig",
@@ -360,14 +370,264 @@
     update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=3,
         message=field_mask_pb2.FieldMask,
     )
 
 
+class ExecuteAirflowCommandRequest(proto.Message):
+    r"""Execute Airflow Command request.
+
+    Attributes:
+        environment (str):
+            The resource name of the environment in the
+            form:
+            "projects/{projectId}/locations/{locationId}/environments/{environmentId}".
+        command (str):
+            Airflow command.
+        subcommand (str):
+            Airflow subcommand.
+        parameters (MutableSequence[str]):
+            Parameters for the Airflow command/subcommand as an array of
+            arguments. It may contain positional arguments like
+            ``["my-dag-id"]``, key-value parameters like
+            ``["--foo=bar"]`` or ``["--foo","bar"]``, or other flags
+            like ``["-f"]``.
+    """
+
+    environment: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    command: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    subcommand: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    parameters: MutableSequence[str] = proto.RepeatedField(
+        proto.STRING,
+        number=4,
+    )
+
+
+class ExecuteAirflowCommandResponse(proto.Message):
+    r"""Response to ExecuteAirflowCommandRequest.
+
+    Attributes:
+        execution_id (str):
+            The unique ID of the command execution for
+            polling.
+        pod (str):
+            The name of the pod where the command is
+            executed.
+        pod_namespace (str):
+            The namespace of the pod where the command is
+            executed.
+        error (str):
+            Error message. Empty if there was no error.
+    """
+
+    execution_id: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    pod: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    pod_namespace: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    error: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+
+
+class StopAirflowCommandRequest(proto.Message):
+    r"""Stop Airflow Command request.
+
+    Attributes:
+        environment (str):
+            The resource name of the environment in the
+            form:
+            "projects/{projectId}/locations/{locationId}/environments/{environmentId}".
+        execution_id (str):
+            The unique ID of the command execution.
+        pod (str):
+            The name of the pod where the command is
+            executed.
+        pod_namespace (str):
+            The namespace of the pod where the command is
+            executed.
+        force (bool):
+            If true, the execution is terminated
+            forcefully (SIGKILL). If false, the execution is
+            stopped gracefully, giving it time for cleanup.
+    """
+
+    environment: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    execution_id: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    pod: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    pod_namespace: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    force: bool = proto.Field(
+        proto.BOOL,
+        number=5,
+    )
+
+
+class StopAirflowCommandResponse(proto.Message):
+    r"""Response to StopAirflowCommandRequest.
+
+    Attributes:
+        is_done (bool):
+            Whether the execution is still running.
+        output (MutableSequence[str]):
+            Output message from stopping execution
+            request.
+    """
+
+    is_done: bool = proto.Field(
+        proto.BOOL,
+        number=1,
+    )
+    output: MutableSequence[str] = proto.RepeatedField(
+        proto.STRING,
+        number=2,
+    )
+
+
+class PollAirflowCommandRequest(proto.Message):
+    r"""Poll Airflow Command request.
+
+    Attributes:
+        environment (str):
+            The resource name of the environment in the
+            form:
+            "projects/{projectId}/locations/{locationId}/environments/{environmentId}".
+        execution_id (str):
+            The unique ID of the command execution.
+        pod (str):
+            The name of the pod where the command is
+            executed.
+        pod_namespace (str):
+            The namespace of the pod where the command is
+            executed.
+        next_line_number (int):
+            Line number from which new logs should be
+            fetched.
+    """
+
+    environment: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    execution_id: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    pod: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    pod_namespace: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    next_line_number: int = proto.Field(
+        proto.INT32,
+        number=5,
+    )
+
+
+class PollAirflowCommandResponse(proto.Message):
+    r"""Response to PollAirflowCommandRequest.
+
+    Attributes:
+        output (MutableSequence[google.cloud.orchestration.airflow.service_v1.types.PollAirflowCommandResponse.Line]):
+            Output from the command execution. It may not
+            contain the full output and the caller may need
+            to poll for more lines.
+        output_end (bool):
+            Whether the command execution has finished
+            and there is no more output.
+        exit_info (google.cloud.orchestration.airflow.service_v1.types.PollAirflowCommandResponse.ExitInfo):
+            The result exit status of the command.
+    """
+
+    class Line(proto.Message):
+        r"""Contains information about a single line from logs.
+
+        Attributes:
+            line_number (int):
+                Number of the line.
+            content (str):
+                Text content of the log line.
+        """
+
+        line_number: int = proto.Field(
+            proto.INT32,
+            number=1,
+        )
+        content: str = proto.Field(
+            proto.STRING,
+            number=2,
+        )
+
+    class ExitInfo(proto.Message):
+        r"""Information about how a command ended.
+
+        Attributes:
+            exit_code (int):
+                The exit code from the command execution.
+            error (str):
+                Error message. Empty if there was no error.
+        """
+
+        exit_code: int = proto.Field(
+            proto.INT32,
+            number=1,
+        )
+        error: str = proto.Field(
+            proto.STRING,
+            number=2,
+        )
+
+    output: MutableSequence[Line] = proto.RepeatedField(
+        proto.MESSAGE,
+        number=1,
+        message=Line,
+    )
+    output_end: bool = proto.Field(
+        proto.BOOL,
+        number=2,
+    )
+    exit_info: ExitInfo = proto.Field(
+        proto.MESSAGE,
+        number=3,
+        message=ExitInfo,
+    )
+
+
 class SaveSnapshotRequest(proto.Message):
     r"""Request to create a snapshot of a Cloud Composer environment.
 
     Attributes:
         environment (str):
             The resource name of the source environment
             in the form:
@@ -457,14 +717,83 @@
     )
 
 
 class LoadSnapshotResponse(proto.Message):
     r"""Response to LoadSnapshotRequest."""
 
 
+class DatabaseFailoverRequest(proto.Message):
+    r"""Request to trigger database failover (only for highly
+    resilient environments).
+
+    Attributes:
+        environment (str):
+            Target environment:
+            "projects/{projectId}/locations/{locationId}/environments/{environmentId}".
+    """
+
+    environment: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+
+
+class DatabaseFailoverResponse(proto.Message):
+    r"""Response for DatabaseFailoverRequest."""
+
+
+class FetchDatabasePropertiesRequest(proto.Message):
+    r"""Request to fetch properties of environment's database.
+
+    Attributes:
+        environment (str):
+            Required. The resource name of the
+            environment, in the form:
+            "projects/{projectId}/locations/{locationId}/environments/{environmentId}".
+    """
+
+    environment: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+
+
+class FetchDatabasePropertiesResponse(proto.Message):
+    r"""Response for FetchDatabasePropertiesRequest.
+
+    Attributes:
+        primary_gce_zone (str):
+            The Compute Engine zone that the instance is
+            currently serving from.
+        secondary_gce_zone (str):
+            The Compute Engine zone that the failover
+            instance is currently serving from for a
+            regional Cloud SQL instance.
+        is_failover_replica_available (bool):
+            The availability status of the failover
+            replica. A false status indicates that the
+            failover replica is out of sync. The primary
+            instance can only fail over to the failover
+            replica when the status is true.
+    """
+
+    primary_gce_zone: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    secondary_gce_zone: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    is_failover_replica_available: bool = proto.Field(
+        proto.BOOL,
+        number=3,
+    )
+
+
 class EnvironmentConfig(proto.Message):
     r"""Configuration information for an environment.
 
     Attributes:
         gke_cluster (str):
             Output only. The Kubernetes Engine cluster
             used to run this environment.
@@ -559,14 +888,19 @@
             - in case of public environment: disabled.
         recovery_config (google.cloud.orchestration.airflow.service_v1.types.RecoveryConfig):
             Optional. The Recovery settings configuration of an
             environment.
 
             This field is supported for Cloud Composer environments in
             versions composer-2.\ *.*-airflow-*.*.\* and newer.
+        resilience_mode (google.cloud.orchestration.airflow.service_v1.types.EnvironmentConfig.ResilienceMode):
+            Optional. Resilience mode of the Cloud Composer Environment.
+
+            This field is supported for Cloud Composer environments in
+            versions composer-2.2.0-airflow-\ *.*.\* and newer.
     """
 
     class EnvironmentSize(proto.Enum):
         r"""The size of the Cloud Composer environment.
 
         Values:
             ENVIRONMENT_SIZE_UNSPECIFIED (0):
@@ -579,14 +913,28 @@
                 The environment size is large.
         """
         ENVIRONMENT_SIZE_UNSPECIFIED = 0
         ENVIRONMENT_SIZE_SMALL = 1
         ENVIRONMENT_SIZE_MEDIUM = 2
         ENVIRONMENT_SIZE_LARGE = 3
 
+    class ResilienceMode(proto.Enum):
+        r"""Resilience mode of the Cloud Composer Environment.
+
+        Values:
+            RESILIENCE_MODE_UNSPECIFIED (0):
+                Default mode doesn't change environment
+                parameters.
+            HIGH_RESILIENCE (1):
+                Enabled High Resilience mode, including Cloud
+                SQL HA.
+        """
+        RESILIENCE_MODE_UNSPECIFIED = 0
+        HIGH_RESILIENCE = 1
+
     gke_cluster: str = proto.Field(
         proto.STRING,
         number=1,
     )
     dag_gcs_prefix: str = proto.Field(
         proto.STRING,
         number=2,
@@ -659,14 +1007,19 @@
         message="MasterAuthorizedNetworksConfig",
     )
     recovery_config: "RecoveryConfig" = proto.Field(
         proto.MESSAGE,
         number=18,
         message="RecoveryConfig",
     )
+    resilience_mode: ResilienceMode = proto.Field(
+        proto.ENUM,
+        number=19,
+        enum=ResilienceMode,
+    )
 
 
 class WebServerNetworkAccessControl(proto.Message):
     r"""Network-level access control policy for the Airflow web
     server.
 
     Attributes:
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/image_versions.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/types/image_versions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1/types/operations.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/types/operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.cloud.orchestration.airflow.service.v1",
+    package="google.cloud.orchestration.airflow.service.v1beta1",
     manifest={
         "OperationMetadata",
     },
 )
 
 
 class OperationMetadata(proto.Message):
     r"""Metadata describing an operation.
 
     Attributes:
-        state (google.cloud.orchestration.airflow.service_v1.types.OperationMetadata.State):
+        state (google.cloud.orchestration.airflow.service_v1beta1.types.OperationMetadata.State):
             Output only. The current operation state.
-        operation_type (google.cloud.orchestration.airflow.service_v1.types.OperationMetadata.Type):
+        operation_type (google.cloud.orchestration.airflow.service_v1beta1.types.OperationMetadata.Type):
             Output only. The type of operation being
             performed.
         resource (str):
             Output only. The resource being operated on, as a `relative
             resource
             name </apis/design/resource_names#relative_resource_name>`__.
         resource_uuid (str):
@@ -61,27 +61,23 @@
             STATE_UNSPECIFIED (0):
                 Unused.
             PENDING (1):
                 The operation has been created but is not yet
                 started.
             RUNNING (2):
                 The operation is underway.
-            SUCCEEDED (3):
-                The operation completed successfully.
             SUCCESSFUL (3):
-                No description available.
+                The operation completed successfully.
             FAILED (4):
                 The operation is no longer running but did
                 not succeed.
         """
-        _pb_options = {"allow_alias": True}
         STATE_UNSPECIFIED = 0
         PENDING = 1
         RUNNING = 2
-        SUCCEEDED = 3
         SUCCESSFUL = 3
         FAILED = 4
 
     class Type(proto.Enum):
         r"""Type of longrunning operation.
 
         Values:
@@ -95,22 +91,27 @@
                 A resource update operation.
             CHECK (4):
                 A resource check operation.
             SAVE_SNAPSHOT (5):
                 Saves snapshot of the resource operation.
             LOAD_SNAPSHOT (6):
                 Loads snapshot of the resource operation.
+            DATABASE_FAILOVER (7):
+                Triggers failover of environment's Cloud SQL
+                instance (only for highly resilient
+                environments).
         """
         TYPE_UNSPECIFIED = 0
         CREATE = 1
         DELETE = 2
         UPDATE = 3
         CHECK = 4
         SAVE_SNAPSHOT = 5
         LOAD_SNAPSHOT = 6
+        DATABASE_FAILOVER = 7
 
     state: State = proto.Field(
         proto.ENUM,
         number=1,
         enum=State,
     )
     operation_type: Type = proto.Field(
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/types/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,101 +9,104 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.orchestration.airflow.service_v1beta1 import (
-    gapic_version as package_version,
-)
-
-__version__ = package_version.__version__
-
-
-from .services.environments import EnvironmentsAsyncClient, EnvironmentsClient
-from .services.image_versions import ImageVersionsAsyncClient, ImageVersionsClient
-from .types.environments import (
+from .environments import (
     CheckUpgradeRequest,
     CheckUpgradeResponse,
     CloudDataLineageIntegration,
     CreateEnvironmentRequest,
     DatabaseConfig,
+    DatabaseFailoverRequest,
+    DatabaseFailoverResponse,
     DeleteEnvironmentRequest,
     EncryptionConfig,
     Environment,
     EnvironmentConfig,
+    ExecuteAirflowCommandRequest,
     ExecuteAirflowCommandResponse,
+    FetchDatabasePropertiesRequest,
+    FetchDatabasePropertiesResponse,
     GetEnvironmentRequest,
     IPAllocationPolicy,
     ListEnvironmentsRequest,
     ListEnvironmentsResponse,
     LoadSnapshotRequest,
     LoadSnapshotResponse,
     MaintenanceWindow,
     MasterAuthorizedNetworksConfig,
     NetworkingConfig,
     NodeConfig,
+    PollAirflowCommandRequest,
     PollAirflowCommandResponse,
     PrivateClusterConfig,
     PrivateEnvironmentConfig,
     RecoveryConfig,
     RestartWebServerRequest,
     SaveSnapshotRequest,
     SaveSnapshotResponse,
     ScheduledSnapshotsConfig,
     SoftwareConfig,
+    StopAirflowCommandRequest,
+    StopAirflowCommandResponse,
     UpdateEnvironmentRequest,
     WebServerConfig,
     WebServerNetworkAccessControl,
     WorkloadsConfig,
 )
-from .types.image_versions import (
+from .image_versions import (
     ImageVersion,
     ListImageVersionsRequest,
     ListImageVersionsResponse,
 )
-from .types.operations import OperationMetadata
+from .operations import OperationMetadata
 
 __all__ = (
-    "EnvironmentsAsyncClient",
-    "ImageVersionsAsyncClient",
     "CheckUpgradeRequest",
     "CheckUpgradeResponse",
     "CloudDataLineageIntegration",
     "CreateEnvironmentRequest",
     "DatabaseConfig",
+    "DatabaseFailoverRequest",
+    "DatabaseFailoverResponse",
     "DeleteEnvironmentRequest",
     "EncryptionConfig",
     "Environment",
     "EnvironmentConfig",
-    "EnvironmentsClient",
+    "ExecuteAirflowCommandRequest",
     "ExecuteAirflowCommandResponse",
+    "FetchDatabasePropertiesRequest",
+    "FetchDatabasePropertiesResponse",
     "GetEnvironmentRequest",
     "IPAllocationPolicy",
-    "ImageVersion",
-    "ImageVersionsClient",
     "ListEnvironmentsRequest",
     "ListEnvironmentsResponse",
-    "ListImageVersionsRequest",
-    "ListImageVersionsResponse",
     "LoadSnapshotRequest",
     "LoadSnapshotResponse",
     "MaintenanceWindow",
     "MasterAuthorizedNetworksConfig",
     "NetworkingConfig",
     "NodeConfig",
-    "OperationMetadata",
+    "PollAirflowCommandRequest",
     "PollAirflowCommandResponse",
     "PrivateClusterConfig",
     "PrivateEnvironmentConfig",
     "RecoveryConfig",
     "RestartWebServerRequest",
     "SaveSnapshotRequest",
     "SaveSnapshotResponse",
     "ScheduledSnapshotsConfig",
     "SoftwareConfig",
+    "StopAirflowCommandRequest",
+    "StopAirflowCommandResponse",
     "UpdateEnvironmentRequest",
     "WebServerConfig",
     "WebServerNetworkAccessControl",
     "WorkloadsConfig",
+    "ImageVersion",
+    "ListImageVersionsRequest",
+    "ListImageVersionsResponse",
+    "OperationMetadata",
 )
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/gapic_metadata.json` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/gapic_metadata.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8326822916666666%*

 * *Differences: {"'libraryPackage'": "'google.cloud.orchestration.airflow.service_v1'",*

 * * "'protoPackage'": "'google.cloud.orchestration.airflow.service.v1'",*

 * * "'services'": "{'Environments': {'clients': {'grpc': {'rpcs': {'DatabaseFailover': "*

 * *               "OrderedDict([('methods', ['database_failover'])]), 'ExecuteAirflowCommand': "*

 * *               "OrderedDict([('methods', ['execute_airflow_command'])]), "*

 * *               "'FetchDatabaseProperties': OrderedDict([('methods', "*

 * *               "['fetch_database_properties'] […]*

```diff
@@ -1,34 +1,44 @@
 {
     "comment": "This file maps proto services/RPCs to the corresponding library clients/methods",
     "language": "python",
-    "libraryPackage": "google.cloud.orchestration.airflow.service_v1beta1",
-    "protoPackage": "google.cloud.orchestration.airflow.service.v1beta1",
+    "libraryPackage": "google.cloud.orchestration.airflow.service_v1",
+    "protoPackage": "google.cloud.orchestration.airflow.service.v1",
     "schema": "1.0",
     "services": {
         "Environments": {
             "clients": {
                 "grpc": {
                     "libraryClient": "EnvironmentsClient",
                     "rpcs": {
-                        "CheckUpgrade": {
+                        "CreateEnvironment": {
                             "methods": [
-                                "check_upgrade"
+                                "create_environment"
                             ]
                         },
-                        "CreateEnvironment": {
+                        "DatabaseFailover": {
                             "methods": [
-                                "create_environment"
+                                "database_failover"
                             ]
                         },
                         "DeleteEnvironment": {
                             "methods": [
                                 "delete_environment"
                             ]
                         },
+                        "ExecuteAirflowCommand": {
+                            "methods": [
+                                "execute_airflow_command"
+                            ]
+                        },
+                        "FetchDatabaseProperties": {
+                            "methods": [
+                                "fetch_database_properties"
+                            ]
+                        },
                         "GetEnvironment": {
                             "methods": [
                                 "get_environment"
                             ]
                         },
                         "ListEnvironments": {
                             "methods": [
@@ -36,49 +46,64 @@
                             ]
                         },
                         "LoadSnapshot": {
                             "methods": [
                                 "load_snapshot"
                             ]
                         },
-                        "RestartWebServer": {
+                        "PollAirflowCommand": {
                             "methods": [
-                                "restart_web_server"
+                                "poll_airflow_command"
                             ]
                         },
                         "SaveSnapshot": {
                             "methods": [
                                 "save_snapshot"
                             ]
                         },
+                        "StopAirflowCommand": {
+                            "methods": [
+                                "stop_airflow_command"
+                            ]
+                        },
                         "UpdateEnvironment": {
                             "methods": [
                                 "update_environment"
                             ]
                         }
                     }
                 },
                 "grpc-async": {
                     "libraryClient": "EnvironmentsAsyncClient",
                     "rpcs": {
-                        "CheckUpgrade": {
+                        "CreateEnvironment": {
                             "methods": [
-                                "check_upgrade"
+                                "create_environment"
                             ]
                         },
-                        "CreateEnvironment": {
+                        "DatabaseFailover": {
                             "methods": [
-                                "create_environment"
+                                "database_failover"
                             ]
                         },
                         "DeleteEnvironment": {
                             "methods": [
                                 "delete_environment"
                             ]
                         },
+                        "ExecuteAirflowCommand": {
+                            "methods": [
+                                "execute_airflow_command"
+                            ]
+                        },
+                        "FetchDatabaseProperties": {
+                            "methods": [
+                                "fetch_database_properties"
+                            ]
+                        },
                         "GetEnvironment": {
                             "methods": [
                                 "get_environment"
                             ]
                         },
                         "ListEnvironments": {
                             "methods": [
@@ -86,49 +111,64 @@
                             ]
                         },
                         "LoadSnapshot": {
                             "methods": [
                                 "load_snapshot"
                             ]
                         },
-                        "RestartWebServer": {
+                        "PollAirflowCommand": {
                             "methods": [
-                                "restart_web_server"
+                                "poll_airflow_command"
                             ]
                         },
                         "SaveSnapshot": {
                             "methods": [
                                 "save_snapshot"
                             ]
                         },
+                        "StopAirflowCommand": {
+                            "methods": [
+                                "stop_airflow_command"
+                            ]
+                        },
                         "UpdateEnvironment": {
                             "methods": [
                                 "update_environment"
                             ]
                         }
                     }
                 },
                 "rest": {
                     "libraryClient": "EnvironmentsClient",
                     "rpcs": {
-                        "CheckUpgrade": {
+                        "CreateEnvironment": {
                             "methods": [
-                                "check_upgrade"
+                                "create_environment"
                             ]
                         },
-                        "CreateEnvironment": {
+                        "DatabaseFailover": {
                             "methods": [
-                                "create_environment"
+                                "database_failover"
                             ]
                         },
                         "DeleteEnvironment": {
                             "methods": [
                                 "delete_environment"
                             ]
                         },
+                        "ExecuteAirflowCommand": {
+                            "methods": [
+                                "execute_airflow_command"
+                            ]
+                        },
+                        "FetchDatabaseProperties": {
+                            "methods": [
+                                "fetch_database_properties"
+                            ]
+                        },
                         "GetEnvironment": {
                             "methods": [
                                 "get_environment"
                             ]
                         },
                         "ListEnvironments": {
                             "methods": [
@@ -136,24 +176,29 @@
                             ]
                         },
                         "LoadSnapshot": {
                             "methods": [
                                 "load_snapshot"
                             ]
                         },
-                        "RestartWebServer": {
+                        "PollAirflowCommand": {
                             "methods": [
-                                "restart_web_server"
+                                "poll_airflow_command"
                             ]
                         },
                         "SaveSnapshot": {
                             "methods": [
                                 "save_snapshot"
                             ]
                         },
+                        "StopAirflowCommand": {
+                            "methods": [
+                                "stop_airflow_command"
+                            ]
+                        },
                         "UpdateEnvironment": {
                             "methods": [
                                 "update_environment"
                             ]
                         }
                     }
                 }
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/gapic_version.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.0"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/async_client.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/async_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1223,14 +1223,256 @@
             environments.CheckUpgradeResponse,
             metadata_type=operations.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
+    async def execute_airflow_command(
+        self,
+        request: Optional[
+            Union[environments.ExecuteAirflowCommandRequest, dict]
+        ] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> environments.ExecuteAirflowCommandResponse:
+        r"""Executes Airflow CLI command.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1beta1
+
+            async def sample_execute_airflow_command():
+                # Create a client
+                client = service_v1beta1.EnvironmentsAsyncClient()
+
+                # Initialize request argument(s)
+                request = service_v1beta1.ExecuteAirflowCommandRequest(
+                )
+
+                # Make the request
+                response = await client.execute_airflow_command(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.orchestration.airflow.service_v1beta1.types.ExecuteAirflowCommandRequest, dict]]):
+                The request object. Execute Airflow Command request.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.orchestration.airflow.service_v1beta1.types.ExecuteAirflowCommandResponse:
+                Response to
+                ExecuteAirflowCommandRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        request = environments.ExecuteAirflowCommandRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.execute_airflow_command,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def stop_airflow_command(
+        self,
+        request: Optional[Union[environments.StopAirflowCommandRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> environments.StopAirflowCommandResponse:
+        r"""Stops Airflow CLI command execution.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1beta1
+
+            async def sample_stop_airflow_command():
+                # Create a client
+                client = service_v1beta1.EnvironmentsAsyncClient()
+
+                # Initialize request argument(s)
+                request = service_v1beta1.StopAirflowCommandRequest(
+                )
+
+                # Make the request
+                response = await client.stop_airflow_command(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.orchestration.airflow.service_v1beta1.types.StopAirflowCommandRequest, dict]]):
+                The request object. Stop Airflow Command request.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.orchestration.airflow.service_v1beta1.types.StopAirflowCommandResponse:
+                Response to
+                StopAirflowCommandRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        request = environments.StopAirflowCommandRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.stop_airflow_command,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def poll_airflow_command(
+        self,
+        request: Optional[Union[environments.PollAirflowCommandRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> environments.PollAirflowCommandResponse:
+        r"""Polls Airflow CLI command execution and fetches logs.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1beta1
+
+            async def sample_poll_airflow_command():
+                # Create a client
+                client = service_v1beta1.EnvironmentsAsyncClient()
+
+                # Initialize request argument(s)
+                request = service_v1beta1.PollAirflowCommandRequest(
+                )
+
+                # Make the request
+                response = await client.poll_airflow_command(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.orchestration.airflow.service_v1beta1.types.PollAirflowCommandRequest, dict]]):
+                The request object. Poll Airflow Command request.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.orchestration.airflow.service_v1beta1.types.PollAirflowCommandResponse:
+                Response to
+                PollAirflowCommandRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        request = environments.PollAirflowCommandRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.poll_airflow_command,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
     async def save_snapshot(
         self,
         request: Optional[Union[environments.SaveSnapshotRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
@@ -1421,14 +1663,196 @@
             environments.LoadSnapshotResponse,
             metadata_type=operations.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
+    async def database_failover(
+        self,
+        request: Optional[Union[environments.DatabaseFailoverRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation_async.AsyncOperation:
+        r"""Triggers database failover (only for highly resilient
+        environments).
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1beta1
+
+            async def sample_database_failover():
+                # Create a client
+                client = service_v1beta1.EnvironmentsAsyncClient()
+
+                # Initialize request argument(s)
+                request = service_v1beta1.DatabaseFailoverRequest(
+                )
+
+                # Make the request
+                operation = client.database_failover(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = (await operation).result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.orchestration.airflow.service_v1beta1.types.DatabaseFailoverRequest, dict]]):
+                The request object. Request to trigger database failover
+                (only for highly resilient
+                environments).
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation_async.AsyncOperation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be
+                :class:`google.cloud.orchestration.airflow.service_v1beta1.types.DatabaseFailoverResponse`
+                Response for DatabaseFailoverRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        request = environments.DatabaseFailoverRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.database_failover,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation_async.from_gapic(
+            response,
+            self._client._transport.operations_client,
+            environments.DatabaseFailoverResponse,
+            metadata_type=operations.OperationMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def fetch_database_properties(
+        self,
+        request: Optional[
+            Union[environments.FetchDatabasePropertiesRequest, dict]
+        ] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> environments.FetchDatabasePropertiesResponse:
+        r"""Fetches database properties.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1beta1
+
+            async def sample_fetch_database_properties():
+                # Create a client
+                client = service_v1beta1.EnvironmentsAsyncClient()
+
+                # Initialize request argument(s)
+                request = service_v1beta1.FetchDatabasePropertiesRequest(
+                    environment="environment_value",
+                )
+
+                # Make the request
+                response = await client.fetch_database_properties(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.orchestration.airflow.service_v1beta1.types.FetchDatabasePropertiesRequest, dict]]):
+                The request object. Request to fetch properties of
+                environment's database.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.orchestration.airflow.service_v1beta1.types.FetchDatabasePropertiesResponse:
+                Response for
+                FetchDatabasePropertiesRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        request = environments.FetchDatabasePropertiesRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.fetch_database_properties,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
     async def list_operations(
         self,
         request: Optional[operations_pb2.ListOperationsRequest] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/client.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1458,14 +1458,259 @@
             environments.CheckUpgradeResponse,
             metadata_type=operations.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
+    def execute_airflow_command(
+        self,
+        request: Optional[
+            Union[environments.ExecuteAirflowCommandRequest, dict]
+        ] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> environments.ExecuteAirflowCommandResponse:
+        r"""Executes Airflow CLI command.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1beta1
+
+            def sample_execute_airflow_command():
+                # Create a client
+                client = service_v1beta1.EnvironmentsClient()
+
+                # Initialize request argument(s)
+                request = service_v1beta1.ExecuteAirflowCommandRequest(
+                )
+
+                # Make the request
+                response = client.execute_airflow_command(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.orchestration.airflow.service_v1beta1.types.ExecuteAirflowCommandRequest, dict]):
+                The request object. Execute Airflow Command request.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.orchestration.airflow.service_v1beta1.types.ExecuteAirflowCommandResponse:
+                Response to
+                ExecuteAirflowCommandRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Minor optimization to avoid making a copy if the user passes
+        # in a environments.ExecuteAirflowCommandRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, environments.ExecuteAirflowCommandRequest):
+            request = environments.ExecuteAirflowCommandRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.execute_airflow_command]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def stop_airflow_command(
+        self,
+        request: Optional[Union[environments.StopAirflowCommandRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> environments.StopAirflowCommandResponse:
+        r"""Stops Airflow CLI command execution.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1beta1
+
+            def sample_stop_airflow_command():
+                # Create a client
+                client = service_v1beta1.EnvironmentsClient()
+
+                # Initialize request argument(s)
+                request = service_v1beta1.StopAirflowCommandRequest(
+                )
+
+                # Make the request
+                response = client.stop_airflow_command(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.orchestration.airflow.service_v1beta1.types.StopAirflowCommandRequest, dict]):
+                The request object. Stop Airflow Command request.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.orchestration.airflow.service_v1beta1.types.StopAirflowCommandResponse:
+                Response to
+                StopAirflowCommandRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Minor optimization to avoid making a copy if the user passes
+        # in a environments.StopAirflowCommandRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, environments.StopAirflowCommandRequest):
+            request = environments.StopAirflowCommandRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.stop_airflow_command]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def poll_airflow_command(
+        self,
+        request: Optional[Union[environments.PollAirflowCommandRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> environments.PollAirflowCommandResponse:
+        r"""Polls Airflow CLI command execution and fetches logs.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1beta1
+
+            def sample_poll_airflow_command():
+                # Create a client
+                client = service_v1beta1.EnvironmentsClient()
+
+                # Initialize request argument(s)
+                request = service_v1beta1.PollAirflowCommandRequest(
+                )
+
+                # Make the request
+                response = client.poll_airflow_command(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.orchestration.airflow.service_v1beta1.types.PollAirflowCommandRequest, dict]):
+                The request object. Poll Airflow Command request.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.orchestration.airflow.service_v1beta1.types.PollAirflowCommandResponse:
+                Response to
+                PollAirflowCommandRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Minor optimization to avoid making a copy if the user passes
+        # in a environments.PollAirflowCommandRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, environments.PollAirflowCommandRequest):
+            request = environments.PollAirflowCommandRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.poll_airflow_command]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
     def save_snapshot(
         self,
         request: Optional[Union[environments.SaveSnapshotRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
@@ -1658,14 +1903,200 @@
             environments.LoadSnapshotResponse,
             metadata_type=operations.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
+    def database_failover(
+        self,
+        request: Optional[Union[environments.DatabaseFailoverRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation.Operation:
+        r"""Triggers database failover (only for highly resilient
+        environments).
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1beta1
+
+            def sample_database_failover():
+                # Create a client
+                client = service_v1beta1.EnvironmentsClient()
+
+                # Initialize request argument(s)
+                request = service_v1beta1.DatabaseFailoverRequest(
+                )
+
+                # Make the request
+                operation = client.database_failover(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = operation.result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.orchestration.airflow.service_v1beta1.types.DatabaseFailoverRequest, dict]):
+                The request object. Request to trigger database failover
+                (only for highly resilient
+                environments).
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation.Operation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be
+                :class:`google.cloud.orchestration.airflow.service_v1beta1.types.DatabaseFailoverResponse`
+                Response for DatabaseFailoverRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Minor optimization to avoid making a copy if the user passes
+        # in a environments.DatabaseFailoverRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, environments.DatabaseFailoverRequest):
+            request = environments.DatabaseFailoverRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.database_failover]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation.from_gapic(
+            response,
+            self._transport.operations_client,
+            environments.DatabaseFailoverResponse,
+            metadata_type=operations.OperationMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def fetch_database_properties(
+        self,
+        request: Optional[
+            Union[environments.FetchDatabasePropertiesRequest, dict]
+        ] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> environments.FetchDatabasePropertiesResponse:
+        r"""Fetches database properties.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud.orchestration.airflow import service_v1beta1
+
+            def sample_fetch_database_properties():
+                # Create a client
+                client = service_v1beta1.EnvironmentsClient()
+
+                # Initialize request argument(s)
+                request = service_v1beta1.FetchDatabasePropertiesRequest(
+                    environment="environment_value",
+                )
+
+                # Make the request
+                response = client.fetch_database_properties(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.orchestration.airflow.service_v1beta1.types.FetchDatabasePropertiesRequest, dict]):
+                The request object. Request to fetch properties of
+                environment's database.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.orchestration.airflow.service_v1beta1.types.FetchDatabasePropertiesResponse:
+                Response for
+                FetchDatabasePropertiesRequest.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Minor optimization to avoid making a copy if the user passes
+        # in a environments.FetchDatabasePropertiesRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, environments.FetchDatabasePropertiesRequest):
+            request = environments.FetchDatabasePropertiesRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[
+            self._transport.fetch_database_properties
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("environment", request.environment),)
+            ),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
     def __enter__(self) -> "EnvironmentsClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/pagers.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/base.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -156,24 +156,49 @@
                 client_info=client_info,
             ),
             self.check_upgrade: gapic_v1.method.wrap_method(
                 self.check_upgrade,
                 default_timeout=None,
                 client_info=client_info,
             ),
+            self.execute_airflow_command: gapic_v1.method.wrap_method(
+                self.execute_airflow_command,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.stop_airflow_command: gapic_v1.method.wrap_method(
+                self.stop_airflow_command,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.poll_airflow_command: gapic_v1.method.wrap_method(
+                self.poll_airflow_command,
+                default_timeout=None,
+                client_info=client_info,
+            ),
             self.save_snapshot: gapic_v1.method.wrap_method(
                 self.save_snapshot,
                 default_timeout=None,
                 client_info=client_info,
             ),
             self.load_snapshot: gapic_v1.method.wrap_method(
                 self.load_snapshot,
                 default_timeout=None,
                 client_info=client_info,
             ),
+            self.database_failover: gapic_v1.method.wrap_method(
+                self.database_failover,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.fetch_database_properties: gapic_v1.method.wrap_method(
+                self.fetch_database_properties,
+                default_timeout=None,
+                client_info=client_info,
+            ),
         }
 
     def close(self):
         """Closes resources associated with the transport.
 
         .. warning::
              Only call this method if the transport is NOT shared
@@ -249,14 +274,50 @@
     ) -> Callable[
         [environments.CheckUpgradeRequest],
         Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
     ]:
         raise NotImplementedError()
 
     @property
+    def execute_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.ExecuteAirflowCommandRequest],
+        Union[
+            environments.ExecuteAirflowCommandResponse,
+            Awaitable[environments.ExecuteAirflowCommandResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def stop_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.StopAirflowCommandRequest],
+        Union[
+            environments.StopAirflowCommandResponse,
+            Awaitable[environments.StopAirflowCommandResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def poll_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.PollAirflowCommandRequest],
+        Union[
+            environments.PollAirflowCommandResponse,
+            Awaitable[environments.PollAirflowCommandResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def save_snapshot(
         self,
     ) -> Callable[
         [environments.SaveSnapshotRequest],
         Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
     ]:
         raise NotImplementedError()
@@ -267,14 +328,35 @@
     ) -> Callable[
         [environments.LoadSnapshotRequest],
         Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
     ]:
         raise NotImplementedError()
 
     @property
+    def database_failover(
+        self,
+    ) -> Callable[
+        [environments.DatabaseFailoverRequest],
+        Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def fetch_database_properties(
+        self,
+    ) -> Callable[
+        [environments.FetchDatabasePropertiesRequest],
+        Union[
+            environments.FetchDatabasePropertiesResponse,
+            Awaitable[environments.FetchDatabasePropertiesResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def list_operations(
         self,
     ) -> Callable[
         [operations_pb2.ListOperationsRequest],
         Union[
             operations_pb2.ListOperationsResponse,
             Awaitable[operations_pb2.ListOperationsResponse],
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/grpc.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/grpc.py`

 * *Files 14% similar despite different names*

```diff
@@ -428,14 +428,101 @@
                 "/google.cloud.orchestration.airflow.service.v1beta1.Environments/CheckUpgrade",
                 request_serializer=environments.CheckUpgradeRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["check_upgrade"]
 
     @property
+    def execute_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.ExecuteAirflowCommandRequest],
+        environments.ExecuteAirflowCommandResponse,
+    ]:
+        r"""Return a callable for the execute airflow command method over gRPC.
+
+        Executes Airflow CLI command.
+
+        Returns:
+            Callable[[~.ExecuteAirflowCommandRequest],
+                    ~.ExecuteAirflowCommandResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "execute_airflow_command" not in self._stubs:
+            self._stubs["execute_airflow_command"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1beta1.Environments/ExecuteAirflowCommand",
+                request_serializer=environments.ExecuteAirflowCommandRequest.serialize,
+                response_deserializer=environments.ExecuteAirflowCommandResponse.deserialize,
+            )
+        return self._stubs["execute_airflow_command"]
+
+    @property
+    def stop_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.StopAirflowCommandRequest],
+        environments.StopAirflowCommandResponse,
+    ]:
+        r"""Return a callable for the stop airflow command method over gRPC.
+
+        Stops Airflow CLI command execution.
+
+        Returns:
+            Callable[[~.StopAirflowCommandRequest],
+                    ~.StopAirflowCommandResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "stop_airflow_command" not in self._stubs:
+            self._stubs["stop_airflow_command"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1beta1.Environments/StopAirflowCommand",
+                request_serializer=environments.StopAirflowCommandRequest.serialize,
+                response_deserializer=environments.StopAirflowCommandResponse.deserialize,
+            )
+        return self._stubs["stop_airflow_command"]
+
+    @property
+    def poll_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.PollAirflowCommandRequest],
+        environments.PollAirflowCommandResponse,
+    ]:
+        r"""Return a callable for the poll airflow command method over gRPC.
+
+        Polls Airflow CLI command execution and fetches logs.
+
+        Returns:
+            Callable[[~.PollAirflowCommandRequest],
+                    ~.PollAirflowCommandResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "poll_airflow_command" not in self._stubs:
+            self._stubs["poll_airflow_command"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1beta1.Environments/PollAirflowCommand",
+                request_serializer=environments.PollAirflowCommandRequest.serialize,
+                response_deserializer=environments.PollAirflowCommandResponse.deserialize,
+            )
+        return self._stubs["poll_airflow_command"]
+
+    @property
     def save_snapshot(
         self,
     ) -> Callable[[environments.SaveSnapshotRequest], operations_pb2.Operation]:
         r"""Return a callable for the save snapshot method over gRPC.
 
         Creates a snapshots of a Cloud Composer environment.
         As a result of this operation, snapshot of environment's
@@ -485,14 +572,70 @@
             self._stubs["load_snapshot"] = self.grpc_channel.unary_unary(
                 "/google.cloud.orchestration.airflow.service.v1beta1.Environments/LoadSnapshot",
                 request_serializer=environments.LoadSnapshotRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["load_snapshot"]
 
+    @property
+    def database_failover(
+        self,
+    ) -> Callable[[environments.DatabaseFailoverRequest], operations_pb2.Operation]:
+        r"""Return a callable for the database failover method over gRPC.
+
+        Triggers database failover (only for highly resilient
+        environments).
+
+        Returns:
+            Callable[[~.DatabaseFailoverRequest],
+                    ~.Operation]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "database_failover" not in self._stubs:
+            self._stubs["database_failover"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1beta1.Environments/DatabaseFailover",
+                request_serializer=environments.DatabaseFailoverRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["database_failover"]
+
+    @property
+    def fetch_database_properties(
+        self,
+    ) -> Callable[
+        [environments.FetchDatabasePropertiesRequest],
+        environments.FetchDatabasePropertiesResponse,
+    ]:
+        r"""Return a callable for the fetch database properties method over gRPC.
+
+        Fetches database properties.
+
+        Returns:
+            Callable[[~.FetchDatabasePropertiesRequest],
+                    ~.FetchDatabasePropertiesResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "fetch_database_properties" not in self._stubs:
+            self._stubs["fetch_database_properties"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1beta1.Environments/FetchDatabaseProperties",
+                request_serializer=environments.FetchDatabasePropertiesRequest.serialize,
+                response_deserializer=environments.FetchDatabasePropertiesResponse.deserialize,
+            )
+        return self._stubs["fetch_database_properties"]
+
     def close(self):
         self.grpc_channel.close()
 
     @property
     def delete_operation(
         self,
     ) -> Callable[[operations_pb2.DeleteOperationRequest], None]:
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/grpc_asyncio.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/grpc_asyncio.py`

 * *Files 12% similar despite different names*

```diff
@@ -446,14 +446,101 @@
                 "/google.cloud.orchestration.airflow.service.v1beta1.Environments/CheckUpgrade",
                 request_serializer=environments.CheckUpgradeRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["check_upgrade"]
 
     @property
+    def execute_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.ExecuteAirflowCommandRequest],
+        Awaitable[environments.ExecuteAirflowCommandResponse],
+    ]:
+        r"""Return a callable for the execute airflow command method over gRPC.
+
+        Executes Airflow CLI command.
+
+        Returns:
+            Callable[[~.ExecuteAirflowCommandRequest],
+                    Awaitable[~.ExecuteAirflowCommandResponse]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "execute_airflow_command" not in self._stubs:
+            self._stubs["execute_airflow_command"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1beta1.Environments/ExecuteAirflowCommand",
+                request_serializer=environments.ExecuteAirflowCommandRequest.serialize,
+                response_deserializer=environments.ExecuteAirflowCommandResponse.deserialize,
+            )
+        return self._stubs["execute_airflow_command"]
+
+    @property
+    def stop_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.StopAirflowCommandRequest],
+        Awaitable[environments.StopAirflowCommandResponse],
+    ]:
+        r"""Return a callable for the stop airflow command method over gRPC.
+
+        Stops Airflow CLI command execution.
+
+        Returns:
+            Callable[[~.StopAirflowCommandRequest],
+                    Awaitable[~.StopAirflowCommandResponse]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "stop_airflow_command" not in self._stubs:
+            self._stubs["stop_airflow_command"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1beta1.Environments/StopAirflowCommand",
+                request_serializer=environments.StopAirflowCommandRequest.serialize,
+                response_deserializer=environments.StopAirflowCommandResponse.deserialize,
+            )
+        return self._stubs["stop_airflow_command"]
+
+    @property
+    def poll_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.PollAirflowCommandRequest],
+        Awaitable[environments.PollAirflowCommandResponse],
+    ]:
+        r"""Return a callable for the poll airflow command method over gRPC.
+
+        Polls Airflow CLI command execution and fetches logs.
+
+        Returns:
+            Callable[[~.PollAirflowCommandRequest],
+                    Awaitable[~.PollAirflowCommandResponse]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "poll_airflow_command" not in self._stubs:
+            self._stubs["poll_airflow_command"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1beta1.Environments/PollAirflowCommand",
+                request_serializer=environments.PollAirflowCommandRequest.serialize,
+                response_deserializer=environments.PollAirflowCommandResponse.deserialize,
+            )
+        return self._stubs["poll_airflow_command"]
+
+    @property
     def save_snapshot(
         self,
     ) -> Callable[
         [environments.SaveSnapshotRequest], Awaitable[operations_pb2.Operation]
     ]:
         r"""Return a callable for the save snapshot method over gRPC.
 
@@ -507,14 +594,72 @@
             self._stubs["load_snapshot"] = self.grpc_channel.unary_unary(
                 "/google.cloud.orchestration.airflow.service.v1beta1.Environments/LoadSnapshot",
                 request_serializer=environments.LoadSnapshotRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["load_snapshot"]
 
+    @property
+    def database_failover(
+        self,
+    ) -> Callable[
+        [environments.DatabaseFailoverRequest], Awaitable[operations_pb2.Operation]
+    ]:
+        r"""Return a callable for the database failover method over gRPC.
+
+        Triggers database failover (only for highly resilient
+        environments).
+
+        Returns:
+            Callable[[~.DatabaseFailoverRequest],
+                    Awaitable[~.Operation]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "database_failover" not in self._stubs:
+            self._stubs["database_failover"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1beta1.Environments/DatabaseFailover",
+                request_serializer=environments.DatabaseFailoverRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["database_failover"]
+
+    @property
+    def fetch_database_properties(
+        self,
+    ) -> Callable[
+        [environments.FetchDatabasePropertiesRequest],
+        Awaitable[environments.FetchDatabasePropertiesResponse],
+    ]:
+        r"""Return a callable for the fetch database properties method over gRPC.
+
+        Fetches database properties.
+
+        Returns:
+            Callable[[~.FetchDatabasePropertiesRequest],
+                    Awaitable[~.FetchDatabasePropertiesResponse]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "fetch_database_properties" not in self._stubs:
+            self._stubs["fetch_database_properties"] = self.grpc_channel.unary_unary(
+                "/google.cloud.orchestration.airflow.service.v1beta1.Environments/FetchDatabaseProperties",
+                request_serializer=environments.FetchDatabasePropertiesRequest.serialize,
+                response_deserializer=environments.FetchDatabasePropertiesResponse.deserialize,
+            )
+        return self._stubs["fetch_database_properties"]
+
     def close(self):
         return self.grpc_channel.close()
 
     @property
     def delete_operation(
         self,
     ) -> Callable[[operations_pb2.DeleteOperationRequest], None]:
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/rest.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/environments/transports/rest.py`

 * *Files 19% similar despite different names*

```diff
@@ -84,22 +84,46 @@
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_create_environment(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_database_failover(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_database_failover(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_delete_environment(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_delete_environment(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_execute_airflow_command(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_execute_airflow_command(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
+            def pre_fetch_database_properties(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_fetch_database_properties(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_get_environment(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_get_environment(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -116,14 +140,22 @@
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_load_snapshot(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_poll_airflow_command(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_poll_airflow_command(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_restart_web_server(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_restart_web_server(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -132,14 +164,22 @@
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_save_snapshot(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_stop_airflow_command(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_stop_airflow_command(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_update_environment(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_update_environment(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -192,14 +232,37 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the Environments server but before
         it is returned to user code.
         """
         return response
 
+    def pre_database_failover(
+        self,
+        request: environments.DatabaseFailoverRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[environments.DatabaseFailoverRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for database_failover
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the Environments server.
+        """
+        return request, metadata
+
+    def post_database_failover(
+        self, response: operations_pb2.Operation
+    ) -> operations_pb2.Operation:
+        """Post-rpc interceptor for database_failover
+
+        Override in a subclass to manipulate the response
+        after it is returned by the Environments server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_delete_environment(
         self,
         request: environments.DeleteEnvironmentRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[environments.DeleteEnvironmentRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for delete_environment
 
@@ -215,14 +278,60 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the Environments server but before
         it is returned to user code.
         """
         return response
 
+    def pre_execute_airflow_command(
+        self,
+        request: environments.ExecuteAirflowCommandRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[environments.ExecuteAirflowCommandRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for execute_airflow_command
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the Environments server.
+        """
+        return request, metadata
+
+    def post_execute_airflow_command(
+        self, response: environments.ExecuteAirflowCommandResponse
+    ) -> environments.ExecuteAirflowCommandResponse:
+        """Post-rpc interceptor for execute_airflow_command
+
+        Override in a subclass to manipulate the response
+        after it is returned by the Environments server but before
+        it is returned to user code.
+        """
+        return response
+
+    def pre_fetch_database_properties(
+        self,
+        request: environments.FetchDatabasePropertiesRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[environments.FetchDatabasePropertiesRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for fetch_database_properties
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the Environments server.
+        """
+        return request, metadata
+
+    def post_fetch_database_properties(
+        self, response: environments.FetchDatabasePropertiesResponse
+    ) -> environments.FetchDatabasePropertiesResponse:
+        """Post-rpc interceptor for fetch_database_properties
+
+        Override in a subclass to manipulate the response
+        after it is returned by the Environments server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_get_environment(
         self,
         request: environments.GetEnvironmentRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[environments.GetEnvironmentRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for get_environment
 
@@ -284,14 +393,37 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the Environments server but before
         it is returned to user code.
         """
         return response
 
+    def pre_poll_airflow_command(
+        self,
+        request: environments.PollAirflowCommandRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[environments.PollAirflowCommandRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for poll_airflow_command
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the Environments server.
+        """
+        return request, metadata
+
+    def post_poll_airflow_command(
+        self, response: environments.PollAirflowCommandResponse
+    ) -> environments.PollAirflowCommandResponse:
+        """Post-rpc interceptor for poll_airflow_command
+
+        Override in a subclass to manipulate the response
+        after it is returned by the Environments server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_restart_web_server(
         self,
         request: environments.RestartWebServerRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[environments.RestartWebServerRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for restart_web_server
 
@@ -330,14 +462,37 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the Environments server but before
         it is returned to user code.
         """
         return response
 
+    def pre_stop_airflow_command(
+        self,
+        request: environments.StopAirflowCommandRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[environments.StopAirflowCommandRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for stop_airflow_command
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the Environments server.
+        """
+        return request, metadata
+
+    def post_stop_airflow_command(
+        self, response: environments.StopAirflowCommandResponse
+    ) -> environments.StopAirflowCommandResponse:
+        """Post-rpc interceptor for stop_airflow_command
+
+        Override in a subclass to manipulate the response
+        after it is returned by the Environments server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_update_environment(
         self,
         request: environments.UpdateEnvironmentRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[environments.UpdateEnvironmentRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for update_environment
 
@@ -737,14 +892,103 @@
 
             # Return the response
             resp = operations_pb2.Operation()
             json_format.Parse(response.content, resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_create_environment(resp)
             return resp
 
+    class _DatabaseFailover(EnvironmentsRestStub):
+        def __hash__(self):
+            return hash("DatabaseFailover")
+
+        def __call__(
+            self,
+            request: environments.DatabaseFailoverRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> operations_pb2.Operation:
+            r"""Call the database failover method over HTTP.
+
+            Args:
+                request (~.environments.DatabaseFailoverRequest):
+                    The request object. Request to trigger database failover
+                (only for highly resilient
+                environments).
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.operations_pb2.Operation:
+                    This resource represents a
+                long-running operation that is the
+                result of a network API call.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "post",
+                    "uri": "/v1beta1/{environment=projects/*/locations/*/environments/*}:databaseFailover",
+                    "body": "*",
+                },
+            ]
+            request, metadata = self._interceptor.pre_database_failover(
+                request, metadata
+            )
+            pb_request = environments.DatabaseFailoverRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            # Jsonify the request body
+
+            body = json_format.MessageToJson(
+                transcoded_request["body"],
+                including_default_value_fields=False,
+                use_integers_for_enums=True,
+            )
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = operations_pb2.Operation()
+            json_format.Parse(response.content, resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_database_failover(resp)
+            return resp
+
     class _DeleteEnvironment(EnvironmentsRestStub):
         def __hash__(self):
             return hash("DeleteEnvironment")
 
         def __call__(
             self,
             request: environments.DeleteEnvironmentRequest,
@@ -815,14 +1059,193 @@
 
             # Return the response
             resp = operations_pb2.Operation()
             json_format.Parse(response.content, resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_delete_environment(resp)
             return resp
 
+    class _ExecuteAirflowCommand(EnvironmentsRestStub):
+        def __hash__(self):
+            return hash("ExecuteAirflowCommand")
+
+        def __call__(
+            self,
+            request: environments.ExecuteAirflowCommandRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> environments.ExecuteAirflowCommandResponse:
+            r"""Call the execute airflow command method over HTTP.
+
+            Args:
+                request (~.environments.ExecuteAirflowCommandRequest):
+                    The request object. Execute Airflow Command request.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.environments.ExecuteAirflowCommandResponse:
+                    Response to
+                ExecuteAirflowCommandRequest.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "post",
+                    "uri": "/v1beta1/{environment=projects/*/locations/*/environments/*}:executeAirflowCommand",
+                    "body": "*",
+                },
+            ]
+            request, metadata = self._interceptor.pre_execute_airflow_command(
+                request, metadata
+            )
+            pb_request = environments.ExecuteAirflowCommandRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            # Jsonify the request body
+
+            body = json_format.MessageToJson(
+                transcoded_request["body"],
+                including_default_value_fields=False,
+                use_integers_for_enums=True,
+            )
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = environments.ExecuteAirflowCommandResponse()
+            pb_resp = environments.ExecuteAirflowCommandResponse.pb(resp)
+
+            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_execute_airflow_command(resp)
+            return resp
+
+    class _FetchDatabaseProperties(EnvironmentsRestStub):
+        def __hash__(self):
+            return hash("FetchDatabaseProperties")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: environments.FetchDatabasePropertiesRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> environments.FetchDatabasePropertiesResponse:
+            r"""Call the fetch database properties method over HTTP.
+
+            Args:
+                request (~.environments.FetchDatabasePropertiesRequest):
+                    The request object. Request to fetch properties of
+                environment's database.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.environments.FetchDatabasePropertiesResponse:
+                    Response for
+                FetchDatabasePropertiesRequest.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1beta1/{environment=projects/*/locations/*/environments/*}:fetchDatabaseProperties",
+                },
+            ]
+            request, metadata = self._interceptor.pre_fetch_database_properties(
+                request, metadata
+            )
+            pb_request = environments.FetchDatabasePropertiesRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = environments.FetchDatabasePropertiesResponse()
+            pb_resp = environments.FetchDatabasePropertiesResponse.pb(resp)
+
+            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_fetch_database_properties(resp)
+            return resp
+
     class _GetEnvironment(EnvironmentsRestStub):
         def __hash__(self):
             return hash("GetEnvironment")
 
         def __call__(
             self,
             request: environments.GetEnvironmentRequest,
@@ -1058,14 +1481,102 @@
 
             # Return the response
             resp = operations_pb2.Operation()
             json_format.Parse(response.content, resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_load_snapshot(resp)
             return resp
 
+    class _PollAirflowCommand(EnvironmentsRestStub):
+        def __hash__(self):
+            return hash("PollAirflowCommand")
+
+        def __call__(
+            self,
+            request: environments.PollAirflowCommandRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> environments.PollAirflowCommandResponse:
+            r"""Call the poll airflow command method over HTTP.
+
+            Args:
+                request (~.environments.PollAirflowCommandRequest):
+                    The request object. Poll Airflow Command request.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.environments.PollAirflowCommandResponse:
+                    Response to
+                PollAirflowCommandRequest.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "post",
+                    "uri": "/v1beta1/{environment=projects/*/locations/*/environments/*}:pollAirflowCommand",
+                    "body": "*",
+                },
+            ]
+            request, metadata = self._interceptor.pre_poll_airflow_command(
+                request, metadata
+            )
+            pb_request = environments.PollAirflowCommandRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            # Jsonify the request body
+
+            body = json_format.MessageToJson(
+                transcoded_request["body"],
+                including_default_value_fields=False,
+                use_integers_for_enums=True,
+            )
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = environments.PollAirflowCommandResponse()
+            pb_resp = environments.PollAirflowCommandResponse.pb(resp)
+
+            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_poll_airflow_command(resp)
+            return resp
+
     class _RestartWebServer(EnvironmentsRestStub):
         def __hash__(self):
             return hash("RestartWebServer")
 
         def __call__(
             self,
             request: environments.RestartWebServerRequest,
@@ -1231,14 +1742,102 @@
 
             # Return the response
             resp = operations_pb2.Operation()
             json_format.Parse(response.content, resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_save_snapshot(resp)
             return resp
 
+    class _StopAirflowCommand(EnvironmentsRestStub):
+        def __hash__(self):
+            return hash("StopAirflowCommand")
+
+        def __call__(
+            self,
+            request: environments.StopAirflowCommandRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> environments.StopAirflowCommandResponse:
+            r"""Call the stop airflow command method over HTTP.
+
+            Args:
+                request (~.environments.StopAirflowCommandRequest):
+                    The request object. Stop Airflow Command request.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.environments.StopAirflowCommandResponse:
+                    Response to
+                StopAirflowCommandRequest.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "post",
+                    "uri": "/v1beta1/{environment=projects/*/locations/*/environments/*}:stopAirflowCommand",
+                    "body": "*",
+                },
+            ]
+            request, metadata = self._interceptor.pre_stop_airflow_command(
+                request, metadata
+            )
+            pb_request = environments.StopAirflowCommandRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            # Jsonify the request body
+
+            body = json_format.MessageToJson(
+                transcoded_request["body"],
+                including_default_value_fields=False,
+                use_integers_for_enums=True,
+            )
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = environments.StopAirflowCommandResponse()
+            pb_resp = environments.StopAirflowCommandResponse.pb(resp)
+
+            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_stop_airflow_command(resp)
+            return resp
+
     class _UpdateEnvironment(EnvironmentsRestStub):
         def __hash__(self):
             return hash("UpdateEnvironment")
 
         __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {
             "updateMask": {},
         }
@@ -1348,22 +1947,52 @@
         self,
     ) -> Callable[[environments.CreateEnvironmentRequest], operations_pb2.Operation]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._CreateEnvironment(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def database_failover(
+        self,
+    ) -> Callable[[environments.DatabaseFailoverRequest], operations_pb2.Operation]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._DatabaseFailover(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def delete_environment(
         self,
     ) -> Callable[[environments.DeleteEnvironmentRequest], operations_pb2.Operation]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._DeleteEnvironment(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def execute_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.ExecuteAirflowCommandRequest],
+        environments.ExecuteAirflowCommandResponse,
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._ExecuteAirflowCommand(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
+    def fetch_database_properties(
+        self,
+    ) -> Callable[
+        [environments.FetchDatabasePropertiesRequest],
+        environments.FetchDatabasePropertiesResponse,
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._FetchDatabaseProperties(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def get_environment(
         self,
     ) -> Callable[[environments.GetEnvironmentRequest], environments.Environment]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._GetEnvironment(self._session, self._host, self._interceptor)  # type: ignore
 
@@ -1382,14 +2011,25 @@
         self,
     ) -> Callable[[environments.LoadSnapshotRequest], operations_pb2.Operation]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._LoadSnapshot(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def poll_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.PollAirflowCommandRequest],
+        environments.PollAirflowCommandResponse,
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._PollAirflowCommand(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def restart_web_server(
         self,
     ) -> Callable[[environments.RestartWebServerRequest], operations_pb2.Operation]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._RestartWebServer(self._session, self._host, self._interceptor)  # type: ignore
 
@@ -1398,14 +2038,25 @@
         self,
     ) -> Callable[[environments.SaveSnapshotRequest], operations_pb2.Operation]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._SaveSnapshot(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def stop_airflow_command(
+        self,
+    ) -> Callable[
+        [environments.StopAirflowCommandRequest],
+        environments.StopAirflowCommandResponse,
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._StopAirflowCommand(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def update_environment(
         self,
     ) -> Callable[[environments.UpdateEnvironmentRequest], operations_pb2.Operation]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._UpdateEnvironment(self._session, self._host, self._interceptor)  # type: ignore
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/async_client.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/client.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/pagers.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/grpc.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/grpc_asyncio.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/rest.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/services/image_versions/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,86 +9,119 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from .environments import (
-    CheckUpgradeRequest,
+from google.cloud.orchestration.airflow.service import gapic_version as package_version
+
+__version__ = package_version.__version__
+
+
+from google.cloud.orchestration.airflow.service_v1.services.environments.async_client import (
+    EnvironmentsAsyncClient,
+)
+from google.cloud.orchestration.airflow.service_v1.services.environments.client import (
+    EnvironmentsClient,
+)
+from google.cloud.orchestration.airflow.service_v1.services.image_versions.async_client import (
+    ImageVersionsAsyncClient,
+)
+from google.cloud.orchestration.airflow.service_v1.services.image_versions.client import (
+    ImageVersionsClient,
+)
+from google.cloud.orchestration.airflow.service_v1.types.environments import (
     CheckUpgradeResponse,
-    CloudDataLineageIntegration,
     CreateEnvironmentRequest,
     DatabaseConfig,
+    DatabaseFailoverRequest,
+    DatabaseFailoverResponse,
     DeleteEnvironmentRequest,
     EncryptionConfig,
     Environment,
     EnvironmentConfig,
+    ExecuteAirflowCommandRequest,
     ExecuteAirflowCommandResponse,
+    FetchDatabasePropertiesRequest,
+    FetchDatabasePropertiesResponse,
     GetEnvironmentRequest,
     IPAllocationPolicy,
     ListEnvironmentsRequest,
     ListEnvironmentsResponse,
     LoadSnapshotRequest,
     LoadSnapshotResponse,
     MaintenanceWindow,
     MasterAuthorizedNetworksConfig,
     NetworkingConfig,
     NodeConfig,
+    PollAirflowCommandRequest,
     PollAirflowCommandResponse,
     PrivateClusterConfig,
     PrivateEnvironmentConfig,
     RecoveryConfig,
-    RestartWebServerRequest,
     SaveSnapshotRequest,
     SaveSnapshotResponse,
     ScheduledSnapshotsConfig,
     SoftwareConfig,
+    StopAirflowCommandRequest,
+    StopAirflowCommandResponse,
     UpdateEnvironmentRequest,
     WebServerConfig,
     WebServerNetworkAccessControl,
     WorkloadsConfig,
 )
-from .image_versions import (
+from google.cloud.orchestration.airflow.service_v1.types.image_versions import (
     ImageVersion,
     ListImageVersionsRequest,
     ListImageVersionsResponse,
 )
-from .operations import OperationMetadata
+from google.cloud.orchestration.airflow.service_v1.types.operations import (
+    OperationMetadata,
+)
 
 __all__ = (
-    "CheckUpgradeRequest",
+    "EnvironmentsClient",
+    "EnvironmentsAsyncClient",
+    "ImageVersionsClient",
+    "ImageVersionsAsyncClient",
     "CheckUpgradeResponse",
-    "CloudDataLineageIntegration",
     "CreateEnvironmentRequest",
     "DatabaseConfig",
+    "DatabaseFailoverRequest",
+    "DatabaseFailoverResponse",
     "DeleteEnvironmentRequest",
     "EncryptionConfig",
     "Environment",
     "EnvironmentConfig",
+    "ExecuteAirflowCommandRequest",
     "ExecuteAirflowCommandResponse",
+    "FetchDatabasePropertiesRequest",
+    "FetchDatabasePropertiesResponse",
     "GetEnvironmentRequest",
     "IPAllocationPolicy",
     "ListEnvironmentsRequest",
     "ListEnvironmentsResponse",
     "LoadSnapshotRequest",
     "LoadSnapshotResponse",
     "MaintenanceWindow",
     "MasterAuthorizedNetworksConfig",
     "NetworkingConfig",
     "NodeConfig",
+    "PollAirflowCommandRequest",
     "PollAirflowCommandResponse",
     "PrivateClusterConfig",
     "PrivateEnvironmentConfig",
     "RecoveryConfig",
-    "RestartWebServerRequest",
     "SaveSnapshotRequest",
     "SaveSnapshotResponse",
     "ScheduledSnapshotsConfig",
     "SoftwareConfig",
+    "StopAirflowCommandRequest",
+    "StopAirflowCommandResponse",
     "UpdateEnvironmentRequest",
     "WebServerConfig",
     "WebServerNetworkAccessControl",
     "WorkloadsConfig",
     "ImageVersion",
     "ListImageVersionsRequest",
     "ListImageVersionsResponse",
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/environments.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/types/environments.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,20 +27,28 @@
         "CreateEnvironmentRequest",
         "GetEnvironmentRequest",
         "ListEnvironmentsRequest",
         "ListEnvironmentsResponse",
         "DeleteEnvironmentRequest",
         "UpdateEnvironmentRequest",
         "RestartWebServerRequest",
+        "ExecuteAirflowCommandRequest",
         "ExecuteAirflowCommandResponse",
+        "StopAirflowCommandRequest",
+        "StopAirflowCommandResponse",
+        "PollAirflowCommandRequest",
         "PollAirflowCommandResponse",
         "SaveSnapshotRequest",
         "SaveSnapshotResponse",
         "LoadSnapshotRequest",
         "LoadSnapshotResponse",
+        "DatabaseFailoverRequest",
+        "DatabaseFailoverResponse",
+        "FetchDatabasePropertiesRequest",
+        "FetchDatabasePropertiesResponse",
         "EnvironmentConfig",
         "WebServerNetworkAccessControl",
         "SoftwareConfig",
         "IPAllocationPolicy",
         "NodeConfig",
         "PrivateClusterConfig",
         "NetworkingConfig",
@@ -415,14 +423,52 @@
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
+class ExecuteAirflowCommandRequest(proto.Message):
+    r"""Execute Airflow Command request.
+
+    Attributes:
+        environment (str):
+            The resource name of the environment in the
+            form:
+            "projects/{projectId}/locations/{locationId}/environments/{environmentId}".
+        command (str):
+            Airflow command.
+        subcommand (str):
+            Airflow subcommand.
+        parameters (MutableSequence[str]):
+            Parameters for the Airflow command/subcommand as an array of
+            arguments. It may contain positional arguments like
+            ``["my-dag-id"]``, key-value parameters like
+            ``["--foo=bar"]`` or ``["--foo","bar"]``, or other flags
+            like ``["-f"]``.
+    """
+
+    environment: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    command: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    subcommand: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    parameters: MutableSequence[str] = proto.RepeatedField(
+        proto.STRING,
+        number=4,
+    )
+
+
 class ExecuteAirflowCommandResponse(proto.Message):
     r"""Response to ExecuteAirflowCommandRequest.
 
     Attributes:
         execution_id (str):
             The unique ID of the command execution for
             polling.
@@ -450,14 +496,122 @@
     )
     error: str = proto.Field(
         proto.STRING,
         number=4,
     )
 
 
+class StopAirflowCommandRequest(proto.Message):
+    r"""Stop Airflow Command request.
+
+    Attributes:
+        environment (str):
+            The resource name of the environment in the
+            form:
+            "projects/{projectId}/locations/{locationId}/environments/{environmentId}".
+        execution_id (str):
+            The unique ID of the command execution.
+        pod (str):
+            The name of the pod where the command is
+            executed.
+        pod_namespace (str):
+            The namespace of the pod where the command is
+            executed.
+        force (bool):
+            If true, the execution is terminated
+            forcefully (SIGKILL). If false, the execution is
+            stopped gracefully, giving it time for cleanup.
+    """
+
+    environment: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    execution_id: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    pod: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    pod_namespace: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    force: bool = proto.Field(
+        proto.BOOL,
+        number=5,
+    )
+
+
+class StopAirflowCommandResponse(proto.Message):
+    r"""Response to StopAirflowCommandRequest.
+
+    Attributes:
+        is_done (bool):
+            Whether the execution is still running.
+        output (MutableSequence[str]):
+            Output message from stopping execution
+            request.
+    """
+
+    is_done: bool = proto.Field(
+        proto.BOOL,
+        number=1,
+    )
+    output: MutableSequence[str] = proto.RepeatedField(
+        proto.STRING,
+        number=2,
+    )
+
+
+class PollAirflowCommandRequest(proto.Message):
+    r"""Poll Airflow Command request.
+
+    Attributes:
+        environment (str):
+            The resource name of the environment in the
+            form:
+            "projects/{projectId}/locations/{locationId}/environments/{environmentId}".
+        execution_id (str):
+            The unique ID of the command execution.
+        pod (str):
+            The name of the pod where the command is
+            executed.
+        pod_namespace (str):
+            The namespace of the pod where the command is
+            executed.
+        next_line_number (int):
+            Line number from which new logs should be
+            fetched.
+    """
+
+    environment: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    execution_id: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    pod: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    pod_namespace: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    next_line_number: int = proto.Field(
+        proto.INT32,
+        number=5,
+    )
+
+
 class PollAirflowCommandResponse(proto.Message):
     r"""Response to PollAirflowCommandRequest.
 
     Attributes:
         output (MutableSequence[google.cloud.orchestration.airflow.service_v1beta1.types.PollAirflowCommandResponse.Line]):
             Output from the command execution. It may not
             contain the full output and the caller may need
@@ -616,14 +770,83 @@
     )
 
 
 class LoadSnapshotResponse(proto.Message):
     r"""Response to LoadSnapshotRequest."""
 
 
+class DatabaseFailoverRequest(proto.Message):
+    r"""Request to trigger database failover (only for highly
+    resilient environments).
+
+    Attributes:
+        environment (str):
+            Target environment:
+            "projects/{projectId}/locations/{locationId}/environments/{environmentId}".
+    """
+
+    environment: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+
+
+class DatabaseFailoverResponse(proto.Message):
+    r"""Response for DatabaseFailoverRequest."""
+
+
+class FetchDatabasePropertiesRequest(proto.Message):
+    r"""Request to fetch properties of environment's database.
+
+    Attributes:
+        environment (str):
+            Required. The resource name of the
+            environment, in the form:
+            "projects/{projectId}/locations/{locationId}/environments/{environmentId}".
+    """
+
+    environment: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+
+
+class FetchDatabasePropertiesResponse(proto.Message):
+    r"""Response for FetchDatabasePropertiesRequest.
+
+    Attributes:
+        primary_gce_zone (str):
+            The Compute Engine zone that the instance is
+            currently serving from.
+        secondary_gce_zone (str):
+            The Compute Engine zone that the failover
+            instance is currently serving from for a
+            regional Cloud SQL instance.
+        is_failover_replica_available (bool):
+            The availability status of the failover
+            replica. A false status indicates that the
+            failover replica is out of sync. The primary
+            instance can only fail over to the failover
+            replica when the status is true.
+    """
+
+    primary_gce_zone: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    secondary_gce_zone: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    is_failover_replica_available: bool = proto.Field(
+        proto.BOOL,
+        number=3,
+    )
+
+
 class EnvironmentConfig(proto.Message):
     r"""Configuration information for an environment.
 
     Attributes:
         gke_cluster (str):
             Output only. The Kubernetes Engine cluster
             used to run this environment.
@@ -721,14 +944,19 @@
             - in case of public environment: disabled.
         recovery_config (google.cloud.orchestration.airflow.service_v1beta1.types.RecoveryConfig):
             Optional. The Recovery settings configuration of an
             environment.
 
             This field is supported for Cloud Composer environments in
             versions composer-2.\ *.*-airflow-*.*.\* and newer.
+        resilience_mode (google.cloud.orchestration.airflow.service_v1beta1.types.EnvironmentConfig.ResilienceMode):
+            Optional. Resilience mode of the Cloud Composer Environment.
+
+            This field is supported for Cloud Composer environments in
+            versions composer-2.2.0-airflow-\ *.*.\* and newer.
     """
 
     class EnvironmentSize(proto.Enum):
         r"""The size of the Cloud Composer environment.
 
         Values:
             ENVIRONMENT_SIZE_UNSPECIFIED (0):
@@ -741,14 +969,28 @@
                 The environment size is large.
         """
         ENVIRONMENT_SIZE_UNSPECIFIED = 0
         ENVIRONMENT_SIZE_SMALL = 1
         ENVIRONMENT_SIZE_MEDIUM = 2
         ENVIRONMENT_SIZE_LARGE = 3
 
+    class ResilienceMode(proto.Enum):
+        r"""Resilience mode of the Cloud Composer Environment.
+
+        Values:
+            RESILIENCE_MODE_UNSPECIFIED (0):
+                Default mode doesn't change environment
+                parameters.
+            HIGH_RESILIENCE (1):
+                Enabled High Resilience mode, including Cloud
+                SQL HA.
+        """
+        RESILIENCE_MODE_UNSPECIFIED = 0
+        HIGH_RESILIENCE = 1
+
     gke_cluster: str = proto.Field(
         proto.STRING,
         number=1,
     )
     dag_gcs_prefix: str = proto.Field(
         proto.STRING,
         number=2,
@@ -821,14 +1063,19 @@
         message="MasterAuthorizedNetworksConfig",
     )
     recovery_config: "RecoveryConfig" = proto.Field(
         proto.MESSAGE,
         number=18,
         message="RecoveryConfig",
     )
+    resilience_mode: ResilienceMode = proto.Field(
+        proto.ENUM,
+        number=20,
+        enum=ResilienceMode,
+    )
 
 
 class WebServerNetworkAccessControl(proto.Message):
     r"""Network-level access control policy for the Airflow web
     server.
 
     Attributes:
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/image_versions.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1beta1/types/image_versions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/google/cloud/orchestration/airflow/service_v1beta1/types/operations.py` & `google-cloud-orchestration-airflow-1.9.0/google/cloud/orchestration/airflow/service_v1/types/operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.cloud.orchestration.airflow.service.v1beta1",
+    package="google.cloud.orchestration.airflow.service.v1",
     manifest={
         "OperationMetadata",
     },
 )
 
 
 class OperationMetadata(proto.Message):
     r"""Metadata describing an operation.
 
     Attributes:
-        state (google.cloud.orchestration.airflow.service_v1beta1.types.OperationMetadata.State):
+        state (google.cloud.orchestration.airflow.service_v1.types.OperationMetadata.State):
             Output only. The current operation state.
-        operation_type (google.cloud.orchestration.airflow.service_v1beta1.types.OperationMetadata.Type):
+        operation_type (google.cloud.orchestration.airflow.service_v1.types.OperationMetadata.Type):
             Output only. The type of operation being
             performed.
         resource (str):
             Output only. The resource being operated on, as a `relative
             resource
             name </apis/design/resource_names#relative_resource_name>`__.
         resource_uuid (str):
@@ -61,23 +61,27 @@
             STATE_UNSPECIFIED (0):
                 Unused.
             PENDING (1):
                 The operation has been created but is not yet
                 started.
             RUNNING (2):
                 The operation is underway.
-            SUCCESSFUL (3):
+            SUCCEEDED (3):
                 The operation completed successfully.
+            SUCCESSFUL (3):
+                No description available.
             FAILED (4):
                 The operation is no longer running but did
                 not succeed.
         """
+        _pb_options = {"allow_alias": True}
         STATE_UNSPECIFIED = 0
         PENDING = 1
         RUNNING = 2
+        SUCCEEDED = 3
         SUCCESSFUL = 3
         FAILED = 4
 
     class Type(proto.Enum):
         r"""Type of longrunning operation.
 
         Values:
@@ -91,22 +95,27 @@
                 A resource update operation.
             CHECK (4):
                 A resource check operation.
             SAVE_SNAPSHOT (5):
                 Saves snapshot of the resource operation.
             LOAD_SNAPSHOT (6):
                 Loads snapshot of the resource operation.
+            DATABASE_FAILOVER (7):
+                Triggers failover of environment's Cloud SQL
+                instance (only for highly resilient
+                environments).
         """
         TYPE_UNSPECIFIED = 0
         CREATE = 1
         DELETE = 2
         UPDATE = 3
         CHECK = 4
         SAVE_SNAPSHOT = 5
         LOAD_SNAPSHOT = 6
+        DATABASE_FAILOVER = 7
 
     state: State = proto.Field(
         proto.ENUM,
         number=1,
         enum=State,
     )
     operation_type: Type = proto.Field(
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/PKG-INFO` & `google-cloud-orchestration-airflow-1.9.0/google_cloud_orchestration_airflow.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-orchestration-airflow
-Version: 1.8.0
+Version: 1.9.0
 Summary: Google Cloud Orchestration Airflow API client library
-Home-page: https://github.com/googleapis/python-orchestration-airflow
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for Cloud Composer API
-====================================
+Python Client for Cloud Composer
+================================
 
 |stable| |pypi| |versions|
 
-`Cloud Composer API`_: is a managed Apache Airflow service that helps you create, schedule, monitor and manage workflows. Cloud Composer automation helps you create Airflow environments quickly and use Airflow-native tools, such as the powerful Airflow web interface and command line tools, so you can focus on your workflows and not your infrastructure.
+`Cloud Composer`_: is a managed Apache Airflow service that helps you create, schedule, monitor and manage workflows. Cloud Composer automation helps you create Airflow environments quickly and use Airflow-native tools, such as the powerful Airflow web interface and command line tools, so you can focus on your workflows and not your infrastructure.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-orchestration-airflow.svg
    :target: https://pypi.org/project/google-cloud-orchestration-airflow/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-orchestration-airflow.svg
    :target: https://pypi.org/project/google-cloud-orchestration-airflow/
-.. _Cloud Composer API: https://cloud.google.com/composer/
+.. _Cloud Composer: https://cloud.google.com/composer/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/composer/latest
 .. _Product Documentation:  https://cloud.google.com/composer/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Composer API.`_
+3. `Enable the Cloud Composer.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Composer API.:  https://cloud.google.com/composer/
+.. _Enable the Cloud Composer.:  https://cloud.google.com/composer/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-orchestration-airflow
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Composer API
+-  Read the `Client Library Documentation`_ for Cloud Composer
    to see other available methods on the client.
--  Read the `Cloud Composer API Product documentation`_ to learn
+-  Read the `Cloud Composer Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Composer API Product documentation:  https://cloud.google.com/composer/
+.. _Cloud Composer Product documentation:  https://cloud.google.com/composer/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/google_cloud_orchestration_airflow.egg-info/SOURCES.txt` & `google-cloud-orchestration-airflow-1.9.0/google_cloud_orchestration_airflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/setup.py` & `google-cloud-orchestration-airflow-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-orchestration-airflow"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/tests/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/tests/unit/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/tests/unit/gapic/service_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1/test_environments.py` & `google-cloud-orchestration-airflow-1.9.0/tests/unit/gapic/service_v1/test_environments.py`

 * *Files 16% similar despite different names*

```diff
@@ -2133,14 +2133,511 @@
             name="name_value",
         )
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
+        environments.ExecuteAirflowCommandRequest,
+        dict,
+    ],
+)
+def test_execute_airflow_command(request_type, transport: str = "grpc"):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.execute_airflow_command), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = environments.ExecuteAirflowCommandResponse(
+            execution_id="execution_id_value",
+            pod="pod_value",
+            pod_namespace="pod_namespace_value",
+            error="error_value",
+        )
+        response = client.execute_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.ExecuteAirflowCommandRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.ExecuteAirflowCommandResponse)
+    assert response.execution_id == "execution_id_value"
+    assert response.pod == "pod_value"
+    assert response.pod_namespace == "pod_namespace_value"
+    assert response.error == "error_value"
+
+
+def test_execute_airflow_command_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.execute_airflow_command), "__call__"
+    ) as call:
+        client.execute_airflow_command()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.ExecuteAirflowCommandRequest()
+
+
+@pytest.mark.asyncio
+async def test_execute_airflow_command_async(
+    transport: str = "grpc_asyncio",
+    request_type=environments.ExecuteAirflowCommandRequest,
+):
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.execute_airflow_command), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            environments.ExecuteAirflowCommandResponse(
+                execution_id="execution_id_value",
+                pod="pod_value",
+                pod_namespace="pod_namespace_value",
+                error="error_value",
+            )
+        )
+        response = await client.execute_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.ExecuteAirflowCommandRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.ExecuteAirflowCommandResponse)
+    assert response.execution_id == "execution_id_value"
+    assert response.pod == "pod_value"
+    assert response.pod_namespace == "pod_namespace_value"
+    assert response.error == "error_value"
+
+
+@pytest.mark.asyncio
+async def test_execute_airflow_command_async_from_dict():
+    await test_execute_airflow_command_async(request_type=dict)
+
+
+def test_execute_airflow_command_field_headers():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.ExecuteAirflowCommandRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.execute_airflow_command), "__call__"
+    ) as call:
+        call.return_value = environments.ExecuteAirflowCommandResponse()
+        client.execute_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_execute_airflow_command_field_headers_async():
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.ExecuteAirflowCommandRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.execute_airflow_command), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            environments.ExecuteAirflowCommandResponse()
+        )
+        await client.execute_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        environments.StopAirflowCommandRequest,
+        dict,
+    ],
+)
+def test_stop_airflow_command(request_type, transport: str = "grpc"):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.stop_airflow_command), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = environments.StopAirflowCommandResponse(
+            is_done=True,
+            output=["output_value"],
+        )
+        response = client.stop_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.StopAirflowCommandRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.StopAirflowCommandResponse)
+    assert response.is_done is True
+    assert response.output == ["output_value"]
+
+
+def test_stop_airflow_command_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.stop_airflow_command), "__call__"
+    ) as call:
+        client.stop_airflow_command()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.StopAirflowCommandRequest()
+
+
+@pytest.mark.asyncio
+async def test_stop_airflow_command_async(
+    transport: str = "grpc_asyncio", request_type=environments.StopAirflowCommandRequest
+):
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.stop_airflow_command), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            environments.StopAirflowCommandResponse(
+                is_done=True,
+                output=["output_value"],
+            )
+        )
+        response = await client.stop_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.StopAirflowCommandRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.StopAirflowCommandResponse)
+    assert response.is_done is True
+    assert response.output == ["output_value"]
+
+
+@pytest.mark.asyncio
+async def test_stop_airflow_command_async_from_dict():
+    await test_stop_airflow_command_async(request_type=dict)
+
+
+def test_stop_airflow_command_field_headers():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.StopAirflowCommandRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.stop_airflow_command), "__call__"
+    ) as call:
+        call.return_value = environments.StopAirflowCommandResponse()
+        client.stop_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_stop_airflow_command_field_headers_async():
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.StopAirflowCommandRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.stop_airflow_command), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            environments.StopAirflowCommandResponse()
+        )
+        await client.stop_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        environments.PollAirflowCommandRequest,
+        dict,
+    ],
+)
+def test_poll_airflow_command(request_type, transport: str = "grpc"):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.poll_airflow_command), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = environments.PollAirflowCommandResponse(
+            output_end=True,
+        )
+        response = client.poll_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.PollAirflowCommandRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.PollAirflowCommandResponse)
+    assert response.output_end is True
+
+
+def test_poll_airflow_command_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.poll_airflow_command), "__call__"
+    ) as call:
+        client.poll_airflow_command()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.PollAirflowCommandRequest()
+
+
+@pytest.mark.asyncio
+async def test_poll_airflow_command_async(
+    transport: str = "grpc_asyncio", request_type=environments.PollAirflowCommandRequest
+):
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.poll_airflow_command), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            environments.PollAirflowCommandResponse(
+                output_end=True,
+            )
+        )
+        response = await client.poll_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.PollAirflowCommandRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.PollAirflowCommandResponse)
+    assert response.output_end is True
+
+
+@pytest.mark.asyncio
+async def test_poll_airflow_command_async_from_dict():
+    await test_poll_airflow_command_async(request_type=dict)
+
+
+def test_poll_airflow_command_field_headers():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.PollAirflowCommandRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.poll_airflow_command), "__call__"
+    ) as call:
+        call.return_value = environments.PollAirflowCommandResponse()
+        client.poll_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_poll_airflow_command_field_headers_async():
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.PollAirflowCommandRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.poll_airflow_command), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            environments.PollAirflowCommandResponse()
+        )
+        await client.poll_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
         environments.SaveSnapshotRequest,
         dict,
     ],
 )
 def test_save_snapshot(request_type, transport: str = "grpc"):
     client = EnvironmentsClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2421,14 +2918,337 @@
         "environment=environment_value",
     ) in kw["metadata"]
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
+        environments.DatabaseFailoverRequest,
+        dict,
+    ],
+)
+def test_database_failover(request_type, transport: str = "grpc"):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.database_failover), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation(name="operations/spam")
+        response = client.database_failover(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.DatabaseFailoverRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+def test_database_failover_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.database_failover), "__call__"
+    ) as call:
+        client.database_failover()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.DatabaseFailoverRequest()
+
+
+@pytest.mark.asyncio
+async def test_database_failover_async(
+    transport: str = "grpc_asyncio", request_type=environments.DatabaseFailoverRequest
+):
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.database_failover), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.database_failover(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.DatabaseFailoverRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+@pytest.mark.asyncio
+async def test_database_failover_async_from_dict():
+    await test_database_failover_async(request_type=dict)
+
+
+def test_database_failover_field_headers():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.DatabaseFailoverRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.database_failover), "__call__"
+    ) as call:
+        call.return_value = operations_pb2.Operation(name="operations/op")
+        client.database_failover(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_database_failover_field_headers_async():
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.DatabaseFailoverRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.database_failover), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/op")
+        )
+        await client.database_failover(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        environments.FetchDatabasePropertiesRequest,
+        dict,
+    ],
+)
+def test_fetch_database_properties(request_type, transport: str = "grpc"):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.fetch_database_properties), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = environments.FetchDatabasePropertiesResponse(
+            primary_gce_zone="primary_gce_zone_value",
+            secondary_gce_zone="secondary_gce_zone_value",
+            is_failover_replica_available=True,
+        )
+        response = client.fetch_database_properties(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.FetchDatabasePropertiesRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.FetchDatabasePropertiesResponse)
+    assert response.primary_gce_zone == "primary_gce_zone_value"
+    assert response.secondary_gce_zone == "secondary_gce_zone_value"
+    assert response.is_failover_replica_available is True
+
+
+def test_fetch_database_properties_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.fetch_database_properties), "__call__"
+    ) as call:
+        client.fetch_database_properties()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.FetchDatabasePropertiesRequest()
+
+
+@pytest.mark.asyncio
+async def test_fetch_database_properties_async(
+    transport: str = "grpc_asyncio",
+    request_type=environments.FetchDatabasePropertiesRequest,
+):
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.fetch_database_properties), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            environments.FetchDatabasePropertiesResponse(
+                primary_gce_zone="primary_gce_zone_value",
+                secondary_gce_zone="secondary_gce_zone_value",
+                is_failover_replica_available=True,
+            )
+        )
+        response = await client.fetch_database_properties(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.FetchDatabasePropertiesRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.FetchDatabasePropertiesResponse)
+    assert response.primary_gce_zone == "primary_gce_zone_value"
+    assert response.secondary_gce_zone == "secondary_gce_zone_value"
+    assert response.is_failover_replica_available is True
+
+
+@pytest.mark.asyncio
+async def test_fetch_database_properties_async_from_dict():
+    await test_fetch_database_properties_async(request_type=dict)
+
+
+def test_fetch_database_properties_field_headers():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.FetchDatabasePropertiesRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.fetch_database_properties), "__call__"
+    ) as call:
+        call.return_value = environments.FetchDatabasePropertiesResponse()
+        client.fetch_database_properties(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_fetch_database_properties_field_headers_async():
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.FetchDatabasePropertiesRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.fetch_database_properties), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            environments.FetchDatabasePropertiesResponse()
+        )
+        await client.fetch_database_properties(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
         environments.CreateEnvironmentRequest,
         dict,
     ],
 )
 def test_create_environment_rest(request_type):
     client = EnvironmentsClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2530,14 +3350,15 @@
                 "scheduled_snapshots_config": {
                     "enabled": True,
                     "snapshot_location": "snapshot_location_value",
                     "snapshot_creation_schedule": "snapshot_creation_schedule_value",
                     "time_zone": "time_zone_value",
                 }
             },
+            "resilience_mode": 1,
         },
         "uuid": "uuid_value",
         "state": 1,
         "create_time": {},
         "update_time": {},
         "labels": {},
     }
@@ -2723,14 +3544,15 @@
                 "scheduled_snapshots_config": {
                     "enabled": True,
                     "snapshot_location": "snapshot_location_value",
                     "snapshot_creation_schedule": "snapshot_creation_schedule_value",
                     "time_zone": "time_zone_value",
                 }
             },
+            "resilience_mode": 1,
         },
         "uuid": "uuid_value",
         "state": 1,
         "create_time": {},
         "update_time": {},
         "labels": {},
     }
@@ -3346,14 +4168,15 @@
                 "scheduled_snapshots_config": {
                     "enabled": True,
                     "snapshot_location": "snapshot_location_value",
                     "snapshot_creation_schedule": "snapshot_creation_schedule_value",
                     "time_zone": "time_zone_value",
                 }
             },
+            "resilience_mode": 1,
         },
         "uuid": "uuid_value",
         "state": 1,
         "create_time": {},
         "update_time": {},
         "labels": {},
     }
@@ -3539,14 +4362,15 @@
                 "scheduled_snapshots_config": {
                     "enabled": True,
                     "snapshot_location": "snapshot_location_value",
                     "snapshot_creation_schedule": "snapshot_creation_schedule_value",
                     "time_zone": "time_zone_value",
                 }
             },
+            "resilience_mode": 1,
         },
         "uuid": "uuid_value",
         "state": 1,
         "create_time": {},
         "update_time": {},
         "labels": {},
     }
@@ -3811,14 +4635,412 @@
         credentials=ga_credentials.AnonymousCredentials(), transport="rest"
     )
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
+        environments.ExecuteAirflowCommandRequest,
+        dict,
+    ],
+)
+def test_execute_airflow_command_rest(request_type):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = environments.ExecuteAirflowCommandResponse(
+            execution_id="execution_id_value",
+            pod="pod_value",
+            pod_namespace="pod_namespace_value",
+            error="error_value",
+        )
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = environments.ExecuteAirflowCommandResponse.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.execute_airflow_command(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.ExecuteAirflowCommandResponse)
+    assert response.execution_id == "execution_id_value"
+    assert response.pod == "pod_value"
+    assert response.pod_namespace == "pod_namespace_value"
+    assert response.error == "error_value"
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_execute_airflow_command_rest_interceptors(null_interceptor):
+    transport = transports.EnvironmentsRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.EnvironmentsRestInterceptor(),
+    )
+    client = EnvironmentsClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "post_execute_airflow_command"
+    ) as post, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "pre_execute_airflow_command"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = environments.ExecuteAirflowCommandRequest.pb(
+            environments.ExecuteAirflowCommandRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = environments.ExecuteAirflowCommandResponse.to_json(
+            environments.ExecuteAirflowCommandResponse()
+        )
+
+        request = environments.ExecuteAirflowCommandRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = environments.ExecuteAirflowCommandResponse()
+
+        client.execute_airflow_command(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_execute_airflow_command_rest_bad_request(
+    transport: str = "rest", request_type=environments.ExecuteAirflowCommandRequest
+):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.execute_airflow_command(request)
+
+
+def test_execute_airflow_command_rest_error():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        environments.StopAirflowCommandRequest,
+        dict,
+    ],
+)
+def test_stop_airflow_command_rest(request_type):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = environments.StopAirflowCommandResponse(
+            is_done=True,
+            output=["output_value"],
+        )
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = environments.StopAirflowCommandResponse.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.stop_airflow_command(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.StopAirflowCommandResponse)
+    assert response.is_done is True
+    assert response.output == ["output_value"]
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_stop_airflow_command_rest_interceptors(null_interceptor):
+    transport = transports.EnvironmentsRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.EnvironmentsRestInterceptor(),
+    )
+    client = EnvironmentsClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "post_stop_airflow_command"
+    ) as post, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "pre_stop_airflow_command"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = environments.StopAirflowCommandRequest.pb(
+            environments.StopAirflowCommandRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = environments.StopAirflowCommandResponse.to_json(
+            environments.StopAirflowCommandResponse()
+        )
+
+        request = environments.StopAirflowCommandRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = environments.StopAirflowCommandResponse()
+
+        client.stop_airflow_command(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_stop_airflow_command_rest_bad_request(
+    transport: str = "rest", request_type=environments.StopAirflowCommandRequest
+):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.stop_airflow_command(request)
+
+
+def test_stop_airflow_command_rest_error():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        environments.PollAirflowCommandRequest,
+        dict,
+    ],
+)
+def test_poll_airflow_command_rest(request_type):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = environments.PollAirflowCommandResponse(
+            output_end=True,
+        )
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = environments.PollAirflowCommandResponse.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.poll_airflow_command(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.PollAirflowCommandResponse)
+    assert response.output_end is True
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_poll_airflow_command_rest_interceptors(null_interceptor):
+    transport = transports.EnvironmentsRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.EnvironmentsRestInterceptor(),
+    )
+    client = EnvironmentsClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "post_poll_airflow_command"
+    ) as post, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "pre_poll_airflow_command"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = environments.PollAirflowCommandRequest.pb(
+            environments.PollAirflowCommandRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = environments.PollAirflowCommandResponse.to_json(
+            environments.PollAirflowCommandResponse()
+        )
+
+        request = environments.PollAirflowCommandRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = environments.PollAirflowCommandResponse()
+
+        client.poll_airflow_command(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_poll_airflow_command_rest_bad_request(
+    transport: str = "rest", request_type=environments.PollAirflowCommandRequest
+):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.poll_airflow_command(request)
+
+
+def test_poll_airflow_command_rest_error():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
         environments.SaveSnapshotRequest,
         dict,
     ],
 )
 def test_save_snapshot_rest(request_type):
     client = EnvironmentsClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -4064,14 +5286,366 @@
 
 def test_load_snapshot_rest_error():
     client = EnvironmentsClient(
         credentials=ga_credentials.AnonymousCredentials(), transport="rest"
     )
 
 
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        environments.DatabaseFailoverRequest,
+        dict,
+    ],
+)
+def test_database_failover_rest(request_type):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = operations_pb2.Operation(name="operations/spam")
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.database_failover(request)
+
+    # Establish that the response is the type that we expect.
+    assert response.operation.name == "operations/spam"
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_database_failover_rest_interceptors(null_interceptor):
+    transport = transports.EnvironmentsRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.EnvironmentsRestInterceptor(),
+    )
+    client = EnvironmentsClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        operation.Operation, "_set_result_from_operation"
+    ), mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "post_database_failover"
+    ) as post, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "pre_database_failover"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = environments.DatabaseFailoverRequest.pb(
+            environments.DatabaseFailoverRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = json_format.MessageToJson(
+            operations_pb2.Operation()
+        )
+
+        request = environments.DatabaseFailoverRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = operations_pb2.Operation()
+
+        client.database_failover(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_database_failover_rest_bad_request(
+    transport: str = "rest", request_type=environments.DatabaseFailoverRequest
+):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.database_failover(request)
+
+
+def test_database_failover_rest_error():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        environments.FetchDatabasePropertiesRequest,
+        dict,
+    ],
+)
+def test_fetch_database_properties_rest(request_type):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = environments.FetchDatabasePropertiesResponse(
+            primary_gce_zone="primary_gce_zone_value",
+            secondary_gce_zone="secondary_gce_zone_value",
+            is_failover_replica_available=True,
+        )
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = environments.FetchDatabasePropertiesResponse.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.fetch_database_properties(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.FetchDatabasePropertiesResponse)
+    assert response.primary_gce_zone == "primary_gce_zone_value"
+    assert response.secondary_gce_zone == "secondary_gce_zone_value"
+    assert response.is_failover_replica_available is True
+
+
+def test_fetch_database_properties_rest_required_fields(
+    request_type=environments.FetchDatabasePropertiesRequest,
+):
+    transport_class = transports.EnvironmentsRestTransport
+
+    request_init = {}
+    request_init["environment"] = ""
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(
+            pb_request,
+            including_default_value_fields=False,
+            use_integers_for_enums=False,
+        )
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).fetch_database_properties._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    jsonified_request["environment"] = "environment_value"
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).fetch_database_properties._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+    assert "environment" in jsonified_request
+    assert jsonified_request["environment"] == "environment_value"
+
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = environments.FetchDatabasePropertiesResponse()
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "get",
+                "query_params": pb_request,
+            }
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+
+            pb_return_value = environments.FetchDatabasePropertiesResponse.pb(
+                return_value
+            )
+            json_return_value = json_format.MessageToJson(pb_return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.fetch_database_properties(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_fetch_database_properties_rest_unset_required_fields():
+    transport = transports.EnvironmentsRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.fetch_database_properties._get_unset_required_fields({})
+    assert set(unset_fields) == (set(()) & set(("environment",)))
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_fetch_database_properties_rest_interceptors(null_interceptor):
+    transport = transports.EnvironmentsRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.EnvironmentsRestInterceptor(),
+    )
+    client = EnvironmentsClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "post_fetch_database_properties"
+    ) as post, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "pre_fetch_database_properties"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = environments.FetchDatabasePropertiesRequest.pb(
+            environments.FetchDatabasePropertiesRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = (
+            environments.FetchDatabasePropertiesResponse.to_json(
+                environments.FetchDatabasePropertiesResponse()
+            )
+        )
+
+        request = environments.FetchDatabasePropertiesRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = environments.FetchDatabasePropertiesResponse()
+
+        client.fetch_database_properties(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_fetch_database_properties_rest_bad_request(
+    transport: str = "rest", request_type=environments.FetchDatabasePropertiesRequest
+):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.fetch_database_properties(request)
+
+
+def test_fetch_database_properties_rest_error():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
     transport = transports.EnvironmentsGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = EnvironmentsClient(
@@ -4208,16 +5782,21 @@
     # raise NotImplementedError.
     methods = (
         "create_environment",
         "get_environment",
         "list_environments",
         "update_environment",
         "delete_environment",
+        "execute_airflow_command",
+        "stop_airflow_command",
+        "poll_airflow_command",
         "save_snapshot",
         "load_snapshot",
+        "database_failover",
+        "fetch_database_properties",
         "get_operation",
         "delete_operation",
         "list_operations",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
@@ -4505,20 +6084,35 @@
     assert session1 != session2
     session1 = client1.transport.update_environment._session
     session2 = client2.transport.update_environment._session
     assert session1 != session2
     session1 = client1.transport.delete_environment._session
     session2 = client2.transport.delete_environment._session
     assert session1 != session2
+    session1 = client1.transport.execute_airflow_command._session
+    session2 = client2.transport.execute_airflow_command._session
+    assert session1 != session2
+    session1 = client1.transport.stop_airflow_command._session
+    session2 = client2.transport.stop_airflow_command._session
+    assert session1 != session2
+    session1 = client1.transport.poll_airflow_command._session
+    session2 = client2.transport.poll_airflow_command._session
+    assert session1 != session2
     session1 = client1.transport.save_snapshot._session
     session2 = client2.transport.save_snapshot._session
     assert session1 != session2
     session1 = client1.transport.load_snapshot._session
     session2 = client2.transport.load_snapshot._session
     assert session1 != session2
+    session1 = client1.transport.database_failover._session
+    session2 = client2.transport.database_failover._session
+    assert session1 != session2
+    session1 = client1.transport.fetch_database_properties._session
+    session2 = client2.transport.fetch_database_properties._session
+    assert session1 != session2
 
 
 def test_environments_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.EnvironmentsGrpcTransport(
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1/test_image_versions.py` & `google-cloud-orchestration-airflow-1.9.0/tests/unit/gapic/service_v1/test_image_versions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1beta1/__init__.py` & `google-cloud-orchestration-airflow-1.9.0/tests/unit/gapic/service_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1beta1/test_environments.py` & `google-cloud-orchestration-airflow-1.9.0/tests/unit/gapic/service_v1beta1/test_environments.py`

 * *Files 13% similar despite different names*

```diff
@@ -2434,14 +2434,511 @@
         "environment=environment_value",
     ) in kw["metadata"]
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
+        environments.ExecuteAirflowCommandRequest,
+        dict,
+    ],
+)
+def test_execute_airflow_command(request_type, transport: str = "grpc"):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.execute_airflow_command), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = environments.ExecuteAirflowCommandResponse(
+            execution_id="execution_id_value",
+            pod="pod_value",
+            pod_namespace="pod_namespace_value",
+            error="error_value",
+        )
+        response = client.execute_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.ExecuteAirflowCommandRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.ExecuteAirflowCommandResponse)
+    assert response.execution_id == "execution_id_value"
+    assert response.pod == "pod_value"
+    assert response.pod_namespace == "pod_namespace_value"
+    assert response.error == "error_value"
+
+
+def test_execute_airflow_command_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.execute_airflow_command), "__call__"
+    ) as call:
+        client.execute_airflow_command()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.ExecuteAirflowCommandRequest()
+
+
+@pytest.mark.asyncio
+async def test_execute_airflow_command_async(
+    transport: str = "grpc_asyncio",
+    request_type=environments.ExecuteAirflowCommandRequest,
+):
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.execute_airflow_command), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            environments.ExecuteAirflowCommandResponse(
+                execution_id="execution_id_value",
+                pod="pod_value",
+                pod_namespace="pod_namespace_value",
+                error="error_value",
+            )
+        )
+        response = await client.execute_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.ExecuteAirflowCommandRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.ExecuteAirflowCommandResponse)
+    assert response.execution_id == "execution_id_value"
+    assert response.pod == "pod_value"
+    assert response.pod_namespace == "pod_namespace_value"
+    assert response.error == "error_value"
+
+
+@pytest.mark.asyncio
+async def test_execute_airflow_command_async_from_dict():
+    await test_execute_airflow_command_async(request_type=dict)
+
+
+def test_execute_airflow_command_field_headers():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.ExecuteAirflowCommandRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.execute_airflow_command), "__call__"
+    ) as call:
+        call.return_value = environments.ExecuteAirflowCommandResponse()
+        client.execute_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_execute_airflow_command_field_headers_async():
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.ExecuteAirflowCommandRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.execute_airflow_command), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            environments.ExecuteAirflowCommandResponse()
+        )
+        await client.execute_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        environments.StopAirflowCommandRequest,
+        dict,
+    ],
+)
+def test_stop_airflow_command(request_type, transport: str = "grpc"):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.stop_airflow_command), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = environments.StopAirflowCommandResponse(
+            is_done=True,
+            output=["output_value"],
+        )
+        response = client.stop_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.StopAirflowCommandRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.StopAirflowCommandResponse)
+    assert response.is_done is True
+    assert response.output == ["output_value"]
+
+
+def test_stop_airflow_command_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.stop_airflow_command), "__call__"
+    ) as call:
+        client.stop_airflow_command()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.StopAirflowCommandRequest()
+
+
+@pytest.mark.asyncio
+async def test_stop_airflow_command_async(
+    transport: str = "grpc_asyncio", request_type=environments.StopAirflowCommandRequest
+):
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.stop_airflow_command), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            environments.StopAirflowCommandResponse(
+                is_done=True,
+                output=["output_value"],
+            )
+        )
+        response = await client.stop_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.StopAirflowCommandRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.StopAirflowCommandResponse)
+    assert response.is_done is True
+    assert response.output == ["output_value"]
+
+
+@pytest.mark.asyncio
+async def test_stop_airflow_command_async_from_dict():
+    await test_stop_airflow_command_async(request_type=dict)
+
+
+def test_stop_airflow_command_field_headers():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.StopAirflowCommandRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.stop_airflow_command), "__call__"
+    ) as call:
+        call.return_value = environments.StopAirflowCommandResponse()
+        client.stop_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_stop_airflow_command_field_headers_async():
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.StopAirflowCommandRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.stop_airflow_command), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            environments.StopAirflowCommandResponse()
+        )
+        await client.stop_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        environments.PollAirflowCommandRequest,
+        dict,
+    ],
+)
+def test_poll_airflow_command(request_type, transport: str = "grpc"):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.poll_airflow_command), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = environments.PollAirflowCommandResponse(
+            output_end=True,
+        )
+        response = client.poll_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.PollAirflowCommandRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.PollAirflowCommandResponse)
+    assert response.output_end is True
+
+
+def test_poll_airflow_command_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.poll_airflow_command), "__call__"
+    ) as call:
+        client.poll_airflow_command()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.PollAirflowCommandRequest()
+
+
+@pytest.mark.asyncio
+async def test_poll_airflow_command_async(
+    transport: str = "grpc_asyncio", request_type=environments.PollAirflowCommandRequest
+):
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.poll_airflow_command), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            environments.PollAirflowCommandResponse(
+                output_end=True,
+            )
+        )
+        response = await client.poll_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.PollAirflowCommandRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.PollAirflowCommandResponse)
+    assert response.output_end is True
+
+
+@pytest.mark.asyncio
+async def test_poll_airflow_command_async_from_dict():
+    await test_poll_airflow_command_async(request_type=dict)
+
+
+def test_poll_airflow_command_field_headers():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.PollAirflowCommandRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.poll_airflow_command), "__call__"
+    ) as call:
+        call.return_value = environments.PollAirflowCommandResponse()
+        client.poll_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_poll_airflow_command_field_headers_async():
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.PollAirflowCommandRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.poll_airflow_command), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            environments.PollAirflowCommandResponse()
+        )
+        await client.poll_airflow_command(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
         environments.SaveSnapshotRequest,
         dict,
     ],
 )
 def test_save_snapshot(request_type, transport: str = "grpc"):
     client = EnvironmentsClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2722,14 +3219,337 @@
         "environment=environment_value",
     ) in kw["metadata"]
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
+        environments.DatabaseFailoverRequest,
+        dict,
+    ],
+)
+def test_database_failover(request_type, transport: str = "grpc"):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.database_failover), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation(name="operations/spam")
+        response = client.database_failover(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.DatabaseFailoverRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+def test_database_failover_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.database_failover), "__call__"
+    ) as call:
+        client.database_failover()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.DatabaseFailoverRequest()
+
+
+@pytest.mark.asyncio
+async def test_database_failover_async(
+    transport: str = "grpc_asyncio", request_type=environments.DatabaseFailoverRequest
+):
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.database_failover), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.database_failover(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.DatabaseFailoverRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+@pytest.mark.asyncio
+async def test_database_failover_async_from_dict():
+    await test_database_failover_async(request_type=dict)
+
+
+def test_database_failover_field_headers():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.DatabaseFailoverRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.database_failover), "__call__"
+    ) as call:
+        call.return_value = operations_pb2.Operation(name="operations/op")
+        client.database_failover(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_database_failover_field_headers_async():
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.DatabaseFailoverRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.database_failover), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/op")
+        )
+        await client.database_failover(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        environments.FetchDatabasePropertiesRequest,
+        dict,
+    ],
+)
+def test_fetch_database_properties(request_type, transport: str = "grpc"):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.fetch_database_properties), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = environments.FetchDatabasePropertiesResponse(
+            primary_gce_zone="primary_gce_zone_value",
+            secondary_gce_zone="secondary_gce_zone_value",
+            is_failover_replica_available=True,
+        )
+        response = client.fetch_database_properties(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.FetchDatabasePropertiesRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.FetchDatabasePropertiesResponse)
+    assert response.primary_gce_zone == "primary_gce_zone_value"
+    assert response.secondary_gce_zone == "secondary_gce_zone_value"
+    assert response.is_failover_replica_available is True
+
+
+def test_fetch_database_properties_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.fetch_database_properties), "__call__"
+    ) as call:
+        client.fetch_database_properties()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.FetchDatabasePropertiesRequest()
+
+
+@pytest.mark.asyncio
+async def test_fetch_database_properties_async(
+    transport: str = "grpc_asyncio",
+    request_type=environments.FetchDatabasePropertiesRequest,
+):
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.fetch_database_properties), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            environments.FetchDatabasePropertiesResponse(
+                primary_gce_zone="primary_gce_zone_value",
+                secondary_gce_zone="secondary_gce_zone_value",
+                is_failover_replica_available=True,
+            )
+        )
+        response = await client.fetch_database_properties(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == environments.FetchDatabasePropertiesRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.FetchDatabasePropertiesResponse)
+    assert response.primary_gce_zone == "primary_gce_zone_value"
+    assert response.secondary_gce_zone == "secondary_gce_zone_value"
+    assert response.is_failover_replica_available is True
+
+
+@pytest.mark.asyncio
+async def test_fetch_database_properties_async_from_dict():
+    await test_fetch_database_properties_async(request_type=dict)
+
+
+def test_fetch_database_properties_field_headers():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.FetchDatabasePropertiesRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.fetch_database_properties), "__call__"
+    ) as call:
+        call.return_value = environments.FetchDatabasePropertiesResponse()
+        client.fetch_database_properties(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_fetch_database_properties_field_headers_async():
+    client = EnvironmentsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = environments.FetchDatabasePropertiesRequest()
+
+    request.environment = "environment_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.fetch_database_properties), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            environments.FetchDatabasePropertiesResponse()
+        )
+        await client.fetch_database_properties(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "environment=environment_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
         environments.CreateEnvironmentRequest,
         dict,
     ],
 )
 def test_create_environment_rest(request_type):
     client = EnvironmentsClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2834,14 +3654,15 @@
                 "scheduled_snapshots_config": {
                     "enabled": True,
                     "snapshot_location": "snapshot_location_value",
                     "snapshot_creation_schedule": "snapshot_creation_schedule_value",
                     "time_zone": "time_zone_value",
                 }
             },
+            "resilience_mode": 1,
         },
         "uuid": "uuid_value",
         "state": 1,
         "create_time": {},
         "update_time": {},
         "labels": {},
     }
@@ -3030,14 +3851,15 @@
                 "scheduled_snapshots_config": {
                     "enabled": True,
                     "snapshot_location": "snapshot_location_value",
                     "snapshot_creation_schedule": "snapshot_creation_schedule_value",
                     "time_zone": "time_zone_value",
                 }
             },
+            "resilience_mode": 1,
         },
         "uuid": "uuid_value",
         "state": 1,
         "create_time": {},
         "update_time": {},
         "labels": {},
     }
@@ -3656,14 +4478,15 @@
                 "scheduled_snapshots_config": {
                     "enabled": True,
                     "snapshot_location": "snapshot_location_value",
                     "snapshot_creation_schedule": "snapshot_creation_schedule_value",
                     "time_zone": "time_zone_value",
                 }
             },
+            "resilience_mode": 1,
         },
         "uuid": "uuid_value",
         "state": 1,
         "create_time": {},
         "update_time": {},
         "labels": {},
     }
@@ -3934,14 +4757,15 @@
                 "scheduled_snapshots_config": {
                     "enabled": True,
                     "snapshot_location": "snapshot_location_value",
                     "snapshot_creation_schedule": "snapshot_creation_schedule_value",
                     "time_zone": "time_zone_value",
                 }
             },
+            "resilience_mode": 1,
         },
         "uuid": "uuid_value",
         "state": 1,
         "create_time": {},
         "update_time": {},
         "labels": {},
     }
@@ -4458,14 +5282,412 @@
         credentials=ga_credentials.AnonymousCredentials(), transport="rest"
     )
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
+        environments.ExecuteAirflowCommandRequest,
+        dict,
+    ],
+)
+def test_execute_airflow_command_rest(request_type):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = environments.ExecuteAirflowCommandResponse(
+            execution_id="execution_id_value",
+            pod="pod_value",
+            pod_namespace="pod_namespace_value",
+            error="error_value",
+        )
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = environments.ExecuteAirflowCommandResponse.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.execute_airflow_command(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.ExecuteAirflowCommandResponse)
+    assert response.execution_id == "execution_id_value"
+    assert response.pod == "pod_value"
+    assert response.pod_namespace == "pod_namespace_value"
+    assert response.error == "error_value"
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_execute_airflow_command_rest_interceptors(null_interceptor):
+    transport = transports.EnvironmentsRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.EnvironmentsRestInterceptor(),
+    )
+    client = EnvironmentsClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "post_execute_airflow_command"
+    ) as post, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "pre_execute_airflow_command"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = environments.ExecuteAirflowCommandRequest.pb(
+            environments.ExecuteAirflowCommandRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = environments.ExecuteAirflowCommandResponse.to_json(
+            environments.ExecuteAirflowCommandResponse()
+        )
+
+        request = environments.ExecuteAirflowCommandRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = environments.ExecuteAirflowCommandResponse()
+
+        client.execute_airflow_command(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_execute_airflow_command_rest_bad_request(
+    transport: str = "rest", request_type=environments.ExecuteAirflowCommandRequest
+):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.execute_airflow_command(request)
+
+
+def test_execute_airflow_command_rest_error():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        environments.StopAirflowCommandRequest,
+        dict,
+    ],
+)
+def test_stop_airflow_command_rest(request_type):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = environments.StopAirflowCommandResponse(
+            is_done=True,
+            output=["output_value"],
+        )
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = environments.StopAirflowCommandResponse.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.stop_airflow_command(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.StopAirflowCommandResponse)
+    assert response.is_done is True
+    assert response.output == ["output_value"]
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_stop_airflow_command_rest_interceptors(null_interceptor):
+    transport = transports.EnvironmentsRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.EnvironmentsRestInterceptor(),
+    )
+    client = EnvironmentsClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "post_stop_airflow_command"
+    ) as post, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "pre_stop_airflow_command"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = environments.StopAirflowCommandRequest.pb(
+            environments.StopAirflowCommandRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = environments.StopAirflowCommandResponse.to_json(
+            environments.StopAirflowCommandResponse()
+        )
+
+        request = environments.StopAirflowCommandRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = environments.StopAirflowCommandResponse()
+
+        client.stop_airflow_command(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_stop_airflow_command_rest_bad_request(
+    transport: str = "rest", request_type=environments.StopAirflowCommandRequest
+):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.stop_airflow_command(request)
+
+
+def test_stop_airflow_command_rest_error():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        environments.PollAirflowCommandRequest,
+        dict,
+    ],
+)
+def test_poll_airflow_command_rest(request_type):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = environments.PollAirflowCommandResponse(
+            output_end=True,
+        )
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = environments.PollAirflowCommandResponse.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.poll_airflow_command(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.PollAirflowCommandResponse)
+    assert response.output_end is True
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_poll_airflow_command_rest_interceptors(null_interceptor):
+    transport = transports.EnvironmentsRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.EnvironmentsRestInterceptor(),
+    )
+    client = EnvironmentsClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "post_poll_airflow_command"
+    ) as post, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "pre_poll_airflow_command"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = environments.PollAirflowCommandRequest.pb(
+            environments.PollAirflowCommandRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = environments.PollAirflowCommandResponse.to_json(
+            environments.PollAirflowCommandResponse()
+        )
+
+        request = environments.PollAirflowCommandRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = environments.PollAirflowCommandResponse()
+
+        client.poll_airflow_command(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_poll_airflow_command_rest_bad_request(
+    transport: str = "rest", request_type=environments.PollAirflowCommandRequest
+):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.poll_airflow_command(request)
+
+
+def test_poll_airflow_command_rest_error():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
         environments.SaveSnapshotRequest,
         dict,
     ],
 )
 def test_save_snapshot_rest(request_type):
     client = EnvironmentsClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -4711,14 +5933,366 @@
 
 def test_load_snapshot_rest_error():
     client = EnvironmentsClient(
         credentials=ga_credentials.AnonymousCredentials(), transport="rest"
     )
 
 
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        environments.DatabaseFailoverRequest,
+        dict,
+    ],
+)
+def test_database_failover_rest(request_type):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = operations_pb2.Operation(name="operations/spam")
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.database_failover(request)
+
+    # Establish that the response is the type that we expect.
+    assert response.operation.name == "operations/spam"
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_database_failover_rest_interceptors(null_interceptor):
+    transport = transports.EnvironmentsRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.EnvironmentsRestInterceptor(),
+    )
+    client = EnvironmentsClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        operation.Operation, "_set_result_from_operation"
+    ), mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "post_database_failover"
+    ) as post, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "pre_database_failover"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = environments.DatabaseFailoverRequest.pb(
+            environments.DatabaseFailoverRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = json_format.MessageToJson(
+            operations_pb2.Operation()
+        )
+
+        request = environments.DatabaseFailoverRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = operations_pb2.Operation()
+
+        client.database_failover(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_database_failover_rest_bad_request(
+    transport: str = "rest", request_type=environments.DatabaseFailoverRequest
+):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.database_failover(request)
+
+
+def test_database_failover_rest_error():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        environments.FetchDatabasePropertiesRequest,
+        dict,
+    ],
+)
+def test_fetch_database_properties_rest(request_type):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = environments.FetchDatabasePropertiesResponse(
+            primary_gce_zone="primary_gce_zone_value",
+            secondary_gce_zone="secondary_gce_zone_value",
+            is_failover_replica_available=True,
+        )
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = environments.FetchDatabasePropertiesResponse.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.fetch_database_properties(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, environments.FetchDatabasePropertiesResponse)
+    assert response.primary_gce_zone == "primary_gce_zone_value"
+    assert response.secondary_gce_zone == "secondary_gce_zone_value"
+    assert response.is_failover_replica_available is True
+
+
+def test_fetch_database_properties_rest_required_fields(
+    request_type=environments.FetchDatabasePropertiesRequest,
+):
+    transport_class = transports.EnvironmentsRestTransport
+
+    request_init = {}
+    request_init["environment"] = ""
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(
+            pb_request,
+            including_default_value_fields=False,
+            use_integers_for_enums=False,
+        )
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).fetch_database_properties._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    jsonified_request["environment"] = "environment_value"
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).fetch_database_properties._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+    assert "environment" in jsonified_request
+    assert jsonified_request["environment"] == "environment_value"
+
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = environments.FetchDatabasePropertiesResponse()
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "get",
+                "query_params": pb_request,
+            }
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+
+            pb_return_value = environments.FetchDatabasePropertiesResponse.pb(
+                return_value
+            )
+            json_return_value = json_format.MessageToJson(pb_return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.fetch_database_properties(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_fetch_database_properties_rest_unset_required_fields():
+    transport = transports.EnvironmentsRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.fetch_database_properties._get_unset_required_fields({})
+    assert set(unset_fields) == (set(()) & set(("environment",)))
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_fetch_database_properties_rest_interceptors(null_interceptor):
+    transport = transports.EnvironmentsRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.EnvironmentsRestInterceptor(),
+    )
+    client = EnvironmentsClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "post_fetch_database_properties"
+    ) as post, mock.patch.object(
+        transports.EnvironmentsRestInterceptor, "pre_fetch_database_properties"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = environments.FetchDatabasePropertiesRequest.pb(
+            environments.FetchDatabasePropertiesRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = (
+            environments.FetchDatabasePropertiesResponse.to_json(
+                environments.FetchDatabasePropertiesResponse()
+            )
+        )
+
+        request = environments.FetchDatabasePropertiesRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = environments.FetchDatabasePropertiesResponse()
+
+        client.fetch_database_properties(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_fetch_database_properties_rest_bad_request(
+    transport: str = "rest", request_type=environments.FetchDatabasePropertiesRequest
+):
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "environment": "projects/sample1/locations/sample2/environments/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.fetch_database_properties(request)
+
+
+def test_fetch_database_properties_rest_error():
+    client = EnvironmentsClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
     transport = transports.EnvironmentsGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = EnvironmentsClient(
@@ -4857,16 +6431,21 @@
         "create_environment",
         "get_environment",
         "list_environments",
         "update_environment",
         "delete_environment",
         "restart_web_server",
         "check_upgrade",
+        "execute_airflow_command",
+        "stop_airflow_command",
+        "poll_airflow_command",
         "save_snapshot",
         "load_snapshot",
+        "database_failover",
+        "fetch_database_properties",
         "get_operation",
         "delete_operation",
         "list_operations",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
@@ -5160,20 +6739,35 @@
     assert session1 != session2
     session1 = client1.transport.restart_web_server._session
     session2 = client2.transport.restart_web_server._session
     assert session1 != session2
     session1 = client1.transport.check_upgrade._session
     session2 = client2.transport.check_upgrade._session
     assert session1 != session2
+    session1 = client1.transport.execute_airflow_command._session
+    session2 = client2.transport.execute_airflow_command._session
+    assert session1 != session2
+    session1 = client1.transport.stop_airflow_command._session
+    session2 = client2.transport.stop_airflow_command._session
+    assert session1 != session2
+    session1 = client1.transport.poll_airflow_command._session
+    session2 = client2.transport.poll_airflow_command._session
+    assert session1 != session2
     session1 = client1.transport.save_snapshot._session
     session2 = client2.transport.save_snapshot._session
     assert session1 != session2
     session1 = client1.transport.load_snapshot._session
     session2 = client2.transport.load_snapshot._session
     assert session1 != session2
+    session1 = client1.transport.database_failover._session
+    session2 = client2.transport.database_failover._session
+    assert session1 != session2
+    session1 = client1.transport.fetch_database_properties._session
+    session2 = client2.transport.fetch_database_properties._session
+    assert session1 != session2
 
 
 def test_environments_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.EnvironmentsGrpcTransport(
```

### Comparing `google-cloud-orchestration-airflow-1.8.0/tests/unit/gapic/service_v1beta1/test_image_versions.py` & `google-cloud-orchestration-airflow-1.9.0/tests/unit/gapic/service_v1beta1/test_image_versions.py`

 * *Files identical despite different names*

