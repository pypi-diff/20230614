# Comparing `tmp/rapyuta-io-cli-3.0.0.tar.gz` & `tmp/rapyuta-io-cli-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapyuta-io-cli-3.0.0.tar", last modified: Wed May 17 13:12:46 2023, max compression
+gzip compressed data, was "rapyuta-io-cli-3.1.0.tar", last modified: Wed Jun 14 14:34:11 2023, max compression
```

## Comparing `rapyuta-io-cli-3.0.0.tar` & `rapyuta-io-cli-3.1.0.tar`

### file list

```diff
@@ -1,212 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.554149 rapyuta-io-cli-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-05-17 13:12:46.554149 rapyuta-io-cli-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.538149 rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-05-17 13:12:46.000000 rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4616 2023-05-17 13:12:46.000000 rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 13:12:46.000000 rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-17 13:12:46.000000 rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-05-17 13:12:46.000000 rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-17 13:12:46.000000 rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.538149 rapyuta-io-cli-3.0.0/riocli/
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.538149 rapyuta-io-cli-3.0.0/riocli/apply/
--rw-r--r--   0 runner    (1001) docker     (122)     3908 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1465 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/apply/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)    15241 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/apply/parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     8273 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/apply/resolver.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/apply/template.py
--rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/apply/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.538149 rapyuta-io-cli-3.0.0/riocli/auth/
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4016 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/auth/login.py
--rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/auth/logout.py
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/auth/refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (122)     2663 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/auth/staging.py
--rw-r--r--   0 runner    (1001) docker     (122)      911 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/auth/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/auth/token.py
--rw-r--r--   0 runner    (1001) docker     (122)     3799 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/auth/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.538149 rapyuta-io-cli-3.0.0/riocli/build/
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/import_build.py
--rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/trigger.py
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.542149 rapyuta-io-cli-3.0.0/riocli/chart/
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/chart/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     3182 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/chart/chart.py
--rw-r--r--   0 runner    (1001) docker     (122)     2138 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/chart/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/chart/info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/chart/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1208 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/chart/search.py
--rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/chart/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.542149 rapyuta-io-cli-3.0.0/riocli/completion/
--rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/completion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.542149 rapyuta-io-cli-3.0.0/riocli/config/
--rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.542149 rapyuta-io-cli-3.0.0/riocli/deployment/
--rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1513 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)    10299 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2861 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)    16564 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/model.py
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     2495 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     5648 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.542149 rapyuta-io-cli-3.0.0/riocli/device/
--rw-r--r--   0 runner    (1001) docker     (122)     1975 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4447 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/deployment.py
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/execute.py
--rw-r--r--   0 runner    (1001) docker     (122)     6340 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/files.py
--rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     4083 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/label.py
--rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3301 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/metric.py
--rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/onboard.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/device/tools/
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/tools/device_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/tools/forward.py
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/tools/rapyuta_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/tools/scp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/tools/service.py
--rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/tools/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/topic.py
--rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/disk/
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/disk/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/disk/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/disk/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/disk/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/disk/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/jsonschema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/jsonschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/jsonschema/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/managedservice/
--rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/managedservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/managedservice/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/managedservice/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1325 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/managedservice/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1273 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/managedservice/list_providers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/managedservice/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/model/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5730 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/network/
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4206 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/native_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/routed_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     6168 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/organization/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/organization/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1594 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/organization/select.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/package/
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/package/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/package/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/package/deployment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/package/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/package/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     9344 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/package/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/package/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.550149 rapyuta-io-cli-3.0.0/riocli/parameter/
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2982 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/parameter/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/parameter/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/parameter/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/parameter/download.py
--rw-r--r--   0 runner    (1001) docker     (122)     1187 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/parameter/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/parameter/upload.py
--rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/parameter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.550149 rapyuta-io-cli-3.0.0/riocli/project/
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/delete.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.550149 rapyuta-io-cli-3.0.0/riocli/project/features/
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/features/vpn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2642 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     4111 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.550149 rapyuta-io-cli-3.0.0/riocli/rosbag/
--rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/rosbag/blob.py
--rw-r--r--   0 runner    (1001) docker     (122)    11554 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/rosbag/job.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/rosbag/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.550149 rapyuta-io-cli-3.0.0/riocli/secret/
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/docker_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     3442 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/import_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1965 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/source_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.550149 rapyuta-io-cli-3.0.0/riocli/shell/
--rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/shell/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.554149 rapyuta-io-cli-3.0.0/riocli/static_route/
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/static_route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/static_route/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/static_route/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/static_route/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/static_route/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1849 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/static_route/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/static_route/open.py
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/static_route/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.554149 rapyuta-io-cli-3.0.0/riocli/usergroup/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/usergroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/usergroup/list.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.554149 rapyuta-io-cli-3.0.0/riocli/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (122)     2386 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/utils/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/utils/selector.py
--rw-r--r--   0 runner    (1001) docker     (122)     1602 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/utils/spinner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/utils/ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.554149 rapyuta-io-cli-3.0.0/riocli/v2client/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/v2client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11183 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/v2client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.554149 rapyuta-io-cli-3.0.0/riocli/vpn/
--rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/vpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4909 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/vpn/connect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/vpn/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/vpn/ping.py
--rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/vpn/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     3224 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/vpn/util.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 13:12:46.554149 rapyuta-io-cli-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1692 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.461439 rapyuta-io-cli-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.445438 rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-06-14 14:34:11.000000 rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4645 2023-06-14 14:34:11.000000 rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 14:34:11.000000 rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-14 14:34:11.000000 rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-14 14:34:11.000000 rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-14 14:34:11.000000 rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.445438 rapyuta-io-cli-3.1.0/riocli/
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.445438 rapyuta-io-cli-3.1.0/riocli/apply/
+-rw-r--r--   0 runner    (1001) docker     (122)     4468 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1465 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/apply/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15434 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/apply/parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8273 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/apply/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/apply/template.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/apply/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.445438 rapyuta-io-cli-3.1.0/riocli/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4480 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/auth/login.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/auth/logout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/auth/refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2663 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/auth/staging.py
+-rw-r--r--   0 runner    (1001) docker     (122)      911 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/auth/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/auth/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4735 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/auth/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.449439 rapyuta-io-cli-3.1.0/riocli/build/
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3526 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3661 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/import_build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/build/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.449439 rapyuta-io-cli-3.1.0/riocli/chart/
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/chart/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3182 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/chart/chart.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2138 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/chart/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/chart/info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/chart/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1208 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/chart/search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/chart/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.449439 rapyuta-io-cli-3.1.0/riocli/completion/
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/completion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.449439 rapyuta-io-cli-3.1.0/riocli/config/
+-rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.449439 rapyuta-io-cli-3.1.0/riocli/deployment/
+-rw-r--r--   0 runner    (1001) docker     (122)     1638 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1513 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10299 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2861 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16564 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2495 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5648 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/deployment/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.449439 rapyuta-io-cli-3.1.0/riocli/device/
+-rw-r--r--   0 runner    (1001) docker     (122)     1975 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4447 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2837 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6340 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4083 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/label.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3301 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/metric.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/onboard.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.449439 rapyuta-io-cli-3.1.0/riocli/device/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/tools/device_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/tools/forward.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/tools/rapyuta_logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/tools/scp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/tools/service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/tools/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/topic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/device/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/disk/
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/disk/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/disk/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/disk/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/disk/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/disk/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/jsonschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/jsonschema/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/managedservice/
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/managedservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/managedservice/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/managedservice/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1325 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/managedservice/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1273 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/managedservice/list_providers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/managedservice/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/model/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5730 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/network/
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4206 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/native_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/routed_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6168 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/network/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/organization/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/organization/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1594 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/organization/select.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/package/
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1485 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/package/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/package/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/package/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/package/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/package/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9492 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/package/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/package/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.453439 rapyuta-io-cli-3.1.0/riocli/parameter/
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2982 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/parameter/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/parameter/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/parameter/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/parameter/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1187 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/parameter/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/parameter/upload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/parameter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/project/
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/delete.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/project/features/
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/features/vpn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2642 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4111 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/project/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/rosbag/blob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11554 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/rosbag/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/rosbag/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/secret/
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2449 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/docker_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3459 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/import_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1965 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/source_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/secret/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/shell/
+-rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/shell/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/static_route/
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/static_route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/static_route/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/static_route/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/static_route/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/static_route/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1849 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/static_route/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/static_route/open.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/static_route/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/usergroup/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/usergroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/usergroup/list.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2364 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/utils/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/utils/selector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1602 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/utils/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/utils/ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/v2client/
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/v2client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11183 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/v2client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:34:11.457439 rapyuta-io-cli-3.1.0/riocli/vpn/
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/vpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4909 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/vpn/connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/vpn/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/vpn/ping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/vpn/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3224 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/riocli/vpn/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-14 14:34:11.461439 rapyuta-io-cli-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1693 2023-06-14 14:34:00.000000 rapyuta-io-cli-3.1.0/setup.py
```

### Comparing `rapyuta-io-cli-3.0.0/PKG-INFO` & `rapyuta-io-cli-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapyuta-io-cli
-Version: 3.0.0
+Version: 3.1.0
 Summary: Rapyuta.io CLI Python command line application.
 Home-page: http://docs.rapyuta.io
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
 License: UNKNOWN
 Description: # Rapyuta CLI
