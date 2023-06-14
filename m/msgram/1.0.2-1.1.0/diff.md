# Comparing `tmp/msgram-1.0.2.tar.gz` & `tmp/msgram-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgram-1.0.2.tar", last modified: Mon Feb  6 02:32:11 2023, max compression
+gzip compressed data, was "msgram-1.1.0.tar", last modified: Thu May 25 23:32:15 2023, max compression
```

## Comparing `msgram-1.0.2.tar` & `msgram-1.1.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 02:32:11.224518 msgram-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-02-06 02:31:52.000000 msgram-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    45026 2023-02-06 02:32:11.224518 msgram-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-02-06 02:31:52.000000 msgram-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 02:32:11.216518 msgram-1.0.2/msgram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45026 2023-02-06 02:32:11.000000 msgram-1.0.2/msgram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-02-06 02:32:11.000000 msgram-1.0.2/msgram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 02:32:11.000000 msgram-1.0.2/msgram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-06 02:32:11.000000 msgram-1.0.2/msgram.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-06 02:32:11.000000 msgram-1.0.2/msgram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-06 02:32:11.000000 msgram-1.0.2/msgram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-02-06 02:31:52.000000 msgram-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 02:32:11.224518 msgram-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 02:32:11.216518 msgram-1.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 02:31:52.000000 msgram-1.0.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 02:32:11.220518 msgram-1.0.2/src/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 02:32:11.220518 msgram-1.0.2/src/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/commands/cmd_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/commands/cmd_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/commands/cmd_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 02:32:11.220518 msgram-1.0.2/src/cli/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 02:32:11.220518 msgram-1.0.2/src/cli/jsonReader/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/jsonReader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/jsonReader/jsonReader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 02:32:11.220518 msgram-1.0.2/src/cli/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/resources/characteristic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/resources/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/resources/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/resources/sqc.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/resources/subcharacteristic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-02-06 02:31:52.000000 msgram-1.0.2/src/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 02:32:11.220518 msgram-1.0.2/src/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 02:31:52.000000 msgram-1.0.2/src/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-02-06 02:31:52.000000 msgram-1.0.2/src/config/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-02-06 02:31:52.000000 msgram-1.0.2/src/config/setup_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 02:32:11.220518 msgram-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 02:31:52.000000 msgram-1.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 02:32:11.220518 msgram-1.0.2/tests/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 02:31:52.000000 msgram-1.0.2/tests/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-02-06 02:31:52.000000 msgram-1.0.2/tests/system/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-02-06 02:31:52.000000 msgram-1.0.2/tests/system/test_help.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-06 02:31:52.000000 msgram-1.0.2/tests/system/test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 02:32:11.220518 msgram-1.0.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 02:31:52.000000 msgram-1.0.2/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 02:32:11.220518 msgram-1.0.2/tests/unit/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-02-06 02:31:52.000000 msgram-1.0.2/tests/unit/data/file_reader_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-02-06 02:31:52.000000 msgram-1.0.2/tests/unit/test_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-02-06 02:31:52.000000 msgram-1.0.2/tests/unit/test_characteristic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-02-06 02:31:52.000000 msgram-1.0.2/tests/unit/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-02-06 02:31:52.000000 msgram-1.0.2/tests/unit/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-02-06 02:31:52.000000 msgram-1.0.2/tests/unit/test_jsonReader.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-02-06 02:31:52.000000 msgram-1.0.2/tests/unit/test_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-02-06 02:31:52.000000 msgram-1.0.2/tests/unit/test_sqc.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-06 02:31:52.000000 msgram-1.0.2/tests/unit/test_subcharacteristic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:32:15.714201 msgram-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-05-25 23:31:58.000000 msgram-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    45026 2023-05-25 23:32:15.714201 msgram-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-25 23:31:58.000000 msgram-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:32:15.706200 msgram-1.1.0/msgram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45026 2023-05-25 23:32:15.000000 msgram-1.1.0/msgram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-25 23:32:15.000000 msgram-1.1.0/msgram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 23:32:15.000000 msgram-1.1.0/msgram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 23:32:15.000000 msgram-1.1.0/msgram.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-25 23:32:15.000000 msgram-1.1.0/msgram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 23:32:15.000000 msgram-1.1.0/msgram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-25 23:31:58.000000 msgram-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 23:32:15.714201 msgram-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:32:15.710201 msgram-1.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:31:58.000000 msgram-1.1.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:32:15.710201 msgram-1.1.0/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:32:15.710201 msgram-1.1.0/src/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/commands/cmd_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/commands/cmd_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/commands/cmd_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:32:15.710201 msgram-1.1.0/src/cli/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:32:15.710201 msgram-1.1.0/src/cli/jsonReader/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/jsonReader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/jsonReader/jsonReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:32:15.710201 msgram-1.1.0/src/cli/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/resources/characteristic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/resources/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/resources/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/resources/sqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/resources/subcharacteristic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-25 23:31:58.000000 msgram-1.1.0/src/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:32:15.710201 msgram-1.1.0/src/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:31:58.000000 msgram-1.1.0/src/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-25 23:31:58.000000 msgram-1.1.0/src/config/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-25 23:31:58.000000 msgram-1.1.0/src/config/setup_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:32:15.710201 msgram-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:31:58.000000 msgram-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:32:15.714201 msgram-1.1.0/tests/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:31:58.000000 msgram-1.1.0/tests/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-25 23:31:58.000000 msgram-1.1.0/tests/system/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-25 23:31:58.000000 msgram-1.1.0/tests/system/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-25 23:31:58.000000 msgram-1.1.0/tests/system/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:32:15.714201 msgram-1.1.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:31:58.000000 msgram-1.1.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:32:15.714201 msgram-1.1.0/tests/unit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-05-25 23:31:58.000000 msgram-1.1.0/tests/unit/data/file_reader_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-05-25 23:31:58.000000 msgram-1.1.0/tests/unit/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-25 23:31:58.000000 msgram-1.1.0/tests/unit/test_characteristic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-25 23:31:58.000000 msgram-1.1.0/tests/unit/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-25 23:31:58.000000 msgram-1.1.0/tests/unit/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-05-25 23:31:58.000000 msgram-1.1.0/tests/unit/test_jsonReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-25 23:31:58.000000 msgram-1.1.0/tests/unit/test_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-25 23:31:58.000000 msgram-1.1.0/tests/unit/test_sqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-25 23:31:58.000000 msgram-1.1.0/tests/unit/test_subcharacteristic.py
```

### Comparing `msgram-1.0.2/LICENSE` & `msgram-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/PKG-INFO` & `msgram-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram
-Version: 1.0.2
+Version: 1.1.0
 Summary: The msgram CLI is a command-line interface to use MeasureSoftGram software
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -672,29 +672,29 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# 2022-2-MeasureSoftGram-CLI
+# 2023-1-MeasureSoftGram-CLI
 
 ## Badges
 
