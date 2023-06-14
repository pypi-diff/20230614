# Comparing `tmp/aliyun-secret-manager-client-0.1.0.tar.gz` & `tmp/aliyun-secret-manager-client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-secret-manager-client-0.1.0.tar", last modified: Mon Dec 19 02:37:06 2022, max compression
+gzip compressed data, was "dist/aliyun-secret-manager-client-0.1.1.tar", last modified: Wed Jun 14 09:45:03 2023, max compression
```

## Comparing `aliyun-secret-manager-client-0.1.0.tar` & `aliyun-secret-manager-client-0.1.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     6007 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4272 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2610 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/
--rw-r--r--   0 root         (0) root         (0)       22 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/auth/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      481 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/auth/client_key_signer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1259 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/cache/cache_secret_store_strategy.py
--rw-r--r--   0 root         (0) root         (0)     1676 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/cache/default_secret_cache_hook.py
--rw-r--r--   0 root         (0) root         (0)     4992 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/cache/file_cache_secret_store_strategy.py
--rw-r--r--   0 root         (0) root         (0)     1427 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/cache/memory_cache_secret_store_strategy.py
--rw-r--r--   0 root         (0) root         (0)     1369 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/cache/secret_cache_hook.py
--rw-r--r--   0 root         (0) root         (0)     1000 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/cache_client_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/model/
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)      155 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/model/client_key_credentials.py
--rw-r--r--   0 root         (0) root         (0)      747 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/model/credentials_properties.py
--rw-r--r--   0 root         (0) root         (0)     2139 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/model/dkms_config.py
--rw-r--r--   0 root         (0) root         (0)     1557 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/model/region_info.py
--rw-r--r--   0 root         (0) root         (0)     4101 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/model/secret_info.py
--rw-r--r--   0 root         (0) root         (0)     9952 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/secret_manager_cache_client.py
--rw-r--r--   0 root         (0) root         (0)     5303 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/secret_manager_cache_client_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/service/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/service/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1076 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/service/back_off_strategy.py
--rw-r--r--   0 root         (0) root         (0)     2333 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/service/default_refresh_secret_strategy.py
--rw-r--r--   0 root         (0) root         (0)    21857 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/service/default_secret_manager_client_builder.py
--rw-r--r--   0 root         (0) root         (0)     1677 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/service/full_jitter_back_off_strategy.py
--rw-r--r--   0 root         (0) root         (0)     1459 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/service/refresh_secret_strategy.py
--rw-r--r--   0 root         (0) root         (0)     1138 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/service/secret_manager_client.py
--rw-r--r--   0 root         (0) root         (0)     1274 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/service/user_agent_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2115 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/aes_utils.py
--rw-r--r--   0 root         (0) root         (0)     1651 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/backoff_utils.py
--rw-r--r--   0 root         (0) root         (0)      937 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/byte_buffer_utils.py
--rw-r--r--   0 root         (0) root         (0)     2088 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/client_key_utils.py
--rw-r--r--   0 root         (0) root         (0)     1143 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/common_logger.py
--rw-r--r--   0 root         (0) root         (0)     1255 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/config_utils.py
--rw-r--r--   0 root         (0) root         (0)     1942 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/const.py
--rw-r--r--   0 root         (0) root         (0)     8640 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/credentials_properties_utils.py
--rw-r--r--   0 root         (0) root         (0)     2679 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/env_const.py
--rw-r--r--   0 root         (0) root         (0)     1370 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/err_code_const.py
--rw-r--r--   0 root         (0) root         (0)     1236 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/json_utils.py
--rw-r--r--   0 root         (0) root         (0)     1051 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/kms_end_point_utils.py
--rw-r--r--   0 root         (0) root         (0)     1614 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/ping_utils.py
--rw-r--r--   0 root         (0) root         (0)     1600 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/secret_const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/aliyun_secret_manager_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6007 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/aliyun_secret_manager_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3123 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/aliyun_secret_manager_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/aliyun_secret_manager_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      636 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/aliyun_secret_manager_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/src/aliyun_secret_manager_client.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/test/
--rw-r--r--   0 root         (0) root         (0)     3619 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/test/test_secret_cache_client.py
--rw-r--r--   0 root         (0) root         (0)      808 2022-12-19 02:37:06.000000 aliyun-secret-manager-client-0.1.0/test/test_sort_region_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:45:03.000000 aliyun-secret-manager-client-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     6111 2023-06-14 09:45:03.000000 aliyun-secret-manager-client-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4344 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 09:45:03.000000 aliyun-secret-manager-client-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2610 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:45:03.000000 aliyun-secret-manager-client-0.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:45:03.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:45:03.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/auth/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      481 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/auth/client_key_signer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:45:03.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/cache/cache_secret_store_strategy.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/cache/default_secret_cache_hook.py
+-rw-r--r--   0 root         (0) root         (0)     4992 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/cache/file_cache_secret_store_strategy.py
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/cache/memory_cache_secret_store_strategy.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/cache/secret_cache_hook.py
+-rw-r--r--   0 root         (0) root         (0)     1000 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/cache_client_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:45:03.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/model/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      155 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/model/client_key_credentials.py
+-rw-r--r--   0 root         (0) root         (0)      747 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/model/credentials_properties.py
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/model/dkms_config.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/model/region_info.py
+-rw-r--r--   0 root         (0) root         (0)     4101 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/model/secret_info.py
+-rw-r--r--   0 root         (0) root         (0)     9952 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/secret_manager_cache_client.py
+-rw-r--r--   0 root         (0) root         (0)     5303 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/secret_manager_cache_client_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:45:03.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/service/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/service/back_off_strategy.py
+-rw-r--r--   0 root         (0) root         (0)     2333 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/service/default_refresh_secret_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    21857 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/service/default_secret_manager_client_builder.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/service/full_jitter_back_off_strategy.py
+-rw-r--r--   0 root         (0) root         (0)     1459 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/service/refresh_secret_strategy.py
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/service/secret_manager_client.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/service/user_agent_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:45:03.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/aes_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/backoff_utils.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/byte_buffer_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/client_key_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/common_logger.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/config_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/const.py
+-rw-r--r--   0 root         (0) root         (0)     8640 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/credentials_properties_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/env_const.py
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/err_code_const.py
+-rw-r--r--   0 root         (0) root         (0)     1236 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/json_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/kms_end_point_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/ping_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/secret_const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:45:03.000000 aliyun-secret-manager-client-0.1.1/src/aliyun_secret_manager_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6111 2023-06-14 09:45:03.000000 aliyun-secret-manager-client-0.1.1/src/aliyun_secret_manager_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3123 2023-06-14 09:45:03.000000 aliyun-secret-manager-client-0.1.1/src/aliyun_secret_manager_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 09:45:03.000000 aliyun-secret-manager-client-0.1.1/src/aliyun_secret_manager_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      636 2023-06-14 09:45:03.000000 aliyun-secret-manager-client-0.1.1/src/aliyun_secret_manager_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-14 09:45:03.000000 aliyun-secret-manager-client-0.1.1/src/aliyun_secret_manager_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:45:03.000000 aliyun-secret-manager-client-0.1.1/test/
+-rw-r--r--   0 root         (0) root         (0)     3619 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/test/test_secret_cache_client.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-06-14 09:45:02.000000 aliyun-secret-manager-client-0.1.1/test/test_sort_region_list.py
```

### Comparing `aliyun-secret-manager-client-0.1.0/PKG-INFO` & `aliyun-secret-manager-client-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aliyun-secret-manager-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Alibaba Cloud Secrets Manager Client implementation for Python
 Home-page: UNKNOWN
 Author: Alibaba Cloud
 Maintainer: Alibaba Cloud
 License: Apache License 2.0
 Description: Aliyun Secrets Manager Client for Python
         ========================================
