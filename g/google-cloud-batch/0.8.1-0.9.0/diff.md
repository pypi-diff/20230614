# Comparing `tmp/google-cloud-batch-0.8.1.tar.gz` & `tmp/google-cloud-batch-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-batch-0.8.1.tar", last modified: Mon Jan 23 16:16:07 2023, max compression
+gzip compressed data, was "google-cloud-batch-0.9.0.tar", last modified: Tue Feb  7 15:53:52 2023, max compression
```

## Comparing `google-cloud-batch-0.8.1.tar` & `google-cloud-batch-0.9.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.552609 google-cloud-batch-0.8.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4377 2023-01-23 16:16:07.552609 google-cloud-batch-0.8.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3480 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.540607 google-cloud-batch-0.8.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.540607 google-cloud-batch-0.8.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.540607 google-cloud-batch-0.8.1/google/cloud/batch/
--rw-rw-r--   0 root         (0)     1003     2186 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       79 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.540607 google-cloud-batch-0.8.1/google/cloud/batch_v1/
--rw-rw-r--   0 root         (0)     1003     1996 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2660 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       79 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.544607 google-cloud-batch-0.8.1/google/cloud/batch_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.544607 google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/
--rw-rw-r--   0 root         (0)     1003      761 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    61801 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    71507 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/client.py
--rw-rw-r--   0 root         (0)     1003    10253 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.544607 google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11891 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    26369 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    26757 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    68232 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.544607 google-cloud-batch-0.8.1/google/cloud/batch_v1/types/
--rw-rw-r--   0 root         (0)     1003     1726 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    10221 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/types/batch.py
--rw-rw-r--   0 root         (0)     1003    30464 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/types/job.py
--rw-rw-r--   0 root         (0)     1003    19276 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/types/task.py
--rw-rw-r--   0 root         (0)     1003     4303 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1/types/volume.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.548608 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/
--rw-rw-r--   0 root         (0)     1003     2050 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003     2670 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       79 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.548608 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.548608 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/
--rw-rw-r--   0 root         (0)     1003      761 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    61981 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    71687 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/client.py
--rw-rw-r--   0 root         (0)     1003    10338 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.548608 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11916 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    26419 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    26807 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    68352 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.548608 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/types/
--rw-rw-r--   0 root         (0)     1003     1780 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    10251 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/types/batch.py
--rw-rw-r--   0 root         (0)     1003    37392 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/types/job.py
--rw-rw-r--   0 root         (0)     1003    19734 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/types/task.py
--rw-rw-r--   0 root         (0)     1003     5397 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/types/volume.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.552609 google-cloud-batch-0.8.1/google_cloud_batch.egg-info/
--rw-r--r--   0 root         (0)     1003     4377 2023-01-23 16:16:07.000000 google-cloud-batch-0.8.1/google_cloud_batch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2662 2023-01-23 16:16:07.000000 google-cloud-batch-0.8.1/google_cloud_batch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:16:07.000000 google-cloud-batch-0.8.1/google_cloud_batch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-23 16:16:07.000000 google-cloud-batch-0.8.1/google_cloud_batch.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:16:07.000000 google-cloud-batch-0.8.1/google_cloud_batch.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-01-23 16:16:07.000000 google-cloud-batch-0.8.1/google_cloud_batch.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-23 16:16:07.000000 google-cloud-batch-0.8.1/google_cloud_batch.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-23 16:16:07.556610 google-cloud-batch-0.8.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3014 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.552609 google-cloud-batch-0.8.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.552609 google-cloud-batch-0.8.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.552609 google-cloud-batch-0.8.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.552609 google-cloud-batch-0.8.1/tests/unit/gapic/batch_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/tests/unit/gapic/batch_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   251789 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/tests/unit/gapic/batch_v1/test_batch_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:16:07.552609 google-cloud-batch-0.8.1/tests/unit/gapic/batch_v1alpha/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/tests/unit/gapic/batch_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003   256064 2023-01-23 16:13:19.000000 google-cloud-batch-0.8.1/tests/unit/gapic/batch_v1alpha/test_batch_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.957927 google-cloud-batch-0.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4377 2023-02-07 15:53:52.957927 google-cloud-batch-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3480 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.941917 google-cloud-batch-0.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.941917 google-cloud-batch-0.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.945919 google-cloud-batch-0.9.0/google/cloud/batch/
+-rw-rw-r--   0 root         (0)     1003     2186 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       79 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.945919 google-cloud-batch-0.9.0/google/cloud/batch_v1/
+-rw-rw-r--   0 root         (0)     1003     1999 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2660 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       79 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.945919 google-cloud-batch-0.9.0/google/cloud/batch_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.945919 google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/
+-rw-rw-r--   0 root         (0)     1003      761 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    61801 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    71507 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10253 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.945919 google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11891 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    26369 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    26757 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    68232 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.949922 google-cloud-batch-0.9.0/google/cloud/batch_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1726 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10221 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/types/batch.py
+-rw-rw-r--   0 root         (0)     1003    32564 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/types/job.py
+-rw-rw-r--   0 root         (0)     1003    19276 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/types/task.py
+-rw-rw-r--   0 root         (0)     1003     4303 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1/types/volume.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.949922 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/
+-rw-rw-r--   0 root         (0)     1003     2058 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2670 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       79 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.949922 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.949922 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/
+-rw-rw-r--   0 root         (0)     1003      761 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    61981 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    71687 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10338 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.949922 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11916 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    26419 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    26807 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    68352 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.953925 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/types/
+-rw-rw-r--   0 root         (0)     1003     1780 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10251 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/types/batch.py
+-rw-rw-r--   0 root         (0)     1003    38761 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/types/job.py
+-rw-rw-r--   0 root         (0)     1003    19734 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/types/task.py
+-rw-rw-r--   0 root         (0)     1003     5397 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/types/volume.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.953925 google-cloud-batch-0.9.0/google_cloud_batch.egg-info/
+-rw-r--r--   0 root         (0)     1003     4377 2023-02-07 15:53:52.000000 google-cloud-batch-0.9.0/google_cloud_batch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2662 2023-02-07 15:53:52.000000 google-cloud-batch-0.9.0/google_cloud_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-02-07 15:53:52.000000 google-cloud-batch-0.9.0/google_cloud_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-02-07 15:53:52.000000 google-cloud-batch-0.9.0/google_cloud_batch.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-02-07 15:53:52.000000 google-cloud-batch-0.9.0/google_cloud_batch.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-02-07 15:53:52.000000 google-cloud-batch-0.9.0/google_cloud_batch.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-02-07 15:53:52.000000 google-cloud-batch-0.9.0/google_cloud_batch.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-02-07 15:53:52.957927 google-cloud-batch-0.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3014 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.953925 google-cloud-batch-0.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.953925 google-cloud-batch-0.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.953925 google-cloud-batch-0.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.953925 google-cloud-batch-0.9.0/tests/unit/gapic/batch_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/tests/unit/gapic/batch_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   251961 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/tests/unit/gapic/batch_v1/test_batch_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-02-07 15:53:52.953925 google-cloud-batch-0.9.0/tests/unit/gapic/batch_v1alpha/
+-rw-rw-r--   0 root         (0)     1003      600 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/tests/unit/gapic/batch_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003   256064 2023-02-07 15:51:55.000000 google-cloud-batch-0.9.0/tests/unit/gapic/batch_v1alpha/test_batch_service.py
```

### Comparing `google-cloud-batch-0.8.1/LICENSE` & `google-cloud-batch-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/MANIFEST.in` & `google-cloud-batch-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/PKG-INFO` & `google-cloud-batch-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-batch
-Version: 0.8.1
+Version: 0.9.0
 Summary: Google Cloud Batch API client library
 Home-page: https://github.com/googleapis/python-batch
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-batch-0.8.1/README.rst` & `google-cloud-batch-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch/__init__.py` & `google-cloud-batch-0.9.0/google/cloud/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch/gapic_version.py` & `google-cloud-batch-0.9.0/google/cloud/batch/gapic_version.py`

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
-__version__ = "0.8.1"  # {x-release-please-version}
+__version__ = "0.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/__init__.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.batch import gapic_version as package_version
+from google.cloud.batch_v1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .services.batch_service import BatchServiceAsyncClient, BatchServiceClient
 from .types.batch import (
     CreateJobRequest,
```

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/gapic_metadata.json` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/gapic_version.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/gapic_version.py`

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
-__version__ = "0.8.1"  # {x-release-please-version}
+__version__ = "0.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/services/__init__.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/__init__.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/async_client.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/client.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/pagers.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/transports/__init__.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/transports/base.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/transports/grpc.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/transports/grpc_asyncio.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/services/batch_service/transports/rest.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/services/batch_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/types/__init__.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/types/batch.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/types/batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/types/job.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/types/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -190,15 +190,15 @@
     """
 
     class State(proto.Enum):
         r"""Valid Job states.
 
         Values:
             STATE_UNSPECIFIED (0):
