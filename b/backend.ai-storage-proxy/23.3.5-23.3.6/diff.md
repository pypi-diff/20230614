# Comparing `tmp/backend.ai-storage-proxy-23.3.5.tar.gz` & `tmp/backend.ai-storage-proxy-23.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-storage-proxy-23.3.5.tar", last modified: Tue Jun 13 03:42:13 2023, max compression
+gzip compressed data, was "backend.ai-storage-proxy-23.3.6.tar", last modified: Wed Jun 14 11:13:21 2023, max compression
```

## Comparing `backend.ai-storage-proxy-23.3.5.tar` & `backend.ai-storage-proxy-23.3.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.000276 backend.ai-storage-proxy-23.3.5/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.000276 backend.ai-storage-proxy-23.3.5/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.004276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.004276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14443 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/api/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.004276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/cephfs/
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/cephfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.004276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/dellemc/
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/dellemc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/dellemc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/dellemc/onefs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/gpfs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/netapp/
--rw-r--r--   0 runner    (1001) docker     (123)    20336 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/netapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19998 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/netapp/netappclient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/purestorage/
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/purestorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/purestorage/purity.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/subproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/vfs/
--rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/vfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/weka/
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/weka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/weka/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/weka/weka_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/xfs/
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/xfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.469671 backend.ai-storage-proxy-23.3.6/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.469671 backend.ai-storage-proxy-23.3.6/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.469671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.469671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14443 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/api/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.469671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/cephfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/cephfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.469671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/dellemc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/dellemc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/dellemc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/dellemc/onefs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.469671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/gpfs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/netapp/
+-rw-r--r--   0 runner    (1001) docker     (123)    20336 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/netapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19998 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/netapp/netappclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/purestorage/
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/purestorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/purestorage/purity.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/subproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/vfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/vfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/weka/
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/weka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/weka/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/weka/weka_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/xfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/xfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-06-14 11:13:21.000000 backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-14 11:13:21.000000 backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:21.000000 backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:21.000000 backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:21.000000 backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-14 11:13:21.000000 backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-14 11:13:21.000000 backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/setup.py
```

### Comparing `backend.ai-storage-proxy-23.3.5/PKG-INFO` & `backend.ai-storage-proxy-23.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 23.3.5
+Version: 23.3.6
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/abc.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/abc.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/api/client.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/api/client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/api/manager.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/api/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/cephfs/__init__.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/cephfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/config.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/context.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/dellemc/__init__.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/dellemc/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/dellemc/exceptions.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/dellemc/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/dellemc/onefs_client.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/dellemc/onefs_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/exception.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/exception.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/__init__.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/exceptions.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/gpfs_client.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/gpfs_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/types.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/migration.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/migration.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
                     else:
                         current_size = None
                     if quota_scope_id not in created_quota_scopes:
                         await volume.quota_model.create_quota_scope(quota_scope_id)
                         created_quota_scopes.add(quota_scope_id)
                     await volume.fsop_model.move_tree(
                         volume.mangle_vfpath(orig_vfid),
-                        volume.quota_model.mangle_qspath(dst_vfid),
+                        volume.mangle_vfpath(dst_vfid),
                     )
                 except Exception:
                     log.exception("error during migration of vfolder {}", folder_id)
                     async with (
                         connect_database(ctx.dsn) as conn,
                         conn.transaction(),
                     ):
```

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/netapp/__init__.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/netapp/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/netapp/netappclient.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/netapp/netappclient.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/purestorage/__init__.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/purestorage/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/purestorage/purity.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/purestorage/purity.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/server.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/server.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/subproc.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/subproc.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/types.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/utils.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/vfs/__init__.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/vfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/weka/__init__.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/weka/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/weka/exceptions.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/weka/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/weka/weka_client.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/weka/weka_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/ai/backend/storage/xfs/__init__.py` & `backend.ai-storage-proxy-23.3.6/ai/backend/storage/xfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/PKG-INFO` & `backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 23.3.5
+Version: 23.3.6
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/SOURCES.txt` & `backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/backend_shim.py` & `backend.ai-storage-proxy-23.3.6/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.5/setup.py` & `backend.ai-storage-proxy-23.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         'aiofiles~=0.8.0',
         'aiohttp_cors~=0.7',
         'aiohttp~=3.8.1',
         'aiomonitor-ng~=0.7.2',
         'aiotools~=1.6.1',
         'asyncpg>=0.27.0',
         'attrs>=20.3',
-        """backend.ai-common==23.03.5
+        """backend.ai-common==23.03.6
 """,
         'click>=7.1.2',
         'dataclasses-json~=0.5.7',
         'janus~=1.0.0',
         'more-itertools~=8.13.0',
         'setproctitle~=1.3.2',
         'tenacity>=8.0',
@@ -250,11 +250,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.5
+    'version': """23.03.6
 """,
     'zip_safe': False,
 })
```

