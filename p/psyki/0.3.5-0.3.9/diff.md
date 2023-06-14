# Comparing `tmp/psyki-0.3.5.tar.gz` & `tmp/psyki-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyki-0.3.5.tar", last modified: Mon Mar 20 15:10:03 2023, max compression
+gzip compressed data, was "psyki-0.3.9.tar", last modified: Thu Mar 23 16:58:36 2023, max compression
```

## Comparing `psyki-0.3.5.tar` & `psyki-0.3.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.008067 psyki-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-03-20 15:08:34.000000 psyki-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-20 15:08:34.000000 psyki-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-03-20 15:10:03.008067 psyki-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-03-20 15:08:34.000000 psyki-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-20 15:10:02.000000 psyki-0.3.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.000067 psyki-0.3.5/psyki/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-20 15:09:55.000000 psyki-0.3.5/psyki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.000067 psyki-0.3.5/psyki/fuzzifiers/
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/fuzzifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.000067 psyki-0.3.5/psyki/fuzzifiers/lukasciewicz/
--rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/fuzzifiers/lukasciewicz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.000067 psyki-0.3.5/psyki/fuzzifiers/netbuilder/
--rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/fuzzifiers/netbuilder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.000067 psyki-0.3.5/psyki/fuzzifiers/towell/
--rw-r--r--   0 runner    (1001) docker     (123)    16088 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/fuzzifiers/towell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.000067 psyki-0.3.5/psyki/logic/
--rw-r--r--   0 runner    (1001) docker     (123)    17386 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/logic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.000067 psyki-0.3.5/psyki/logic/operators/
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/logic/operators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.000067 psyki-0.3.5/psyki/logic/prolog/
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/logic/prolog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.004067 psyki-0.3.5/psyki/qos/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/qos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/qos/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/qos/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/qos/latency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/qos/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/qos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.004067 psyki-0.3.5/psyki/ski/
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/ski/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.004067 psyki-0.3.5/psyki/ski/kbann/
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/ski/kbann/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.004067 psyki-0.3.5/psyki/ski/kill/
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/ski/kill/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.004067 psyki-0.3.5/psyki/ski/kins/
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/ski/kins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.004067 psyki-0.3.5/psyki/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/utils/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.004067 psyki-0.3.5/psyki/utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/utils/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.004067 psyki-0.3.5/psyki/wiki/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/wiki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-20 15:08:34.000000 psyki-0.3.5/psyki/wiki/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.000067 psyki-0.3.5/psyki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-03-20 15:10:02.000000 psyki-0.3.5/psyki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-20 15:10:02.000000 psyki-0.3.5/psyki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 15:10:02.000000 psyki-0.3.5/psyki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 15:10:02.000000 psyki-0.3.5/psyki.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-20 15:10:02.000000 psyki-0.3.5/psyki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-20 15:10:02.000000 psyki-0.3.5/psyki.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-20 15:08:34.000000 psyki-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-20 15:08:34.000000 psyki-0.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 15:10:03.008067 psyki-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-03-20 15:08:34.000000 psyki-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:02.996067 psyki-0.3.5/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.004067 psyki-0.3.5/test/psyki/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-20 15:08:34.000000 psyki-0.3.5/test/psyki/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.004067 psyki-0.3.5/test/psyki/fuzzifiers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 15:08:34.000000 psyki-0.3.5/test/psyki/fuzzifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-03-20 15:08:34.000000 psyki-0.3.5/test/psyki/fuzzifiers/test_lukasiewicz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-03-20 15:08:34.000000 psyki-0.3.5/test/psyki/fuzzifiers/test_subnetwork_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-20 15:08:34.000000 psyki-0.3.5/test/psyki/fuzzifiers/test_towell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.008067 psyki-0.3.5/test/psyki/injectors/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-20 15:08:34.000000 psyki-0.3.5/test/psyki/injectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-03-20 15:08:34.000000 psyki-0.3.5/test/psyki/injectors/test_kbann.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-03-20 15:08:34.000000 psyki-0.3.5/test/psyki/injectors/test_kill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-20 15:08:34.000000 psyki-0.3.5/test/psyki/injectors/test_kins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.008067 psyki-0.3.5/test/psyki/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 15:08:34.000000 psyki-0.3.5/test/psyki/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-20 15:08:34.000000 psyki-0.3.5/test/psyki/logic/test_formula.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.008067 psyki-0.3.5/test/psyki/qos/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-20 15:08:34.000000 psyki-0.3.5/test/psyki/qos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-03-20 15:08:34.000000 psyki-0.3.5/test/psyki/qos/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-03-20 15:08:34.000000 psyki-0.3.5/test/psyki/qos/test_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-20 15:08:34.000000 psyki-0.3.5/test/psyki/qos/test_latency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-03-20 15:08:34.000000 psyki-0.3.5/test/psyki/qos/test_memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.008067 psyki-0.3.5/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 15:08:34.000000 psyki-0.3.5/test/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.008067 psyki-0.3.5/test/resources/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-03-20 15:08:34.000000 psyki-0.3.5/test/resources/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.008067 psyki-0.3.5/test/resources/knowledge/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-20 15:08:34.000000 psyki-0.3.5/test/resources/knowledge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:10:03.008067 psyki-0.3.5/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-03-20 15:08:34.000000 psyki-0.3.5/test/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.309127 psyki-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-03-23 16:56:56.000000 psyki-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-23 16:56:56.000000 psyki-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-03-23 16:58:36.309127 psyki-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-03-23 16:56:56.000000 psyki-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-23 16:58:36.000000 psyki-0.3.9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.297127 psyki-0.3.9/psyki/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-23 16:58:25.000000 psyki-0.3.9/psyki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.297127 psyki-0.3.9/psyki/fuzzifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/fuzzifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.297127 psyki-0.3.9/psyki/fuzzifiers/lukasciewicz/
+-rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/fuzzifiers/lukasciewicz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.301127 psyki-0.3.9/psyki/fuzzifiers/netbuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/fuzzifiers/netbuilder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.301127 psyki-0.3.9/psyki/fuzzifiers/towell/
+-rw-r--r--   0 runner    (1001) docker     (123)    16088 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/fuzzifiers/towell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.301127 psyki-0.3.9/psyki/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)    17373 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/logic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.301127 psyki-0.3.9/psyki/logic/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/logic/operators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.301127 psyki-0.3.9/psyki/logic/prolog/
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/logic/prolog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.301127 psyki-0.3.9/psyki/qos/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/qos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/qos/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/qos/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/qos/latency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/qos/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/qos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.301127 psyki-0.3.9/psyki/ski/
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/ski/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.301127 psyki-0.3.9/psyki/ski/kbann/
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/ski/kbann/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.301127 psyki-0.3.9/psyki/ski/kill/
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/ski/kill/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.301127 psyki-0.3.9/psyki/ski/kins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/ski/kins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.301127 psyki-0.3.9/psyki/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/utils/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.301127 psyki-0.3.9/psyki/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/utils/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.305127 psyki-0.3.9/psyki/wiki/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/wiki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-23 16:56:56.000000 psyki-0.3.9/psyki/wiki/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.297127 psyki-0.3.9/psyki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-03-23 16:58:36.000000 psyki-0.3.9/psyki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-23 16:58:36.000000 psyki-0.3.9/psyki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 16:58:36.000000 psyki-0.3.9/psyki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 16:58:36.000000 psyki-0.3.9/psyki.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-23 16:58:36.000000 psyki-0.3.9/psyki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-23 16:58:36.000000 psyki-0.3.9/psyki.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-23 16:56:56.000000 psyki-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-23 16:56:56.000000 psyki-0.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 16:58:36.309127 psyki-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-03-23 16:56:56.000000 psyki-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.297127 psyki-0.3.9/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.305127 psyki-0.3.9/test/psyki/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:56:56.000000 psyki-0.3.9/test/psyki/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.305127 psyki-0.3.9/test/psyki/fuzzifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:56:56.000000 psyki-0.3.9/test/psyki/fuzzifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-03-23 16:56:56.000000 psyki-0.3.9/test/psyki/fuzzifiers/test_lukasiewicz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-03-23 16:56:56.000000 psyki-0.3.9/test/psyki/fuzzifiers/test_subnetwork_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-23 16:56:56.000000 psyki-0.3.9/test/psyki/fuzzifiers/test_towell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.305127 psyki-0.3.9/test/psyki/injectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-23 16:56:56.000000 psyki-0.3.9/test/psyki/injectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-03-23 16:56:56.000000 psyki-0.3.9/test/psyki/injectors/test_kbann.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-03-23 16:56:56.000000 psyki-0.3.9/test/psyki/injectors/test_kill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-23 16:56:56.000000 psyki-0.3.9/test/psyki/injectors/test_kins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.305127 psyki-0.3.9/test/psyki/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:56:56.000000 psyki-0.3.9/test/psyki/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-23 16:56:56.000000 psyki-0.3.9/test/psyki/logic/test_formula.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.305127 psyki-0.3.9/test/psyki/qos/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-23 16:56:56.000000 psyki-0.3.9/test/psyki/qos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-03-23 16:56:56.000000 psyki-0.3.9/test/psyki/qos/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-03-23 16:56:56.000000 psyki-0.3.9/test/psyki/qos/test_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-23 16:56:56.000000 psyki-0.3.9/test/psyki/qos/test_latency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-03-23 16:56:56.000000 psyki-0.3.9/test/psyki/qos/test_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.305127 psyki-0.3.9/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:56:56.000000 psyki-0.3.9/test/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.305127 psyki-0.3.9/test/resources/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-03-23 16:56:56.000000 psyki-0.3.9/test/resources/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.309127 psyki-0.3.9/test/resources/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-23 16:56:56.000000 psyki-0.3.9/test/resources/knowledge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:58:36.309127 psyki-0.3.9/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-03-23 16:56:56.000000 psyki-0.3.9/test/utils/__init__.py
```

### Comparing `psyki-0.3.5/LICENSE` & `psyki-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/PKG-INFO` & `psyki-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyki
-Version: 0.3.5
+Version: 0.3.9
 Summary: Python-based implementation of PSyKI, i.e. a Platform for Symbolic Knowledge Injection
 Home-page: https://github.com/psykei/psyki-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyki-python/issues
 Project-URL: Source, https://github.com/psykei/psyki-python
