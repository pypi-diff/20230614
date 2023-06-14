# Comparing `tmp/sinabs-dynapcnn-1.0.9.dev9.tar.gz` & `tmp/sinabs-dynapcnn-1.0.9.dev97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sinabs-dynapcnn-1.0.9.dev9.tar", last modified: Fri Nov 25 02:59:54 2022, max compression
+gzip compressed data, was "dist/sinabs-dynapcnn-1.0.9.dev97.tar", last modified: Mon Dec 26 06:35:37 2022, max compression
```

## Comparing `sinabs-dynapcnn-1.0.9.dev9.tar` & `sinabs-dynapcnn-1.0.9.dev97.tar`

### file list

```diff
@@ -1,96 +1,124 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/
--rw-rw-rw-   0 root         (0) root         (0)     1235 2022-04-25 14:02:39.000000 sinabs-dynapcnn-1.0.9.dev9/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      893 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)    15927 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/ChangeLog
--rw-r--r--   0 root         (0) root         (0)     1592 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      214 2022-10-23 20:51:13.000000 sinabs-dynapcnn-1.0.9.dev9/Pipfile
--rw-rw-rw-   0 root         (0) root         (0)    21705 2022-10-23 20:51:13.000000 sinabs-dynapcnn-1.0.9.dev9/Pipfile.lock
--rw-rw-rw-   0 root         (0) root         (0)      668 2021-08-04 05:05:57.000000 sinabs-dynapcnn-1.0.9.dev9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      764 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       70 2022-04-29 10:31:30.000000 sinabs-dynapcnn-1.0.9.dev9/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)    19527 2022-04-29 10:31:30.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/_static/sinabs-logo-lowercase-whitebg.png
--rw-rw-rw-   0 root         (0) root         (0)     3178 2022-04-29 10:35:24.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/advanced_concepts.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/api/
--rw-rw-rw-   0 root         (0) root         (0)       44 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/api/api.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/api/dynapcnn/
--rw-rw-rw-   0 root         (0) root         (0)      125 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/api/dynapcnn/chip_factory.rst
--rw-rw-rw-   0 root         (0) root         (0)      133 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/api/dynapcnn/config_builder.rst
--rw-rw-rw-   0 root         (0) root         (0)       82 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/api/dynapcnn/crop2d.rst
--rw-rw-rw-   0 root         (0) root         (0)      189 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/api/dynapcnn/discretize.rst
--rw-rw-rw-   0 root         (0) root         (0)      113 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/api/dynapcnn/dvs_layer.rst
--rw-rw-rw-   0 root         (0) root         (0)      235 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/api/dynapcnn/dynapcnn.rst
--rw-rw-rw-   0 root         (0) root         (0)      222 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/api/dynapcnn/dynapcnn_layer.rst
--rw-rw-rw-   0 root         (0) root         (0)      259 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/api/dynapcnn/dynapcnn_network.rst
--rw-rw-rw-   0 root         (0) root         (0)      226 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/api/dynapcnn/exceptions.rst
--rw-rw-rw-   0 root         (0) root         (0)      110 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/api/dynapcnn/flipdims.rst
--rw-rw-rw-   0 root         (0) root         (0)      156 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/api/dynapcnn/io.rst
--rw-rw-rw-   0 root         (0) root         (0)      146 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/api/dynapcnn/mapping.rst
--rw-rw-rw-   0 root         (0) root         (0)       73 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/api/dynapcnn/utils.rst
--rw-rw-rw-   0 root         (0) root         (0)      420 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/change_log.rst
--rw-rw-rw-   0 root         (0) root         (0)     3137 2022-04-29 10:31:30.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      602 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/dangers.md
--rw-rw-rw-   0 root         (0) root         (0)     1578 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/development.md
--rw-rw-rw-   0 root         (0) root         (0)     8425 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/dynapcnn_model.md
--rw-rw-rw-   0 root         (0) root         (0)      905 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      828 2022-04-29 10:31:30.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/installation.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)    22592 2022-04-29 10:35:24.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/notebooks/cnn_to_dynapcnn.ipynb
--rw-rw-rw-   0 root         (0) root         (0)       64 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/docs/source/tutorials.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/examples/
--rw-rw-rw-   0 root         (0) root         (0)     3107 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev9/examples/mnist_dynapcnn.py
--rw-rw-rw-   0 root         (0) root         (0)   491676 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/examples/mnist_params.pt
--rw-rw-rw-   0 root         (0) root         (0)      109 2022-04-25 14:02:39.000000 sinabs-dynapcnn-1.0.9.dev9/jupyterlab-requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-11-18 15:55:34.000000 sinabs-dynapcnn-1.0.9.dev9/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1020 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       80 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/
--rw-rw-rw-   0 root         (0) root         (0)      214 2022-04-29 10:31:30.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6057 2022-11-25 02:03:31.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/chip_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/chips/
--rw-rw-rw-   0 root         (0) root         (0)      268 2022-11-22 18:17:51.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/chips/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11753 2022-11-23 03:34:16.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/chips/dynapcnn.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-11-23 03:34:16.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/chips/speck2.py
--rw-rw-rw-   0 root         (0) root         (0)      746 2022-11-23 03:34:16.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/chips/speck2b.py
--rw-rw-rw-   0 root         (0) root         (0)     2031 2022-11-23 03:34:16.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/chips/speck2cmini.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2022-11-23 03:34:16.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/chips/speck2dmini.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2022-11-23 03:34:16.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/chips/speck2e.py
--rw-rw-rw-   0 root         (0) root         (0)     4191 2022-11-25 02:03:31.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/config_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     1508 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/crop2d.py
--rw-rw-rw-   0 root         (0) root         (0)    13386 2022-11-21 09:50:49.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/discretize.py
--rw-rw-rw-   0 root         (0) root         (0)     9027 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/dvs_layer.py
--rw-rw-rw-   0 root         (0) root         (0)     6705 2022-10-27 10:08:00.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/dynapcnn_layer.py
--rw-rw-rw-   0 root         (0) root         (0)    16200 2022-11-25 02:03:31.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/dynapcnn_network.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      867 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/flipdims.py
--rw-rw-rw-   0 root         (0) root         (0)     7001 2022-11-25 02:03:31.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/io.py
--rw-rw-rw-   0 root         (0) root         (0)     6693 2022-04-29 10:35:24.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/mapping.py
--rw-rw-rw-   0 root         (0) root         (0)    13929 2022-10-27 14:17:32.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs_dynapcnn.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1592 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs_dynapcnn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2536 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs_dynapcnn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs_dynapcnn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs_dynapcnn.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs_dynapcnn.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       32 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs_dynapcnn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/sinabs_dynapcnn.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 02:59:54.000000 sinabs-dynapcnn-1.0.9.dev9/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1202 2022-10-23 20:51:13.000000 sinabs-dynapcnn-1.0.9.dev9/tests/test_auto_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)     5074 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev9/tests/test_compatible_layer_build.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2022-10-23 20:51:13.000000 sinabs-dynapcnn-1.0.9.dev9/tests/test_config_making.py
--rw-rw-rw-   0 root         (0) root         (0)     1077 2022-10-23 20:51:13.000000 sinabs-dynapcnn-1.0.9.dev9/tests/test_device_movement.py
--rw-rw-rw-   0 root         (0) root         (0)     1151 2022-11-25 02:03:31.000000 sinabs-dynapcnn-1.0.9.dev9/tests/test_discover_device.py
--rw-rw-rw-   0 root         (0) root         (0)    12139 2022-11-21 09:50:49.000000 sinabs-dynapcnn-1.0.9.dev9/tests/test_discretized.py
--rw-rw-rw-   0 root         (0) root         (0)     2687 2022-10-27 14:43:24.000000 sinabs-dynapcnn-1.0.9.dev9/tests/test_doorbell.py
--rw-rw-rw-   0 root         (0) root         (0)    10475 2022-10-27 14:54:12.000000 sinabs-dynapcnn-1.0.9.dev9/tests/test_dvs_input.py
--rw-rw-rw-   0 root         (0) root         (0)     2634 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev9/tests/test_dvs_layer.py
--rw-rw-rw-   0 root         (0) root         (0)     5647 2022-10-27 14:43:24.000000 sinabs-dynapcnn-1.0.9.dev9/tests/test_individual_cases.py
--rw-rw-rw-   0 root         (0) root         (0)     4776 2022-10-27 14:43:24.000000 sinabs-dynapcnn-1.0.9.dev9/tests/test_large_net.py
--rw-rw-rw-   0 root         (0) root         (0)     2601 2022-11-25 02:03:31.000000 sinabs-dynapcnn-1.0.9.dev9/tests/test_learning.py
--rw-rw-rw-   0 root         (0) root         (0)     3521 2022-10-23 20:51:13.000000 sinabs-dynapcnn-1.0.9.dev9/tests/test_monitoring.py
--rw-rw-rw-   0 root         (0) root         (0)     3035 2022-10-23 20:51:13.000000 sinabs-dynapcnn-1.0.9.dev9/tests/test_speckmini_config_making.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2022-12-09 10:07:40.000000 sinabs-dynapcnn-1.0.9.dev97/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)     1882 2022-12-09 10:07:40.000000 sinabs-dynapcnn-1.0.9.dev97/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      965 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)    19369 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)     1766 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      214 2022-10-23 20:51:13.000000 sinabs-dynapcnn-1.0.9.dev97/Pipfile
+-rw-rw-rw-   0 root         (0) root         (0)    21705 2022-10-23 20:51:13.000000 sinabs-dynapcnn-1.0.9.dev97/Pipfile.lock
+-rw-rw-rw-   0 root         (0) root         (0)      825 2022-12-09 10:07:40.000000 sinabs-dynapcnn-1.0.9.dev97/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      764 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       82 2022-12-09 10:07:40.000000 sinabs-dynapcnn-1.0.9.dev97/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/Overview/
+-rw-rw-rw-   0 root         (0) root         (0)    41488 2022-12-19 02:50:35.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/Overview/dataflow_layers.png
+-rw-rw-rw-   0 root         (0) root         (0)    20394 2022-12-19 02:50:35.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/Overview/event_preprocessing_pipeline.png
+-rw-rw-rw-   0 root         (0) root         (0)    34971 2022-12-19 02:50:35.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/Overview/memory_constraints.png
+-rw-rw-rw-   0 root         (0) root         (0)    56246 2022-12-19 02:50:35.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/Overview/sinabs-dynapcnn-role.png
+-rw-rw-rw-   0 root         (0) root         (0)    24493 2022-12-19 02:50:35.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/Overview/speck_dynapcnn.png
+-rw-rw-rw-   0 root         (0) root         (0)   345972 2022-12-19 03:10:59.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/Overview/speck_top_level.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/power_monitoring/
+-rw-rw-rw-   0 root         (0) root         (0)    36805 2022-12-19 05:52:58.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/power_monitoring/dynamic_power_samna_graph.png
+-rw-rw-rw-   0 root         (0) root         (0)    24621 2022-12-19 05:52:58.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/power_monitoring/idle_power_samna_graph.png
+-rw-rw-rw-   0 root         (0) root         (0)    30647 2022-12-19 05:52:58.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/power_monitoring/power_plot.png
+-rw-rw-rw-   0 root         (0) root         (0)    19527 2022-04-29 10:31:30.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/sinabs-logo-lowercase-whitebg.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/using_readout_layer/
+-rw-rw-rw-   0 root         (0) root         (0)    80444 2022-12-19 05:52:58.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/using_readout_layer/handcraft_weights.png
+-rw-rw-rw-   0 root         (0) root         (0)    28534 2022-12-19 05:52:58.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/using_readout_layer/neuron_id_mismatch.png
+-rw-rw-rw-   0 root         (0) root         (0)    48829 2022-12-19 05:52:58.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/using_readout_layer/readout_layer.png
+-rw-rw-rw-   0 root         (0) root         (0)    59701 2022-12-19 05:52:58.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/using_readout_layer/samna_graph.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/visualize_speck_dvs/
+-rw-rw-rw-   0 root         (0) root         (0)    21577 2022-12-19 05:52:58.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/visualize_speck_dvs/samna_graph.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/visualize_spike_count/
+-rw-rw-rw-   0 root         (0) root         (0)    53316 2022-12-19 06:45:30.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/visualize_spike_count/samna_graph.png
+-rw-rw-rw-   0 root         (0) root         (0)    18218 2022-12-19 05:52:58.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/visualize_spike_count/spike_count.png
+-rw-rw-rw-   0 root         (0) root         (0)     3178 2022-04-29 10:35:24.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/advanced_concepts.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/api/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/api/api.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/api/dynapcnn/
+-rw-rw-rw-   0 root         (0) root         (0)      125 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/api/dynapcnn/chip_factory.rst
+-rw-rw-rw-   0 root         (0) root         (0)      133 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/api/dynapcnn/config_builder.rst
+-rw-rw-rw-   0 root         (0) root         (0)       82 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/api/dynapcnn/crop2d.rst
+-rw-rw-rw-   0 root         (0) root         (0)      189 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/api/dynapcnn/discretize.rst
+-rw-rw-rw-   0 root         (0) root         (0)      113 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/api/dynapcnn/dvs_layer.rst
+-rw-rw-rw-   0 root         (0) root         (0)      235 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/api/dynapcnn/dynapcnn.rst
+-rw-rw-rw-   0 root         (0) root         (0)      222 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/api/dynapcnn/dynapcnn_layer.rst
+-rw-rw-rw-   0 root         (0) root         (0)      259 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/api/dynapcnn/dynapcnn_network.rst
+-rw-rw-rw-   0 root         (0) root         (0)      226 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/api/dynapcnn/exceptions.rst
+-rw-rw-rw-   0 root         (0) root         (0)      110 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/api/dynapcnn/flipdims.rst
+-rw-rw-rw-   0 root         (0) root         (0)      156 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/api/dynapcnn/io.rst
+-rw-rw-rw-   0 root         (0) root         (0)      146 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/api/dynapcnn/mapping.rst
+-rw-rw-rw-   0 root         (0) root         (0)       73 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/api/dynapcnn/utils.rst
+-rw-rw-rw-   0 root         (0) root         (0)      420 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/change_log.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3216 2022-12-09 10:07:40.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      602 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/dangers.md
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/development.md
+-rw-rw-rw-   0 root         (0) root         (0)     8425 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/dynapcnn_model.md
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2022-12-09 10:07:40.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      828 2022-04-29 10:31:30.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/installation.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)    14757 2022-12-19 03:10:59.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/notebooks/Overview.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    23771 2022-12-22 06:28:21.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/notebooks/cnn_to_dynapcnn.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    65521 2022-12-19 05:52:58.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/notebooks/power_monitoring.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    63276 2022-12-19 05:52:58.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/notebooks/using_readout_layer.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    11469 2022-12-19 05:52:58.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/notebooks/visualize_speck_dvs_input.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    45950 2022-12-19 06:45:30.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/notebooks/visualize_spike_count.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      227 2022-12-19 06:45:30.000000 sinabs-dynapcnn-1.0.9.dev97/docs/source/tutorials.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     3107 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev97/examples/mnist_dynapcnn.py
+-rw-rw-rw-   0 root         (0) root         (0)   491676 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/examples/mnist_params.pt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2022-04-25 14:02:39.000000 sinabs-dynapcnn-1.0.9.dev97/jupyterlab-requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       37 2022-12-19 05:52:58.000000 sinabs-dynapcnn-1.0.9.dev97/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1020 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       80 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/
+-rw-rw-rw-   0 root         (0) root         (0)      214 2022-04-29 10:31:30.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6788 2022-12-09 10:07:40.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/chip_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/chips/
+-rw-rw-rw-   0 root         (0) root         (0)      268 2022-11-22 18:17:51.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/chips/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11645 2022-12-22 06:01:01.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/chips/dynapcnn.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2022-12-09 10:17:59.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/chips/speck2.py
+-rw-rw-rw-   0 root         (0) root         (0)      728 2022-12-26 06:35:33.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/chips/speck2b.py
+-rw-rw-rw-   0 root         (0) root         (0)     1976 2022-12-09 10:07:40.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/chips/speck2cmini.py
+-rw-rw-rw-   0 root         (0) root         (0)      718 2022-12-09 10:07:40.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/chips/speck2dmini.py
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-22 06:01:01.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/chips/speck2e.py
+-rw-rw-rw-   0 root         (0) root         (0)     4808 2022-12-09 08:15:41.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/config_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1508 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/crop2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    13476 2022-12-13 12:10:09.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/discretize.py
+-rw-rw-rw-   0 root         (0) root         (0)     9027 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/dvs_layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6705 2022-10-27 10:08:00.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/dynapcnn_layer.py
+-rw-rw-rw-   0 root         (0) root         (0)    17086 2022-12-21 16:04:51.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/dynapcnn_network.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      867 2021-08-04 04:34:29.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/flipdims.py
+-rw-rw-rw-   0 root         (0) root         (0)     7489 2022-12-09 10:07:40.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     6693 2022-04-29 10:35:24.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)    14981 2022-12-21 16:04:51.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs_dynapcnn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1766 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs_dynapcnn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3724 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs_dynapcnn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs_dynapcnn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs_dynapcnn.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs_dynapcnn.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       32 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs_dynapcnn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/sinabs_dynapcnn.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 06:35:37.000000 sinabs-dynapcnn-1.0.9.dev97/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2022-10-23 20:51:13.000000 sinabs-dynapcnn-1.0.9.dev97/tests/test_auto_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)     5074 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev97/tests/test_compatible_layer_build.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2022-10-23 20:51:13.000000 sinabs-dynapcnn-1.0.9.dev97/tests/test_config_making.py
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2022-10-23 20:51:13.000000 sinabs-dynapcnn-1.0.9.dev97/tests/test_device_movement.py
+-rw-rw-rw-   0 root         (0) root         (0)      388 2022-12-09 10:07:40.000000 sinabs-dynapcnn-1.0.9.dev97/tests/test_device_name_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)     1151 2022-11-28 16:21:31.000000 sinabs-dynapcnn-1.0.9.dev97/tests/test_discover_device.py
+-rw-rw-rw-   0 root         (0) root         (0)    12147 2022-12-13 12:10:09.000000 sinabs-dynapcnn-1.0.9.dev97/tests/test_discretized.py
+-rw-rw-rw-   0 root         (0) root         (0)     2687 2022-10-27 14:43:24.000000 sinabs-dynapcnn-1.0.9.dev97/tests/test_doorbell.py
+-rw-rw-rw-   0 root         (0) root         (0)    10475 2022-10-27 14:54:12.000000 sinabs-dynapcnn-1.0.9.dev97/tests/test_dvs_input.py
+-rw-rw-rw-   0 root         (0) root         (0)     2634 2022-03-23 12:23:00.000000 sinabs-dynapcnn-1.0.9.dev97/tests/test_dvs_layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5961 2022-12-21 16:13:09.000000 sinabs-dynapcnn-1.0.9.dev97/tests/test_individual_cases.py
+-rw-rw-rw-   0 root         (0) root         (0)     4776 2022-10-27 14:43:24.000000 sinabs-dynapcnn-1.0.9.dev97/tests/test_large_net.py
+-rw-rw-rw-   0 root         (0) root         (0)     2601 2022-11-28 16:21:31.000000 sinabs-dynapcnn-1.0.9.dev97/tests/test_learning.py
+-rw-rw-rw-   0 root         (0) root         (0)     3521 2022-10-23 20:51:13.000000 sinabs-dynapcnn-1.0.9.dev97/tests/test_monitoring.py
+-rw-rw-rw-   0 root         (0) root         (0)     3035 2022-10-23 20:51:13.000000 sinabs-dynapcnn-1.0.9.dev97/tests/test_speckmini_config_making.py
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/.gitlab-ci.yml` & `sinabs-dynapcnn-1.0.9.dev97/.gitlab-ci.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,112 @@
 image: aictx/ci-python-arch:latest
 