@@ -76,41 +76,45 @@
                print(secret_info.__dict__)
         
         -  Build Secrets Manager Client by the given parameters(accessKey,
            accessSecret, regionId, etc)
         
         .. code:: python
         
+           import os
+        
            from alibaba_cloud_secretsmanager_client.secret_manager_cache_client_builder import SecretManagerCacheClientBuilder
            from alibaba_cloud_secretsmanager_client.service.default_secret_manager_client_builder import DefaultSecretManagerClientBuilder
         
            if __name__ == '__main__':
                secret_cache_client = SecretManagerCacheClientBuilder.new_cache_client_builder(DefaultSecretManagerClientBuilder.standard() \
-                   .with_access_key("#accessKeyId#", "#accessKeySecret#") \
+                   .with_access_key(os.getenv("#accessKeyId#"), os.getenv("#accessKeySecret#")) \
                    .with_region("#regionId#").build()) \
                .build();
                secret_info = secret_cache_client.get_secret_info("#secretName#")
                print(secret_info.__dict__)
         
         Particular User Sample Code
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         -  Use custom parameters or customized implementation
         
         .. code:: python
         
+           import os
+        
            from alibaba_cloud_secretsmanager_client.secret_manager_cache_client_builder import SecretManagerCacheClientBuilder
            from alibaba_cloud_secretsmanager_client.cache.file_cache_secret_store_strategy import FileCacheSecretStoreStrategy
            from alibaba_cloud_secretsmanager_client.service.default_secret_manager_client_builder import DefaultSecretManagerClientBuilder
            from alibaba_cloud_secretsmanager_client.service.default_refresh_secret_strategy import DefaultRefreshSecretStrategy
            from alibaba_cloud_secretsmanager_client.service.full_jitter_back_off_strategy import FullJitterBackoffStrategy
         
            if __name__ == '__main__':
                secret_cache_client = SecretManagerCacheClientBuilder \