```

### Comparing `rapyuta-io-cli-3.0.0/README.md` & `rapyuta-io-cli-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/PKG-INFO` & `rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapyuta-io-cli
-Version: 3.0.0
+Version: 3.1.0
 Summary: Rapyuta.io CLI Python command line application.
 Home-page: http://docs.rapyuta.io
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
 License: UNKNOWN
 Description: # Rapyuta CLI
```

### Comparing `rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/SOURCES.txt` & `rapyuta-io-cli-3.1.0/rapyuta_io_cli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 riocli/chart/util.py
 riocli/completion/__init__.py
 riocli/config/__init__.py
 riocli/config/config.py
 riocli/deployment/__init__.py
 riocli/deployment/delete.py
 riocli/deployment/errors.py
+riocli/deployment/execute.py
 riocli/deployment/inspect.py
 riocli/deployment/list.py
 riocli/deployment/logs.py
 riocli/deployment/model.py
 riocli/deployment/run.py
 riocli/deployment/ssh.py
 riocli/deployment/status.py
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/__main__.py` & `rapyuta-io-cli-3.1.0/riocli/__main__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/apply/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/apply/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,26 +25,42 @@
 
 @click.command(
     'apply',
     cls=HelpColorsCommand,
     help_headers_color='yellow',
     help_options_color='green',
 )
-@click.option('--dryrun', '-d', is_flag=True, default=False, help='dry run the yaml files without applying any change')
+@click.option('--dryrun', '-d', is_flag=True, default=False,
+              help='dry run the yaml files without applying any change')
+@click.option('--show-graph', '-g', is_flag=True, default=False,
+              help='Opens a mermaid.live dependency graph')
 @click.option('--values', '-v',
-              help="path to values yaml file. key/values specified in the values file can be used as variables in template yamls")
+              help="path to values yaml file. key/values "
+                   "specified in the values file can be "
+                   "used as variables in template YAMLs")
 @click.option('--secrets', '-s',
-              help="secret files are sops encoded value files. rio-cli expects sops to be authorized for decoding files on this computer")
-@click.option('--workers', '-w', help="number of parallel workers while running apply command. defaults to 6.",
-              type=int)
-@click.option('-f', '--force', '--silent', 'silent', is_flag=True, type=click.BOOL, default=False,
+              help="secret files are sops encoded value files. "
+                   "rio-cli expects sops to be authorized for "
+                   "decoding files on this computer")
+@click.option('--workers', '-w',
+              help="number of parallel workers while running apply "
+                   "command. defaults to 6.", type=int)
+@click.option('-f', '--force', '--silent', 'silent', is_flag=True,
+              type=click.BOOL, default=False,
               help="Skip confirmation")
 @click.argument('files', nargs=-1)
-def apply(values: str, secrets: str, files: Iterable[str], dryrun: bool = False, workers: int = 6,
-          silent: bool = False) -> None:
+def apply(
+        values: str,
+        secrets: str,
+        files: Iterable[str],
+        dryrun: bool = False,
+        workers: int = 6,
+        silent: bool = False,
+        show_graph: bool = False,
+) -> None:
     """
     Apply resource manifests
     """
     glob_files, abs_values, abs_secrets = process_files_values_secrets(
         files, values, secrets)
 
     if len(glob_files) == 0:
@@ -54,14 +70,23 @@
     click.secho("----- Files Processed ----", fg="yellow")
     for file in glob_files:
         click.secho(file, fg="yellow")
 
     rc = Applier(glob_files, abs_values, abs_secrets)
     rc.parse_dependencies()
 
