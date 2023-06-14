# Comparing `tmp/pyatlan-0.1.1.tar.gz` & `tmp/pyatlan-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.1.1.tar", last modified: Mon Jun 12 11:46:00 2023, max compression
+gzip compressed data, was "pyatlan-0.1.2.tar", last modified: Wed Jun 14 12:25:50 2023, max compression
```

## Comparing `pyatlan-0.1.1.tar` & `pyatlan-0.1.2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.166763 pyatlan-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-06-12 11:45:48.000000 pyatlan-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 11:45:48.000000 pyatlan-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-12 11:45:48.000000 pyatlan-0.1.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-12 11:46:00.166763 pyatlan-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-12 11:45:48.000000 pyatlan-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.158763 pyatlan-0.1.1/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.158763 pyatlan-0.1.1/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/cache/classification_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/cache/enum_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/cache/group_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/cache/role_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/cache/user_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.158763 pyatlan-0.1.1/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42383 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.158763 pyatlan-0.1.1/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.158763 pyatlan-0.1.1/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.162763 pyatlan-0.1.1/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   899802 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/atlan_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    54041 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    59796 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.158763 pyatlan-0.1.1/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-12 11:46:00.000000 pyatlan-0.1.1/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-12 11:46:00.000000 pyatlan-0.1.1/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 11:46:00.000000 pyatlan-0.1.1/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 11:45:59.000000 pyatlan-0.1.1/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 11:46:00.000000 pyatlan-0.1.1/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 11:46:00.000000 pyatlan-0.1.1/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 11:46:00.166763 pyatlan-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-12 11:45:48.000000 pyatlan-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.162763 pyatlan-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.162763 pyatlan-0.1.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/admin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/classification_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    35609 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/lineage_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/s3_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/test_index_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/test_sql_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.166763 pyatlan-0.1.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_classification_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    64432 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31770 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.303921 pyatlan-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-06-14 12:25:38.000000 pyatlan-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 12:25:38.000000 pyatlan-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-14 12:25:38.000000 pyatlan-0.1.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-14 12:25:50.303921 pyatlan-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-14 12:25:38.000000 pyatlan-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.291921 pyatlan-0.1.2/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.295921 pyatlan-0.1.2/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/cache/classification_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/cache/enum_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/cache/group_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/cache/role_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/cache/user_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.295921 pyatlan-0.1.2/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42383 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.295921 pyatlan-0.1.2/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.295921 pyatlan-0.1.2/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.299921 pyatlan-0.1.2/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   900272 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/atlan_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54059 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59796 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.295921 pyatlan-0.1.2/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-14 12:25:50.000000 pyatlan-0.1.2/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-14 12:25:50.000000 pyatlan-0.1.2/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:25:50.000000 pyatlan-0.1.2/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:25:50.000000 pyatlan-0.1.2/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-14 12:25:50.000000 pyatlan-0.1.2/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 12:25:50.000000 pyatlan-0.1.2/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 12:25:50.303921 pyatlan-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-14 12:25:38.000000 pyatlan-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.299921 pyatlan-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.299921 pyatlan-0.1.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/admin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35674 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/lineage_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/s3_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/test_index_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/test_sql_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.303921 pyatlan-0.1.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_classification_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64432 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31770 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.1.1/LICENSE` & `pyatlan-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/PKG-INFO` & `pyatlan-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.1.1
+Version: 0.1.2
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.1.1/README.md` & `pyatlan-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/cache/classification_cache.py` & `pyatlan-0.1.2/pyatlan/cache/classification_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.1.2/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/cache/enum_cache.py` & `pyatlan-0.1.2/pyatlan/cache/enum_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/cache/group_cache.py` & `pyatlan-0.1.2/pyatlan/cache/group_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/cache/role_cache.py` & `pyatlan-0.1.2/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/cache/user_cache.py` & `pyatlan-0.1.2/pyatlan/cache/user_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/client/atlan.py` & `pyatlan-0.1.2/pyatlan/client/atlan.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/client/constants.py` & `pyatlan-0.1.2/pyatlan/client/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/error.py` & `pyatlan-0.1.2/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/exceptions.py` & `pyatlan-0.1.2/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.1.2/pyatlan/generator/generate_from_typdefs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/model/assets.py` & `pyatlan-0.1.2/pyatlan/model/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,14 +387,15 @@
         "asset_mc_monitor_types",
         "asset_mc_monitor_schedule_types",
         "asset_mc_incident_types",
         "asset_mc_incident_sub_types",
         "asset_mc_incident_severities",
         "asset_mc_incident_states",
         "asset_mc_last_sync_run_at",