-               .new_cache_client_builder(DefaultSecretManagerClientBuilder.standard().with_access_key("#accessKeyId#", "#accessKeySecret#") \
+               .new_cache_client_builder(DefaultSecretManagerClientBuilder.standard().with_access_key(os.getenv("#accessKeyId#"), os.getenv("#accessKeySecret#")) \
                     .with_back_off_strategy(FullJitterBackoffStrategy(3, 2000, 10000)) \
                     .with_region("#regionId#").build()) \
                 .with_cache_secret_strategy(FileCacheSecretStoreStrategy("#cacheSecretPath#", True,"#salt#")) \
                 .with_refresh_secret_strategy(DefaultRefreshSecretStrategy("#ttlName#")) \
                 .with_cache_stage("#stage#") \
                 .with_secret_ttl("#secretName#", 1 * 60 * 1000l) \
                 .build()
```

### Comparing `aliyun-secret-manager-client-0.1.0/README.rst` & `aliyun-secret-manager-client-0.1.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -68,41 +68,45 @@
        print(secret_info.__dict__)
 
 -  Build Secrets Manager Client by the given parameters(accessKey,
    accessSecret, regionId, etc)
 
 .. code:: python
 
+   import os
+
    from alibaba_cloud_secretsmanager_client.secret_manager_cache_client_builder import SecretManagerCacheClientBuilder
    from alibaba_cloud_secretsmanager_client.service.default_secret_manager_client_builder import DefaultSecretManagerClientBuilder
 
    if __name__ == '__main__':
        secret_cache_client = SecretManagerCacheClientBuilder.new_cache_client_builder(DefaultSecretManagerClientBuilder.standard() \
-           .with_access_key("#accessKeyId#", "#accessKeySecret#") \
+           .with_access_key(os.getenv("#accessKeyId#"), os.getenv("#accessKeySecret#")) \
            .with_region("#regionId#").build()) \
        .build();
        secret_info = secret_cache_client.get_secret_info("#secretName#")
        print(secret_info.__dict__)
 
 Particular User Sample Code
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 -  Use custom parameters or customized implementation
 
 .. code:: python
 
+   import os
+
    from alibaba_cloud_secretsmanager_client.secret_manager_cache_client_builder import SecretManagerCacheClientBuilder
    from alibaba_cloud_secretsmanager_client.cache.file_cache_secret_store_strategy import FileCacheSecretStoreStrategy
    from alibaba_cloud_secretsmanager_client.service.default_secret_manager_client_builder import DefaultSecretManagerClientBuilder
    from alibaba_cloud_secretsmanager_client.service.default_refresh_secret_strategy import DefaultRefreshSecretStrategy
    from alibaba_cloud_secretsmanager_client.service.full_jitter_back_off_strategy import FullJitterBackoffStrategy
 
    if __name__ == '__main__':
        secret_cache_client = SecretManagerCacheClientBuilder \
-       .new_cache_client_builder(DefaultSecretManagerClientBuilder.standard().with_access_key("#accessKeyId#", "#accessKeySecret#") \
+       .new_cache_client_builder(DefaultSecretManagerClientBuilder.standard().with_access_key(os.getenv("#accessKeyId#"), os.getenv("#accessKeySecret#")) \
             .with_back_off_strategy(FullJitterBackoffStrategy(3, 2000, 10000)) \
             .with_region("#regionId#").build()) \
         .with_cache_secret_strategy(FileCacheSecretStoreStrategy("#cacheSecretPath#", True,"#salt#")) \
         .with_refresh_secret_strategy(DefaultRefreshSecretStrategy("#ttlName#")) \
         .with_cache_stage("#stage#") \
         .with_secret_ttl("#secretName#", 1 * 60 * 1000l) \
         .build()
```

### Comparing `aliyun-secret-manager-client-0.1.0/setup.py` & `aliyun-secret-manager-client-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/cache/cache_secret_store_strategy.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/cache/cache_secret_store_strategy.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/cache/default_secret_cache_hook.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/cache/default_secret_cache_hook.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/cache/file_cache_secret_store_strategy.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/cache/file_cache_secret_store_strategy.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/cache/memory_cache_secret_store_strategy.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/cache/memory_cache_secret_store_strategy.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/cache/secret_cache_hook.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/cache/secret_cache_hook.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/cache_client_builder.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/cache_client_builder.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/model/credentials_properties.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/model/credentials_properties.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/model/dkms_config.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/model/dkms_config.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/model/region_info.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/model/region_info.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/model/secret_info.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/model/secret_info.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/secret_manager_cache_client.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/secret_manager_cache_client.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/secret_manager_cache_client_builder.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/secret_manager_cache_client_builder.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/service/back_off_strategy.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/service/back_off_strategy.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/service/default_refresh_secret_strategy.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/service/default_refresh_secret_strategy.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/service/default_secret_manager_client_builder.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/service/default_secret_manager_client_builder.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/service/full_jitter_back_off_strategy.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/service/full_jitter_back_off_strategy.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/service/refresh_secret_strategy.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/service/refresh_secret_strategy.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/service/secret_manager_client.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/service/secret_manager_client.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/service/user_agent_manager.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/service/user_agent_manager.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/aes_utils.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/aes_utils.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/backoff_utils.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/backoff_utils.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/byte_buffer_utils.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/byte_buffer_utils.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/client_key_utils.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/client_key_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,8 +43,8 @@
     if password is None or password == "":
         raise ValueError("client key password is not provided")
     return password
 
 
 def read_password_file(password_file_path):
     with open(password_file_path) as f:
-        return f.read()
+        return f.read().strip().replace('\n', '').replace('\r', '')
```

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/common_logger.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/common_logger.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/config_utils.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/config_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def get_properties(self):
         pro_file = None
         try:
             if not os.path.exists(self.file_name):
                 return None
             pro_file = open(self.file_name, 'Ur')
             for line in pro_file.readlines():
-                line = line.strip().replace('\n', '')
+                line = line.strip().replace('\n', '').replace('\r', '')
                 if line.find("#") != -1:
                     line = line[0:line.find('#')]
                 if line.find('=') > 0:
                     strs = line.split('=')
                     strs[1] = line[len(strs[0]) + 1:]
                     self.__get_dict(strs[0].strip(), self.properties, strs[1].strip())
         except Exception as e:
```

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/const.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/const.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/credentials_properties_utils.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/credentials_properties_utils.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/env_const.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/env_const.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/err_code_const.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/err_code_const.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/json_utils.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/kms_end_point_utils.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/kms_end_point_utils.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/ping_utils.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/ping_utils.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/alibaba_cloud_secretsmanager_client/utils/secret_const.py` & `aliyun-secret-manager-client-0.1.1/src/alibaba_cloud_secretsmanager_client/utils/secret_const.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/aliyun_secret_manager_client.egg-info/PKG-INFO` & `aliyun-secret-manager-client-0.1.1/src/aliyun_secret_manager_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aliyun-secret-manager-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Alibaba Cloud Secrets Manager Client implementation for Python
 Home-page: UNKNOWN
 Author: Alibaba Cloud
 Maintainer: Alibaba Cloud
 License: Apache License 2.0
 Description: Aliyun Secrets Manager Client for Python
         ========================================
@@ -76,41 +76,45 @@
                print(secret_info.__dict__)
         
         -  Build Secrets Manager Client by the given parameters(accessKey,
            accessSecret, regionId, etc)
         
         .. code:: python
         
+           import os
+        
            from alibaba_cloud_secretsmanager_client.secret_manager_cache_client_builder import SecretManagerCacheClientBuilder
            from alibaba_cloud_secretsmanager_client.service.default_secret_manager_client_builder import DefaultSecretManagerClientBuilder
         
            if __name__ == '__main__':
                secret_cache_client = SecretManagerCacheClientBuilder.new_cache_client_builder(DefaultSecretManagerClientBuilder.standard() \
-                   .with_access_key("#accessKeyId#", "#accessKeySecret#") \
+                   .with_access_key(os.getenv("#accessKeyId#"), os.getenv("#accessKeySecret#")) \
                    .with_region("#regionId#").build()) \
                .build();
                secret_info = secret_cache_client.get_secret_info("#secretName#")
                print(secret_info.__dict__)
         
         Particular User Sample Code
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         -  Use custom parameters or customized implementation
         
         .. code:: python
         
+           import os
+        
            from alibaba_cloud_secretsmanager_client.secret_manager_cache_client_builder import SecretManagerCacheClientBuilder
            from alibaba_cloud_secretsmanager_client.cache.file_cache_secret_store_strategy import FileCacheSecretStoreStrategy
            from alibaba_cloud_secretsmanager_client.service.default_secret_manager_client_builder import DefaultSecretManagerClientBuilder
            from alibaba_cloud_secretsmanager_client.service.default_refresh_secret_strategy import DefaultRefreshSecretStrategy
            from alibaba_cloud_secretsmanager_client.service.full_jitter_back_off_strategy import FullJitterBackoffStrategy
         
            if __name__ == '__main__':
                secret_cache_client = SecretManagerCacheClientBuilder \
-               .new_cache_client_builder(DefaultSecretManagerClientBuilder.standard().with_access_key("#accessKeyId#", "#accessKeySecret#") \
+               .new_cache_client_builder(DefaultSecretManagerClientBuilder.standard().with_access_key(os.getenv("#accessKeyId#"), os.getenv("#accessKeySecret#")) \
                     .with_back_off_strategy(FullJitterBackoffStrategy(3, 2000, 10000)) \
                     .with_region("#regionId#").build()) \
                 .with_cache_secret_strategy(FileCacheSecretStoreStrategy("#cacheSecretPath#", True,"#salt#")) \
                 .with_refresh_secret_strategy(DefaultRefreshSecretStrategy("#ttlName#")) \
                 .with_cache_stage("#stage#") \
                 .with_secret_ttl("#secretName#", 1 * 60 * 1000l) \
                 .build()
```

### Comparing `aliyun-secret-manager-client-0.1.0/src/aliyun_secret_manager_client.egg-info/SOURCES.txt` & `aliyun-secret-manager-client-0.1.1/src/aliyun_secret_manager_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/src/aliyun_secret_manager_client.egg-info/requires.txt` & `aliyun-secret-manager-client-0.1.1/src/aliyun_secret_manager_client.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/test/test_secret_cache_client.py` & `aliyun-secret-manager-client-0.1.1/test/test_secret_cache_client.py`

 * *Files identical despite different names*

### Comparing `aliyun-secret-manager-client-0.1.0/test/test_sort_region_list.py` & `aliyun-secret-manager-client-0.1.1/test/test_sort_region_list.py`

 * *Files identical despite different names*