+stages:
+    - build
+    - test
+    - coverage
+    - deploy
+
 before_script:
   - pacman -Sy graphviz --noconfirm
   - pacman -Sy libxrandr libxi libxinerama libxcursor glu --noconfirm
   - pip install torchvision -U
   - pip install --upgrade pip
   - pip install -r requirements.txt
   - pip install . --no-cache-dir
   - pip install -r docs/requirements.txt
+  - export PYTHON_SITE_PACKAGES=$(python -c 'import sysconfig; print(sysconfig.get_paths()["purelib"])')
+
 
 dist_build:
   tags:
     - python
     - aiCTX
-
   stage: build
-
   only:
     refs:
       - master
-
   before_script:
     - pip install wheel
-
   script:
     - python setup.py sdist bdist_wheel
-
   artifacts:
     paths:
       - dist
 
 pages:
   tags:
     - python
     - aiCTX
-
   stage: deploy
   only:
     refs:
       - master
-
   script:
     - python setup.py build_sphinx
     - mv docs/build/html/ public/
-
   artifacts:
     paths:
       - public
 
-doc_tests:
+test coverage:
   tags:
     - python
     - aiCTX
+  stage: coverage
+  dependencies:
+   - unittests
+  script:
+    - pip install pytest-cov
+    - pytest --cov
 
-  stage: test
+test coverage deplop:
+  tags:
+    - python
+    - aiCTX
+  stage: deploy
+  dependencies:
+    - test coverage
+  only:
+    refs:
+      - master
+  script:
+    - pip install pytest-cov
+    - pytest --cov
+    - coverage report
+    - coverage xml
+    - curl -Os https://uploader.codecov.io/latest/linux/codecov
+    - chmod +x codecov
+    - ./codecov
 
+doc_tests:
+  tags:
+    - python
+    - aiCTX
+  stage: test
   script:
     - python setup.py build_sphinx
 
 unittests:
   tags:
     - python
     - aiCTX
-
   stage: test
-
   script:
     - pytest
 
-
 pypi_deploy:
   tags:
     - python
     - aiCTX
-
   stage: deploy
-
   only:
     refs:
       - master
     variables:
       - $TWINE_USERNAME == "sheiksadique"
-
   dependencies:
     - dist_build
-
   before_script:
     - pip install --upgrade twine