+        "starred_by",
         "mc_monitors",
         "files",
         "mc_incidents",
         "links",
         "metrics",
         "readme",
         "assigned_terms",
@@ -1646,14 +1647,24 @@
     @asset_mc_last_sync_run_at.setter
     def asset_mc_last_sync_run_at(self, asset_mc_last_sync_run_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_mc_last_sync_run_at = asset_mc_last_sync_run_at
 
     @property
+    def starred_by(self) -> Optional[set[str]]:
+        return self.attributes.starred_by
+
+    @starred_by.setter
+    def starred_by(self, starred_by: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.starred_by = starred_by
+
+    @property
     def mc_monitors(self) -> Optional[list[MCMonitor]]:
         return self.attributes.mc_monitors
 
     @mc_monitors.setter
     def mc_monitors(self, mc_monitors: Optional[list[MCMonitor]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -2087,14 +2098,15 @@
         )
         asset_mc_incident_states: Optional[set[str]] = Field(
             None, description="", alias="assetMcIncidentStates"
         )
         asset_mc_last_sync_run_at: Optional[datetime] = Field(
             None, description="", alias="assetMcLastSyncRunAt"
         )
+        starred_by: Optional[set[str]] = Field(None, description="", alias="starredBy")
         mc_monitors: Optional[list[MCMonitor]] = Field(
             None, description="", alias="mcMonitors"
         )  # relationship
         files: Optional[list[File]] = Field(
             None, description="", alias="files"
         )  # relationship
         mc_incidents: Optional[list[MCIncident]] = Field(
@@ -2988,20 +3000,21 @@
         *,
         name: StrictStr,
         cm_name: str,
         cm_attribute: str,
         badge_conditions: list[BadgeCondition],
     ) -> Badge:
         return cls(
+            status=EntityStatus.ACTIVE,
             attributes=Badge.Attributes.create(
                 name=name,
                 cm_name=cm_name,
                 cm_attribute=cm_attribute,
                 badge_conditions=badge_conditions,
-            )
+            ),
         )
 
     class Attributes(Asset.Attributes):
         badge_conditions: Optional[list[BadgeCondition]] = Field(
             None, description="", alias="badgeConditions"
         )
         badge_metadata_attribute: Optional[str] = Field(
```

### Comparing `pyatlan-0.1.1/pyatlan/model/atlan_image.py` & `pyatlan-0.1.2/pyatlan/model/atlan_image.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/model/core.py` & `pyatlan-0.1.2/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/model/custom_metadata.py` & `pyatlan-0.1.2/pyatlan/model/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/model/enums.py` & `pyatlan-0.1.2/pyatlan/model/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,14 +368,15 @@
     ZIP = "zip"
 
 
 class AtlanClassificationColor(str, Enum):
     GREEN = "Green"
     YELLOW = "Yellow"
     RED = "Red"
+    GRAY = "Gray"
 
 
 class QueryParserSourceType(str, Enum):
     ANSI = "ansi"
     BIGQUERY = "bigquery"
     HANA = "hana"
     HIVE = "hive"
```

### Comparing `pyatlan-0.1.1/pyatlan/model/group.py` & `pyatlan-0.1.2/pyatlan/model/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/model/lineage.py` & `pyatlan-0.1.2/pyatlan/model/lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/model/query.py` & `pyatlan-0.1.2/pyatlan/model/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/model/response.py` & `pyatlan-0.1.2/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/model/role.py` & `pyatlan-0.1.2/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/model/search.py` & `pyatlan-0.1.2/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/model/structs.py` & `pyatlan-0.1.2/pyatlan/model/structs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -37,43 +37,72 @@
         None, description="", alias="awsCloudWatchMetricName"
     )
     aws_cloud_watch_metric_scope: "str" = Field(
         None, description="", alias="awsCloudWatchMetricScope"
     )
 
 
+class Histogram(AtlanObject):
+    """Description"""
+
+    boundaries: "set[float]" = Field(None, description="", alias="boundaries")
+    frequencies: "set[float]" = Field(None, description="", alias="frequencies")
+
+
 class KafkaTopicConsumption(AtlanObject):
     """Description"""
 
     topic_name: Optional["str"] = Field(None, description="", alias="topicName")
     topic_partition: Optional["str"] = Field(
         None, description="", alias="topicPartition"
     )
     topic_lag: Optional["int"] = Field(None, description="", alias="topicLag")
     topic_current_offset: Optional["int"] = Field(
         None, description="", alias="topicCurrentOffset"
     )
 
 
-class Histogram(AtlanObject):
-    """Description"""
-
-    boundaries: "set[float]" = Field(None, description="", alias="boundaries")
-    frequencies: "set[float]" = Field(None, description="", alias="frequencies")
-
-
 class ColumnValueFrequencyMap(AtlanObject):
     """Description"""
 
     column_value: Optional["str"] = Field(None, description="", alias="columnValue")
     column_value_frequency: Optional["int"] = Field(
         None, description="", alias="columnValueFrequency"
     )
 
 
+class SourceTagAttachment(AtlanObject):
+    """Description"""
+
+    source_tag_name: Optional["str"] = Field(
+        None, description="", alias="sourceTagName"
+    )
+    source_tag_qualified_name: Optional["str"] = Field(
+        None, description="", alias="sourceTagQualifiedName"
+    )
+    source_tag_guid: Optional["str"] = Field(
+        None, description="", alias="sourceTagGuid"
+    )
+    source_tag_connector_name: Optional["str"] = Field(
+        None, description="", alias="sourceTagConnectorName"
+    )
+    source_tag_value: Optional["list[SourceTagAttachmentValue]"] = Field(
+        None, description="", alias="sourceTagValue"
+    )
+    is_source_tag_synced: Optional["bool"] = Field(
+        None, description="", alias="isSourceTagSynced"
+    )
+    source_tag_sync_timestamp: Optional["datetime"] = Field(
+        None, description="", alias="sourceTagSyncTimestamp"
+    )
+    source_tag_sync_error: Optional["str"] = Field(
+        None, description="", alias="sourceTagSyncError"
+    )
+
+
 class SourceTagAttachmentValue(AtlanObject):
     """Description"""
 
     tag_attachment_key: Optional["str"] = Field(
         None, description="", alias="tagAttachmentKey"
     )
     tag_attachment_value: Optional["str"] = Field(
@@ -116,43 +145,14 @@
         None, description="", alias="badgeConditionValue"
     )
     badge_condition_colorhex: Optional["str"] = Field(
         None, description="", alias="badgeConditionColorhex"
     )
 
 
-class SourceTagAttachment(AtlanObject):
-    """Description"""
-
-    source_tag_name: Optional["str"] = Field(
-        None, description="", alias="sourceTagName"
-    )
-    source_tag_qualified_name: Optional["str"] = Field(
-        None, description="", alias="sourceTagQualifiedName"
-    )
-    source_tag_guid: Optional["str"] = Field(
-        None, description="", alias="sourceTagGuid"
-    )
-    source_tag_connector_name: Optional["str"] = Field(
-        None, description="", alias="sourceTagConnectorName"
-    )
-    source_tag_value: Optional["list[SourceTagAttachmentValue]"] = Field(
-        None, description="", alias="sourceTagValue"
-    )
-    is_source_tag_synced: Optional["bool"] = Field(
-        None, description="", alias="isSourceTagSynced"
-    )
-    source_tag_sync_timestamp: Optional["datetime"] = Field(
-        None, description="", alias="sourceTagSyncTimestamp"
-    )
-    source_tag_sync_error: Optional["str"] = Field(
-        None, description="", alias="sourceTagSyncError"
-    )
-
-
 class AzureTag(AtlanObject):
     """Description"""
 
     azure_tag_key: "str" = Field(None, description="", alias="azureTagKey")
     azure_tag_value: "str" = Field(None, description="", alias="azureTagValue")
```

### Comparing `pyatlan-0.1.1/pyatlan/model/typedef.py` & `pyatlan-0.1.2/pyatlan/model/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/model/user.py` & `pyatlan-0.1.2/pyatlan/model/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/multipart_data_generator.py` & `pyatlan-0.1.2/pyatlan/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan/utils.py` & `pyatlan-0.1.2/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.1.2/pyatlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.1.1
+Version: 0.1.2
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.1.1/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.1.2/pyatlan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/setup.py` & `pyatlan-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/integration/admin_test.py` & `pyatlan-0.1.2/tests/integration/admin_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/integration/classification_test.py` & `pyatlan-0.1.2/tests/integration/classification_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/integration/client.py` & `pyatlan-0.1.2/tests/integration/client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/integration/connection_test.py` & `pyatlan-0.1.2/tests/integration/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/integration/custom_metadata_test.py` & `pyatlan-0.1.2/tests/integration/custom_metadata_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from pyatlan.model.assets import AtlasGlossary, AtlasGlossaryTerm, Badge, BadgeCondition
 from pyatlan.model.custom_metadata import CustomMetadataDict
 from pyatlan.model.enums import (
     AtlanCustomAttributePrimitiveType,
     AtlanTypeCategory,
     BadgeComparisonOperator,
     BadgeConditionColor,
+    EntityStatus,
 )
 from pyatlan.model.group import AtlanGroup, CreateGroupResponse
 from pyatlan.model.search import DSL, Bool, Exists, IndexSearchRequest, Term
 from pyatlan.model.typedef import AttributeDef, CustomMetadataDef, EnumDef
 from tests.integration.admin_test import create_group, delete_group
 from tests.integration.client import TestId, delete_asset
 from tests.integration.glossary_test import create_glossary, create_term
@@ -965,11 +966,12 @@
                 badge_condition_operator=BadgeComparisonOperator.LTE,
                 badge_condition_value="2",
                 badge_condition_colorhex=BadgeConditionColor.RED,
             ),
         ],
     )
     badge.user_description = "How many data quality checks ran against this asset."