-[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=bugs)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=duplicated_lines_density)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=sqale_index)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=coverage)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
+[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=bugs)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=duplicated_lines_density)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=sqale_index)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=coverage)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
 [![Downloads](https://pepy.tech/badge/msgram)](https://pepy.tech/project/msgram)
 [![Downloads](https://pepy.tech/badge/msgram/month)](https://pepy.tech/project/msgram)
 [![Downloads](https://pepy.tech/badge/msgram/week)](https://pepy.tech/project/msgram)
 
 [![PyPI](https://img.shields.io/pypi/v/msgram.svg)](https://pypi.python.org/pypi/msgram/)
 
 ## What is the MeasureSoftGram-CLI?
@@ -766,21 +766,21 @@
 
 ## License
 
 AGPL-3.0 License
 
 ## Documentation
 
-The documentation of this project can be accessed at this website: [Documentation](https://github.com/fga-eps-mds/2022-2-MeasureSoftGram-Doc).
+The documentation of this project can be accessed at this website: [Documentation](https://github.com/fga-eps-mds/2023-1-MeasureSoftGram-Doc).
 
 ## Contribute
 
 Do you want to contribute with our project? Access our [contribution guide](https://github.com/fga-eps-mds/2022-2-MeasureSoftGram-Doc/blob/main/docs/politicas/contribuindo.md) where we explain how you do it. 
 
 ## Another informations
 Our services are available on [Docker Hub](https://hub.docker.com/):
 - [Core](https://hub.docker.com/r/measuresoftgram/core)
 - [Service](https://hub.docker.com/r/measuresoftgram/service)
 
 ### Wiki
 For more informations, you can see our wiki:
-- [Wiki](https://fga-eps-mds.github.io/2022-2-MeasureSoftGram-Doc/)
+- [Wiki](https://fga-eps-mds.github.io/2023-1-MeasureSoftGram-Doc/)
```

### Comparing `msgram-1.0.2/README.md` & `msgram-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# 2022-2-MeasureSoftGram-CLI
+# 2023-1-MeasureSoftGram-CLI
 
 ## Badges
 
-[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=bugs)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=duplicated_lines_density)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=sqale_index)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=coverage)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
+[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=bugs)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=duplicated_lines_density)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=sqale_index)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=coverage)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
 [![Downloads](https://pepy.tech/badge/msgram)](https://pepy.tech/project/msgram)
 [![Downloads](https://pepy.tech/badge/msgram/month)](https://pepy.tech/project/msgram)
 [![Downloads](https://pepy.tech/badge/msgram/week)](https://pepy.tech/project/msgram)
 
 [![PyPI](https://img.shields.io/pypi/v/msgram.svg)](https://pypi.python.org/pypi/msgram/)
 
 ## What is the MeasureSoftGram-CLI?
@@ -88,21 +88,21 @@
 
 ## License
 
 AGPL-3.0 License
 
 ## Documentation
 
-The documentation of this project can be accessed at this website: [Documentation](https://github.com/fga-eps-mds/2022-2-MeasureSoftGram-Doc).
+The documentation of this project can be accessed at this website: [Documentation](https://github.com/fga-eps-mds/2023-1-MeasureSoftGram-Doc).
 
 ## Contribute
 
 Do you want to contribute with our project? Access our [contribution guide](https://github.com/fga-eps-mds/2022-2-MeasureSoftGram-Doc/blob/main/docs/politicas/contribuindo.md) where we explain how you do it. 
 
 ## Another informations
 Our services are available on [Docker Hub](https://hub.docker.com/):
 - [Core](https://hub.docker.com/r/measuresoftgram/core)
 - [Service](https://hub.docker.com/r/measuresoftgram/service)
 
 ### Wiki
 For more informations, you can see our wiki:
-- [Wiki](https://fga-eps-mds.github.io/2022-2-MeasureSoftGram-Doc/)
+- [Wiki](https://fga-eps-mds.github.io/2023-1-MeasureSoftGram-Doc/)
```

### Comparing `msgram-1.0.2/msgram.egg-info/PKG-INFO` & `msgram-1.1.0/msgram.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram
-Version: 1.0.2
+Version: 1.1.0
 Summary: The msgram CLI is a command-line interface to use MeasureSoftGram software
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -672,29 +672,29 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# 2022-2-MeasureSoftGram-CLI
+# 2023-1-MeasureSoftGram-CLI
 
 ## Badges
 
-[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=bugs)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=duplicated_lines_density)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=sqale_index)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=coverage)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
-[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-CLI&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-CLI)
+[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=bugs)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=duplicated_lines_density)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=sqale_index)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=coverage)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
+[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-CLI&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-CLI)
 [![Downloads](https://pepy.tech/badge/msgram)](https://pepy.tech/project/msgram)
 [![Downloads](https://pepy.tech/badge/msgram/month)](https://pepy.tech/project/msgram)
 [![Downloads](https://pepy.tech/badge/msgram/week)](https://pepy.tech/project/msgram)
 
 [![PyPI](https://img.shields.io/pypi/v/msgram.svg)](https://pypi.python.org/pypi/msgram/)
 
 ## What is the MeasureSoftGram-CLI?
@@ -766,21 +766,21 @@
 
 ## License
 
 AGPL-3.0 License
 
 ## Documentation
 
-The documentation of this project can be accessed at this website: [Documentation](https://github.com/fga-eps-mds/2022-2-MeasureSoftGram-Doc).
+The documentation of this project can be accessed at this website: [Documentation](https://github.com/fga-eps-mds/2023-1-MeasureSoftGram-Doc).
 
 ## Contribute
 
 Do you want to contribute with our project? Access our [contribution guide](https://github.com/fga-eps-mds/2022-2-MeasureSoftGram-Doc/blob/main/docs/politicas/contribuindo.md) where we explain how you do it. 
 
 ## Another informations
 Our services are available on [Docker Hub](https://hub.docker.com/):
 - [Core](https://hub.docker.com/r/measuresoftgram/core)
 - [Service](https://hub.docker.com/r/measuresoftgram/service)
 
 ### Wiki
 For more informations, you can see our wiki:
-- [Wiki](https://fga-eps-mds.github.io/2022-2-MeasureSoftGram-Doc/)
+- [Wiki](https://fga-eps-mds.github.io/2023-1-MeasureSoftGram-Doc/)
```

### Comparing `msgram-1.0.2/msgram.egg-info/SOURCES.txt` & `msgram-1.1.0/msgram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/pyproject.toml` & `msgram-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgram"
-version = "1.0.2"
+version = "1.1.0"
 description = "The msgram CLI is a command-line interface to use MeasureSoftGram software"
 readme = "README.md"
 authors = [
     { name = "MeasureSoftGram", email = "measuresoftgram@gmail.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `msgram-1.0.2/src/cli/cli.py` & `msgram-1.1.0/src/cli/cli.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/src/cli/commands/cmd_calculate.py` & `msgram-1.1.0/src/cli/commands/cmd_calculate.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         title="Done",
         menssage="> See our docs for more information: \n"
         " https://github.com/fga-eps-mds/2022-2-MeasureSoftGram-CLI",
     )
 
 
 def calculate_all(json_data, file_name, config):
-    data_measures, _ = calculate_measures(json_data)
+    data_measures, _ = calculate_measures(json_data, config)
 
     data_subcharacteristics, _ = calculate_subcharacteristics(
         config, data_measures["measures"]
     )
 
     data_characteristics, _ = calculate_characteristics(
         config, data_subcharacteristics["subcharacteristics"]
```

### Comparing `msgram-1.0.2/src/cli/commands/cmd_extract.py` & `msgram-1.1.0/src/cli/commands/cmd_extract.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/src/cli/commands/cmd_init.py` & `msgram-1.1.0/src/cli/commands/cmd_init.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/src/cli/exceptions/exceptions.py` & `msgram-1.1.0/src/cli/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/src/cli/jsonReader/jsonReader.py` & `msgram-1.1.0/src/cli/jsonReader/jsonReader.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/src/cli/parsers.py` & `msgram-1.1.0/src/cli/parsers.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/src/cli/resources/characteristic.py` & `msgram-1.1.0/src/cli/resources/characteristic.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/src/cli/resources/measure.py` & `msgram-1.1.0/src/cli/resources/measure.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,23 +19,23 @@
                 "weight": measure["weight"],
             }
         )
 
     return measures_calculated
 
 
-def calculate_measures(json_data):
+def calculate_measures(json_data, config: dict = {"thresholds": {}}):
     extracted = get_metric_value(json_data)
 
     calculate_infos = []
     for measures in SONARQUBE_SUPPORTED_MEASURES:
         calculate_infos.append(
             {
                 "key": list(measures.keys())[0],
                 "parameters": {
                     metric: extracted[metric] for metric in list(measures.values())[0]["metrics"]
                 },
             }
         )
 
     headers = ["Id", "Name", "Description", "Value", "Created at"]
-    return core_calculate({"measures": calculate_infos}), headers
+    return core_calculate({"measures": calculate_infos}, config), headers
```

### Comparing `msgram-1.0.2/src/cli/resources/metrics.py` & `msgram-1.1.0/src/cli/resources/metrics.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/src/cli/resources/subcharacteristic.py` & `msgram-1.1.0/src/cli/resources/subcharacteristic.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/src/cli/utils.py` & `msgram-1.1.0/src/cli/utils.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/src/config/setup_log.py` & `msgram-1.1.0/src/config/setup_log.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/tests/system/test_extract.py` & `msgram-1.1.0/tests/system/test_extract.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/tests/system/test_help.py` & `msgram-1.1.0/tests/system/test_help.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/tests/system/test_init.py` & `msgram-1.1.0/tests/system/test_init.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/tests/unit/data/file_reader_response.py` & `msgram-1.1.0/tests/unit/data/file_reader_response.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/tests/unit/test_calculate.py` & `msgram-1.1.0/tests/unit/test_calculate.py`

 * *Files 12% similar despite different names*

```diff
@@ -82,35 +82,33 @@
 
 def test_calculate_all_dict():
     file_name = "fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-05-2023-21-40-30-develop-extracted.msgram"
     json_data = open_json_file(Path(f"tests/unit/data/{file_name}"))
     config = open_json_file(Path('tests/unit/data/msgram.json'))
 
     calculated = calculate_all(json_data, file_name, config)
-
     assert calculated == {
         'repository': [{'key': 'repository', 'value': 'fga-eps-mds-2022-2-MeasureSoftGram-CLI'}],
         'version': [{'key': 'version', 'value': '01-05-2023-21-40'}],
         'measures': [
             {'key': 'passed_tests', 'value': 1.0},
-            {'key': 'test_builds', 'value': 0.9999969696180555},
-            {'key': 'test_coverage', 'value': 0.5153846153846154},
-            {'key': 'non_complex_file_density', 'value': 0.4829268292682926},
-            {'key': 'commented_file_density', 'value': 0.029230769230769227},
+            {'key': 'test_builds', 'value': pytest.approx(0.9999969696180555, 0.00000000000001)},
+            {'key': 'test_coverage', 'value': pytest.approx(0.5153846153846154, 0.00000000000001)},
+            {'key': 'non_complex_file_density', 'value': pytest.approx(0.3789488966318234, 0.00000000000001)},
+            {'key': 'commented_file_density', 'value': pytest.approx(0.029230769230769227, 0.00000000000001)},
             {'key': 'duplication_absense', 'value': 1.0}
         ],
         'subcharacteristics': [
-            {'key': 'testing_status', 'value': 0.8633460569923477},
-            {'key': 'modifiability', 'value': 0.650528195701257}
+            {'key': 'testing_status', 'value': pytest.approx(0.8633460569923477, 0.00000000000001)},
+            {'key': 'modifiability', 'value': pytest.approx(0.6276266582884098, 0.00000000000001)}
         ],
         'characteristics': [
-            {'key': 'reliability', 'value': 0.8633460569923477},
-            {'key': 'maintainability', 'value': 0.650528195701257}
-        ],
-        'sqc': [{'key': 'sqc', 'value': 0.7643799276297641}]
+            {'key': 'reliability', 'value': pytest.approx(0.8633460569923477, 0.00000000000001)},
+            {'key': 'maintainability', 'value': pytest.approx(0.6276266582884098, 0.00000000000001)}],
+        'sqc': [{'key': 'sqc', 'value': pytest.approx(0.754745532056504, 0.00000000000001)}]
     }
 
 
 def test_calculate_invalid_config_file():
     captured_output = StringIO()
     sys.stdout = captured_output
```

### Comparing `msgram-1.0.2/tests/unit/test_characteristic.py` & `msgram-1.1.0/tests/unit/test_characteristic.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/tests/unit/test_extract.py` & `msgram-1.1.0/tests/unit/test_extract.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/tests/unit/test_init.py` & `msgram-1.1.0/tests/unit/test_init.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/tests/unit/test_jsonReader.py` & `msgram-1.1.0/tests/unit/test_jsonReader.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/tests/unit/test_measures.py` & `msgram-1.1.0/tests/unit/test_measures.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 
 def test_calculate_measures():
     json_data = open_json_file(Path(
         'tests/unit/data/fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-05-2023-21-40-30-develop-extracted.msgram'))
 
     infos, headers = calculate_measures(json_data)
-
+    print(infos)
     assert headers == ["Id", "Name", "Description", "Value", "Created at"]
     assert infos == {'measures': [
         {'key': 'passed_tests', 'value': 1.0},
         {'key': 'test_builds', 'value': 0.9999969696180555},
         {'key': 'test_coverage', 'value': 0.5153846153846154},
-        {'key': 'non_complex_file_density', 'value': 0.4829268292682926},
+        {'key': 'non_complex_file_density', 'value': 0.3789488966318234},
         {'key': 'commented_file_density', 'value': 0.029230769230769227},
         {'key': 'duplication_absense', 'value': 1.0}
     ]}
```

### Comparing `msgram-1.0.2/tests/unit/test_sqc.py` & `msgram-1.1.0/tests/unit/test_sqc.py`

 * *Files identical despite different names*

### Comparing `msgram-1.0.2/tests/unit/test_subcharacteristic.py` & `msgram-1.1.0/tests/unit/test_subcharacteristic.py`

 * *Files identical despite different names*