-
   script:
     - twine upload dist/*
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/AUTHORS` & `sinabs-dynapcnn-1.0.9.dev97/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 Carsten Nielsen <carsten.nielsen@ai-ctx.com>
 Felix Bauer <felix.bauer@aictx.ai>
+Gregor Lenz <gregor.lenz@synsense.ai>
 Gregor Lenz <mail@lenzgregor.com>
 Martino Sorbaro <martino.sorbaro@ed.ac.uk>
 Martino Sorbaro <martino.sorbaro@posteo.net>
 Nogay Küpelioglu <nogay.kuepelioglu@synsense.ai>
 Nogay Küpelioğlu <kupelioglun@mef.edu.tr>
 Roberto Cattaneo <roberto.cattaneo@synsense.ai>
 Sadique Sheik <sadique.sheik@aictx.ai>
@@ -16,7 +17,8 @@
 nogay.kuepelioglu <kupelioglun@mef.edu.tr>
 nogay.kuepelioglu <nogay.kuepelioglu@synsense.ai>
 sadique.sheik <sadique.sheik@ai-ctx.com>
 sadique.sheik <sadique.sheik@synsense.ai>
 yalun.hu <yalun.hu@synsense.ai>
 yannan xing <yannan.xing@synsense.ai>
 yannan.xing <yannan.xing@synsense.ai>
+yijing.lv <yijing.lv@synsense.ai>
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/ChangeLog` & `sinabs-dynapcnn-1.0.9.dev97/ChangeLog`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,77 @@
 CHANGES
 =======
 
+* add a time.sleep statement after dynapcnn network reset-states to wait the config take effect
+* test updated to check for type
+* added checks if the network is empty
+* add spike count visualization notebook into tutorials.rst
+* fix typo in the notebook of visualize spike count
+* delete chip top level figure
+* change the speck top level figure path
+* change top level figure
+* add notebooks into docs/source/tutorials.rst
+* update the noteboob
+* Update requirements.txt
+* notebook and image for spike counts visualization
+* modify the parent folder name identical to the notebook
+* modify the image load path
+* make spike\_threshold and min\_v\_mem a parameter
+* fix test which seems to have relied on older version of PyTorch
+* fix wrong calculation formula in remapping neruon index function
+* fix conflict when merge develop into 34-add-readout-layer-usage-instruction-notebook
+* add samna graph plot for power monitor notebook
+* add notebook for power monitoring
+* update the readout-layer intro notebook
+* add FAQ and known dev kit bugs
+* rm change in tutorials.rst to avoid merge conflict
+* add figures for overview notebook
+* add overview tutorial notebook for speck/dynapcnn
+* removed all samna checks from imports
+* imports fixed and type annotation for Tuple corrected
+* add notebook about dvs input visualization
+* added standardize\_device\_id before all IO methods
+* add codecov badges
+* pytest command fixed for coverage
+* added path to installation for coverage
+* try hard-coded path for coverage
+* added conditional deplopment
+* rerunning test in deploy stage
+* custom stage added
+* added dependenct to unitttests
+* two stage coverage deployment
+* changed command for acquiring code coverage
+* coverage path fixed
+* remove gallery from docs as not needed at the moment
+* added galary template, updated config -> sinabs
+* add coverage config file that specifies the folder to include in the coverage, excluding the test folder
+* remove some whitespace in the gitlab ci config
+* use codecov token so that hopefully CI is pushed via gitlab.com
+* update gitlab CI to produce html coverage report for pages
+* try using gitlab pages for coverage report
+* adding test coverage job to CI pipeline according to Python template from gitlab.com
+* remove gallery from docs as not needed at the moment
+* add figures for the readout layer intro notebook
+* add readout layer usage example notebook
+* added galary template, updated config -> sinabs
+* init tutorial file
+* Fix to the issue
+* Change last uint
+* Remove comment
+* Uint64 to int
+* Check the timestamp and delay factor for negative values
+* Casting to int after conversion
+* Do not sleep while resetting the states when the function is called. Stop the input graph, while the neuron values are written. Sleep for a bit and then start the graph again
+* Fix to the bug
 * update ChangeLog after add support of speck2e
 * add speck2e devkit and testboard support
 * remove redundant comment code
+* Device input graph stopped on destruction of the DynapcnnNetwork object
+* Writing all v mem to zeros changed. -> Now when you call this method it creates a temporary buffer and a temporary graph, starts the graph, writes the events, stops the graph then it is destroyed
+* Implement an input buffer for all devices: -> In the config\_builder there is now a function called get\_input\_buffer which gives a source node. -> For each chip this is implemented to get the appropriate source node. -> To method changed to construct the input buffer. -> Forward method changed to write the events to this source node
 * Name added to io
 * naive copy of config generation
 * moved kill bits to a separate method
 
 v1.0.8
 ------
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/PKG-INFO` & `sinabs-dynapcnn-1.0.9.dev97/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: sinabs-dynapcnn
-Version: 1.0.9.dev9
+Version: 1.0.9.dev97
 Summary: sinabs plugin for porting models to chips with DYNAP-CNN technology
 Home-page: UNKNOWN
 Author: SynSense
 Author-email: sinabs@synsense.ai
 License: GNU AGPLv3
 Project-URL: Source Code, https://gitlab.com/synsense/sinabs-dynapcnn
 Project-URL: Documentation, https://synsense.gitlab.io/sinabs-dynapcnn
 Description: sinabs-dynapcnn
         ===============
         
+        [![codecov](https://codecov.io/gl/synsense/sinabs-dynapcnn/branch/master/graph/badge.svg?token=TJJJBJTHWK)](https://codecov.io/gl/synsense/sinabs-dynapcnn)
+        
         This `sinabs` plugin enables porting sinabs models to chips and dev-kits with DYNAP-CNN technology.
         
         Documentation
         -------------
         
         You can find the latest documentation at [https://synsense.gitlab.io/sinabs-dynapcnn/](https://synsense.gitlab.io/sinabs-dynapcnn/)
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/Pipfile.lock` & `sinabs-dynapcnn-1.0.9.dev97/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/README.md` & `sinabs-dynapcnn-1.0.9.dev97/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 sinabs-dynapcnn
 ===============
 
+[![codecov](https://codecov.io/gl/synsense/sinabs-dynapcnn/branch/master/graph/badge.svg?token=TJJJBJTHWK)](https://codecov.io/gl/synsense/sinabs-dynapcnn)
+
 This `sinabs` plugin enables porting sinabs models to chips and dev-kits with DYNAP-CNN technology.
 
 Documentation
 -------------
 
 You can find the latest documentation at [https://synsense.gitlab.io/sinabs-dynapcnn/](https://synsense.gitlab.io/sinabs-dynapcnn/)
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/docs/Makefile` & `sinabs-dynapcnn-1.0.9.dev97/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/docs/make.bat` & `sinabs-dynapcnn-1.0.9.dev97/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/docs/source/_static/sinabs-logo-lowercase-whitebg.png` & `sinabs-dynapcnn-1.0.9.dev97/docs/source/_static/sinabs-logo-lowercase-whitebg.png`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/docs/source/advanced_concepts.rst` & `sinabs-dynapcnn-1.0.9.dev97/docs/source/advanced_concepts.rst`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/docs/source/conf.py` & `sinabs-dynapcnn-1.0.9.dev97/docs/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,50 +13,50 @@
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 import sinabs.backend.dynapcnn
 
 # -- Project information -----------------------------------------------------
 
-project = 'sinabs-dynapcnn'
-copyright = '2020-2022, Synsense AG'
-author = 'Sadique Sheik, Martino Sorbaro, Felix Bauer'
+project = "sinabs-dynapcnn"
+copyright = "2020-2022, Synsense AG"
+author = "Sadique Sheik, Martino Sorbaro, Felix Bauer"
 
 # The full version, including alpha/beta/rc tags
 # release = '0.0.1'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    #'nbsphinx',
-    "pbr.sphinxext",
-    'sphinx.ext.autodoc',
-    'sphinx.ext.napoleon',
-    'sphinx.ext.graphviz',
-    'sphinx.ext.mathjax',
     "myst_nb",
-    #'m2r2',
+    "pbr.sphinxext",
+    "sphinx.ext.autodoc",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.graphviz",
 ]
 
 # Napoleon settings
 napoleon_google_docstring = True
 napoleon_numpy_docstring = True
 
 # MyST settings
 suppress_warnings = ["myst.header"]
-jupyter_execute_notebooks = "off"
+nb_execution_mode = "off"
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
-#source_suffix = {".rst": 'restructuredtext',
+# source_suffix = {".rst": 'restructuredtext',
 #                 ".txt": 'markdown',
 #                 ".md": 'markdown',
 #                 }
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
@@ -72,29 +72,31 @@
 html_logo = "_static/sinabs-logo-lowercase-whitebg.png"
 html_show_sourcelink = True
 html_sourcelink_suffix = ""
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 html_theme_options = {
     "repository_url": "https://gitlab.com/synsense/sinabs-dynapcnn",
     "use_repository_button": True,
     "use_issues_button": True,
     "use_edit_page_button": True,
-    "repository_branch": "main",
+    "repository_branch": "develop",
     "path_to_docs": "docs",
     "use_fullscreen_button": True,
 }
 
 
-
 # Include __init__ docstring in method documentation
-autoclass_content = 'both'
+autoclass_content = "both"
 
 # Include return type in line
 napoleon_use_rtype = False
 
 # API module name display
 add_module_names = False
+
+# Graphviz output format
+graphviz_output_format = "svg"
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/docs/source/dangers.md` & `sinabs-dynapcnn-1.0.9.dev97/docs/source/dangers.md`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/docs/source/development.md` & `sinabs-dynapcnn-1.0.9.dev97/docs/source/development.md`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/docs/source/dynapcnn_model.md` & `sinabs-dynapcnn-1.0.9.dev97/docs/source/dynapcnn_model.md`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/docs/source/index.rst` & `sinabs-dynapcnn-1.0.9.dev97/docs/source/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,17 @@
    sphinx-quickstart on Fri Jun 12 16:48:59 2020.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Welcome to sinabs-dynapcnn's documentation!
 ===========================================
 
+.. image:: https://codecov.io/gl/synsense/sinabs-dynapcnn/branch/master/graph/badge.svg?token=TJJJBJTHWK 
+ :target: https://codecov.io/gl/synsense/sinabs-dynapcnn
+   
 This `sinabs` plugin enables porting sinabs models to chips and dev-kits with DYNAP-CNN technology.
 
 To get started take a look at the
 
 - The documentation below
 - :doc:`cnn-to-dynapcnn tutorial<notebooks/cnn_to_dynapcnn>`.
 - `examples <https://gitlab.com/synsense/sinabs-dynapcnn/~/tree/master/examples>`_
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/docs/source/installation.md` & `sinabs-dynapcnn-1.0.9.dev97/docs/source/installation.md`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/docs/source/notebooks/cnn_to_dynapcnn.ipynb` & `sinabs-dynapcnn-1.0.9.dev97/docs/source/notebooks/cnn_to_dynapcnn.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9931393035404266%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(10, 'import time\\n')]}}, 12: {'outputs': {0: {'text': "*

 * *            "{insert: [(2, '  (1): IAFSqueeze(spike_threshold=1.0, min_v_mem=-1, batch_size=1, "*

 * *            "num_timesteps=-1)\\n'), (5, '  (4): IAFSqueeze(spike_threshold=1.0, min_v_mem=-1, "*

 * *            "batch_size=1, num_timesteps=-1)\\n'), (8, '  (7): IAFSqueeze(spike_threshold=1.0, "*

 * *            "min_v_mem=-1, batch_size=1, num_timesteps=-1)\\n'), (12, '  (11): "*

 * *            "IAFSqueeze(spike_threshold=1.0, […]*

```diff
@@ -30,14 +30,15 @@
                 "import warnings\n",
                 "\n",
                 "warnings.filterwarnings(\"ignore\")\n",
                 "\n",
                 "# - Import statements\n",
                 "import torch\n",
                 "import samna\n",
+                "import time\n",
                 "from tqdm.auto import tqdm\n",
                 "import numpy as np\n",
                 "import torch.nn as nn\n",
                 "from torchvision import datasets\n",
                 "import sinabs\n",
                 "from sinabs.from_torch import from_model\n",
                 "from sinabs.backend.dynapcnn import io\n",
@@ -195,34 +196,35 @@
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Sequential(\n",
                         "  (0): Conv2d(1, 20, kernel_size=(5, 5), stride=(1, 1), bias=False)\n",
-                        "  (1): IAFSqueeze(spike_threshold=1.0, min_v_mem=-1)\n",
+                        "  (1): IAFSqueeze(spike_threshold=1.0, min_v_mem=-1, batch_size=1, num_timesteps=-1)\n",
                         "  (2): AvgPool2d(kernel_size=2, stride=2, padding=0)\n",
                         "  (3): Conv2d(20, 32, kernel_size=(5, 5), stride=(1, 1), bias=False)\n",
-                        "  (4): IAFSqueeze(spike_threshold=1.0, min_v_mem=-1)\n",
+                        "  (4): IAFSqueeze(spike_threshold=1.0, min_v_mem=-1, batch_size=1, num_timesteps=-1)\n",
                         "  (5): AvgPool2d(kernel_size=2, stride=2, padding=0)\n",
                         "  (6): Conv2d(32, 128, kernel_size=(3, 3), stride=(1, 1), bias=False)\n",
-                        "  (7): IAFSqueeze(spike_threshold=1.0, min_v_mem=-1)\n",
+                        "  (7): IAFSqueeze(spike_threshold=1.0, min_v_mem=-1, batch_size=1, num_timesteps=-1)\n",
                         "  (8): AvgPool2d(kernel_size=2, stride=2, padding=0)\n",
                         "  (9): Flatten(start_dim=1, end_dim=-1)\n",
                         "  (10): Linear(in_features=128, out_features=500, bias=False)\n",
-                        "  (11): IAFSqueeze(spike_threshold=1.0, min_v_mem=-1)\n",
+                        "  (11): IAFSqueeze(spike_threshold=1.0, min_v_mem=-1, batch_size=1, num_timesteps=-1)\n",
                         "  (12): Linear(in_features=500, out_features=10, bias=False)\n",
-                        "  (Spiking output): IAFSqueeze(spike_threshold=1.0, min_v_mem=-1)\n",
+                        "  (spike_output): IAFSqueeze(spike_threshold=1.0, min_v_mem=-1, batch_size=1, num_timesteps=-1)\n",
                         ")\n",
-                        "-1\n"
+                        "Parameter containing:\n",
+                        "tensor(-1)\n"
                     ]
                 }
             ],
             "source": [
-                "sinabs_model = from_model(ann, add_spiking_output=True, min_v_mem=-1)\n",
+                "sinabs_model = from_model(ann, add_spiking_output=True, min_v_mem=-1, batch_size=1)\n",
                 "print(sinabs_model.spiking_model)\n",
                 "\n",
                 "print(sinabs_model.spiking_model[1].min_v_mem)"
             ]
         },
         {
             "cell_type": "markdown",
@@ -248,34 +250,34 @@
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "DynapcnnNetwork(\n",
                         "  (sequence): Sequential(\n",
                         "    (0): DynapcnnLayer(\n",
                         "      (conv_layer): Conv2d(1, 20, kernel_size=(5, 5), stride=(1, 1), bias=False)\n",
-                        "      (spk_layer): IAFSqueeze(spike_threshold=795.0, min_v_mem=-795.0)\n",
+                        "      (spk_layer): IAFSqueeze(spike_threshold=799.0, min_v_mem=-799.0, batch_size=1, num_timesteps=-1)\n",
                         "      (pool_layer): SumPool2d(norm_type=1, kernel_size=(2, 2), stride=None, ceil_mode=False)\n",
                         "    )\n",
                         "    (1): DynapcnnLayer(\n",
                         "      (conv_layer): Conv2d(20, 32, kernel_size=(5, 5), stride=(1, 1), bias=False)\n",
-                        "      (spk_layer): IAFSqueeze(spike_threshold=2122.0, min_v_mem=-2122.0)\n",
+                        "      (spk_layer): IAFSqueeze(spike_threshold=2396.0, min_v_mem=-2396.0, batch_size=1, num_timesteps=-1)\n",
                         "      (pool_layer): SumPool2d(norm_type=1, kernel_size=(2, 2), stride=None, ceil_mode=False)\n",
                         "    )\n",
                         "    (2): DynapcnnLayer(\n",
                         "      (conv_layer): Conv2d(32, 128, kernel_size=(3, 3), stride=(1, 1), bias=False)\n",
-                        "      (spk_layer): IAFSqueeze(spike_threshold=2366.0, min_v_mem=-2366.0)\n",
+                        "      (spk_layer): IAFSqueeze(spike_threshold=2260.0, min_v_mem=-2260.0, batch_size=1, num_timesteps=-1)\n",
                         "      (pool_layer): SumPool2d(norm_type=1, kernel_size=(2, 2), stride=None, ceil_mode=False)\n",
                         "    )\n",
                         "    (3): DynapcnnLayer(\n",
                         "      (conv_layer): Conv2d(128, 500, kernel_size=(1, 1), stride=(1, 1), bias=False)\n",
-                        "      (spk_layer): IAFSqueeze(spike_threshold=1613.0, min_v_mem=-1613.0)\n",
+                        "      (spk_layer): IAFSqueeze(spike_threshold=1518.0, min_v_mem=-1518.0, batch_size=1, num_timesteps=-1)\n",
                         "    )\n",
                         "    (4): DynapcnnLayer(\n",
                         "      (conv_layer): Conv2d(500, 10, kernel_size=(1, 1), stride=(1, 1), bias=False)\n",
-                        "      (spk_layer): IAFSqueeze(spike_threshold=1005.0, min_v_mem=-1005.0)\n",
+                        "      (spk_layer): IAFSqueeze(spike_threshold=1065.0, min_v_mem=-1065.0, batch_size=1, num_timesteps=-1)\n",
                         "    )\n",
                         "  )\n",
                         ")\n"
                     ]
                 }
             ],
             "source": [
@@ -301,19 +303,26 @@
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        " 99%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2589| 99/100 [00:38<00:00,  2.58it/s, acc=99]  \n"
-                    ]
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "5f6e92e5dd134bf69fa67755b4841247",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "  0%|          | 0/100 [00:00<?, ?it/s]"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "with torch.no_grad():\n",
                 "    correct = 0\n",
                 "    samples = 0\n",
                 "    # we will only use the first 100 samples to save some time\n",
@@ -406,40 +415,47 @@
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Network is valid\n"
                     ]
                 },
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "[2022-12-22 14:25:22.331] [Default] [warning] The write method of a model is DEPRECATED, please use BasicSourceNode to write events.\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/plain": [
                             "DynapcnnNetwork(\n",
                             "  (sequence): Sequential(\n",
                             "    (0): DynapcnnLayer(\n",
                             "      (conv_layer): Conv2d(1, 20, kernel_size=(5, 5), stride=(1, 1), bias=False)\n",
-                            "      (spk_layer): IAFSqueeze(spike_threshold=795.0, min_v_mem=-795.0)\n",
+                            "      (spk_layer): IAFSqueeze(spike_threshold=799.0, min_v_mem=-799.0, batch_size=1, num_timesteps=-1)\n",
                             "      (pool_layer): SumPool2d(norm_type=1, kernel_size=(2, 2), stride=None, ceil_mode=False)\n",
                             "    )\n",
                             "    (1): DynapcnnLayer(\n",
                             "      (conv_layer): Conv2d(20, 32, kernel_size=(5, 5), stride=(1, 1), bias=False)\n",
-                            "      (spk_layer): IAFSqueeze(spike_threshold=2122.0, min_v_mem=-2122.0)\n",
+                            "      (spk_layer): IAFSqueeze(spike_threshold=2396.0, min_v_mem=-2396.0, batch_size=1, num_timesteps=-1)\n",
                             "      (pool_layer): SumPool2d(norm_type=1, kernel_size=(2, 2), stride=None, ceil_mode=False)\n",
                             "    )\n",
                             "    (2): DynapcnnLayer(\n",
                             "      (conv_layer): Conv2d(32, 128, kernel_size=(3, 3), stride=(1, 1), bias=False)\n",
-                            "      (spk_layer): IAFSqueeze(spike_threshold=2366.0, min_v_mem=-2366.0)\n",
+                            "      (spk_layer): IAFSqueeze(spike_threshold=2260.0, min_v_mem=-2260.0, batch_size=1, num_timesteps=-1)\n",
                             "      (pool_layer): SumPool2d(norm_type=1, kernel_size=(2, 2), stride=None, ceil_mode=False)\n",
                             "    )\n",
                             "    (3): DynapcnnLayer(\n",
                             "      (conv_layer): Conv2d(128, 500, kernel_size=(1, 1), stride=(1, 1), bias=False)\n",
-                            "      (spk_layer): IAFSqueeze(spike_threshold=1613.0, min_v_mem=-1613.0)\n",
+                            "      (spk_layer): IAFSqueeze(spike_threshold=1518.0, min_v_mem=-1518.0, batch_size=1, num_timesteps=-1)\n",
                             "    )\n",
                             "    (4): DynapcnnLayer(\n",
                             "      (conv_layer): Conv2d(500, 10, kernel_size=(1, 1), stride=(1, 1), bias=False)\n",
-                            "      (spk_layer): IAFSqueeze(spike_threshold=1005.0, min_v_mem=-1005.0)\n",
+                            "      (spk_layer): IAFSqueeze(spike_threshold=1065.0, min_v_mem=-1065.0, batch_size=1, num_timesteps=-1)\n",
                             "    )\n",
                             "  )\n",
                             ")"
                         ]
                     },
                     "execution_count": 11,
                     "metadata": {},
@@ -593,36 +609,45 @@
         {
             "cell_type": "code",
             "execution_count": 16,
             "metadata": {},
             "outputs": [],
             "source": [
                 "dynapcnn_net.reset_states()\n",
+                "time.sleep(6.0)  # wait until the configuration take effect, this step is necessary when use a speck2edevkit!"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 17,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "events_out = dynapcnn_net(events_in)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We receive spike objects from the hardware as output. We expect them to be from the last layer of the model (chip_layers_ordering[-1]) and for the data we sent in, we expect most spikes to be from the neuron index equal to label. Let's convert those to a tensor/raster format for easy slicing. Since the last layer has dimensions (10, 1, 1) for (feature, y, x), we are interested in the feature value of the neuron."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "tensor([  3.,   0.,  53.,  37.,   0.,   0.,   0., 164.,   0.,  30.])"
+                            "tensor([  3.,   0.,  48.,  34.,   0.,   0.,   0., 152.,   0.,  28.])"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "output = factory.events_to_raster(events_out)\n",
                 "output.sum([0,2,3])"
@@ -633,24 +658,24 @@
             "metadata": {},
             "source": [
                 "We can see above that neuron 7 produced most spikes. Lets see what the original label of our data was."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "tensor(7)"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "label"
             ]
@@ -675,13 +700,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.5"
+            "version": "3.8.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/examples/mnist_dynapcnn.py` & `sinabs-dynapcnn-1.0.9.dev97/examples/mnist_dynapcnn.py`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/examples/mnist_params.pt` & `sinabs-dynapcnn-1.0.9.dev97/examples/mnist_params.pt`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/setup.cfg` & `sinabs-dynapcnn-1.0.9.dev97/setup.cfg`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/chip_factory.py` & `sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/chip_factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import torch
 import numpy as np
 from typing import List, Tuple, Optional
-from .utils import _parse_device_string
+from .utils import parse_device_id
 from .config_builder import ConfigBuilder
 from .chips import *
 
 
 class ChipFactory:
 
     supported_devices = {
         "dynapcnndevkit": DynapcnnConfigBuilder,
         "speck2b": Speck2BConfigBuilder,
-        "speck2btiny": Speck2BConfigBuilder, # It is the same chip, so doesn't require a separate builder
+        "speck2btiny": Speck2BConfigBuilder,  # It is the same chip, so doesn't require a separate builder
         "speck2cmini": Speck2CMiniConfigBuilder,
         "speck2dmini": Speck2DMiniConfigBuilder,
         "speck2e": Speck2EConfigBuilder,
         "speck2edevkit": Speck2EConfigBuilder,
     }
 
     device_name: str
@@ -25,22 +25,29 @@
         """
         Factory class to access config builder and other device specific methods
 
         Parameters
         ----------
         device_str
         """
-        self.device_name, self.device_id = _parse_device_string(device_str)
+        self.device_name, self.device_id = parse_device_id(device_str)
         if self.device_name not in self.supported_devices:
             raise Exception(f"Builder not found for device type: {self.device_name}")
 
     def get_config_builder(self) -> ConfigBuilder:
         return self.supported_devices[self.device_name]()
 
-    def raster_to_events(self, raster: torch.Tensor, layer, dt=1e-3, truncate: bool = False, delay_factor: float = 0) -> List:
+    def raster_to_events(
+        self,
+        raster: torch.Tensor,
+        layer,
+        dt=1e-3,
+        truncate: bool = False,
+        delay_factor: float = 0,
+    ) -> List:
         """
         Convert spike raster to events for DynapcnnNetworks
 
         Parameters
         ----------
 
         raster: torch.Tensor
@@ -61,14 +68,15 @@
 
         Returns
         -------
 
         events: List[Spike]
             A list of events that will be streamed to the device
         """
+        assert delay_factor >= 0.0, print("Delay factor cannot be a negative value!")
         samna_module = self.get_config_builder().get_samna_module()
         # Get the appropriate Spike class
         Spike = samna_module.event.Spike
         if truncate:
             t, ch, y, x = torch.where(raster)
             evData = torch.stack((t, ch, y, x), dim=0).T
         else:
@@ -84,19 +92,23 @@
         events = []
         for row in evData:
             ev = Spike()
             ev.layer = layer
             ev.x = row[3]
             ev.y = row[2]
             ev.feature = row[1]
-            ev.timestamp = int(row[0].item() * 1e6 * dt) + int(delay_factor * 1e6)  # Time in uS
+            ev.timestamp = int(
+                (row[0].item() * 1e6 * dt) + (delay_factor * 1e6)
+            )  # Time in uS
             events.append(ev)
         return events
 
-    def xytp_to_events(self, xytp: np.ndarray, layer, reset_timestamps, delay_factor: float = 0) -> List:
+    def xytp_to_events(
+        self, xytp: np.ndarray, layer, reset_timestamps, delay_factor: float = 0
+    ) -> List:
         """
         Convert series of spikes in a structured array (eg. from aermanager) to events for DynaapcnnDevKit
 
         Parameters
         ----------
 
         xytp: torch.Tensor
@@ -113,34 +125,44 @@
 
         Returns
         -------
 
         events: List[Spike]
             A list of events that will be streamed to the device
         """
+
+        # Check delay factor as it being negative will crash the method.
+        assert delay_factor >= 0, print("Delay factor cannot be a negative value!")
+
+        # Check the smallest timestamp is larger or equal to zero to prevent overflows.
+        tstart = xytp["t"].min()
+        assert tstart >= 0, print("Timestamps cannot be negative values!")
         samna_module = self.get_config_builder().get_samna_module()
         # Get the appropriate Spike class
         Spike = samna_module.event.Spike
 
         events = []
-        tstart = xytp["t"].min()
         for row in xytp:
             ev = Spike()
             ev.layer = layer
             ev.x = row["x"]
             ev.y = row["y"]
             ev.feature = row["p"]
             if reset_timestamps:
-                ev.timestamp = row["t"] - tstart + int(delay_factor * 1e6)# Time in uS
+                ev.timestamp = int(
+                    row["t"] - tstart + (delay_factor * 1e6)
+                )  # Time in uS
             else:
-                ev.timestamp = row["t"] + int(delay_factor * 1e6)
+                ev.timestamp = int(row["t"] + (delay_factor * 1e6))
             events.append(ev)
         return events
 
-    def events_to_raster(self, events: List, dt: float =1e-3, shape: Optional[Tuple]=None) -> torch.Tensor:
+    def events_to_raster(
+        self, events: List, dt: float = 1e-3, shape: Optional[Tuple] = None
+    ) -> torch.Tensor:
         """
         Convert events from DynapcnnNetworks to spike raster
 
         Parameters
         ----------
 
         events: List[Spike]
@@ -161,16 +183,25 @@
         timestamps = [ts - start_timestamp for ts in timestamps]
         xs = [event.x for event in events]
         ys = [event.y for event in events]
         features = [event.feature for event in events]
 
         # Initialize an empty raster
         if shape:
-            shape = (int(max(timestamps)*dt)+1, *shape)
+            shape = (int(max(timestamps) * dt) + 1, *shape)
             raster = torch.zeros(shape)
         else:
-            raster = torch.zeros(int(max(timestamps)*dt)+1, max(features)+1, max(xs)+1, max(ys)+1)
+            raster = torch.zeros(
+                int(max(timestamps) * dt) + 1,
+                max(features) + 1,
+                max(xs) + 1,
+                max(ys) + 1,
+            )
 
         for event in events:
-            raster[int((event.timestamp - start_timestamp)*dt), event.feature, event.x, event.y] += 1
+            raster[
+                int((event.timestamp - start_timestamp) * dt),
+                event.feature,
+                event.x,
+                event.y,
+            ] += 1
         return raster
-
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/chips/dynapcnn.py` & `sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/chips/dynapcnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,20 @@
-from subprocess import CalledProcessError
 import copy
-try:
-    import samna
-    from samna.dynapcnn.configuration import DynapcnnConfiguration
-except (ImportError, ModuleNotFoundError, CalledProcessError):
-    SAMNA_AVAILABLE = False
-else:
-    SAMNA_AVAILABLE = True
+from typing import List
 
+import samna
 import torch
-from typing import List
+from samna.dynapcnn.configuration import DynapcnnConfiguration
+
 import sinabs
 from sinabs.backend.dynapcnn.config_builder import ConfigBuilder
+from sinabs.backend.dynapcnn.dvs_layer import DVSLayer, expand_to_pair
+from sinabs.backend.dynapcnn.dynapcnn_layer import DynapcnnLayer
 from sinabs.backend.dynapcnn.mapping import LayerConstraints
 
-from sinabs.backend.dynapcnn.dvs_layer import DVSLayer
-from sinabs.backend.dynapcnn.dynapcnn_layer import DynapcnnLayer
-from sinabs.backend.dynapcnn.dvs_layer import expand_to_pair
 
 class DynapcnnConfigBuilder(ConfigBuilder):
 
     @classmethod
     def get_samna_module(cls):
         return samna.dynapcnn
 
@@ -275,14 +269,18 @@
             config.dvs_layer.monitor_enable = True
             monitor_layers.remove("dvs")
         for lyr_indx in monitor_layers:
             config.cnn_layers[lyr_indx].monitor_enable = True
         return config
 
     @classmethod
+    def get_input_buffer(cls):
+        return samna.BasicSourceNode_dynapcnn_event_input_event()
+
+    @classmethod
     def get_output_buffer(cls):
         return samna.BasicSinkNode_dynapcnn_event_output_event()
 
     @classmethod
     def reset_states(cls, config: DynapcnnConfiguration, randomize=False):
         for idx, lyr in enumerate(config.cnn_layers):
             shape = torch.tensor(lyr.neurons_initial_value).shape
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/chips/speck2.py` & `sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/chips/speck2b.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from subprocess import CalledProcessError
-try:
-    import samna
-    from samna.speck2.configuration import SpeckConfiguration
-except (ImportError, ModuleNotFoundError, CalledProcessError):
-    SAMNA_AVAILABLE = False
-else:
-    SAMNA_AVAILABLE = True
 
-from .dynapcnn import DynapcnnConfigBuilder
+import samna
+from samna.speck2b.configuration import SpeckConfiguration
 
+from .dynapcnn import DynapcnnConfigBuilder
 
 # Since most of the configuration is identical to DYNAP-CNN, we can simply inherit this class
 
-class Speck2ConfigBuilder(DynapcnnConfigBuilder):
+class Speck2BConfigBuilder(DynapcnnConfigBuilder):
 
     @classmethod
     def get_samna_module(cls):
-        return samna.speck2
+        return samna.speck2b
 
     @classmethod
     def get_default_config(cls) -> "SpeckConfiguration":
         return SpeckConfiguration()
+    
+    @classmethod
+    def get_input_buffer(cls):
+        return samna.BasicSourceNode_speck2b_event_input_event()
 
     @classmethod
     def get_output_buffer(cls):
-        return samna.BasicSinkNode_speck2_event_output_event()
+        return samna.BasicSinkNode_speck2b_event_output_event()
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/chips/speck2b.py` & `sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/chips/speck2dmini.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from subprocess import CalledProcessError
-try:
-    import samna
-    from samna.speck2b.configuration import SpeckConfiguration
-except (ImportError, ModuleNotFoundError, CalledProcessError):
-    SAMNA_AVAILABLE = False
-else:
-    SAMNA_AVAILABLE = True
-from .dynapcnn import DynapcnnConfigBuilder
+import samna
+from samna.speck2dMini.configuration import SpeckConfiguration
 
+from .speck2cmini import Speck2CMiniConfigBuilder
 
 # Since most of the configuration is identical to DYNAP-CNN, we can simply inherit this class
 
-class Speck2BConfigBuilder(DynapcnnConfigBuilder):
+class Speck2DMiniConfigBuilder(Speck2CMiniConfigBuilder):
 
     @classmethod
     def get_samna_module(cls):
-        return samna.speck2b
+        return samna.speck2dMini
 
     @classmethod
     def get_default_config(cls) -> "SpeckConfiguration":
         return SpeckConfiguration()
+    
+    @classmethod
+    def get_input_buffer(cls):
+        return samna.BasicSourceNode_speck2d_mini_event_input_event()
 
     @classmethod
     def get_output_buffer(cls):
-        return samna.BasicSinkNode_speck2b_event_output_event()
+        return samna.BasicSinkNode_speck2d_mini_event_output_event()
+
+
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/chips/speck2dmini.py` & `sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/chips/speck2e.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,34 @@
-from subprocess import CalledProcessError
-try:
-    import samna
-    from samna.speck2dMini.configuration import SpeckConfiguration
-except (ImportError, ModuleNotFoundError, CalledProcessError):
-    SAMNA_AVAILABLE = False
-else:
-    SAMNA_AVAILABLE = True
-from .speck2cmini import Speck2CMiniConfigBuilder
+import samna
+from samna.speck2e.configuration import SpeckConfiguration
 
+from sinabs.backend.dynapcnn.dynapcnn_layer import DynapcnnLayer
+
+from .dynapcnn import DynapcnnConfigBuilder
 
 # Since most of the configuration is identical to DYNAP-CNN, we can simply inherit this class
 
-class Speck2DMiniConfigBuilder(Speck2CMiniConfigBuilder):
 
+class Speck2EConfigBuilder(DynapcnnConfigBuilder):
     @classmethod
     def get_samna_module(cls):
-        return samna.speck2dMini
+        return samna.speck2e
 
     @classmethod
     def get_default_config(cls) -> "SpeckConfiguration":
         return SpeckConfiguration()
 
     @classmethod
-    def get_output_buffer(cls):
-        return samna.BasicSinkNode_speck2d_mini_event_output_event()
+    def get_input_buffer(cls):
+        return samna.BasicSourceNode_speck2e_event_speck2e_input_event()
 
+    @classmethod
+    def get_output_buffer(cls):
+        return samna.BasicSinkNode_speck2e_event_output_event()
 
+    @classmethod
+    def get_dynapcnn_layer_config_dict(cls, layer: DynapcnnLayer):
+        config_dict = super().get_dynapcnn_layer_config_dict(layer=layer)
+        config_dict.pop("weights_kill_bit")
+        config_dict.pop("biases_kill_bit")
+        config_dict.pop("neurons_value_kill_bit")
+        return config_dict
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/config_builder.py` & `sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/config_builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import samna
+import time
+
 from abc import ABC, abstractmethod
 from typing import List
 from .mapping import LayerConstraints, get_valid_mapping
 from .dvs_layer import DVSLayer
 
 class ConfigBuilder(ABC):
 
@@ -105,14 +108,23 @@
         is_valid, message = cls.get_samna_module().validate_configuration(config)
         if not is_valid:
             print(message)
         return is_valid
 
     @classmethod
     @abstractmethod
+    def get_input_buffer(cls):
+        """
+        Initialize and return the appropriate output buffer object
+        Note that this just the buffer object. This does not actually connect the buffer object to the graph.
+        (It is needed as of samna 0.21.0)
+        """
+    
+    @classmethod
+    @abstractmethod
     def get_output_buffer(cls):
         """
         Initialize and return the appropriate output buffer object
         Note that this just the buffer object. This does not actually connect the buffer object to the graph.
         """
 
     @classmethod
@@ -144,9 +156,17 @@
         events = []
         for i in range(layer_constraint.neuron_memory):
             event = mod.event.WriteNeuronValue()
             event.address = i
             event.layer = layer_id
             event.neuron_state = 0
             events.append(event)
-        samna_device.get_model().write(events)
+        
+        temporary_source_node = cls.get_input_buffer() 
+        temporary_graph = samna.graph.sequential([
+            temporary_source_node,
+            samna_device.get_model().get_sink_node()
+        ])
+        temporary_graph.start()
+        temporary_source_node.write(events)
+        temporary_graph.stop()
         return
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/crop2d.py` & `sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/crop2d.py`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/discretize.py` & `sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/discretize.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,20 +340,20 @@
     # Scale conv_weight, conv_bias and thresholds with common scaling factor and discretize
     if discr_conv:
         conv_weight.data = discretize_tensor(
             conv_weight, scaling, to_int=to_int
         ).float()
         conv_bias.data = discretize_tensor(conv_bias, scaling, to_int=to_int).float()
     if discr_spk:
-        spike_lyr.min_v_mem, spike_lyr.spike_threshold = (
-            discretize_tensor(thresholds, scaling, to_int=to_int)
-            .float()
-            .detach()
-            .numpy()
+        min_v_mem, spike_threshold = discretize_tensor(
+            thresholds, scaling, to_int=to_int
         )
+        spike_lyr.min_v_mem, spike_lyr.spike_threshold = nn.Parameter(
+            min_v_mem, requires_grad=False
+        ), nn.Parameter(spike_threshold, requires_grad=False)
         # Logic changes with use of activation functions
         # TODO: Add check for the activation function in use
         # if spike_lyr.membrane_subtract != spike_lyr.threshold:
         #    warn(
         #        "SpikingConv2dLayer: Subtraction of membrane potential is always by high threshold."
         #    )
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/dvs_layer.py` & `sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/dvs_layer.py`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/dynapcnn_layer.py` & `sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/dynapcnn_layer.py`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/dynapcnn_network.py` & `sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/dynapcnn_network.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 import time
 from subprocess import CalledProcessError
-from sinabs.backend.dynapcnn.chip_factory import ChipFactory
-from .exceptions import InputConfigurationError
-
-try:
-    import samna
-except (ImportError, ModuleNotFoundError, CalledProcessError):
-    SAMNA_AVAILABLE = False
-else:
-    # IO module only works if samna is available
-    from .io import (
-        open_device,
-        enable_timestamps,
-        disable_timestamps,
-        reset_timestamps,
-    )
-
-    SAMNA_AVAILABLE = True
+from typing import List, Optional, Sequence, Tuple, Union
 
+import samna
 import torch
 import torch.nn as nn
+
 import sinabs
-from typing import Tuple, Union, Optional, Sequence, List
-from .dynapcnn_layer import DynapcnnLayer
+from sinabs.backend.dynapcnn.chip_factory import ChipFactory
+
 from .dvs_layer import DVSLayer
-from .utils import convert_model_to_layer_list, build_from_list, infer_input_shape, _parse_device_string
+from .dynapcnn_layer import DynapcnnLayer
+from .exceptions import InputConfigurationError
+from .io import disable_timestamps, enable_timestamps, open_device, reset_timestamps
+from .utils import (
+    build_from_list,
+    convert_model_to_layer_list,
+    infer_input_shape,
+    parse_device_id,
+)
 
 
 class DynapcnnNetwork(nn.Module):
     """
     Given a sinabs spiking network, prepare a dynapcnn-compatible network.
     This can be used to test the network will be equivalent once on DYNAPCNN.
     This class also provides utilities to make the dynapcnn configuration and
@@ -87,32 +81,37 @@
         else:
             self.dvs_input = False
 
         input_shape = infer_input_shape(layers, input_shape=input_shape)
 
         if len(input_shape) != 3:
             raise InputConfigurationError(
-                f"input_shape expected to have length 3 or None but input_shape={input_shape} given.")
+                f"input_shape expected to have length 3 or None but input_shape={input_shape} given."
+            )
 
         # Build model from layers
         self.sequence = build_from_list(
             layers, in_shape=input_shape, discretize=discretize
         )
         # this holds the DynapcnnLayer objects which can be used for testing
         # and also deal with single-layer-level configuration issues
         self.compatible_layers = [*self.sequence]
 
         # Add a DVS layer in case dvs_input is flagged
-        if self.dvs_input and not isinstance(self.compatible_layers[0], DVSLayer):
+        if self.dvs_input:
             dvs_layer = DVSLayer(
                 input_shape=input_shape[1:]
             )  # Ignore the channel dimension
-            self.compatible_layers = [dvs_layer] + self.compatible_layers
+            if self.compatible_layers:
+                if not isinstance(self.compatible_layers[0], DVSLayer):
+                    self.compatible_layers = [dvs_layer] + self.compatible_layers
+            else:
+                # No layers initialized
+                self.compatible_layers = [dvs_layer]
             self.sequence = nn.Sequential(*self.compatible_layers)
-        
 
         if self.dvs_input:
             # Enable dvs pixels
             self.compatible_layers[0].disable_pixel_array = False
 
     def to(
         self,
@@ -152,41 +151,53 @@
         chip_layers_ordering and monitor_layers are used only when using synsense devices.
         For GPU or CPU usage these options are ignored.
         """
         self.device = device
         if isinstance(device, torch.device):
             return super().to(device)
         elif isinstance(device, str):
-            device_name, _ = _parse_device_string(device)
+            device_name, _ = parse_device_id(device)
             if device_name in ChipFactory.supported_devices:
                 # Generate config
                 config = self.make_config(
                     chip_layers_ordering=chip_layers_ordering,
                     device=device,
                     monitor_layers=monitor_layers,
                     config_modifier=config_modifier,
                 )
 
                 # Apply configuration to device
                 self.samna_device = open_device(device)
                 self.samna_device.get_model().apply_configuration(config)
                 time.sleep(1)
 
-                # Create output buffer sink node
                 builder = ChipFactory(device).get_config_builder()
+                # Create input source node
+                self.samna_input_buffer = builder.get_input_buffer()
+                # Create output sink node node
                 self.samna_output_buffer = builder.get_output_buffer()
 
-                # Connect buffer sink node to device
+                # Connect source node to device sink
+                self.device_input_graph = samna.graph.EventFilterGraph()
+                self.device_input_graph.sequential(
+                    [
+                        self.samna_input_buffer,
+                        self.samna_device.get_model().get_sink_node(),
+                    ]
+                )
+
+                # Connect sink node to device
                 self.device_output_graph = samna.graph.EventFilterGraph()
                 self.device_output_graph.sequential(
                     [
                         self.samna_device.get_model().get_source_node(),
-                        self.samna_output_buffer
+                        self.samna_output_buffer,
                     ]
                 )
+                self.device_input_graph.start()
                 self.device_output_graph.start()
                 self.samna_config = config
                 return self
             else:
                 return super().to(device)
         else:
             raise Exception("Unknown device description.")
@@ -235,51 +246,51 @@
 
         Raises
         ------
             ImportError
                 If samna is not available.
         """
 
-        if not SAMNA_AVAILABLE:
-            raise ImportError("`samna` does not appear to be installed.")
-
         config_builder = ChipFactory(device).get_config_builder()
 
         # Figure out layer ordering
         if chip_layers_ordering == "auto":
             chip_layers_ordering = config_builder.get_valid_mapping(self)
         else:
             # Truncate chip_layers_ordering just in case a longer list is passed
             if self.dvs_input:
-                chip_layers_ordering = chip_layers_ordering[: len(self.compatible_layers)-1]
+                chip_layers_ordering = chip_layers_ordering[
+                    : len(self.compatible_layers) - 1
+                ]
             chip_layers_ordering = chip_layers_ordering[: len(self.compatible_layers)]
 
         # Save the chip layers
         self.chip_layers_ordering = chip_layers_ordering
         # Update config
         config = config_builder.build_config(self, chip_layers_ordering)
         if self.input_shape and self.input_shape[0] == 1:
             config.dvs_layer.merge = True
         # Check if any monitoring is enabled and if not, enable monitoring for the last layer
         if monitor_layers is None:
             monitor_layers = [-1]
-        elif monitor_layers == 'all':
+        elif monitor_layers == "all":
             monitor_layers = list(range(len(self.compatible_layers)))
 
         # Enable monitors on the specified layers
         # Find layers corresponding to the chip
-        monitor_chip_layers = [self.find_chip_layer(lyr) for lyr in monitor_layers if lyr != "dvs"]
+        monitor_chip_layers = [
+            self.find_chip_layer(lyr) for lyr in monitor_layers if lyr != "dvs"
+        ]
         if "dvs" in monitor_layers:
             monitor_chip_layers.append("dvs")
         config_builder.monitor_layers(config, monitor_chip_layers)
 
         # Fix default factory setting to not return input events (UGLY!! Ideally this should happen in samna)
         # config.factory_settings.monitor_input_enable = False
 
-
         # Apply user config modifier
         if config_modifier is not None:
             config = config_modifier(config)
 
         # Validate config
         if config_builder.validate_configuration(config):
             print("Network is valid")
@@ -288,28 +299,33 @@
             raise ValueError(f"Generated config is not valid for {device}")
 
     def reset_states(self, randomize=False):
         """
         Reset the states of the network.
         """
         if hasattr(self, "device") and isinstance(self.device, str):
-            device_name, _ = _parse_device_string(self.device)
+            device_name, _ = parse_device_id(self.device)
             if device_name in ChipFactory.supported_devices:
                 config_builder = ChipFactory(self.device).get_config_builder()
                 # Set all the vmem states in the samna config to zero
                 config_builder.reset_states(self.samna_config, randomize=randomize)
                 self.samna_device.get_model().apply_configuration(self.samna_config)
                 # wait for the config to be written
                 time.sleep(1)
                 # Note: The below shouldn't be necessary ideally
                 # Erase all vmem memory
                 if not randomize:
-                    for lyr_idx in self.chip_layers_ordering:
-                        config_builder.set_all_v_mem_to_zeros(self.samna_device, lyr_idx)
-                        time.sleep(0.1)
+                    if hasattr(self, "samna_input_graph"):
+                        self.samna_input_graph.stop()
+                        for lyr_idx in self.chip_layers_ordering:
+                            config_builder.set_all_v_mem_to_zeros(
+                                self.samna_device, lyr_idx
+                            )
+                            time.sleep(0.1)
+                        self.samna_input_graph.start()
                 return
         for layer in self.compatible_layers:
             if isinstance(layer, DynapcnnLayer):
                 layer.spk_layer.reset_states(randomize=randomize)
 
     def find_chip_layer(self, layer_idx):
         """
@@ -330,29 +346,31 @@
             Index of the layer on the chip where the model layer is placed.
         """
         # Compute the expected number of cores
         num_cores_required = len(self.compatible_layers)
         if isinstance(self.compatible_layers[0], DVSLayer):
             num_cores_required -= 1
         if len(self.chip_layers_ordering) != num_cores_required:
-            raise Exception(f"Number of layers specified in chip_layers_ordering {self.chip_layers_ordering} does not correspond to the number of cores required for this model {num_cores_required}")
+            raise Exception(
+                f"Number of layers specified in chip_layers_ordering {self.chip_layers_ordering} does not correspond to the number of cores required for this model {num_cores_required}"
+            )
 
         return self.chip_layers_ordering[layer_idx]
 
     def forward(self, x):
         if (
             hasattr(self, "device")
-            and _parse_device_string(self.device)[0] in ChipFactory.supported_devices
+            and parse_device_id(self.device)[0] in ChipFactory.supported_devices
         ):
             _ = self.samna_output_buffer.get_events()  # Flush buffer
             # NOTE: The code to start and stop time stamping is device specific
             reset_timestamps(self.device)
             enable_timestamps(self.device)
             # Send input
-            self.samna_device.get_model().write(x)
+            self.samna_input_buffer.write(x)
             received_evts = []
             time.sleep(0.1)
             while True:
                 prev_length = len(received_evts)
                 time.sleep(0.1)
                 received_evts.extend(self.samna_output_buffer.get_events())
                 if prev_length == len(received_evts):
@@ -379,30 +397,38 @@
         summary.update({k: list() for k in self.sequence[0].memory_summary().keys()})
         for lyr in self.sequence:
             lyr_summary = lyr.memory_summary()
             for k, v in lyr_summary.items():
                 summary[k].append(v)
         return summary
 
-
     def zero_grad(self, set_to_none: bool = False) -> None:
         for lyr in self.sequence:
             lyr.zero_grad(set_to_none)
-    
+
     def __del__(self):
-        if hasattr(self, 'device_output_graph') and self.device_output_graph:
+        # Stop the input graph
+        if hasattr(self, "device_input_graph") and self.device_input_graph:
+            self.device_input_graph.stop()
+
+        # Stop the output graph.
+        if hasattr(self, "device_output_graph") and self.device_output_graph:
             self.device_output_graph.stop()
 
+
 class DynapcnnCompatibleNetwork(DynapcnnNetwork):
-    """ Deprecated class, use DynapcnnNetwork instead."""
+    """Deprecated class, use DynapcnnNetwork instead."""
 
     def __init__(
         self,
         snn: Union[nn.Sequential, sinabs.Network],
         input_shape: Optional[Tuple[int, int, int]] = None,
         dvs_input: bool = False,
         discretize: bool = True,
     ):
         from warnings import warn
-        warn("DynapcnnCompatibleNetwork has been renamed to DynapcnnNetwork " +
-             "and will be removed in a future release.")
+
+        warn(
+            "DynapcnnCompatibleNetwork has been renamed to DynapcnnNetwork "
+            + "and will be removed in a future release."
+        )
         super().__init__(snn, input_shape, dvs_input, discretize)
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/flipdims.py` & `sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/flipdims.py`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/io.py` & `sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,93 +1,98 @@
 import warnings
+from itertools import groupby
+from typing import Dict, List, Tuple
 
+import numpy as np
 import samna
 import torch
-from itertools import groupby
-from typing import List, Dict
-import numpy as np
-from .utils import _parse_device_string
+
+from .utils import parse_device_id, standardize_device_id
 
 # A map of all device types and their corresponding samna `device_name`
 device_types = {
     "speck": "speck",
     "speck2b": "Speck2bTestboard",
     "speck2devkit": "Speck2DevKit",
     "speck2btiny": "Speck2bDevKitTiny",
-    "speck2e": "Speck2eTestBoard", # with a capital B for board
+    "speck2e": "Speck2eTestBoard",  # with a capital B for board
     "speck2edevkit": "Speck2eDevKit",
     "dynapse1devkit": "Dynapse1DevKit",
     "davis346": "Davis 346",
     "davis240": "Davis 240",
     "dvxplorer": "DVXplorer",
     "pollendevkit": "PollenDevKit",
     "dynapcnndevkit": "DynapcnnDevKit",
     "dynapse2": "DYNAP-SE2 DevBoard",
     "dynapse2_stack": "DYNAP-SE2 Stack",
 }
 
 device_type_map = {v: k for (k, v) in device_types.items()}
 device_map = {}
 
+
 def enable_timestamps(
-        device_id: str,
+    device_id: str,
 ) -> None:
     """
     Disable timestamps of the samna node
 
     Args
     ----
     device_id: str
         Name of the device to initialize. Required for different existing APIs
         for Dynapcnndevkit and Speck chips
     """
-    device_name, device_idx = _parse_device_string(device_id)
+    device_id = standardize_device_id(device_id=device_id)
+    device_name, device_idx = parse_device_id(device_id)
     device_info = device_map[device_id]
     device_handle = samna.device.open_device(device_info)
     if device_name.lower() == "dynapcnndevkit":
         device_handle.get_io_module().write_config(0x0003, 1)
     else:
         device_handle.get_stop_watch().set_enable_value(True)
 
 
 def disable_timestamps(
-        device_id: str,
+    device_id: str,
 ) -> None:
     """
     Disable timestamps of the samna node
 
     Args
     ----
 
     device_id: str
         Name of the device to initialize. Required for different existing APIs
         for Dynapcnndevkit and Speck chips
     """
-    device_name, device_idx = _parse_device_string(device_id)
+    device_id = standardize_device_id(device_id=device_id)
+    device_name, device_idx = parse_device_id(device_id)
     device_info = device_map[device_id]
     device_handle = samna.device.open_device(device_info)
     if device_name.lower() == "dynapcnndevkit":
         device_handle.get_io_module().write_config(0x0003, 0)
     else:
         device_handle.get_stop_watch().set_enable_value(False)
 
 
 def reset_timestamps(
-        device_id: str,
+    device_id: str,
 ) -> None:
     """
     Disable timestamps of the samna node
 
     Args
     ----
     device_id: str
         Name of the device to initialize. Required for different existing APIs
         for Dynapcnndevkit and Speck chips
     """
-    device_name, device_idx = _parse_device_string(device_id)
+    device_id = standardize_device_id(device_id=device_id)
+    device_name, device_idx = parse_device_id(device_id)
     device_info = device_map[device_id]
     device_handle = samna.device.open_device(device_info)
     if device_name.lower() == "dynapcnndevkit":
         device_handle.get_io_module().write_config(0x0003, 1)
     else:
         device_handle.get_stop_watch().reset()
 
@@ -106,15 +111,17 @@
         The index of layer for which the data needs to be converted
 
     Returns
     -------
 
     raster: torch.Tensor
     """
-    evs_filtered = filter(lambda x: isinstance(x, samna.dynapcnn.event.Spike), event_list)
+    evs_filtered = filter(
+        lambda x: isinstance(x, samna.dynapcnn.event.Spike), event_list
+    )
     evs_filtered = filter(lambda x: x.layer == layer, evs_filtered)
     raise NotImplementedError
     raster = map(rasterize, evs_filtered)
     return raster
 
 
 def events_to_xytp(event_list: List, layer: int) -> np.array:
@@ -132,18 +139,28 @@
 
     Returns
     -------
 
     xytc: np.array
         A numpy structured array with columns `x`, `y`, `t`, `channel`.
     """
-    evs_filtered = list(filter(lambda x: isinstance(x, samna.dynapcnn.event.Spike) and x.layer == layer, event_list))
+    evs_filtered = list(
+        filter(
+            lambda x: isinstance(x, samna.dynapcnn.event.Spike) and x.layer == layer,
+            event_list,
+        )
+    )
     xytc = np.empty(
         len(evs_filtered),
-        dtype=[("x", np.uint16), ("y", np.uint16), ("t", np.uint64), ("channel", np.uint16)]
+        dtype=[
+            ("x", np.uint16),
+            ("y", np.uint16),
+            ("t", np.uint64),
+            ("channel", np.uint16),
+        ],
     )
 
     for i, event in enumerate(evs_filtered):
         xytc[i]["x"] = event.x
         xytc[i]["y"] = event.y
         xytc[i]["t"] = event.timestamp
         xytc[i]["channel"] = event.feature
@@ -154,23 +171,27 @@
     """
     Returns
     -------
 
         dict(str: samna.device.DeviceInfo)
         Returns a dict of device name and device identifier.
     """
+
     def sort_devices(devices: List) -> List:
         devices.sort(key=lambda x: x.usb_device_address)
         return devices
+
     # Get all devices available
     devices = samna.device.get_all_devices()
     # Group by device_type_name
     device_groups = groupby(devices, lambda x: x.device_type_name)
     # Switch keys from samna's device_type_name to device_type names
-    device_groups = {device_type_map[k]: sort_devices(list(v)) for k, v in device_groups}
+    device_groups = {
+        device_type_map[k]: sort_devices(list(v)) for k, v in device_groups
+    }
     # Flat map
     for dev_type, dev_list in device_groups.items():
         for i, dev in enumerate(dev_list):
             device_map[f"{dev_type}:{i}"] = dev
     return device_map
 
 
@@ -205,14 +226,15 @@
         The convention is similar to that of pytorch GPU identifier ie cuda:0 , cuda:1 etc.
 
     Returns
     -------
 
     device_info: samna.device.DeviceInfo
     """
+    device_id = standardize_device_id(device_id=device_id)
     device_info = device_map[device_id]
     return device_info
 
 
 def open_device(device_id: str):
     """
     Open device function.
@@ -225,18 +247,19 @@
 
     Returns
     -------
 
     device_handle: samna.device.*
         Device handle received from samna.
     """
+    device_id = standardize_device_id(device_id=device_id)
     device_map = get_device_map()
     device_info = device_map[device_id]
     device_handle = samna.device.open_device(device_info)
-    
+
     if device_handle is not None:
         return device_handle
     else:
         raise IOError("The connection to the device cannot be established.")
 
 
 def close_device(device_id: str):
@@ -246,13 +269,12 @@
     Args
     ----
 
     device_id: str
         device_name:device_id pair given as a string.
         dynapcnndevkit:0 or speck:0 or dynapcnndevkit:1
     """
+    device_id = standardize_device_id(device_id=device_id)
     device_info = device_map[device_id]
     device_handle = samna.device.open_device(device_info)
     print(f"Closing device: {device_id}")
     samna.device.close_device(device_handle)
-
-
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/mapping.py` & `sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/mapping.py`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/sinabs/backend/dynapcnn/utils.py` & `sinabs-dynapcnn-1.0.9.dev97/sinabs/backend/dynapcnn/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .dvs_layer import DVSLayer, expand_to_pair
 import sinabs.layers as sl
 from .exceptions import *
 from .flipdims import FlipDims
 
 
 def infer_input_shape(
-        layers: List[nn.Module], input_shape: Optional[Tuple[int, int, int]] = None
+    layers: List[nn.Module], input_shape: Optional[Tuple[int, int, int]] = None
 ) -> Tuple[int, int, int]:
     """
     Checks if the input_shape is specified.
     If either of them are specified, then it checks if the information is consistent and returns the input shape.
 
     Parameters
     ----------
@@ -27,22 +27,25 @@
 
     Returns
     -------
     Output shape:
         (channels, height, width)
     """
     if input_shape is not None and len(input_shape) != 3:
-        raise InputConfigurationError(f"input_shape expected to have length 3 or None but input_shape={input_shape} given.")
+        raise InputConfigurationError(
+            f"input_shape expected to have length 3 or None but input_shape={input_shape} given."
+        )
 
     input_shape_from_layer = None
-    if isinstance(layers[0], DVSLayer):
+    if layers and isinstance(layers[0], DVSLayer):
         input_shape_from_layer = layers[0].input_shape
         if len(input_shape_from_layer) != 3:
             raise InputConfigurationError(
-                f"input_shape of layer {layers[0]} expected to have length 3 or None but input_shape={input_shape_from_layer} found.")
+                f"input_shape of layer {layers[0]} expected to have length 3 or None but input_shape={input_shape_from_layer} found."
+            )
     if (input_shape is not None) and (input_shape_from_layer is not None):
         if input_shape == input_shape_from_layer:
             return input_shape
         else:
             raise InputConfigurationError(
                 f"Input shape from the layer {input_shape_from_layer} does not match the specified input_shape {input_shape}"
             )
@@ -51,15 +54,15 @@
     elif input_shape is not None:
         return input_shape
     else:
         raise InputConfigurationError("No input shape could be inferred")
 
 
 def convert_cropping2dlayer_to_crop2d(
-        layer: sl.Cropping2dLayer, input_shape: Tuple[int, int]
+    layer: sl.Cropping2dLayer, input_shape: Tuple[int, int]
 ) -> Crop2d:
     """
     Convert a sinabs layer of type Cropping2dLayer to Crop2d layer
 
     Parameters
     ----------
     layer:
@@ -77,16 +80,16 @@
     bottom = h - layer.bottom_crop
     right = w - layer.right_crop
     print(h, w, left, right, top, bottom, layer.right_crop, layer.bottom_crop)
     return Crop2d(((top, bottom), (left, right)))
 
 
 def construct_dvs_layer(
-        layers: List[nn.Module], input_shape: Tuple[int, int, int], idx_start=0
-) -> (Optional[DVSLayer], int, float):
+    layers: List[nn.Module], input_shape: Tuple[int, int, int], idx_start=0
+) -> Tuple[Optional[DVSLayer], int, float]:
     """
     Generate a DVSLayer given a list of layers
     NOTE: The number of channels is implicitly assumed to be 2 because of DVS
 
     Parameters
     ----------
     layers:
@@ -108,15 +111,17 @@
     """
     # Start with defaults
     layer_idx_next = idx_start
     crop_lyr = None
     flip_lyr = None
 
     if len(input_shape) != 3:
-        raise ValueError(f"Input shape should be 3 dimensional but input_shape={input_shape} was given.")
+        raise ValueError(
+            f"Input shape should be 3 dimensional but input_shape={input_shape} was given."
+        )
 
     # Return existing DVS layer as is
     if len(layers) and isinstance(layers[0], DVSLayer):
         return deepcopy(layers[0]), 1, 1
 
     # Construct pooling layer
     pool_lyr, layer_idx_next, rescale_factor = construct_next_pooling_layer(
@@ -194,16 +199,16 @@
     conv.weight.data = c_weight * factor[:, None, None, None]
     conv.bias.data = beta + (c_bias - mu) * factor
 
     return conv
 
 
 def construct_next_pooling_layer(
-        layers: List[nn.Module], idx_start: int
-) -> (Optional[sl.SumPool2d], int, float):
+    layers: List[nn.Module], idx_start: int
+) -> Tuple[Optional[sl.SumPool2d], int, float]:
     """
     Consolidate the first `AvgPool2d` objects in `layers` until the first object of different type.
 
     Parameters
     ----------
         layers: Sequence of layer objects
             Contains `AvgPool2d` and other objects.
@@ -259,20 +264,20 @@
         return None, idx_next, 1
     else:
         lyr_pool = sl.SumPool2d(cumulative_pooling)
         return lyr_pool, idx_next, rescale_factor
 
 
 def construct_next_dynapcnn_layer(
-        layers: List[nn.Module],
-        idx_start: int,
-        in_shape: (int, int, int),
-        discretize: bool,
-        rescale_factor: float = 1,
-) -> (DynapcnnLayer, int, float):
+    layers: List[nn.Module],
+    idx_start: int,
+    in_shape: Tuple[int, int, int],
+    discretize: bool,
+    rescale_factor: float = 1,
+) -> Tuple[DynapcnnLayer, int, float]:
     """
     Generate a DynapcnnLayer from a Conv2d layer and its subsequent spiking and
     pooling layers.
 
     Parameters
     ----------
 
@@ -349,15 +354,15 @@
         rescale_weights=rescale_factor,
     )
 
     return dynapcnn_layer, layer_idx_next, rescale_factor_after_pooling
 
 
 def build_from_list(
-        layers: List[nn.Module], in_shape, discretize=True
+    layers: List[nn.Module], in_shape, discretize=True
 ) -> nn.Sequential:
     """
     Build a sequential model of DVSLayer and DynapcnnLayer(s) given a list of layers comprising a spiking CNN.
 
     Parameters
     ----------
 
@@ -397,15 +402,15 @@
         in_shape = dynapcnn_layer.get_output_shape()
         compatible_layers.append(dynapcnn_layer)
 
     return nn.Sequential(*compatible_layers)
 
 
 def convert_model_to_layer_list(
-        model: Union[nn.Sequential, sinabs.Network]
+    model: Union[nn.Sequential, sinabs.Network]
 ) -> List[nn.Module]:
     """
     Convert a model to a list of layers.
 
     Parameters
     ----------
     model: nn.Sequential or sinabs.Network
@@ -419,23 +424,55 @@
     elif isinstance(model, nn.Sequential):
         layers = [*model]
     else:
         raise TypeError("Expected torch.nn.Sequential or sinabs.Network")
     return layers
 
 
-def _parse_device_string(device_id: str) -> (str, int):
-    """
-    Parse the device identifier
+def parse_device_id(device_id: str) -> Tuple[str, int]:
+    """Parse device id into device type and device index
+
     Args:
-        device_id: str
-            device_name:device_id pair given as a string
+        device_id (str): Device id typically of the form `device_type:index`.
+            In case no index is specified, the default index of zero is returned.
+
     Returns:
-        Tuple(str, int) = (device_name, device_id)
+        Tuple[str, int]: (device_type, index) Returns a tuple with the index and device type.
     """
-    device_splits = device_id.split(":")
-    device_name = device_splits[0]
-    if len(device_splits) > 1:
-        device_num = int(device_splits[1])
+    parts = device_id.split(sep=":")
+    if len(parts) == 1:
+        device_type = parts[0]
+        index = 0
+    elif len(parts) == 2:
+        device_type, index = parts
     else:
-        device_num = 0
-    return device_name, device_num
+        raise Exception(
+            "Device id not understood. A string of form `device_type:index` expected."
+        )
+
+    return device_type, int(index)
+
+
+def get_device_id(device_type: str, index: int) -> str:
+    """Generate a device id string given a device type and its index
+
+    Args:
+        device_type (str): Device type
+        index (int): Device index
+
+    Returns:
+        str: A string of the form `device_type:index`
+    """
+    return f"{device_type}:{index}"
+
+
+def standardize_device_id(device_id: str) -> str:
+    """Standardize device id string
+
+    Args:
+        device_id (str): Device id string. Could be of the form `device_type` or `device_type:index`
+
+    Returns:
+        str: Returns a sanitized device id of the form `device_type:index`
+    """
+    device_type, index = parse_device_id(device_id=device_id)
+    return get_device_id(device_type=device_type, index=index)
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/sinabs_dynapcnn.egg-info/PKG-INFO` & `sinabs-dynapcnn-1.0.9.dev97/sinabs_dynapcnn.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: sinabs-dynapcnn
-Version: 1.0.9.dev9
+Version: 1.0.9.dev97
 Summary: sinabs plugin for porting models to chips with DYNAP-CNN technology
 Home-page: UNKNOWN
 Author: SynSense
 Author-email: sinabs@synsense.ai
 License: GNU AGPLv3
 Project-URL: Source Code, https://gitlab.com/synsense/sinabs-dynapcnn
 Project-URL: Documentation, https://synsense.gitlab.io/sinabs-dynapcnn
 Description: sinabs-dynapcnn
         ===============
         
+        [![codecov](https://codecov.io/gl/synsense/sinabs-dynapcnn/branch/master/graph/badge.svg?token=TJJJBJTHWK)](https://codecov.io/gl/synsense/sinabs-dynapcnn)
+        
         This `sinabs` plugin enables porting sinabs models to chips and dev-kits with DYNAP-CNN technology.
         
         Documentation
         -------------
         
         You can find the latest documentation at [https://synsense.gitlab.io/sinabs-dynapcnn/](https://synsense.gitlab.io/sinabs-dynapcnn/)
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/tests/test_auto_mapping.py` & `sinabs-dynapcnn-1.0.9.dev97/tests/test_auto_mapping.py`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/tests/test_compatible_layer_build.py` & `sinabs-dynapcnn-1.0.9.dev97/tests/test_compatible_layer_build.py`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/tests/test_config_making.py` & `sinabs-dynapcnn-1.0.9.dev97/tests/test_config_making.py`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/tests/test_device_movement.py` & `sinabs-dynapcnn-1.0.9.dev97/tests/test_device_movement.py`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/tests/test_discover_device.py` & `sinabs-dynapcnn-1.0.9.dev97/tests/test_discover_device.py`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/tests/test_discretized.py` & `sinabs-dynapcnn-1.0.9.dev97/tests/test_discretized.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     assert (spk_lyr.v_mem == spk_copy.v_mem).all()
     assert (
         spk_lyr.spike_threshold == spk_copy.spike_threshold
     )
     assert spk_lyr.min_v_mem == spk_copy.min_v_mem
     # Make sure that elements are integers
     for obj in (conv_discr.weight, conv_discr.bias, spk_discr.v_mem):
-        assert torch.equal(obj, obj.int())
+        assert torch.equal(obj, obj.int().float())
     for obj in (
         spk_discr.spike_threshold,
         spk_discr.spike_threshold,
     ):
         # Does not work if this is a tensor
         assert obj == int(obj)
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/tests/test_doorbell.py` & `sinabs-dynapcnn-1.0.9.dev97/tests/test_doorbell.py`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/tests/test_dvs_input.py` & `sinabs-dynapcnn-1.0.9.dev97/tests/test_dvs_input.py`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/tests/test_dvs_layer.py` & `sinabs-dynapcnn-1.0.9.dev97/tests/test_dvs_layer.py`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/tests/test_individual_cases.py` & `sinabs-dynapcnn-1.0.9.dev97/tests/test_individual_cases.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,7 +216,18 @@
         IAFSqueeze(batch_size=1)
     )
 
     with pytest.raises(TypeError):
         DynapcnnNetwork(
             seq, input_shape=input_data.shape[1:], discretize=False
         )
+
+
+def test_no_conv_layers():
+    seq = nn.Sequential()
+
+    from sinabs.backend.dynapcnn.utils import infer_input_shape
+    from sinabs.backend.dynapcnn.dvs_layer import DVSLayer
+
+    net = DynapcnnNetwork(snn=seq, input_shape=(2, 10, 10), dvs_input=True)
+
+    assert isinstance(net.compatible_layers[0], DVSLayer)
```

### Comparing `sinabs-dynapcnn-1.0.9.dev9/tests/test_large_net.py` & `sinabs-dynapcnn-1.0.9.dev97/tests/test_large_net.py`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/tests/test_learning.py` & `sinabs-dynapcnn-1.0.9.dev97/tests/test_learning.py`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/tests/test_monitoring.py` & `sinabs-dynapcnn-1.0.9.dev97/tests/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `sinabs-dynapcnn-1.0.9.dev9/tests/test_speckmini_config_making.py` & `sinabs-dynapcnn-1.0.9.dev97/tests/test_speckmini_config_making.py`

 * *Files identical despite different names*

