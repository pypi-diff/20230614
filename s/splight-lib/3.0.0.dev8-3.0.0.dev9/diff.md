# Comparing `tmp/splight-lib-3.0.0.dev8.tar.gz` & `tmp/splight-lib-3.0.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-lib-3.0.0.dev8.tar", last modified: Fri Jun  9 20:13:25 2023, max compression
+gzip compressed data, was "splight-lib-3.0.0.dev9.tar", last modified: Tue Jun 13 13:04:59 2023, max compression
```

## Comparing `splight-lib-3.0.0.dev8.tar` & `splight-lib-3.0.0.dev9.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:25.441102 splight-lib-3.0.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-09 20:13:25.441102 splight-lib-3.0.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 20:13:25.441102 splight-lib-3.0.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:25.433102 splight-lib-3.0.0.dev8/splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:25.433102 splight-lib-3.0.0.dev8/splight_lib/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/abstract/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:25.433102 splight-lib-3.0.0.dev8/splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/auth/mac_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:25.437101 splight-lib-3.0.0.dev8/splight_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:25.437101 splight-lib-3.0.0.dev8/splight_lib/client/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/communication/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/communication/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/communication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/communication/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/communication/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:25.437101 splight-lib-3.0.0.dev8/splight_lib/client/database/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/database/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/database/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/database/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/database/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:25.437101 splight-lib-3.0.0.dev8/splight_lib/client/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/datalake/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/datalake/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/datalake/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:25.437101 splight-lib-3.0.0.dev8/splight_lib/client/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/hub/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/client/hub/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:25.437101 splight-lib-3.0.0.dev8/splight_lib/communication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/communication/event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:25.437101 splight-lib-3.0.0.dev8/splight_lib/component/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/component/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/component/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:25.437101 splight-lib-3.0.0.dev8/splight_lib/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/logging/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/logging/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/logging/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:25.441102 splight-lib-3.0.0.dev8/splight_lib/models/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/models/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/models/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/models/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/models/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/models/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/models/setpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:25.441102 splight-lib-3.0.0.dev8/splight_lib/restclient/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/restclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/restclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/restclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/restclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:25.441102 splight-lib-3.0.0.dev8/splight_lib/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:25.441102 splight-lib-3.0.0.dev8/splight_lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/utils/custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-09 20:13:24.000000 splight-lib-3.0.0.dev8/splight_lib/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:13:25.433102 splight-lib-3.0.0.dev8/splight_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-09 20:13:25.000000 splight-lib-3.0.0.dev8/splight_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-09 20:13:25.000000 splight-lib-3.0.0.dev8/splight_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 20:13:25.000000 splight-lib-3.0.0.dev8/splight_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 20:13:25.000000 splight-lib-3.0.0.dev8/splight_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-09 20:13:25.000000 splight-lib-3.0.0.dev8/splight_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-09 20:13:25.000000 splight-lib-3.0.0.dev8/splight_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:59.430927 splight-lib-3.0.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-13 13:04:59.430927 splight-lib-3.0.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 13:04:59.430927 splight-lib-3.0.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:59.422927 splight-lib-3.0.0.dev9/splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:59.422927 splight-lib-3.0.0.dev9/splight_lib/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/abstract/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:59.426927 splight-lib-3.0.0.dev9/splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/auth/mac_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:59.426927 splight-lib-3.0.0.dev9/splight_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:59.426927 splight-lib-3.0.0.dev9/splight_lib/client/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/communication/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/communication/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/communication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/communication/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/communication/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:59.426927 splight-lib-3.0.0.dev9/splight_lib/client/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/database/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/database/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/database/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/database/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:59.426927 splight-lib-3.0.0.dev9/splight_lib/client/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/datalake/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/datalake/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:59.426927 splight-lib-3.0.0.dev9/splight_lib/client/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/hub/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/client/hub/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:59.426927 splight-lib-3.0.0.dev9/splight_lib/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/communication/event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:59.426927 splight-lib-3.0.0.dev9/splight_lib/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/component/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/component/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:59.426927 splight-lib-3.0.0.dev9/splight_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/logging/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/logging/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/logging/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:59.430927 splight-lib-3.0.0.dev9/splight_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/models/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/models/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/models/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/models/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/models/setpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:59.430927 splight-lib-3.0.0.dev9/splight_lib/restclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/restclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/restclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/restclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/restclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:59.430927 splight-lib-3.0.0.dev9/splight_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:59.430927 splight-lib-3.0.0.dev9/splight_lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/utils/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-13 13:04:56.000000 splight-lib-3.0.0.dev9/splight_lib/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:04:59.422927 splight-lib-3.0.0.dev9/splight_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-13 13:04:59.000000 splight-lib-3.0.0.dev9/splight_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-13 13:04:59.000000 splight-lib-3.0.0.dev9/splight_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:04:59.000000 splight-lib-3.0.0.dev9/splight_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:04:59.000000 splight-lib-3.0.0.dev9/splight_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-13 13:04:59.000000 splight-lib-3.0.0.dev9/splight_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 13:04:59.000000 splight-lib-3.0.0.dev9/splight_lib.egg-info/top_level.txt
```

### Comparing `splight-lib-3.0.0.dev8/PKG-INFO` & `splight-lib-3.0.0.dev9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 3.0.0.dev8
+Version: 3.0.0.dev9
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-3.0.0.dev8/setup.py` & `splight-lib-3.0.0.dev9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 test_requires = [
     "pytest==7.1.2",
     "mock==4.0.3",
 ]
 
 setup(
     name="splight-lib",
-    version="3.0.0.dev8",
+    version="3.0.0.dev9",
     author="Splight",
     author_email="factory@splight-ae.com",
     packages=find_packages(),
     package_data={},
     include_package_data=True,
     scripts=[],
     url=None,
```

### Comparing `splight-lib-3.0.0.dev8/splight_lib/abstract/client.py` & `splight-lib-3.0.0.dev9/splight_lib/abstract/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/auth/mac_auth.py` & `splight-lib-3.0.0.dev9/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/client/communication/abstract.py` & `splight-lib-3.0.0.dev9/splight_lib/client/communication/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/client/communication/remote_client.py` & `splight-lib-3.0.0.dev9/splight_lib/client/communication/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/client/database/abstract.py` & `splight-lib-3.0.0.dev9/splight_lib/client/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/client/database/builder.py` & `splight-lib-3.0.0.dev9/splight_lib/client/database/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/client/database/classmap.py` & `splight-lib-3.0.0.dev9/splight_lib/client/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/client/database/local_client.py` & `splight-lib-3.0.0.dev9/splight_lib/client/database/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/client/database/remote_client.py` & `splight-lib-3.0.0.dev9/splight_lib/client/database/remote_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,15 +101,16 @@
         """
         logger.debug("Deleting instance %s.", id, tags=LogTags.DATABASE)
         api_path = self._get_api_path(resource_name)
         url = self._base_url / api_path / f"{id}/"
         response = self._restclient.delete(url)
         response.raise_for_status()
 
-    @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=1)
+    # @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=1)
+    @retry(Exception, tries=3, delay=1)
     def _get(
         self,
         resource_name: str,
         first: bool = False,
         **kwargs,
     ) -> Union[Dict, List[Dict]]:
         """Retrieves one or multiple resources. If the parameter id is passed
@@ -141,36 +142,44 @@
             raise InvalidModelName(model_name)
         api_path = api_path.format_map({"prefix": ENGINE_PREFIX, **instance})
         url = self._base_url / api_path
         response = self._restclient.post(url, json=instance)
         response.raise_for_status()
         return response.json()
 
+    # @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=1)
     def _retrieve_multiple(
         self, resource_name: str, first: bool = False, **kwargs
     ) -> List[Dict]:
+        logger.debug(f"Retrieving objects {resource_name}")
         api_path = self._get_api_path(resource_name)
         url = self._base_url / api_path
         instances = []
         for page in self._pages(url, page=1, **kwargs):
             instances.extend(page["results"])
 
         if first:
             return [instances[0]] if instances else []
         return instances
 
-    @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=1)
+    # @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=1)
     def _retrieve_single(self, resource_name: str, id: str) -> Dict:
+        logger.debug(f"Retrieving object {resource_name} with id {id}")
         api_path = self._get_api_path(resource_name)
         url = self._base_url / api_path / f"{id}/"
         response = self._restclient.get(url)
         if response.status_code == codes.NOT_FOUND:
             raise InstanceNotFound(resource_name, id)
         else:
-            response.raise_for_status()
+            try:
+                response.raise_for_status()
+            except Exception as exc:
+                import traceback, sys
+                traceback.print_exc()
+                __import__('ipdb').set_trace()
         return response.json()
 
     @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=1)
     def download(
         self,
         resource_name: str,
         instance: Dict,
```

### Comparing `splight-lib-3.0.0.dev8/splight_lib/client/datalake/abstract.py` & `splight-lib-3.0.0.dev9/splight_lib/client/datalake/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/client/datalake/builder.py` & `splight-lib-3.0.0.dev9/splight_lib/client/datalake/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/client/datalake/local_client.py` & `splight-lib-3.0.0.dev9/splight_lib/client/datalake/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/client/datalake/remote_client.py` & `splight-lib-3.0.0.dev9/splight_lib/client/datalake/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/client/exceptions.py` & `splight-lib-3.0.0.dev9/splight_lib/client/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,22 @@
+from httpx import ConnectError, ReadTimeout
 from requests.exceptions import ConnectionError, Timeout
-from splight_lib.restclient import ConnectError, HTTPError
+
+from splight_lib.restclient import ConnectError as SplightConnectError
+from splight_lib.restclient import HTTPError
 from splight_lib.restclient import Timeout as TimeoutError
 
 REQUEST_EXCEPTIONS = (ConnectionError, Timeout)
-SPLIGHT_REQUEST_EXCEPTIONS = (HTTPError, TimeoutError, ConnectError)
+SPLIGHT_REQUEST_EXCEPTIONS = (
+    HTTPError,
+    TimeoutError,
+    ConnectError,
+    ReadTimeout,
+    SplightConnectError,
+)
 
 
 class InvalidModelName(Exception):
     def __init__(self, model_name: str):
         self._msg = f"Model {model_name} is not a valid database model"
 
     def __str__(self) -> str:
```

### Comparing `splight-lib-3.0.0.dev8/splight_lib/client/file_handler.py` & `splight-lib-3.0.0.dev9/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/client/filter.py` & `splight-lib-3.0.0.dev9/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/client/hub/abstract.py` & `splight-lib-3.0.0.dev9/splight_lib/client/hub/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/client/hub/client.py` & `splight-lib-3.0.0.dev9/splight_lib/client/hub/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/communication/event_handler.py` & `splight-lib-3.0.0.dev9/splight_lib/communication/event_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/component/abstract.py` & `splight-lib-3.0.0.dev9/splight_lib/component/abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from threading import Thread
 from time import sleep
 from typing import Dict, List, Optional, Type
 
 from furl import furl
 from pydantic import BaseModel, create_model
 from retry import retry
+
 from splight_lib.auth import SplightAuthToken
 
 # TODO: Use builder pattern
 from splight_lib.client.communication import RemoteCommunicationClient
 from splight_lib.communication.event_handler import (
     command_event_handler,
     database_object_event_handler,
```

### Comparing `splight-lib-3.0.0.dev8/splight_lib/component/exceptions.py` & `splight-lib-3.0.0.dev9/splight_lib/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/component/spec.py` & `splight-lib-3.0.0.dev9/splight_lib/component/spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Dict, List, Optional, Set, Type
 
 from pydantic import AnyUrl, BaseModel, Field, create_model, validator
+
 from splight_lib.component.exceptions import (
     DuplicatedValuesError,
     ParameterDependencyError,
 )
 from splight_lib.models.base import SplightDatalakeBaseModel
 from splight_lib.models.component import (
     Binding,
```

### Comparing `splight-lib-3.0.0.dev8/splight_lib/encryption.py` & `splight-lib-3.0.0.dev9/splight_lib/encryption.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from functools import cached_property
 from typing import Optional
 
 from cryptography.fernet import Fernet as Branca
 from pydantic import BaseSettings
+from splight_lib.logging._internal import LogTags, get_splight_logger
+
+logger = get_splight_logger()
 
 
 class EncryptionSettings(BaseSettings):
     SPLIGHT_ENCRYPTION_KEY: Optional[str] = None
 
 
 class EncryptionClient:
@@ -23,19 +26,27 @@
     def fernet(self):
         if not self._fernet:
             self._fernet = Branca(self.key)
         return self._fernet
 
     def encrypt(self, value: str):
         if not self.key:
+            logger.warning(
+                "Returning non-encrypted value since encryption key was not found in the environment",
+                tags=LogTags.SECRET,
+            )
             return value
         return self.fernet.encrypt(value.encode()).decode()
 
     def decrypt(self, value: str):
         if not self.key:
+            logger.warning(
+                "Returning encrypted value since encryption key was not found in the environment",
+                tags=LogTags.SECRET,
+            )
             return value
         return self.fernet.decrypt(value.encode()).decode()
 
     def encrypt_file(self, path: str):
         if not self.key:
             return None
         with open(path, "rb+") as f:
```

### Comparing `splight-lib-3.0.0.dev8/splight_lib/execution.py` & `splight-lib-3.0.0.dev9/splight_lib/execution.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/logging/_internal.py` & `splight-lib-3.0.0.dev9/splight_lib/logging/_internal.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/logging/component.py` & `splight-lib-3.0.0.dev9/splight_lib/logging/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/logging/logging.py` & `splight-lib-3.0.0.dev9/splight_lib/logging/logging.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/models/__init__.py` & `splight-lib-3.0.0.dev9/splight_lib/models/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/models/alert.py` & `splight-lib-3.0.0.dev9/splight_lib/models/alert.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/models/asset.py` & `splight-lib-3.0.0.dev9/splight_lib/models/asset.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/models/base.py` & `splight-lib-3.0.0.dev9/splight_lib/models/base.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/models/communication.py` & `splight-lib-3.0.0.dev9/splight_lib/models/communication.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/models/component.py` & `splight-lib-3.0.0.dev9/splight_lib/models/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/models/event.py` & `splight-lib-3.0.0.dev9/splight_lib/models/event.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/models/file.py` & `splight-lib-3.0.0.dev9/splight_lib/models/file.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/models/hub.py` & `splight-lib-3.0.0.dev9/splight_lib/models/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/models/native.py` & `splight-lib-3.0.0.dev9/splight_lib/models/native.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/models/query.py` & `splight-lib-3.0.0.dev9/splight_lib/models/query.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/models/setpoint.py` & `splight-lib-3.0.0.dev9/splight_lib/models/setpoint.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/restclient/client.py` & `splight-lib-3.0.0.dev9/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/restclient/exceptions.py` & `splight-lib-3.0.0.dev9/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/restclient/types.py` & `splight-lib-3.0.0.dev9/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/settings.py` & `splight-lib-3.0.0.dev9/splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/testing/__init__.py` & `splight-lib-3.0.0.dev9/splight_lib/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/utils/custom_model.py` & `splight-lib-3.0.0.dev9/splight_lib/utils/custom_model.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/utils/hub.py` & `splight-lib-3.0.0.dev9/splight_lib/utils/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib/webhook.py` & `splight-lib-3.0.0.dev9/splight_lib/webhook.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib.egg-info/PKG-INFO` & `splight-lib-3.0.0.dev9/splight_lib.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 3.0.0.dev8
+Version: 3.0.0.dev9
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-3.0.0.dev8/splight_lib.egg-info/SOURCES.txt` & `splight-lib-3.0.0.dev9/splight_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.0.dev8/splight_lib.egg-info/requires.txt` & `splight-lib-3.0.0.dev9/splight_lib.egg-info/requires.txt`

 * *Files identical despite different names*

