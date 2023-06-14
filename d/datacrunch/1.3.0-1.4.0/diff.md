# Comparing `tmp/datacrunch-1.3.0.tar.gz` & `tmp/datacrunch-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datacrunch-1.3.0.tar", last modified: Thu May 25 13:47:42 2023, max compression
+gzip compressed data, was "datacrunch-1.4.0.tar", last modified: Wed Jun 14 14:08:27 2023, max compression
```

## Comparing `datacrunch-1.3.0.tar` & `datacrunch-1.4.0.tar`

### file list

```diff
@@ -1,86 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.132008 datacrunch-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-25 13:47:28.000000 datacrunch-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-05-25 13:47:42.132008 datacrunch-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-25 13:47:28.000000 datacrunch-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.124008 datacrunch-1.3.0/datacrunch/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.124008 datacrunch-1.3.0/datacrunch/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/authentication/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.124008 datacrunch-1.3.0/datacrunch/balance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/balance/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.124008 datacrunch-1.3.0/datacrunch/http_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/http_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/http_client/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/datacrunch/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/images/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/datacrunch/instance_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/instance_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/instance_types/instance_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/datacrunch/instances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/instances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/instances/instances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/datacrunch/ssh_keys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/ssh_keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/ssh_keys/ssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/datacrunch/startup_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/startup_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/startup_scripts/startup_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/datacrunch/volume_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/volume_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/volume_types/volume_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/datacrunch/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-05-25 13:47:28.000000 datacrunch-1.3.0/datacrunch/volumes/volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.124008 datacrunch-1.3.0/datacrunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-05-25 13:47:42.000000 datacrunch-1.3.0/datacrunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-25 13:47:42.000000 datacrunch-1.3.0/datacrunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:47:42.000000 datacrunch-1.3.0/datacrunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 13:47:42.000000 datacrunch-1.3.0/datacrunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 13:47:42.000000 datacrunch-1.3.0/datacrunch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:47:42.132008 datacrunch-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-25 13:47:28.000000 datacrunch-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/tests/unit_tests/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/authentication/test_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/tests/unit_tests/balance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/balance/test_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/tests/unit_tests/http_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/http_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/http_client/test_http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.128008 datacrunch-1.3.0/tests/unit_tests/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/images/test_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.132008 datacrunch-1.3.0/tests/unit_tests/instance_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/instance_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/instance_types/test_instance_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.132008 datacrunch-1.3.0/tests/unit_tests/instances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/instances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/instances/test_instances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.132008 datacrunch-1.3.0/tests/unit_tests/ssh_keys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/ssh_keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/ssh_keys/test_ssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.132008 datacrunch-1.3.0/tests/unit_tests/startup_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/startup_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/startup_scripts/test_startup_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/test_datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/test_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.132008 datacrunch-1.3.0/tests/unit_tests/volume_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/volume_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/volume_types/test_volume_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:42.132008 datacrunch-1.3.0/tests/unit_tests/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20505 2023-05-25 13:47:28.000000 datacrunch-1.3.0/tests/unit_tests/volumes/test_volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.131384 datacrunch-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-14 14:08:17.000000 datacrunch-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-14 14:08:27.131384 datacrunch-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-14 14:08:17.000000 datacrunch-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.123384 datacrunch-1.4.0/datacrunch/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.123384 datacrunch-1.4.0/datacrunch/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/authentication/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.123384 datacrunch-1.4.0/datacrunch/balance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/balance/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.123384 datacrunch-1.4.0/datacrunch/http_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/http_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/http_client/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.123384 datacrunch-1.4.0/datacrunch/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/images/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.123384 datacrunch-1.4.0/datacrunch/instance_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/instance_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/instance_types/instance_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/datacrunch/instances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/instances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/instances/instances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/datacrunch/ssh_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/ssh_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/ssh_keys/ssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/datacrunch/startup_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/startup_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/startup_scripts/startup_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/datacrunch/volume_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/volume_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/volume_types/volume_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/datacrunch/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/volumes/volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.123384 datacrunch-1.4.0/datacrunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-14 14:08:27.000000 datacrunch-1.4.0/datacrunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-14 14:08:27.000000 datacrunch-1.4.0/datacrunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:08:27.000000 datacrunch-1.4.0/datacrunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-14 14:08:27.000000 datacrunch-1.4.0/datacrunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 14:08:27.000000 datacrunch-1.4.0/datacrunch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 14:08:27.131384 datacrunch-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-14 14:08:17.000000 datacrunch-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/integration_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/integration_tests/test_volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/authentication/test_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/balance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/balance/test_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/http_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/http_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/http_client/test_http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/images/test_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/instance_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/instance_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/instance_types/test_instance_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/instances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/instances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/instances/test_instances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/ssh_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/ssh_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/ssh_keys/test_ssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/startup_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/startup_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/startup_scripts/test_startup_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/test_datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/test_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.131384 datacrunch-1.4.0/tests/unit_tests/volume_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/volume_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/volume_types/test_volume_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.131384 datacrunch-1.4.0/tests/unit_tests/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20591 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/volumes/test_volumes.py
```

### Comparing `datacrunch-1.3.0/LICENSE` & `datacrunch-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/PKG-INFO` & `datacrunch-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacrunch
-Version: 1.3.0
+Version: 1.4.0
 Summary: Official Python SDK for DataCrunch Public API
 Home-page: https://github.com/DataCrunch-io
 Author: DataCrunch Oy
 Author-email: info@datacrunch.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datacrunch Version: 1.3.0 Summary: Official Python