+    if show_graph and dryrun:
+        click.secho('You cannot dry run and launch the graph together.',
+                    fg='yellow')
+        return
+
+    if show_graph:
+        rc.show_dependency_graph()
+        return
+
     if not silent and not dryrun:
         click.confirm("Do you want to proceed?", default=True, abort=True)
 
     rc.apply(dryrun=dryrun, workers=workers)
 
 
 @click.command(
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/apply/explain.py` & `rapyuta-io-cli-3.1.0/riocli/apply/explain.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/apply/parse.py` & `rapyuta-io-cli-3.1.0/riocli/apply/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 import json
-import os
 import queue
 import threading
 import typing
 from graphlib import TopologicalSorter
 
 import click
 import jinja2
@@ -134,22 +133,28 @@
                     self._apply_manifest(obj, *args, **kwargs)
                 self.graph.done(obj)
 
     def delete(self, *args, **kwargs):
         delete_order = list(self.graph.static_order())
         delete_order.reverse()
         for obj in delete_order:
-            if obj in self.resolved_objects and 'manifest' in self.resolved_objects[obj]:
+            if obj in self.resolved_objects and 'manifest' in \
+                    self.resolved_objects[obj]:
                 self._delete_manifest(obj, *args, **kwargs)
 
     def print_resolved_manifests(self):
         manifests = [o for _, o in self.objects.items()]
         dump_all_yaml(manifests)
 
-    def parse_dependencies(self, check_missing=True, delete=False, template=False):
+    def parse_dependencies(
+            self,
+            check_missing=True,
+            delete=False,
+            template=False,
+    ):
         number_of_objects = 0
         for f, data in self.files.items():
             for model in data:
                 key = self._get_object_key(model)
                 self._parse_dependency(key, model)
                 self._add_graph_node(key)
                 number_of_objects = number_of_objects + 1
@@ -166,15 +171,18 @@
             expected_time = round(
                 self.EXPECTED_TIME.get(kind.lower(), 5) / 60, 2)
             total_time = total_time + expected_time
             resource_list.append([node, action, expected_time])
 
         if not template:
             self._display_context(
-                total_time=total_time, total_objects=number_of_objects, resource_list=resource_list)
+                total_time=total_time,
+                total_objects=number_of_objects,
+                resource_list=resource_list,
+            )
 
         if check_missing:
             missing_resources = []
             for key, item in self.resolved_objects.items():
                 if 'src' in item and item['src'] == 'missing':
                     missing_resources.append(key)
 
@@ -361,22 +369,27 @@
         if kind.lower() == "deployment":
             dependency['guid'] = obj['deploymentId']
 
     def _initialize_kind_dependency(self, kind):
         if not self.dependencies.get(kind):
             self.dependencies[kind] = {}
 
+    def show_dependency_graph(self):
+        """Lauches mermaid.live dependency graph"""
+        link = mermaid_link("\n".join(self.diagram))
+        click.launch(link)
+
     # Utils
-    def _display_context(self, total_time: int, total_objects: int, resource_list: typing.List) -> None:
+    def _display_context(
+            self,
+            total_time: int,
+            total_objects: int,
+            resource_list: typing.List
+    ) -> None:
         # Display context