```

### Comparing `psyki-0.3.5/README.md` & `psyki-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/_logging.py` & `psyki-0.3.9/psyki/_logging.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/fuzzifiers/__init__.py` & `psyki-0.3.9/psyki/fuzzifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/fuzzifiers/lukasciewicz/__init__.py` & `psyki-0.3.9/psyki/fuzzifiers/lukasciewicz/__init__.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/fuzzifiers/netbuilder/__init__.py` & `psyki-0.3.9/psyki/fuzzifiers/netbuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/fuzzifiers/towell/__init__.py` & `psyki-0.3.9/psyki/fuzzifiers/towell/__init__.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/logic/__init__.py` & `psyki-0.3.9/psyki/logic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,22 +44,22 @@
         """
         @param knowledge: list of logic knowledge that represents the prior knowledge to be injected.
                           Or a string that represents a path to a file containing the knowledge.
                           Or a string that represents the knowledge itself.
         @param dataset: dataset containing the domain data.
         @param class_mapping: optional, mapping between class names and class indices.
         """
+        from psyki.logic.prolog import TuProlog
+
         if isinstance(knowledge, str):
             if Path(knowledge).exists():
-                self.formulae: list[Formula] = KnowledgeAdapter.from_file(knowledge)
+                self.formulae: list[Formula] = TuProlog.from_file(knowledge)
             else:
                 try:
-                    self.formulae: list[Formula] = KnowledgeAdapter.from_string(
-                        knowledge
-                    )
+                    self.formulae: list[Formula] = TuProlog.from_string(knowledge)
                 except Exception as e:
                     raise KnowledgeException.not_parsable(knowledge, e)
         else:
             self.formulae: list[Formula] = knowledge
         self.feature_mapping: dict[str, int] = {
             f: i for i, f in enumerate(dataset.columns[:-1])
         }
```

### Comparing `psyki-0.3.5/psyki/logic/operators/__init__.py` & `psyki-0.3.9/psyki/logic/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/logic/prolog/__init__.py` & `psyki-0.3.9/psyki/logic/prolog/__init__.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/qos/__init__.py` & `psyki-0.3.9/psyki/qos/__init__.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/qos/data.py` & `psyki-0.3.9/psyki/qos/data.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/qos/energy.py` & `psyki-0.3.9/psyki/qos/energy.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/qos/latency.py` & `psyki-0.3.9/psyki/qos/latency.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/qos/memory.py` & `psyki-0.3.9/psyki/qos/memory.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/qos/utils.py` & `psyki-0.3.9/psyki/qos/utils.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/ski/__init__.py` & `psyki-0.3.9/psyki/ski/__init__.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/ski/kbann/__init__.py` & `psyki-0.3.9/psyki/ski/kbann/__init__.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/ski/kill/__init__.py` & `psyki-0.3.9/psyki/ski/kill/__init__.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/ski/kins/__init__.py` & `psyki-0.3.9/psyki/ski/kins/__init__.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/utils/__init__.py` & `psyki-0.3.9/psyki/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/utils/exceptions/__init__.py` & `psyki-0.3.9/psyki/utils/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki/wiki/__main__.py` & `psyki-0.3.9/psyki/wiki/__main__.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/psyki.egg-info/PKG-INFO` & `psyki-0.3.9/psyki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyki
-Version: 0.3.5
+Version: 0.3.9
 Summary: Python-based implementation of PSyKI, i.e. a Platform for Symbolic Knowledge Injection
 Home-page: https://github.com/psykei/psyki-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyki-python/issues
 Project-URL: Source, https://github.com/psykei/psyki-python