+Metadata-Version: 2.1 Name: datacrunch Version: 1.4.0 Summary: Official Python
 SDK for DataCrunch Public API Home-page: https://github.com/DataCrunch-io
 Author: DataCrunch Oy Author-email: info@datacrunch.io Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Development Status :: 5 - Production/
```

### Comparing `datacrunch-1.3.0/README.md` & `datacrunch-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/datacrunch/authentication/authentication.py` & `datacrunch-1.4.0/datacrunch/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/datacrunch/balance/balance.py` & `datacrunch-1.4.0/datacrunch/balance/balance.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/datacrunch/constants.py` & `datacrunch-1.4.0/datacrunch/constants.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/datacrunch/datacrunch.py` & `datacrunch-1.4.0/datacrunch/datacrunch.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/datacrunch/exceptions.py` & `datacrunch-1.4.0/datacrunch/exceptions.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/datacrunch/helpers.py` & `datacrunch-1.4.0/datacrunch/helpers.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/datacrunch/http_client/http_client.py` & `datacrunch-1.4.0/datacrunch/http_client/http_client.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/datacrunch/images/images.py` & `datacrunch-1.4.0/datacrunch/images/images.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/datacrunch/instance_types/instance_types.py` & `datacrunch-1.4.0/datacrunch/instance_types/instance_types.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/datacrunch/instances/instances.py` & `datacrunch-1.4.0/datacrunch/instances/instances.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/datacrunch/ssh_keys/ssh_keys.py` & `datacrunch-1.4.0/datacrunch/ssh_keys/ssh_keys.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/datacrunch/startup_scripts/startup_scripts.py` & `datacrunch-1.4.0/datacrunch/startup_scripts/startup_scripts.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/datacrunch/volume_types/volume_types.py` & `datacrunch-1.4.0/datacrunch/volume_types/volume_types.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/datacrunch/volumes/volumes.py` & `datacrunch-1.4.0/datacrunch/volumes/volumes.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
                  type: str,
                  is_os_volume: bool,
                  created_at: str,
                  target: str = None,
                  location: str = "FIN1",
                  instance_id: str = None,
                  ssh_key_ids: List[str] = [],
+                 deleted_at: str = None,
                  ) -> None:
         """Initialize the volume object
 
         :param id: volume id
         :type id: str
         :param status: volume status
         :type status: str
@@ -41,26 +42,29 @@
         :type target: str, optional
         :param location: datacenter location, defaults to "FIN1"
         :type location: str, optional
         :param instance_id: the instance id the volume is attached to, None if detached
         :type instance_id: str
         :param ssh_key_ids: list of ssh keys ids
         :type ssh_key_ids: List[str]
+        :param deleted_at: the time the volume was deleted (UTC), defaults to None
+        :type deleted_at: str, optional
         """
         self._id = id
         self._status = status
         self._name = name
         self._size = size
         self._type = type
         self._is_os_volume = is_os_volume
         self._created_at = created_at
         self._target = target
         self._location = location
         self._instance_id = instance_id
         self._ssh_key_ids = ssh_key_ids