-
-        if os.environ.get('MERMAID'):
-            diagram_link = mermaid_link("\n".join(self.diagram))
-            click.launch(diagram_link)
-
         headers = [click.style('Resource Context', bold=True, fg='yellow')]
         context = [
             ['Expected Time (mins)', round(total_time, 2)],
             ['Files', len(self.files)],
             ['Resources', total_objects],
         ]
         click.echo(tabulate(context, headers=headers,
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/apply/resolver.py` & `rapyuta-io-cli-3.1.0/riocli/apply/resolver.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/apply/template.py` & `rapyuta-io-cli-3.1.0/riocli/apply/template.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/apply/util.py` & `rapyuta-io-cli-3.1.0/riocli/apply/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/auth/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/auth/login.py` & `rapyuta-io-cli-3.1.0/riocli/auth/login.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 from click_help_colors import HelpColorsCommand
 
-from riocli.auth.util import get_token, select_organization, select_project
+from riocli.auth.util import (
+    get_token,
+    select_organization,
+    select_project,
+    validate_token,
+)
 from riocli.utils.context import get_root_context
 
 LOGIN_SUCCESS = click.style('Logged in successfully!', fg='green')
 
 
 @click.command(
     cls=HelpColorsCommand,
@@ -33,43 +38,55 @@
               help=('Context will be set to the organization after '
                     'authentication'))
 @click.option('--project', type=str, default=None,
               help='Context will be set to the project after authentication')
 @click.option('--interactive/--no-interactive', '--interactive/--silent',
               is_flag=True, type=bool, default=True,
               help='Make login interactive')
+@click.option('--auth-token', type=str, default=None,
+              help="Login with auth token only")
 @click.pass_context
 def login(
         ctx: click.Context,
         email: str,
         password: str,
         organization: str,
         project: str,
-        interactive: bool
+        interactive: bool,
+        auth_token: str,
 ) -> None:
     """
-    Log into the Rapyuta.io account using the CLI. This is required
-    to use most of the functionalities of the CLI.
+    Log into your rapyuta.io account using the CLI. This is required to
+    use most commands of the CLI.
+    
+    You can log in with your email and password or just with and auth token
+    if you already have one.
     """
-    if interactive:
-        email = email or click.prompt('Email')
-        password = password or click.prompt('Password', hide_input=True)
-
-    if not email:
-        click.secho('email not specified')
-        raise SystemExit(1)
-
-    if not password:
-        click.secho('password not specified')
-        raise SystemExit(1)
-
     ctx = get_root_context(ctx)
-    ctx.obj.data['email_id'] = email
-    ctx.obj.data['password'] = password
-    ctx.obj.data['auth_token'] = get_token(email, password)
+
+    if auth_token:
+        if not validate_token(auth_token):
+            raise SystemExit(1)
+        ctx.obj.data['auth_token'] = auth_token
+    else:
+        if interactive:
+            email = email or click.prompt('Email')
+            password = password or click.prompt('Password', hide_input=True)
+
+        if not email:
+            click.secho('email not specified')
+            raise SystemExit(1)
+
+        if not password:
+            click.secho('password not specified')
+            raise SystemExit(1)
+
+        ctx.obj.data['email_id'] = email
+        ctx.obj.data['password'] = password
+        ctx.obj.data['auth_token'] = get_token(email, password)
 
     # Save if the file does not already exist
     if not ctx.obj.exists or not interactive:
         ctx.obj.save()
     else:
         click.secho("[Warning] rio already has a config file present",
                     fg='yellow')
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/auth/logout.py` & `rapyuta-io-cli-3.1.0/riocli/auth/logout.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/auth/refresh_token.py` & `rapyuta-io-cli-3.1.0/riocli/auth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/auth/staging.py` & `rapyuta-io-cli-3.1.0/riocli/auth/staging.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/auth/status.py` & `rapyuta-io-cli-3.1.0/riocli/auth/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/auth/token.py` & `rapyuta-io-cli-3.1.0/riocli/package/create.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,32 +7,39 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import json
+
 import click
+import yaml
+from click_spinner import spinner
 
-from riocli.auth.util import get_token
-from riocli.config import Configuration
-from riocli.exceptions import LoggedOut
+from riocli.config import new_client
 
 
-@click.command()
-@click.option("--email", default=None, help="Email of the Rapyuta.io account")
-@click.option("--password", default=None, hide_input=True, help="Password for the Rapyuta.io account")
-def token(email: str, password: str):
+@click.command('create', hidden=True)
+@click.option('--manifest', type=click.File(mode='r', lazy=True),
+              help='Path for the manifest file')
+@click.option('--format', 'format_type', default='json',
+              type=click.Choice(['json', 'yaml'], case_sensitive=False))
+def create_package(manifest: click.File, format_type: str) -> None:
     """
-    Generates a fresh Rapyuta.io token
+    Create a new package
     """
+    data = manifest.read()
+    if format_type == 'json':
+        package = json.loads(data)
+    else:
+        package = yaml.load(data)
 
-    config = Configuration()
-    if not email:
-        email = config.data.get("email_id", None)
-    if not password:
-        password = config.data.get("password", None)
-    if not config.exists or not email or not password:
-        raise LoggedOut
-
-    token = get_token(email, password)
-    click.echo(token)
+    try:
+        client = new_client()
+        with spinner():
+            client.create_package(package)
+        click.secho('Package created successfully!', fg='green')
+    except Exception as e:
+        click.secho(str(e), fg='red')
+        raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/auth/util.py` & `rapyuta-io-cli-3.1.0/riocli/auth/util.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 import click
 from click_spinner import spinner
 from rapyuta_io import Client
+from rapyuta_io.clients.rip_client import AuthTokenLevel
 from rapyuta_io.utils import UnauthorizedError
 
 from riocli.config import Configuration
 from riocli.project.util import find_project_guid, find_organization_guid
 from riocli.utils.selector import show_selection
 
 
-def select_organization(config: Configuration, organization: str = None) -> str:
+def select_organization(config: Configuration,
+                        organization: str = None) -> str:
     client = config.new_client(with_project=False)
 
     org_guid = None
 
     if organization:
         org_guid = organization if organization.startswith(
             'org-') else find_organization_guid(client, name=organization)
@@ -47,64 +49,97 @@
 
     config.data['organization_id'] = org_guid
     config.data['organization_name'] = org_map[org_guid]
 
     return org_guid
 
 
-def select_project(config: Configuration, project: str = None, organization: str = None) -> None:
+def select_project(config: Configuration, project: str = None,
+                   organization: str = None) -> None:
     """
     Launches the project selection prompt by listing all the projects.
     Sets the choice in the given configuration.
     """
     client = config.new_v2_client(with_project=False)
 
     project_guid = None
     if project:
         project_guid = (project if project.startswith('project-') else
-                        find_project_guid(client, project, organization=organization))
+                        find_project_guid(client, project,
+                                          organization=organization))
 
     projects = client.list_projects(organization_guid=organization)
     if len(projects) == 0:
         config.data['project_id'] = ""
         config.data['project_name'] = ""
-        click.secho("There are no projects in this organization", fg='black', bg='white')
+        click.secho("There are no projects in this organization", fg='black',
+                    bg='white')
         return
 
     # Sort projects based on their names for an easier selection
     projects = sorted(projects, key=lambda p: p.metadata.name.lower())
     project_map = dict()
 
     for project in projects:
         project_map[project.metadata.guid] = project.metadata.name
 
     if not project_guid:
-        project_guid = show_selection(project_map, header='Select the project to activate')
+        project_guid = show_selection(
+            project_map, header='Select the project to activate')
 
     config.data['project_id'] = project_guid
     config.data['project_name'] = project_map[project_guid]
 
     confirmation = "Your project has been set to '{}' in the organization '{}'".format(
         config.data['project_name'], config.data['organization_name'],
     )
 
     click.secho(confirmation, fg='green')
 
 
-def get_token(email: str, password: str) -> str:
+TOKEN_LEVELS = {
+    0: AuthTokenLevel.LOW,
+    1: AuthTokenLevel.MED,
+    2: AuthTokenLevel.HIGH
+}
+
+
+def get_token(email: str, password: str, level: int = 1) -> str:
     """
     Generates a new token using email and password.
     """
     config = Configuration()
     if 'environment' in config.data:
         os.environ['RIO_CONFIG'] = config.filepath
 
     try:
         with spinner():
-            token = Client.get_auth_token(email, password)
+            token = Client.get_auth_token(
+                email, password, TOKEN_LEVELS[level])
         return token
     except UnauthorizedError:
-        click.secho("incorrect email/password", fg='red')
+        click.secho("✘ incorrect email/password", fg='red')
         raise SystemExit(1)
     except Exception as e:
         click.secho(e, fg='red')
         raise SystemExit(1)
+
+
+def validate_token(token: str) -> bool:
+    """Validates an auth token."""
+    config = Configuration()
+    if 'environment' in config.data:
+        os.environ['RIO_CONFIG'] = config.filepath
+
+    client = Client(auth_token=token)
+
+    try:
+        user = client.get_authenticated_user()
+        click.secho('Token belongs to user {}'.format(user.email_id),
+                    fg='cyan')
+        return True
+    except UnauthorizedError:
+        click.secho("✘ incorrect auth token", fg='red')
+        return False
+    except Exception as e:
+        click.secho(e, fg='red')
+        return False
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/bootstrap.py` & `rapyuta-io-cli-3.1.0/riocli/bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "3.0.0"
+__version__ = "3.1.0"
 
 import click
 import rapyuta_io.version
 from click import Context
 from click_help_colors import HelpColorsGroup
 from click_plugins import with_plugins
 from pkg_resources import iter_entry_points
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/build/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/build/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/build/create.py` & `rapyuta-io-cli-3.1.0/riocli/build/create.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import click
 from click_spinner import spinner
 from rapyuta_io import Build, SimulationOptions
 
 from riocli.config import new_client
 
 
-@click.command('create')
+@click.command('create', hidden=True)
 @click.option('--strategy', type=click.Choice(['Source', 'Docker']), default='Docker',
               help='Strategy for building the Source')
 @click.option('--branch', default='', help='Git Repository branch')
 @click.option('--context', help='Context directory relative to the Git Repository root', default='')
 @click.option('--arch', help='Architecture for the Build',
               type=click.Choice(['amd64', 'arm32v7', 'arm64v8']), default='amd64')
 @click.option('--ros/--no-ros', is_flag=True, help='Flag to enable ROS support', default=False)
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/build/delete.py` & `rapyuta-io-cli-3.1.0/riocli/build/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/build/import_build.py` & `rapyuta-io-cli-3.1.0/riocli/build/import_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from riocli.config import new_client
 from riocli.utils import run_bash
 from riocli.utils.selector import show_selection
 
 
 @click.group(
     'import',
+    hidden=True,
     invoke_without_command=False,
     cls=HelpColorsGroup,
     help_headers_color='yellow',
     help_options_color='green',
 )
 def import_build():
     """
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/build/inspect.py` & `rapyuta-io-cli-3.1.0/riocli/build/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/build/list.py` & `rapyuta-io-cli-3.1.0/riocli/build/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/build/logs.py` & `rapyuta-io-cli-3.1.0/riocli/build/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/build/model.py` & `rapyuta-io-cli-3.1.0/riocli/build/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/build/trigger.py` & `rapyuta-io-cli-3.1.0/riocli/build/trigger.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/build/util.py` & `rapyuta-io-cli-3.1.0/riocli/build/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/chart/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/chart/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/chart/apply.py` & `rapyuta-io-cli-3.1.0/riocli/chart/apply.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/chart/chart.py` & `rapyuta-io-cli-3.1.0/riocli/chart/chart.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/chart/delete.py` & `rapyuta-io-cli-3.1.0/riocli/chart/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/chart/info.py` & `rapyuta-io-cli-3.1.0/riocli/chart/info.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/chart/list.py` & `rapyuta-io-cli-3.1.0/riocli/chart/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/chart/search.py` & `rapyuta-io-cli-3.1.0/riocli/chart/search.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/chart/util.py` & `rapyuta-io-cli-3.1.0/riocli/chart/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/completion/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/completion/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/config/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/config/config.py` & `rapyuta-io-cli-3.1.0/riocli/config/config.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/deployment/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/deployment/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from riocli.deployment.delete import delete_deployment
 from riocli.deployment.inspect import inspect_deployment
 from riocli.deployment.list import list_deployments
 from riocli.deployment.logs import deployment_logs
 from riocli.deployment.ssh import ssh_init, ssh_deployment
 from riocli.deployment.status import status
 from riocli.deployment.wait import wait_for_deployment
+from riocli.deployment.execute import execute_command
 
 
 @click.group(
     invoke_without_command=False,
     cls=HelpColorsGroup,
     help_headers_color='yellow',
     help_options_color='green',
@@ -40,7 +41,8 @@
 deployment.add_command(inspect_deployment)
 deployment.add_command(list_deployments)
 deployment.add_command(deployment_logs)
 deployment.add_command(wait_for_deployment)
 deployment.add_command(status)
 deployment.add_command(ssh_deployment)
 deployment.add_command(ssh_init)
+deployment.add_command(execute_command)
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/deployment/delete.py` & `rapyuta-io-cli-3.1.0/riocli/deployment/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/deployment/errors.py` & `rapyuta-io-cli-3.1.0/riocli/deployment/errors.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/deployment/inspect.py` & `rapyuta-io-cli-3.1.0/riocli/deployment/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/deployment/list.py` & `rapyuta-io-cli-3.1.0/riocli/deployment/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/deployment/logs.py` & `rapyuta-io-cli-3.1.0/riocli/deployment/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/deployment/model.py` & `rapyuta-io-cli-3.1.0/riocli/deployment/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/deployment/run.py` & `rapyuta-io-cli-3.1.0/riocli/deployment/run.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/deployment/ssh.py` & `rapyuta-io-cli-3.1.0/riocli/deployment/ssh.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/deployment/status.py` & `rapyuta-io-cli-3.1.0/riocli/deployment/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/deployment/util.py` & `rapyuta-io-cli-3.1.0/riocli/deployment/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/deployment/wait.py` & `rapyuta-io-cli-3.1.0/riocli/deployment/wait.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/device/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/config.py` & `rapyuta-io-cli-3.1.0/riocli/device/config.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/create.py` & `rapyuta-io-cli-3.1.0/riocli/device/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from click_spinner import spinner
 from rapyuta_io import ROSDistro
 from rapyuta_io.clients.device import DevicePythonVersion, Device, DeviceRuntime
 
 from riocli.config import new_client
 
 
-@click.command('create')
+@click.command('create', hidden=True)
 @click.option('--description', type=str, help='Description of the device', default='')
 @click.option('--runtime', help='Runtime of the Device', multiple=True,
               type=click.Choice(['preinstalled', 'dockercompose'], case_sensitive=False))
 @click.option('--ros', help='ROS Distribution for the Device', default='melodic',
               type=click.Choice(['kinetic', 'melodic', 'noetic'], case_sensitive=False))
 @click.option('--python', help='Python Version to use on the Device', default='3',
               type=click.Choice(['2', '3'], case_sensitive=False))
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/delete.py` & `rapyuta-io-cli-3.1.0/riocli/device/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/deployment.py` & `rapyuta-io-cli-3.1.0/riocli/device/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/execute.py` & `rapyuta-io-cli-3.1.0/riocli/device/execute.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/files.py` & `rapyuta-io-cli-3.1.0/riocli/device/files.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/inspect.py` & `rapyuta-io-cli-3.1.0/riocli/device/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/label.py` & `rapyuta-io-cli-3.1.0/riocli/device/label.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/list.py` & `rapyuta-io-cli-3.1.0/riocli/device/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/metric.py` & `rapyuta-io-cli-3.1.0/riocli/device/metric.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/model.py` & `rapyuta-io-cli-3.1.0/riocli/device/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/onboard.py` & `rapyuta-io-cli-3.1.0/riocli/device/onboard.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/tools/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/device/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/tools/device_init.py` & `rapyuta-io-cli-3.1.0/riocli/device/tools/device_init.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/tools/forward.py` & `rapyuta-io-cli-3.1.0/riocli/device/tools/forward.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/tools/rapyuta_logs.py` & `rapyuta-io-cli-3.1.0/riocli/device/tools/rapyuta_logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/tools/scp.py` & `rapyuta-io-cli-3.1.0/riocli/device/tools/scp.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/tools/service.py` & `rapyuta-io-cli-3.1.0/riocli/device/tools/service.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/tools/ssh.py` & `rapyuta-io-cli-3.1.0/riocli/device/tools/ssh.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/tools/util.py` & `rapyuta-io-cli-3.1.0/riocli/device/tools/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/topic.py` & `rapyuta-io-cli-3.1.0/riocli/device/topic.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/util.py` & `rapyuta-io-cli-3.1.0/riocli/device/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/device/vpn.py` & `rapyuta-io-cli-3.1.0/riocli/device/vpn.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/disk/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/disk/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/disk/create.py` & `rapyuta-io-cli-3.1.0/riocli/disk/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/disk/delete.py` & `rapyuta-io-cli-3.1.0/riocli/disk/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/disk/list.py` & `rapyuta-io-cli-3.1.0/riocli/disk/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/disk/model.py` & `rapyuta-io-cli-3.1.0/riocli/disk/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/disk/util.py` & `rapyuta-io-cli-3.1.0/riocli/disk/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/exceptions/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/jsonschema/validate.py` & `rapyuta-io-cli-3.1.0/riocli/jsonschema/validate.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/managedservice/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/managedservice/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/managedservice/delete.py` & `rapyuta-io-cli-3.1.0/riocli/managedservice/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/managedservice/inspect.py` & `rapyuta-io-cli-3.1.0/riocli/managedservice/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/managedservice/list.py` & `rapyuta-io-cli-3.1.0/riocli/managedservice/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/managedservice/list_providers.py` & `rapyuta-io-cli-3.1.0/riocli/managedservice/list_providers.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/managedservice/model.py` & `rapyuta-io-cli-3.1.0/riocli/managedservice/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/model/base.py` & `rapyuta-io-cli-3.1.0/riocli/model/base.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/network/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/network/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/network/create.py` & `rapyuta-io-cli-3.1.0/riocli/network/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import click
 
 from riocli.device.util import name_to_guid as device_name_to_guid
 from riocli.network.native_network import create_native_network
 from riocli.network.routed_network import create_routed_network
 
 
-@click.command('create')
+@click.command('create', hidden=True)
 @click.argument('name', type=str)
 @click.option('--network', help='Type of Network',
               type=click.Choice(['routed', 'native']), default='routed')
 @click.option('--ros', help='Version of ROS',
               type=click.Choice(['kinetic', 'melodic', 'noetic']), default='melodic')
 @click.option('--device', 'device_name', help='Device ID of the Device where Network will run (device only)')
 @click.option('--cpu', help='cpu limit for Network (cloud only) ', type=float)
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/network/delete.py` & `rapyuta-io-cli-3.1.0/riocli/network/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/network/inspect.py` & `rapyuta-io-cli-3.1.0/riocli/network/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/network/list.py` & `rapyuta-io-cli-3.1.0/riocli/network/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/network/logs.py` & `rapyuta-io-cli-3.1.0/riocli/network/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/network/model.py` & `rapyuta-io-cli-3.1.0/riocli/network/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/network/native_network.py` & `rapyuta-io-cli-3.1.0/riocli/network/native_network.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/network/routed_network.py` & `rapyuta-io-cli-3.1.0/riocli/network/routed_network.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/network/util.py` & `rapyuta-io-cli-3.1.0/riocli/network/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/organization/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/organization/list.py` & `rapyuta-io-cli-3.1.0/riocli/organization/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/organization/select.py` & `rapyuta-io-cli-3.1.0/riocli/organization/select.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/package/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/package/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/package/create.py` & `rapyuta-io-cli-3.1.0/riocli/parameter/list.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,37 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import json
-
 import click
-import yaml
-from click_spinner import spinner
+from rapyuta_io.utils.rest_client import HttpMethod
 
-from riocli.config import new_client
+from riocli.parameter.utils import _api_call
+from riocli.utils import tabulate_data
 
 
-@click.command('create')
-@click.option('--manifest', type=click.File(mode='r', lazy=True),
-              help='Path for the manifest file')
-@click.option('--format', 'format_type', default='json',
-              type=click.Choice(['json', 'yaml'], case_sensitive=False))
-def create_package(manifest: click.File, format_type: str) -> None:
+@click.command('list')
+def list_configuration_trees() -> None:
     """
-    Create a new package
+    List the Configuration Parameter Trees.
     """
-    data = manifest.read()
-    if format_type == 'json':
-        package = json.loads(data)
-    else:
-        package = yaml.load(data)
-
     try:
-        client = new_client()
-        with spinner():
-            client.create_package(package)
-        click.secho('Package created successfully!', fg='green')
+        data = _api_call(HttpMethod.GET)
+        if 'data' not in data:
+            raise Exception('Something went wrong!')
+
+        trees = [[tree] for tree in data['data']]
+
+        tabulate_data(trees, headers=['Tree Name'])
+
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/package/delete.py` & `rapyuta-io-cli-3.1.0/riocli/package/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/package/deployment.py` & `rapyuta-io-cli-3.1.0/riocli/package/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/package/inspect.py` & `rapyuta-io-cli-3.1.0/riocli/package/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/package/list.py` & `rapyuta-io-cli-3.1.0/riocli/package/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/package/model.py` & `rapyuta-io-cli-3.1.0/riocli/package/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,16 +190,16 @@
             "simulationOptions": {
                 "simulation": exec.simulation if 'simulation' in exec else False
             }
         })
 
         if 'limits' in exec:
             exec_object.limits = {
-                "cpu": exec.limits.cpu,
-                "memory": exec.limits.memory
+                'cpu': exec.limits.get('cpu', 0.0),
+                'memory': exec.limits.get('memory', 0)
             }
 
         if exec.get('runAsBash'):
             if 'command' in exec:
                 exec_object.cmd = ['/bin/bash', '-c', exec.command]
         else:
             # TODO verify this is right for secret?
@@ -208,14 +208,17 @@
 
         if exec.type == 'docker':
             exec_object.docker = exec.docker.image
             if 'pullSecret' in exec.docker and exec.docker.pullSecret.depends:
                 secret_guid, secret = self.rc.find_depends(exec.docker.pullSecret.depends)
                 exec_object.secret = secret_guid
 
+            if exec.docker.get('imagePullPolicy'):
+                exec_object.imagePullPolicy = exec.docker.imagePullPolicy
+
         if exec.type == 'build':
             exec_object.buildGUID = exec.build.depends.guid
             # TODO verify this is right for secret?
             # if exec.docker.pullSecret and exec.docker.pullSecret.depends and exec.docker.pullSecret.depends.guid:
             # exec_object.secret = exec.docker.pullSecret.depends.guid
 
         # TODO handle preinstalled
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/package/util.py` & `rapyuta-io-cli-3.1.0/riocli/package/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/parameter/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/parameter/apply.py` & `rapyuta-io-cli-3.1.0/riocli/parameter/apply.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/parameter/delete.py` & `rapyuta-io-cli-3.1.0/riocli/parameter/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/parameter/diff.py` & `rapyuta-io-cli-3.1.0/riocli/parameter/diff.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/parameter/download.py` & `rapyuta-io-cli-3.1.0/riocli/parameter/download.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/parameter/list.py` & `rapyuta-io-cli-3.1.0/riocli/project/delete.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,42 @@
-# Copyright 2023 Rapyuta Robotics
+# Copyright 2021 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
-from rapyuta_io.utils.rest_client import HttpMethod
+from click_spinner import spinner
 
-from riocli.parameter.utils import _api_call
-from riocli.utils import tabulate_data
+from riocli.config import new_v2_client
+from riocli.project.util import name_to_guid
 
 
-@click.command('list')
-def list_configuration_trees() -> None:
+@click.command('delete')
+@click.option('--force', '-f', '--silent', 'force', is_flag=True,
+              help='Skip confirmation')
+@click.argument('project-name', type=str)
+@name_to_guid
+def delete_project(force: bool, project_name: str, project_guid: str) -> None:
     """
-    List the Configuration Parameter Trees.
+    Deletes the project from the Platform
     """
-    try:
-        data = _api_call(HttpMethod.GET)
-        if 'data' not in data:
-            raise Exception('Something went wrong!')
-
-        trees = [[tree] for tree in data['data']]
-
-        tabulate_data(trees, headers=['Tree Name'])
+    if not force:
+        click.confirm(
+            'Deleting project {} ({})'.format(project_name, project_guid),
+            abort=True)
 
+    try:
+        client = new_v2_client()
+        with spinner():
+            client.delete_project(project_guid)
+        click.secho('Project deleted successfully!', fg='green')
     except Exception as e:
-        click.secho(str(e), fg='red')
+        click.secho('failed to delete project: {}'.format(e), fg='red')
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/parameter/upload.py` & `rapyuta-io-cli-3.1.0/riocli/parameter/upload.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/parameter/utils.py` & `rapyuta-io-cli-3.1.0/riocli/parameter/utils.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/project/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/project/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/project/create.py` & `rapyuta-io-cli-3.1.0/riocli/project/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/project/delete.py` & `rapyuta-io-cli-3.1.0/riocli/static_route/delete.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,33 +10,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 from click_spinner import spinner
 
-from riocli.config import new_v2_client
-from riocli.project.util import name_to_guid
+from riocli.config import new_client
+from riocli.static_route.util import name_to_guid
 
 
 @click.command('delete')
-@click.option('--force', '-f', '--silent', 'force', is_flag=True,
-              help='Skip confirmation')
-@click.argument('project-name', type=str)
+@click.option('--force', '-f', is_flag=True, default=False, help='Skip confirmation')
+@click.argument('static-route', type=str)
 @name_to_guid
-def delete_project(force: bool, project_name: str, project_guid: str) -> None:
+def delete_static_route(static_route: str, static_route_guid: str, force: bool) -> None:
     """
-    Deletes the project from the Platform
+    Deletes the static route resource from the Platform
     """
+
     if not force:
-        click.confirm(
-            'Deleting project {} ({})'.format(project_name, project_guid),
-            abort=True)
+        click.confirm('Deleting static route {} ({})'.format(static_route, static_route_guid),
+                      abort=True)
 
     try:
-        client = new_v2_client()
+        client = new_client()
         with spinner():
-            client.delete_project(project_guid)
-        click.secho('Project deleted successfully!', fg='green')
+            client.delete_static_route(static_route_guid)
+        click.secho('Static Route deleted successfully!', fg='green')
     except Exception as e:
-        click.secho('failed to delete project: {}'.format(e), fg='red')
+        click.secho(str(e), fg='red')
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/project/features/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/project/features/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/project/features/vpn.py` & `rapyuta-io-cli-3.1.0/riocli/project/features/vpn.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/project/inspect.py` & `rapyuta-io-cli-3.1.0/riocli/project/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/project/list.py` & `rapyuta-io-cli-3.1.0/riocli/project/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/project/model.py` & `rapyuta-io-cli-3.1.0/riocli/project/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/project/select.py` & `rapyuta-io-cli-3.1.0/riocli/project/select.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/project/util.py` & `rapyuta-io-cli-3.1.0/riocli/project/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/rosbag/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/rosbag/blob.py` & `rapyuta-io-cli-3.1.0/riocli/rosbag/blob.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/rosbag/job.py` & `rapyuta-io-cli-3.1.0/riocli/rosbag/job.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/secret/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/secret/create.py` & `rapyuta-io-cli-3.1.0/riocli/secret/create.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import click
 from rapyuta_io.clients.secret import DOCKER_HUB_REGISTRY
 
 from riocli.secret.docker_secret import create_docker_secret
 from riocli.secret.source_secret import create_source_secret
 
 
-@click.command('create')
+@click.command('create', hidden=True)
 @click.option('--secret-type', '-t', help='Type of Secret', type=click.Choice(['docker', 'source']))
 @click.option('--username', type=str,
               help='Docker registry username for docker secret, Git username for source secret')
 @click.option('--password', '-p', type=str,
               help='Password (only for docker and source with basic auth)')
 @click.option('--email', type=str,
               help='Email ID for Docker registry')
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/secret/delete.py` & `rapyuta-io-cli-3.1.0/riocli/secret/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/secret/docker_secret.py` & `rapyuta-io-cli-3.1.0/riocli/secret/docker_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/secret/import_secret.py` & `rapyuta-io-cli-3.1.0/riocli/secret/import_secret.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from riocli.config import new_client
 from riocli.utils import random_string, run_bash
 from riocli.utils.selector import show_selection
 
 
 @click.group(
     'import',
+    hidden=True,
     invoke_without_command=False,
     cls=HelpColorsGroup,
     help_headers_color='yellow',
     help_options_color='green',
 )
 def import_secret() -> None:
     """
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/secret/inspect.py` & `rapyuta-io-cli-3.1.0/riocli/secret/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/secret/list.py` & `rapyuta-io-cli-3.1.0/riocli/secret/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/secret/model.py` & `rapyuta-io-cli-3.1.0/riocli/secret/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/secret/source_secret.py` & `rapyuta-io-cli-3.1.0/riocli/secret/source_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/secret/util.py` & `rapyuta-io-cli-3.1.0/riocli/secret/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/shell/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/shell/prompt.py` & `rapyuta-io-cli-3.1.0/riocli/shell/prompt.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/static_route/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/static_route/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/static_route/create.py` & `rapyuta-io-cli-3.1.0/riocli/static_route/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/static_route/delete.py` & `rapyuta-io-cli-3.1.0/riocli/static_route/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,35 +7,75 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import functools
+import typing
+
 import click
-from click_spinner import spinner
+from rapyuta_io import Client
+from rapyuta_io.clients.static_route import StaticRoute
 
 from riocli.config import new_client
-from riocli.static_route.util import name_to_guid
-
 
-@click.command('delete')
-@click.option('--force', '-f', is_flag=True, default=False, help='Skip confirmation')
-@click.argument('static-route', type=str)
-@name_to_guid
-def delete_static_route(static_route: str, static_route_guid: str, force: bool) -> None:
-    """
-    Deletes the static route resource from the Platform
-    """
-
-    if not force:
-        click.confirm('Deleting static route {} ({})'.format(static_route, static_route_guid),
-                      abort=True)
 
-    try:
+def name_to_guid(f: typing.Callable) -> typing.Callable:
+    @functools.wraps(f)
+    def decorated(**kwargs: typing.Any):
         client = new_client()
-        with spinner():
-            client.delete_static_route(static_route_guid)
-        click.secho('Static Route deleted successfully!', fg='green')
-    except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
+        name = kwargs.pop('static_route')
+        guid = None
+
+        if name.startswith('staticroute-'):
+            guid = name
+            name = None
+
+        if name is None:
+            name = get_static_route_name(client, guid)
+
+        if guid is None:
+            guid = find_static_route_guid(client, name)
+
+        kwargs['static_route'] = name
+        kwargs['static_route_guid'] = guid
+        f(**kwargs)
+
+    return decorated
+
+
+def get_static_route_name(client: Client, guid: str) -> str:
+    static_route = client.get_static_route(guid)
+    return static_route.urlPrefix.split("-")[0]
+
+
+def find_static_route_guid(client: Client, name: str) -> str:
+    routes = client.get_all_static_routes()
+    for route in routes:
+        if route.urlPrefix == name or route.urlString == name:
+            return route.guid
+
+    raise StaticRouteNotFound()
+
+
+def repr_static_routes(routes: typing.List[StaticRoute]) -> None:
+    header = '{:<36} {:<25} {:36} {:36} {:32}'.format(
+        'Static Route ID',
+        'Name',
+        'Full URL',
+        'Creator',
+        'Created At',
+    )
+    click.echo(click.style(header, fg='yellow'))
+    for route in routes:
+        click.secho(
+            '{:<36} {:<25} {:36} {:36} {:32}'.
+            format(route.guid, route.urlPrefix, route.urlString, route.creator,
+                   route.CreatedAt))
+
+
+class StaticRouteNotFound(Exception):
+    def __init__(self, message='secret not found'):
+        self.message = message
+        super().__init__(self.message)
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/static_route/inspect.py` & `rapyuta-io-cli-3.1.0/riocli/static_route/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/static_route/list.py` & `rapyuta-io-cli-3.1.0/riocli/static_route/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/static_route/model.py` & `rapyuta-io-cli-3.1.0/riocli/static_route/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/static_route/open.py` & `rapyuta-io-cli-3.1.0/riocli/static_route/open.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/utils/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/utils/context.py` & `rapyuta-io-cli-3.1.0/riocli/utils/context.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/utils/execute.py` & `rapyuta-io-cli-3.1.0/riocli/utils/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     run_on_cloud uses the RunCommand API of the IOBroker to execute arbitrary commands on the cloud deployment
     containers.
     """
     config = Configuration()
     rest = RestClient(_run_cloud_url(config, deployment_guid)).headers(config.get_auth_header()).method(HttpMethod.PUT)
     resp = rest.execute(payload=_run_cloud_data(comp_id, exec_id, pod_name, command))
     data = json.loads(resp.text)
-    click.secho(data)
     if 'err' in data and data['err']:
         raise Exception(data['err'])
 
     return data['stdout'], data['stderr']
 
 
 def _run_cloud_data(comp_id: str, exec_id: str, pod_name: str, command: typing.List[str]) -> dict:
```

### Comparing `rapyuta-io-cli-3.0.0/riocli/utils/selector.py` & `rapyuta-io-cli-3.1.0/riocli/utils/selector.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/utils/spinner.py` & `rapyuta-io-cli-3.1.0/riocli/utils/spinner.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/utils/ssh_tunnel.py` & `rapyuta-io-cli-3.1.0/riocli/utils/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/v2client/client.py` & `rapyuta-io-cli-3.1.0/riocli/v2client/client.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/vpn/__init__.py` & `rapyuta-io-cli-3.1.0/riocli/vpn/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/vpn/connect.py` & `rapyuta-io-cli-3.1.0/riocli/vpn/connect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/vpn/disconnect.py` & `rapyuta-io-cli-3.1.0/riocli/vpn/disconnect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/vpn/ping.py` & `rapyuta-io-cli-3.1.0/riocli/vpn/ping.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/vpn/status.py` & `rapyuta-io-cli-3.1.0/riocli/vpn/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/riocli/vpn/util.py` & `rapyuta-io-cli-3.1.0/riocli/vpn/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-3.0.0/setup.py` & `rapyuta-io-cli-3.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         "dictdiffer>=0.9.0",
         "graphlib-backport>=1.0.3",
         "jinja2>=3.0.1",
         "munch>=2.4.0",
         "python-dateutil>=2.8.2",
         "pytz",
         "pyyaml>=5.4.1",
-        "rapyuta-io>=1.9.0",
+        "rapyuta-io>=1.10.0",
         "requests>=2.20.0",
         "setuptools",
         "six>=1.13.0",
         "tabulate>=0.8.0",
         "urllib3>=1.23",
         "pyrfc3339>=1.1",
         "directory-tree>=0.0.3.1",
```

