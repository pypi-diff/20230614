# Comparing `tmp/storey-1.4.1.tar.gz` & `tmp/storey-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/storey/storey/dist/.tmp-h1mqzsfr/storey-1.4.1.tar", last modified: Tue May 30 12:44:54 2023, max compression
+gzip compressed data, was "/home/runner/work/storey/storey/dist/.tmp-qtid9xr6/storey-1.4.2.tar", last modified: Wed Jun 14 08:27:44 2023, max compression
```

## Comparing `storey-1.4.1.tar` & `storey-1.4.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:44:54.000000 storey-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 12:40:12.000000 storey-1.4.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 12:40:12.000000 storey-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-30 12:40:12.000000 storey-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-30 12:44:54.000000 storey-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-30 12:40:12.000000 storey-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-30 12:40:12.000000 storey-1.4.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:44:54.000000 storey-1.4.1/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-30 12:40:12.000000 storey-1.4.1/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-05-30 12:40:12.000000 storey-1.4.1/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-05-30 12:40:12.000000 storey-1.4.1/integration/integration_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   170272 2023-05-30 12:40:12.000000 storey-1.4.1/integration/test_aggregation_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-05-30 12:40:12.000000 storey-1.4.1/integration/test_azure_filesystem_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21737 2023-05-30 12:40:12.000000 storey-1.4.1/integration/test_filesystems_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    42755 2023-05-30 12:40:12.000000 storey-1.4.1/integration/test_flow_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-05-30 12:40:12.000000 storey-1.4.1/integration/test_kafka_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-30 12:40:12.000000 storey-1.4.1/integration/test_redis_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-05-30 12:40:12.000000 storey-1.4.1/integration/test_s3_filesystem_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-30 12:40:12.000000 storey-1.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 12:44:54.000000 storey-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-30 12:40:12.000000 storey-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:44:54.000000 storey-1.4.1/storey/
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-30 12:44:49.000000 storey-1.4.1/storey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-30 12:40:12.000000 storey-1.4.1/storey/aggregation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-05-30 12:40:12.000000 storey-1.4.1/storey/aggregations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-30 12:40:12.000000 storey-1.4.1/storey/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    28065 2023-05-30 12:40:12.000000 storey-1.4.1/storey/drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15755 2023-05-30 12:40:12.000000 storey-1.4.1/storey/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    50623 2023-05-30 12:40:12.000000 storey-1.4.1/storey/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-30 12:40:12.000000 storey-1.4.1/storey/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    27610 2023-05-30 12:40:12.000000 storey-1.4.1/storey/redis_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    37792 2023-05-30 12:40:12.000000 storey-1.4.1/storey/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-30 12:40:12.000000 storey-1.4.1/storey/sql_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:44:54.000000 storey-1.4.1/storey/steps/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-30 12:40:12.000000 storey-1.4.1/storey/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-30 12:40:12.000000 storey-1.4.1/storey/steps/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-30 12:40:12.000000 storey-1.4.1/storey/steps/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-30 12:40:12.000000 storey-1.4.1/storey/steps/foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-30 12:40:12.000000 storey-1.4.1/storey/steps/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-30 12:40:12.000000 storey-1.4.1/storey/steps/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    79910 2023-05-30 12:40:12.000000 storey-1.4.1/storey/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    50747 2023-05-30 12:40:12.000000 storey-1.4.1/storey/targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:44:54.000000 storey-1.4.1/storey/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-30 12:40:12.000000 storey-1.4.1/storey/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-05-30 12:40:12.000000 storey-1.4.1/storey/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-05-30 12:40:12.000000 storey-1.4.1/storey/windowed_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:44:54.000000 storey-1.4.1/storey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-30 12:44:54.000000 storey-1.4.1/storey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-30 12:44:54.000000 storey-1.4.1/storey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:44:54.000000 storey-1.4.1/storey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-30 12:44:54.000000 storey-1.4.1/storey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 12:44:54.000000 storey-1.4.1/storey.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:44:54.000000 storey-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-30 12:40:12.000000 storey-1.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144374 2023-05-30 12:40:12.000000 storey-1.4.1/tests/test_aggregate_by_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-30 12:40:12.000000 storey-1.4.1/tests/test_aggregate_store.py
--rw-r--r--   0 runner    (1001) docker     (123)   124270 2023-05-30 12:40:12.000000 storey-1.4.1/tests/test_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-05-30 12:40:12.000000 storey-1.4.1/tests/test_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-30 12:40:12.000000 storey-1.4.1/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-30 12:40:12.000000 storey-1.4.1/tests/test_v3io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-30 12:40:12.000000 storey-1.4.1/tests/test_windowed_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:27:44.000000 storey-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-14 08:24:33.000000 storey-1.4.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 08:24:33.000000 storey-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-14 08:24:33.000000 storey-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-06-14 08:27:44.000000 storey-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-14 08:24:33.000000 storey-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-14 08:24:33.000000 storey-1.4.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:27:44.000000 storey-1.4.2/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-14 08:24:33.000000 storey-1.4.2/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-14 08:24:33.000000 storey-1.4.2/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-06-14 08:24:33.000000 storey-1.4.2/integration/integration_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   170272 2023-06-14 08:24:33.000000 storey-1.4.2/integration/test_aggregation_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-06-14 08:24:33.000000 storey-1.4.2/integration/test_azure_filesystem_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21737 2023-06-14 08:24:33.000000 storey-1.4.2/integration/test_filesystems_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42755 2023-06-14 08:24:33.000000 storey-1.4.2/integration/test_flow_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-06-14 08:24:33.000000 storey-1.4.2/integration/test_kafka_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-14 08:24:33.000000 storey-1.4.2/integration/test_redis_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-06-14 08:24:33.000000 storey-1.4.2/integration/test_s3_filesystem_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-14 08:24:33.000000 storey-1.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-14 08:27:44.000000 storey-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-14 08:24:33.000000 storey-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:27:44.000000 storey-1.4.2/storey/
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-14 08:27:39.000000 storey-1.4.2/storey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-14 08:24:33.000000 storey-1.4.2/storey/aggregation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-06-14 08:24:33.000000 storey-1.4.2/storey/aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-06-14 08:24:33.000000 storey-1.4.2/storey/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28065 2023-06-14 08:24:33.000000 storey-1.4.2/storey/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15755 2023-06-14 08:24:33.000000 storey-1.4.2/storey/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50623 2023-06-14 08:24:33.000000 storey-1.4.2/storey/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-14 08:24:33.000000 storey-1.4.2/storey/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27610 2023-06-14 08:24:33.000000 storey-1.4.2/storey/redis_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37793 2023-06-14 08:24:33.000000 storey-1.4.2/storey/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-14 08:24:33.000000 storey-1.4.2/storey/sql_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:27:44.000000 storey-1.4.2/storey/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-14 08:24:33.000000 storey-1.4.2/storey/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-14 08:24:33.000000 storey-1.4.2/storey/steps/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-14 08:24:33.000000 storey-1.4.2/storey/steps/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-14 08:24:33.000000 storey-1.4.2/storey/steps/foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-14 08:24:33.000000 storey-1.4.2/storey/steps/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-14 08:24:33.000000 storey-1.4.2/storey/steps/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79910 2023-06-14 08:24:33.000000 storey-1.4.2/storey/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50747 2023-06-14 08:24:33.000000 storey-1.4.2/storey/targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:27:44.000000 storey-1.4.2/storey/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-14 08:24:33.000000 storey-1.4.2/storey/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-06-14 08:24:33.000000 storey-1.4.2/storey/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-06-14 08:24:33.000000 storey-1.4.2/storey/windowed_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:27:44.000000 storey-1.4.2/storey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-06-14 08:27:44.000000 storey-1.4.2/storey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-14 08:27:44.000000 storey-1.4.2/storey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:27:44.000000 storey-1.4.2/storey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-14 08:27:44.000000 storey-1.4.2/storey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-14 08:27:44.000000 storey-1.4.2/storey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:27:44.000000 storey-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-14 08:24:33.000000 storey-1.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144374 2023-06-14 08:24:33.000000 storey-1.4.2/tests/test_aggregate_by_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-14 08:24:33.000000 storey-1.4.2/tests/test_aggregate_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124403 2023-06-14 08:24:33.000000 storey-1.4.2/tests/test_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-06-14 08:24:33.000000 storey-1.4.2/tests/test_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-14 08:24:33.000000 storey-1.4.2/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-14 08:24:33.000000 storey-1.4.2/tests/test_v3io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-14 08:24:33.000000 storey-1.4.2/tests/test_windowed_store.py
```

### Comparing `storey-1.4.1/LICENSE` & `storey-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/PKG-INFO` & `storey-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storey
-Version: 1.4.1
+Version: 1.4.2
 Summary: Async flows
 Home-page: https://github.com/mlrun/storey
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `storey-1.4.1/README.md` & `storey-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/integration/__init__.py` & `storey-1.4.2/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/integration/conftest.py` & `storey-1.4.2/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/integration/integration_test_utils.py` & `storey-1.4.2/integration/integration_test_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/integration/test_aggregation_integration.py` & `storey-1.4.2/integration/test_aggregation_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/integration/test_azure_filesystem_integration.py` & `storey-1.4.2/integration/test_azure_filesystem_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/integration/test_filesystems_integration.py` & `storey-1.4.2/integration/test_filesystems_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/integration/test_flow_integration.py` & `storey-1.4.2/integration/test_flow_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/integration/test_kafka_integration.py` & `storey-1.4.2/integration/test_kafka_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/integration/test_redis_specific.py` & `storey-1.4.2/integration/test_redis_specific.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/integration/test_s3_filesystem_integration.py` & `storey-1.4.2/integration/test_s3_filesystem_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/setup.py` & `storey-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/__init__.py` & `storey-1.4.2/storey/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.4.1"
+__version__ = "1.4.2"
 
 # Importing supported filesystems explicitly so that they will get registered as an fsspec filesystem
 import v3iofs  # noqa: F401
 
 from .aggregations import AggregateByKey, QueryByKey  # noqa: F401
 from .dataframe import ReduceToDataFrame, ToDataFrame  # noqa: F401
 from .drivers import Driver, NoopDriver, V3ioDriver  # noqa: F401
```

