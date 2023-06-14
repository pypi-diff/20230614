# Comparing `tmp/backend.ai-common-23.3.5.tar.gz` & `tmp/backend.ai-common-23.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-common-23.3.5.tar", last modified: Tue Jun 13 03:42:14 2023, max compression
+gzip compressed data, was "backend.ai-common-23.3.6.tar", last modified: Wed Jun 14 11:13:21 2023, max compression
```

## Comparing `backend.ai-common-23.3.5.tar` & `backend.ai-common-23.3.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.228272 backend.ai-common-23.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-13 03:42:14.228272 backend.ai-common-23.3.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.220272 backend.ai-common-23.3.5/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.220272 backend.ai-common-23.3.5/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.224272 backend.ai-common-23.3.5/ai/backend/common/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/bgtask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/cgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/enum_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/enum_extension.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19237 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)    26339 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    21123 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/netns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.224272 backend.ai-common-23.3.5/ai/backend/common/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/plugin/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/plugin/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/plugin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16566 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/redis_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/sd_notify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/service_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31841 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23523 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.220272 backend.ai-common-23.3.5/ai/backend/common/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.224272 backend.ai-common-23.3.5/ai/backend/common/web/session/
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/web/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/web/session/redis_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.228272 backend.ai-common-23.3.5/backend.ai_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-13 03:42:14.000000 backend.ai-common-23.3.5/backend.ai_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-13 03:42:14.000000 backend.ai-common-23.3.5/backend.ai_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:14.000000 backend.ai-common-23.3.5/backend.ai_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:14.000000 backend.ai-common-23.3.5/backend.ai_common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:14.000000 backend.ai-common-23.3.5/backend.ai_common.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-13 03:42:14.000000 backend.ai-common-23.3.5/backend.ai_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-13 03:42:14.000000 backend.ai-common-23.3.5/backend.ai_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 03:42:14.228272 backend.ai-common-23.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.497671 backend.ai-common-23.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-14 11:13:21.497671 backend.ai-common-23.3.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.489671 backend.ai-common-23.3.6/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.489671 backend.ai-common-23.3.6/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.493671 backend.ai-common-23.3.6/ai/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/bgtask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/cgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/enum_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/enum_extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19237 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26339 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21123 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/netns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.493671 backend.ai-common-23.3.6/ai/backend/common/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/plugin/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/plugin/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/plugin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16566 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/redis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/sd_notify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/service_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31841 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23523 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.489671 backend.ai-common-23.3.6/ai/backend/common/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.493671 backend.ai-common-23.3.6/ai/backend/common/web/session/
+-rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/web/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/ai/backend/common/web/session/redis_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.497671 backend.ai-common-23.3.6/backend.ai_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-14 11:13:21.000000 backend.ai-common-23.3.6/backend.ai_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-14 11:13:21.000000 backend.ai-common-23.3.6/backend.ai_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:21.000000 backend.ai-common-23.3.6/backend.ai_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:21.000000 backend.ai-common-23.3.6/backend.ai_common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:21.000000 backend.ai-common-23.3.6/backend.ai_common.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-14 11:13:21.000000 backend.ai-common-23.3.6/backend.ai_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-14 11:13:21.000000 backend.ai-common-23.3.6/backend.ai_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:13:21.497671 backend.ai-common-23.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-14 11:13:20.000000 backend.ai-common-23.3.6/setup.py
```

### Comparing `backend.ai-common-23.3.5/PKG-INFO` & `backend.ai-common-23.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-common
-Version: 23.3.5
+Version: 23.3.6
 Summary: Backend.AI commons library
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-common-23.3.5/ai/backend/common/argparse.py` & `backend.ai-common-23.3.6/ai/backend/common/argparse.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/asyncio.py` & `backend.ai-common-23.3.6/ai/backend/common/asyncio.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/bgtask.py` & `backend.ai-common-23.3.6/ai/backend/common/bgtask.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/cgroup.py` & `backend.ai-common-23.3.6/ai/backend/common/cgroup.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/cli.py` & `backend.ai-common-23.3.6/ai/backend/common/cli.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/config.py` & `backend.ai-common-23.3.6/ai/backend/common/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/distributed.py` & `backend.ai-common-23.3.6/ai/backend/common/distributed.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/docker.py` & `backend.ai-common-23.3.6/ai/backend/common/docker.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/enum_extension.py` & `backend.ai-common-23.3.6/ai/backend/common/enum_extension.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/enum_extension.pyi` & `backend.ai-common-23.3.6/ai/backend/common/enum_extension.pyi`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/etcd.py` & `backend.ai-common-23.3.6/ai/backend/common/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/events.py` & `backend.ai-common-23.3.6/ai/backend/common/events.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/exception.py` & `backend.ai-common-23.3.6/ai/backend/common/exception.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/files.py` & `backend.ai-common-23.3.6/ai/backend/common/files.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/identity.py` & `backend.ai-common-23.3.6/ai/backend/common/identity.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/lock.py` & `backend.ai-common-23.3.6/ai/backend/common/lock.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/logging.py` & `backend.ai-common-23.3.6/ai/backend/common/logging.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/logging_utils.py` & `backend.ai-common-23.3.6/ai/backend/common/logging_utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/msgpack.py` & `backend.ai-common-23.3.6/ai/backend/common/msgpack.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/netns.py` & `backend.ai-common-23.3.6/ai/backend/common/netns.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/networking.py` & `backend.ai-common-23.3.6/ai/backend/common/networking.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/plugin/__init__.py` & `backend.ai-common-23.3.6/ai/backend/common/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/plugin/hook.py` & `backend.ai-common-23.3.6/ai/backend/common/plugin/hook.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/plugin/monitor.py` & `backend.ai-common-23.3.6/ai/backend/common/plugin/monitor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/redis_helper.py` & `backend.ai-common-23.3.6/ai/backend/common/redis_helper.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/sd_notify.py` & `backend.ai-common-23.3.6/ai/backend/common/sd_notify.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/service_ports.py` & `backend.ai-common-23.3.6/ai/backend/common/service_ports.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/testutils.py` & `backend.ai-common-23.3.6/ai/backend/common/testutils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/types.py` & `backend.ai-common-23.3.6/ai/backend/common/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/utils.py` & `backend.ai-common-23.3.6/ai/backend/common/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/validators.py` & `backend.ai-common-23.3.6/ai/backend/common/validators.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/web/session/__init__.py` & `backend.ai-common-23.3.6/ai/backend/common/web/session/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/ai/backend/common/web/session/redis_storage.py` & `backend.ai-common-23.3.6/ai/backend/common/web/session/redis_storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/backend.ai_common.egg-info/PKG-INFO` & `backend.ai-common-23.3.6/backend.ai_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-common
-Version: 23.3.5
+Version: 23.3.6
 Summary: Backend.AI commons library
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-common-23.3.5/backend.ai_common.egg-info/SOURCES.txt` & `backend.ai-common-23.3.6/backend.ai_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/backend.ai_common.egg-info/requires.txt` & `backend.ai-common-23.3.6/backend.ai_common.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 aiohttp~=3.8.1
 aiomonitor-ng~=0.7.2
 aiotools~=1.6.1
 async_timeout~=4.0
 asynctest>=0.13.0
 asyncudp>=0.4
 attrs>=20.3
-backend.ai-plugin==23.03.5
+backend.ai-plugin==23.03.6
 click>=7.1.2
 coloredlogs~=15.0
 etcetra==0.1.15
 ifaddr~=0.2
 janus~=1.0.0
 msgpack>=1.0.5rc1
 multidict>=6.0
```

### Comparing `backend.ai-common-23.3.5/backend_shim.py` & `backend.ai-common-23.3.6/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.5/setup.py` & `backend.ai-common-23.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         'aiohttp~=3.8.1',
         'aiomonitor-ng~=0.7.2',
         'aiotools~=1.6.1',
         'async_timeout~=4.0',
         'asynctest>=0.13.0',
         'asyncudp>=0.4',
         'attrs>=20.3',
-        """backend.ai-plugin==23.03.5
+        """backend.ai-plugin==23.03.6
 """,
         'click>=7.1.2',
         'coloredlogs~=15.0',
         'etcetra==0.1.15',
         'ifaddr~=0.2',
         'janus~=1.0.0',
         'msgpack>=1.0.5rc1',
@@ -119,11 +119,11 @@
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