```

### Comparing `psyki-0.3.5/psyki.egg-info/SOURCES.txt` & `psyki-0.3.9/psyki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/setup.py` & `psyki-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,17 @@
     ],
     keywords='symbolic knowledge injection, ski, symbolic ai',  # Optional
     # package_dir={'': 'src'},  # Optional
     packages=find_packages(),  # Required
     include_package_data=True,
     python_requires='>=3.9.0, <3.10',
     install_requires=[
-        'tensorflow>=2.7.0',
+        'tensorflow>=2.7.0,<2.12.0',
         'numpy>=1.22.3',
+        '2ppy>=0.4.0',
         'scikit-learn>=1.0.2',
         'pandas>=1.4.2',
         'codecarbon>=2.1.4'
     ],  # Optional
     zip_safe = False,
     platforms = "Independant",
     project_urls={  # Optional
```

### Comparing `psyki-0.3.5/test/psyki/fuzzifiers/test_lukasiewicz.py` & `psyki-0.3.9/test/psyki/fuzzifiers/test_lukasiewicz.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/test/psyki/fuzzifiers/test_subnetwork_builder.py` & `psyki-0.3.9/test/psyki/fuzzifiers/test_subnetwork_builder.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/test/psyki/fuzzifiers/test_towell.py` & `psyki-0.3.9/test/psyki/fuzzifiers/test_towell.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/test/psyki/injectors/test_kbann.py` & `psyki-0.3.9/test/psyki/injectors/test_kbann.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/test/psyki/injectors/test_kill.py` & `psyki-0.3.9/test/psyki/injectors/test_kill.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,24 @@
 from tensorflow.keras.losses import SparseCategoricalCrossentropy
 from tensorflow.python.framework.random_seed import set_seed
 from psyki.logic import Theory
 from psyki.ski import Injector
 from psyki.ski.kill import KILL
 from test.resources.data import SpliceJunction, Poker
 from test.utils import get_mlp, Conditions
+from test.resources.knowledge import PATH as KNOWLEDGE_PATH
 
 
 class TestKillOnSpliceJunction(unittest.TestCase):
     epochs = 100
     batch_size = 32
     verbose = 0
     acceptable_accuracy = 0.9
-    knowledge = SpliceJunction.get_knowledge()
-    for k in knowledge:
-        k.trainable = True
-        k.optimize()
     dataset = SpliceJunction.get_train()
-    theory = Theory(knowledge, dataset, SpliceJunction.class_mapping)
+    theory = Theory(str(KNOWLEDGE_PATH / SpliceJunction.knowledge_filename), dataset, SpliceJunction.class_mapping)
 
     def test_on_dataset(self):
         set_seed(0)
         # Split data
         train, test = train_test_split(self.dataset, train_size=1000, random_state=0, stratify=self.dataset.iloc[:, -1])
         train_x, train_y = train.iloc[:, :-1], train.iloc[:, -1:]
         test_x, test_y = test.iloc[:, :-1], test.iloc[:, -1:]
```

### Comparing `psyki-0.3.5/test/psyki/injectors/test_kins.py` & `psyki-0.3.9/test/psyki/injectors/test_kins.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/test/psyki/logic/test_formula.py` & `psyki-0.3.9/test/psyki/logic/test_formula.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/test/psyki/qos/__init__.py` & `psyki-0.3.9/test/psyki/qos/__init__.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/test/psyki/qos/test_data.py` & `psyki-0.3.9/test/psyki/qos/test_data.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/test/psyki/qos/test_energy.py` & `psyki-0.3.9/test/psyki/qos/test_energy.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/test/psyki/qos/test_latency.py` & `psyki-0.3.9/test/psyki/qos/test_latency.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/test/psyki/qos/test_memory.py` & `psyki-0.3.9/test/psyki/qos/test_memory.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/test/resources/data/__init__.py` & `psyki-0.3.9/test/resources/data/__init__.py`

 * *Files identical despite different names*

### Comparing `psyki-0.3.5/test/utils/__init__.py` & `psyki-0.3.9/test/utils/__init__.py`

 * *Files identical despite different names*