-
+                No description available.
             QUEUED (1):
                 Job is admitted (validated and persisted) and
                 waiting for resources.
             SCHEDULED (2):
                 Job is scheduled to run as soon as resource
                 allocation is ready. The resource allocation may
                 happen at a later time but with a high chance to
@@ -231,14 +231,16 @@
             machine_type (str):
                 The Compute Engine machine type.
             provisioning_model (google.cloud.batch_v1.types.AllocationPolicy.ProvisioningModel):
                 The VM instance provisioning model.
             task_pack (int):
                 The max number of tasks can be assigned to
                 this instance type.
+            boot_disk (google.cloud.batch_v1.types.AllocationPolicy.Disk):
+                The VM boot disk.
         """
 
         machine_type: str = proto.Field(
             proto.STRING,
             number=1,
         )
         provisioning_model: "AllocationPolicy.ProvisioningModel" = proto.Field(
@@ -246,14 +248,19 @@
             number=2,
             enum="AllocationPolicy.ProvisioningModel",
         )
         task_pack: int = proto.Field(
             proto.INT64,
             number=3,
         )
+        boot_disk: "AllocationPolicy.Disk" = proto.Field(
+            proto.MESSAGE,
+            number=4,
+            message="AllocationPolicy.Disk",
+        )
 
     class TaskGroupStatus(proto.Message):
         r"""Aggregated task status for a TaskGroup.
 
         Attributes:
             counts (MutableMapping[str, int]):
                 Count of task in each state in the TaskGroup.