### Comparing `storey-1.4.1/storey/aggregation_utils.py` & `storey-1.4.2/storey/aggregation_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/aggregations.py` & `storey-1.4.2/storey/aggregations.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/dataframe.py` & `storey-1.4.2/storey/dataframe.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/drivers.py` & `storey-1.4.2/storey/drivers.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/dtypes.py` & `storey-1.4.2/storey/dtypes.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/flow.py` & `storey-1.4.2/storey/flow.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/queue.py` & `storey-1.4.2/storey/queue.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/redis_driver.py` & `storey-1.4.2/storey/redis_driver.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/sources.py` & `storey-1.4.2/storey/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -789,15 +789,15 @@
                 date_parser=self._datetime_from_timestamp,
                 storage_options=self._storage_options,
             )
             self._validate_fields(df, path)
             self._dfs.append(df)
 
     def _datetime_from_timestamp(self, timestamp):
-        if timestamp == "" or timestamp is None:
+        if timestamp == "" or pd.isna(timestamp):
             return None
         if self._timestamp_format:
             return pandas.to_datetime(timestamp, format=self._timestamp_format).floor("u").to_pydatetime()
         else:
             return datetime.fromisoformat(timestamp)
 
     def _get_element(self, body: dict, columns: List[str]):
```

### Comparing `storey-1.4.1/storey/sql_driver.py` & `storey-1.4.2/storey/sql_driver.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/steps/__init__.py` & `storey-1.4.2/storey/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/steps/assertion.py` & `storey-1.4.2/storey/steps/assertion.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/steps/flatten.py` & `storey-1.4.2/storey/steps/flatten.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/steps/foreach.py` & `storey-1.4.2/storey/steps/foreach.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/steps/partition.py` & `storey-1.4.2/storey/steps/partition.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/steps/sample.py` & `storey-1.4.2/storey/steps/sample.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/table.py` & `storey-1.4.2/storey/table.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/targets.py` & `storey-1.4.2/storey/targets.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/transformations/__init__.py` & `storey-1.4.2/storey/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/utils.py` & `storey-1.4.2/storey/utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey/windowed_store.py` & `storey-1.4.2/storey/windowed_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/storey.egg-info/PKG-INFO` & `storey-1.4.2/storey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storey
-Version: 1.4.1
+Version: 1.4.2
 Summary: Async flows
 Home-page: https://github.com/mlrun/storey
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `storey-1.4.1/storey.egg-info/SOURCES.txt` & `storey-1.4.2/storey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/tests/__init__.py` & `storey-1.4.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/tests/test_aggregate_by_key.py` & `storey-1.4.2/tests/test_aggregate_by_key.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/tests/test_aggregate_store.py` & `storey-1.4.2/tests/test_aggregate_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/tests/test_flow.py` & `storey-1.4.2/tests/test_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -3469,41 +3469,43 @@
     assert query_by_key._aggrs == []
     assert query_by_key._enrich_cols == ["my_color_5h"]
 
 
 def test_csv_source_with_none_values():
     controller = build_flow(
         [
-            CSVSource("tests/test-with-none-values.csv", key_field="string"),
+            CSVSource("tests/test-with-none-values.csv", key_field="string", parse_dates="date_with_none"),
             Reduce([], append_and_return, full_event=True),
         ]
     ).run()
 
     termination_result = controller.await_termination()
 
     assert len(termination_result) == 2
     assert termination_result[0].key == "a"
     assert termination_result[0].body == [
         "a",
         True,
         False,
         1,
         2.3,
-        "2021-04-21 15:56:53.385444",
+        pd.to_datetime("2021-04-21 15:56:53.385444"),
     ]
     assert termination_result[1].key == "b"
-    excepted_result = ["b", True, math.nan, math.nan, math.nan, math.nan]
+    excepted_result = ["b", True, math.nan, math.nan, math.nan, pd.NaT]
     assert len(termination_result[1].body) == len(excepted_result)
     for x, y in zip(termination_result[1].body, excepted_result):
         if isinstance(x, float):
             assert isinstance(y, float)
             if math.isnan(x):
                 assert math.isnan(y)
             else:
                 assert x == y
+        elif isinstance(x, type(pd.NaT)):
+            assert isinstance(y, type(pd.NaT))
         else:
             assert x == y
 
 
 def test_csv_source_event_metadata():
     controller = build_flow(
         [
```

### Comparing `storey-1.4.1/tests/test_steps.py` & `storey-1.4.2/tests/test_steps.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/tests/test_types.py` & `storey-1.4.2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/tests/test_v3io.py` & `storey-1.4.2/tests/test_v3io.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.1/tests/test_windowed_store.py` & `storey-1.4.2/tests/test_windowed_store.py`

 * *Files identical despite different names*