+        self._deleted_at = deleted_at
 
     @property
     def id(self) -> str:
         """Get the volume id
 
         :return: volume id
         :rtype: str
@@ -153,14 +157,34 @@
         """Get the SSH key IDs of the instance
 
         :return: SSH key IDs
         :rtype: List[str]
         """
         return self._ssh_key_ids
 
+    @property
+    def deleted_at(self) -> Optional[str]:
+        """Get the time when the volume was deleted (UTC)
+
+        :return: time
+        :rtype: str
+        """
+        return self._deleted_at
+
+    @classmethod
+    def create_from_dict(cls: 'Volume', volume_dict: dict) -> 'Volume':
+        """Create a Volume object from a dictionary
+
+        :param volume_dict: dictionary representing the volume
+        :type volume_dict: dict
+        :return: Volume
+        :rtype: Volume
+        """
+        return cls(**volume_dict)
+
     def __str__(self) -> str:
         """Returns a string of the json representation of the volume
 
         :return: json representation of the volume
         :rtype: str
         """
         return stringify_class_object_properties(self)
@@ -178,55 +202,40 @@
         :param status: optional, status of the volumes, defaults to None
         :type status: str, optional
         :return: list of volume details objects
         :rtype: List[Volume]
         """
         volumes_dict = self._http_client.get(
             VOLUMES_ENDPOINT, params={'status': status}).json()
-        volumes = list(map(lambda volume_dict: Volume(
-            id=volume_dict['id'],
-            status=volume_dict['status'],
-            name=volume_dict['name'],
-            size=volume_dict['size'],
-            type=volume_dict['type'],
-            is_os_volume=volume_dict['is_os_volume'],
-            created_at=volume_dict['created_at'],
-            target=volume_dict['target'] if 'target' in volume_dict else None,
-            location=volume_dict['location'],
-            instance_id=volume_dict['instance_id'] if 'instance_id' in volume_dict else None,
-            ssh_key_ids=volume_dict['ssh_key_ids'] if 'ssh_key_ids' in volume_dict else [
-            ],
-        ), volumes_dict))
-        return volumes
+        return list(map(Volume.create_from_dict, volumes_dict))
 
     def get_by_id(self, id: str) -> Volume:
         """Get a specific volume by its
 
         :param id: volume id
         :type id: str
         :return: Volume details object
         :rtype: Volume
         """
         volume_dict = self._http_client.get(
             VOLUMES_ENDPOINT + f'/{id}').json()
-        volume = Volume(
-            id=volume_dict['id'],
-            status=volume_dict['status'],
-            name=volume_dict['name'],
-            size=volume_dict['size'],
-            type=volume_dict['type'],
-            is_os_volume=volume_dict['is_os_volume'],
-            created_at=volume_dict['created_at'],
-            target=volume_dict['target'] if 'target' in volume_dict else None,
-            location=volume_dict['location'],
-            instance_id=volume_dict['instance_id'] if 'instance_id' in volume_dict else None,
-            ssh_key_ids=volume_dict['ssh_key_ids'] if 'ssh_key_ids' in volume_dict else [
-            ],
-        )
-        return volume
+
+        return Volume.create_from_dict(volume_dict)
+
+    def get_in_trash(self) -> List[Volume]:
+        """Get all volumes that are in trash
+
+        :return: list of volume details objects
+        :rtype: List[Volume]
+        """
+        volumes_dicts = self._http_client.get(
+            VOLUMES_ENDPOINT + '/trash'
+        ).json()
+
+        return list(map(Volume.create_from_dict, volumes_dicts))
 
     def create(self,
                type: str,
                name: str,
                size: int,
                instance_id: str = None,
                location: str = "FIN1",
@@ -354,21 +363,22 @@
             "action": VolumeActions.INCREASE_SIZE,
             "size": size,
         }
 
         self._http_client.put(VOLUMES_ENDPOINT, json=payload)
         return
 
-    def delete(self, id_list: Union[List[str], str]) -> None:
+    def delete(self, id_list: Union[List[str], str], is_permanent: bool = False) -> None:
         """Delete multiple volumes or single volume
         Note: if attached to any instances, they need to be shut-down (offline)
 
         :param id_list: list of volume ids, or a volume id
         :type id_list: Union[List[str], str]
         """
         payload = {
             "id": id_list,
             "action": VolumeActions.DELETE,
+            "is_permanent": is_permanent
         }
 
         self._http_client.put(VOLUMES_ENDPOINT, json=payload)
         return