@@ -453,31 +460,46 @@
         Setting any member of the oneof automatically clears all other
         members.
 
         .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
         Attributes:
             image (str):
-                Name of a public or custom image used as the
-                data source.
+                Name of a public or custom image used as the data source.
+                For example, the following are all valid URLs: (1) Specify
+                the image by its family name:
+                projects/{project}/global/images/family/{image_family} (2)
+                Specify the image version:
+                projects/{project}/global/images/{image_version} You can
+                also use Batch customized image in short names. The
+                following image values are supported for a boot disk:
+                "batch-debian": use Batch Debian images. "batch-centos": use
+                Batch CentOS images. "batch-cos": use Batch
+                Container-Optimized images.
 
                 This field is a member of `oneof`_ ``data_source``.
             snapshot (str):
                 Name of a snapshot used as the data source.
 
                 This field is a member of `oneof`_ ``data_source``.
             type_ (str):
-                Disk type as shown in ``gcloud compute disk-types list`` For
-                example, "pd-ssd", "pd-standard", "pd-balanced",
-                "local-ssd".
+                Disk type as shown in ``gcloud compute disk-types list``.
+                For example, local SSD uses type "local-ssd". Persistent
+                disks and boot disks use "pd-balanced", "pd-extreme",
+                "pd-ssd" or "pd-standard".
             size_gb (int):