+    assert badge.status == EntityStatus.ACTIVE
     response = client.upsert(badge)
     assert (badges := response.assets_created(asset_type=Badge))
     assert len(badges) == 1
     client.purge_entity_by_guid(badges[0].guid)
```

### Comparing `pyatlan-0.1.1/tests/integration/glossary_test.py` & `pyatlan-0.1.2/tests/integration/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/integration/lineage_test.py` & `pyatlan-0.1.2/tests/integration/lineage_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/integration/query_parser_test.py` & `pyatlan-0.1.2/tests/integration/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/integration/s3_asset_test.py` & `pyatlan-0.1.2/tests/integration/s3_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/integration/test_client.py` & `pyatlan-0.1.2/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/integration/test_index_search.py` & `pyatlan-0.1.2/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/integration/test_sql_assets.py` & `pyatlan-0.1.2/tests/integration/test_sql_assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/unit/test_classification_name.py` & `pyatlan-0.1.2/tests/unit/test_classification_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/unit/test_client.py` & `pyatlan-0.1.2/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/unit/test_custom_metadata.py` & `pyatlan-0.1.2/tests/unit/test_custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/unit/test_glossary_term.py` & `pyatlan-0.1.2/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/unit/test_lineage.py` & `pyatlan-0.1.2/tests/unit/test_lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/unit/test_model.py` & `pyatlan-0.1.2/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/unit/test_search_model.py` & `pyatlan-0.1.2/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.1/tests/unit/test_typedef_model.py` & `pyatlan-0.1.2/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