```

### Comparing `datacrunch-1.3.0/datacrunch.egg-info/PKG-INFO` & `datacrunch-1.4.0/datacrunch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacrunch
-Version: 1.3.0
+Version: 1.4.0
 Summary: Official Python SDK for DataCrunch Public API
 Home-page: https://github.com/DataCrunch-io
 Author: DataCrunch Oy
 Author-email: info@datacrunch.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datacrunch Version: 1.3.0 Summary: Official Python
+Metadata-Version: 2.1 Name: datacrunch Version: 1.4.0 Summary: Official Python
 SDK for DataCrunch Public API Home-page: https://github.com/DataCrunch-io
 Author: DataCrunch Oy Author-email: info@datacrunch.io Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Development Status :: 5 - Production/
```

### Comparing `datacrunch-1.3.0/datacrunch.egg-info/SOURCES.txt` & `datacrunch-1.4.0/datacrunch.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 datacrunch/startup_scripts/__init__.py
 datacrunch/startup_scripts/startup_scripts.py
 datacrunch/volume_types/__init__.py
 datacrunch/volume_types/volume_types.py
 datacrunch/volumes/__init__.py
 datacrunch/volumes/volumes.py
 tests/__init__.py
+tests/integration_tests/__init__.py
+tests/integration_tests/conftest.py
+tests/integration_tests/test_volumes.py
 tests/unit_tests/__init__.py
 tests/unit_tests/conftest.py
 tests/unit_tests/test_datacrunch.py
 tests/unit_tests/test_exceptions.py
 tests/unit_tests/authentication/__init__.py
 tests/unit_tests/authentication/test_authentication.py
 tests/unit_tests/balance/__init__.py
```

### Comparing `datacrunch-1.3.0/setup.py` & `datacrunch-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/tests/unit_tests/authentication/test_authentication.py` & `datacrunch-1.4.0/tests/unit_tests/authentication/test_authentication.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/tests/unit_tests/balance/test_balance.py` & `datacrunch-1.4.0/tests/unit_tests/balance/test_balance.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/tests/unit_tests/conftest.py` & `datacrunch-1.4.0/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/tests/unit_tests/http_client/test_http_client.py` & `datacrunch-1.4.0/tests/unit_tests/http_client/test_http_client.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/tests/unit_tests/images/test_images.py` & `datacrunch-1.4.0/tests/unit_tests/images/test_images.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/tests/unit_tests/instance_types/test_instance_types.py` & `datacrunch-1.4.0/tests/unit_tests/instance_types/test_instance_types.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/tests/unit_tests/instances/test_instances.py` & `datacrunch-1.4.0/tests/unit_tests/instances/test_instances.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/tests/unit_tests/ssh_keys/test_ssh_keys.py` & `datacrunch-1.4.0/tests/unit_tests/ssh_keys/test_ssh_keys.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/tests/unit_tests/startup_scripts/test_startup_scripts.py` & `datacrunch-1.4.0/tests/unit_tests/startup_scripts/test_startup_scripts.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/tests/unit_tests/test_datacrunch.py` & `datacrunch-1.4.0/tests/unit_tests/test_datacrunch.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/tests/unit_tests/test_exceptions.py` & `datacrunch-1.4.0/tests/unit_tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/tests/unit_tests/volume_types/test_volume_types.py` & `datacrunch-1.4.0/tests/unit_tests/volume_types/test_volume_types.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.3.0/tests/unit_tests/volumes/test_volumes.py` & `datacrunch-1.4.0/tests/unit_tests/volumes/test_volumes.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,15 +463,16 @@
         responses.add(
             responses.PUT,
             endpoint,
             status=202,
             match=[
                 responses.json_params_matcher({
                     "id": NVME_VOL_ID,
-                    "action": VolumeActions.DELETE
+                    "action": VolumeActions.DELETE,
+                    "is_permanent": False
                 })
             ]
         )
 
         # act
         result = volumes_service.delete(NVME_VOL_ID)
 
@@ -485,15 +486,16 @@
             responses.PUT,
             endpoint,
             json={"code": INVALID_REQUEST, "message": INVALID_REQUEST_MESSAGE},
             status=400,
             match=[
                 responses.json_params_matcher({
                     "id": NVME_VOL_ID,
-                    "action": VolumeActions.DELETE
+                    "action": VolumeActions.DELETE,
+                    "is_permanent": False
                 })
             ]
         )
 
         # act
         with pytest.raises(APIException) as excinfo:
             volumes_service.delete(NVME_VOL_ID)
```