-                Disk size in GB. This field is ignored if ``data_source`` is
-                ``disk`` or ``image``. If ``type`` is ``local-ssd``, size_gb
-                should be a multiple of 375GB, otherwise, the final size
-                will be the next greater multiple of 375 GB.
+                Disk size in GB. For persistent disk, this field is ignored
+                if ``data_source`` is ``image`` or ``snapshot``. For local
+                SSD, size_gb should be a multiple of 375GB, otherwise, the
+                final size will be the next greater multiple of 375 GB. For
+                boot disk, Batch will calculate the boot disk size based on
+                source image and task requirements if you do not speicify
+                the size. If both this field and the boot_disk_mib field in
+                task spec's compute_resource are defined, Batch will only
+                honor this field.
             disk_interface (str):
                 Local SSDs are available through both "SCSI"
                 and "NVMe" interfaces. If not indicated, "NVMe"
                 will be the default one for local ssds. We only
                 support "SCSI" for persistent disks now.
         """
 
@@ -586,14 +608,18 @@
                 ``https://cloud.google.com/compute/docs/instances/specify-min-cpu-platform``.
                 Not yet implemented.
             provisioning_model (google.cloud.batch_v1.types.AllocationPolicy.ProvisioningModel):
                 The provisioning model.
             accelerators (MutableSequence[google.cloud.batch_v1.types.AllocationPolicy.Accelerator]):
                 The accelerators attached to each VM
                 instance.
+            boot_disk (google.cloud.batch_v1.types.AllocationPolicy.Disk):
+                Book disk to be created and attached to each
+                VM by this InstancePolicy. Boot disk will be
+                deleted when the VM is deleted.
             disks (MutableSequence[google.cloud.batch_v1.types.AllocationPolicy.AttachedDisk]):
                 Non-boot disks to be attached for each VM
                 created by this InstancePolicy. New disks will
                 be deleted when the VM is deleted.
         """
 
         machine_type: str = proto.Field(
@@ -612,14 +638,19 @@
         accelerators: MutableSequence[
             "AllocationPolicy.Accelerator"
         ] = proto.RepeatedField(
             proto.MESSAGE,
             number=5,
             message="AllocationPolicy.Accelerator",
         )
+        boot_disk: "AllocationPolicy.Disk" = proto.Field(
+            proto.MESSAGE,
+            number=8,
+            message="AllocationPolicy.Disk",
+        )
         disks: MutableSequence["AllocationPolicy.AttachedDisk"] = proto.RepeatedField(
             proto.MESSAGE,
             number=6,
             message="AllocationPolicy.AttachedDisk",
         )
 
     class InstancePolicyOrTemplate(proto.Message):
@@ -849,16 +880,25 @@
             Email address of the service account. If not
             specified, the default Compute Engine service
             account for the project will be used. If
             instance template is being used, the service
             account has to be specified in the instance
             template and it has to match the email field
             here.
+        scopes (MutableSequence[str]):
+            List of scopes to be enabled for this service
+            account on the VM, in addition to the
+            cloud-platform API scope that will be added by
+            default.
     """
 
     email: str = proto.Field(
         proto.STRING,
         number=1,
     )
+    scopes: MutableSequence[str] = proto.RepeatedField(
+        proto.STRING,
+        number=2,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/types/task.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/types/task.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1/types/volume.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1/types/volume.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/__init__.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.batch import gapic_version as package_version
+from google.cloud.batch_v1alpha import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .services.batch_service import BatchServiceAsyncClient, BatchServiceClient
 from .types.batch import (
     CreateJobRequest,
```

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/gapic_metadata.json` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/gapic_version.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/gapic_version.py`

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
-__version__ = "0.8.1"  # {x-release-please-version}
+__version__ = "0.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/__init__.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/__init__.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/async_client.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/client.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/pagers.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/transports/__init__.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/transports/base.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/transports/grpc.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/transports/grpc_asyncio.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/services/batch_service/transports/rest.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/services/batch_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/types/__init__.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/types/batch.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/types/batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/types/job.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/types/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,15 @@
     """
 
     class State(proto.Enum):
         r"""Valid Job states.
 
         Values:
             STATE_UNSPECIFIED (0):
-
+                No description available.
             QUEUED (1):
                 Job is admitted (validated and persisted) and
                 waiting for resources.
             SCHEDULED (2):
                 Job is scheduled to run as soon as resource
                 allocation is ready. The resource allocation may
                 happen at a later time but with a high chance to
@@ -312,14 +312,16 @@
             machine_type (str):
                 The Compute Engine machine type.
             provisioning_model (google.cloud.batch_v1alpha.types.AllocationPolicy.ProvisioningModel):
                 The VM instance provisioning model.
             task_pack (int):
                 The max number of tasks can be assigned to
                 this instance type.
+            boot_disk (google.cloud.batch_v1alpha.types.AllocationPolicy.Disk):
+                The VM boot disk.
         """
 
         machine_type: str = proto.Field(
             proto.STRING,
             number=1,
         )
         provisioning_model: "AllocationPolicy.ProvisioningModel" = proto.Field(
@@ -327,14 +329,19 @@
             number=2,
             enum="AllocationPolicy.ProvisioningModel",
         )
         task_pack: int = proto.Field(
             proto.INT64,
             number=3,
         )
+        boot_disk: "AllocationPolicy.Disk" = proto.Field(
+            proto.MESSAGE,
+            number=4,
+            message="AllocationPolicy.Disk",
+        )
 
     class TaskGroupStatus(proto.Message):
         r"""Aggregated task status for a TaskGroup.
 
         Attributes:
             counts (MutableMapping[str, int]):
                 Count of task in each state in the TaskGroup.
@@ -550,31 +557,46 @@
         Setting any member of the oneof automatically clears all other
         members.
 
         .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
         Attributes:
             image (str):
-                Name of a public or custom image used as the
-                data source.
+                Name of a public or custom image used as the data source.
+                For example, the following are all valid URLs: (1) Specify
+                the image by its family name:
+                projects/{project}/global/images/family/{image_family} (2)
+                Specify the image version:
+                projects/{project}/global/images/{image_version} You can
+                also use Batch customized image in short names. The
+                following image values are supported for a boot disk:
+                "batch-debian": use Batch Debian images. "batch-centos": use
+                Batch CentOS images. "batch-cos": use Batch
+                Container-Optimized images.
 
                 This field is a member of `oneof`_ ``data_source``.
             snapshot (str):
                 Name of a snapshot used as the data source.
 
                 This field is a member of `oneof`_ ``data_source``.
             type_ (str):
-                Disk type as shown in ``gcloud compute disk-types list`` For
-                example, "pd-ssd", "pd-standard", "pd-balanced",
-                "local-ssd".
+                Disk type as shown in ``gcloud compute disk-types list``.
+                For example, local SSD uses type "local-ssd". Persistent
+                disks and boot disks use "pd-balanced", "pd-extreme",
+                "pd-ssd" or "pd-standard".
             size_gb (int):
-                Disk size in GB. This field is ignored if ``data_source`` is
-                ``disk`` or ``image``. If ``type`` is ``local-ssd``, size_gb
-                should be a multiple of 375GB, otherwise, the final size
-                will be the next greater multiple of 375 GB.
+                Disk size in GB. For persistent disk, this field is ignored
+                if ``data_source`` is ``image`` or ``snapshot``. For local
+                SSD, size_gb should be a multiple of 375GB, otherwise, the
+                final size will be the next greater multiple of 375 GB. For
+                boot disk, Batch will calculate the boot disk size based on
+                source image and task requirements if you do not speicify
+                the size. If both this field and the boot_disk_mib field in
+                task spec's compute_resource are defined, Batch will only
+                honor this field.
             disk_interface (str):
                 Local SSDs are available through both "SCSI"
                 and "NVMe" interfaces. If not indicated, "NVMe"
                 will be the default one for local ssds. We only
                 support "SCSI" for persistent disks now.
         """
```

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/types/task.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/types/task.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google/cloud/batch_v1alpha/types/volume.py` & `google-cloud-batch-0.9.0/google/cloud/batch_v1alpha/types/volume.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/google_cloud_batch.egg-info/PKG-INFO` & `google-cloud-batch-0.9.0/google_cloud_batch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-batch
-Version: 0.8.1
+Version: 0.9.0
 Summary: Google Cloud Batch API client library
 Home-page: https://github.com/googleapis/python-batch
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-batch-0.8.1/google_cloud_batch.egg-info/SOURCES.txt` & `google-cloud-batch-0.9.0/google_cloud_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/setup.py` & `google-cloud-batch-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/tests/__init__.py` & `google-cloud-batch-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/tests/unit/__init__.py` & `google-cloud-batch-0.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/tests/unit/gapic/__init__.py` & `google-cloud-batch-0.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/tests/unit/gapic/batch_v1/__init__.py` & `google-cloud-batch-0.9.0/tests/unit/gapic/batch_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/tests/unit/gapic/batch_v1/test_batch_service.py` & `google-cloud-batch-0.9.0/tests/unit/gapic/batch_v1/test_batch_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -2606,33 +2606,37 @@
                         "accelerators": [
                             {
                                 "type_": "type__value",
                                 "count": 553,
                                 "install_gpu_drivers": True,
                             }
                         ],
+                        "boot_disk": {
+                            "image": "image_value",
+                            "snapshot": "snapshot_value",
+                            "type_": "type__value",
+                            "size_gb": 739,
+                            "disk_interface": "disk_interface_value",
+                        },
                         "disks": [
                             {
-                                "new_disk": {
-                                    "image": "image_value",
-                                    "snapshot": "snapshot_value",
-                                    "type_": "type__value",
-                                    "size_gb": 739,
-                                    "disk_interface": "disk_interface_value",
-                                },
+                                "new_disk": {},
                                 "existing_disk": "existing_disk_value",
                                 "device_name": "device_name_value",
                             }
                         ],
                     },
                     "instance_template": "instance_template_value",
                     "install_gpu_drivers": True,
                 }
             ],
-            "service_account": {"email": "email_value"},
+            "service_account": {
+                "email": "email_value",
+                "scopes": ["scopes_value1", "scopes_value2"],
+            },
             "labels": {},
             "network": {
                 "network_interfaces": [
                     {
                         "network": "network_value",
                         "subnetwork": "subnetwork_value",
                         "no_external_ip_address": True,
@@ -2948,33 +2952,37 @@
                         "accelerators": [
                             {
                                 "type_": "type__value",
                                 "count": 553,
                                 "install_gpu_drivers": True,
                             }
                         ],
+                        "boot_disk": {
+                            "image": "image_value",
+                            "snapshot": "snapshot_value",
+                            "type_": "type__value",
+                            "size_gb": 739,
+                            "disk_interface": "disk_interface_value",
+                        },
                         "disks": [
                             {
-                                "new_disk": {
-                                    "image": "image_value",
-                                    "snapshot": "snapshot_value",
-                                    "type_": "type__value",
-                                    "size_gb": 739,
-                                    "disk_interface": "disk_interface_value",
-                                },
+                                "new_disk": {},
                                 "existing_disk": "existing_disk_value",
                                 "device_name": "device_name_value",
                             }
                         ],
                     },
                     "instance_template": "instance_template_value",
                     "install_gpu_drivers": True,
                 }
             ],
-            "service_account": {"email": "email_value"},
+            "service_account": {
+                "email": "email_value",
+                "scopes": ["scopes_value1", "scopes_value2"],
+            },
             "labels": {},
             "network": {
                 "network_interfaces": [
                     {
                         "network": "network_value",
                         "subnetwork": "subnetwork_value",
                         "no_external_ip_address": True,
```

### Comparing `google-cloud-batch-0.8.1/tests/unit/gapic/batch_v1alpha/__init__.py` & `google-cloud-batch-0.9.0/tests/unit/gapic/batch_v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-batch-0.8.1/tests/unit/gapic/batch_v1alpha/test_batch_service.py` & `google-cloud-batch-0.9.0/tests/unit/gapic/batch_v1alpha/test_batch_service.py`

 * *Files identical despite different names*

