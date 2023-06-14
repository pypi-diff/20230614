# Comparing `tmp/quao-0.2.1.tar.gz` & `tmp/quao-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.2.1.tar", last modified: Tue Jun 13 10:13:32 2023, max compression
+gzip compressed data, was "quao-0.2.2.tar", last modified: Wed Jun 14 09:44:35 2023, max compression
```

## Comparing `quao-0.2.1.tar` & `quao-0.2.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.807749 quao-0.2.1/
--rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-06-13 10:13:32.806750 quao-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.2.1/README.md
--rw-rw-rw-   0        0        0      916 2023-06-13 10:09:48.000000 quao-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 10:13:32.807749 quao-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.674815 quao-0.2.1/src/
--rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.676769 quao-0.2.1/src/quao/
--rw-rw-rw-   0        0        0      203 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/__init__.py
--rw-rw-rw-   0        0        0     5614 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/backend.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.712614 quao-0.2.1/src/quao/config/
--rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/config/__init__.py
--rw-rw-rw-   0        0        0      190 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/config/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.714715 quao-0.2.1/src/quao/data/
--rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.716603 quao-0.2.1/src/quao/data/job/
--rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/data/job/__init__.py
--rw-rw-rw-   0        0        0      801 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/data/job/job_response.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.726764 quao-0.2.1/src/quao/data/request/
--rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/data/request/__init__.py
--rw-rw-rw-   0        0        0      566 2023-06-01 02:42:52.000000 quao-0.2.1/src/quao/data/request/request_data.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.769379 quao-0.2.1/src/quao/enum/
--rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/enum/__init__.py
--rw-rw-rw-   0        0        0      212 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/enum/http_status.py
--rw-rw-rw-   0        0        0      213 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/enum/job_status.py
--rw-rw-rw-   0        0        0      258 2023-06-01 02:42:52.000000 quao-0.2.1/src/quao/enum/media_type.py
--rw-rw-rw-   0        0        0      205 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/enum/processing_unit.py
--rw-rw-rw-   0        0        0      297 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/enum/provider_type.py
--rw-rw-rw-   0        0        0      179 2023-06-01 02:42:52.000000 quao-0.2.1/src/quao/enum/sdk.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.775210 quao-0.2.1/src/quao/factory/
--rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.1/src/quao/factory/__init__.py
--rw-rw-rw-   0        0        0     1555 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/factory/device_factory.py
--rw-rw-rw-   0        0        0     1351 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/factory/provider_factory.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.777226 quao-0.2.1/src/quao/model/
--rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.1/src/quao/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.789781 quao-0.2.1/src/quao/model/device/
--rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.1/src/quao/model/device/__init__.py
--rw-rw-rw-   0        0        0     1540 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/device/aws_braket_device.py
--rw-rw-rw-   0        0        0     3144 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/device/device.py
--rw-rw-rw-   0        0        0     1014 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/device/ibm_cloud_device.py
--rw-rw-rw-   0        0        0      794 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/device/ibm_quantum_device.py
--rw-rw-rw-   0        0        0      778 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/device/qiskit_device.py
--rw-rw-rw-   0        0        0     2513 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/device/quao_device.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.792457 quao-0.2.1/src/quao/model/job/
--rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.1/src/quao/model/job/__init__.py
--rw-rw-rw-   0        0        0     2693 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/job/qiskit_status.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.801349 quao-0.2.1/src/quao/model/provider/
--rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.1/src/quao/model/provider/__init__.py
--rw-rw-rw-   0        0        0     1257 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/provider/aws_braket_provider.py
--rw-rw-rw-   0        0        0     1010 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/provider/ibm_cloud_provider.py
--rw-rw-rw-   0        0        0      880 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/provider/ibm_quantum_provider.py
--rw-rw-rw-   0        0        0      589 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/provider/provider.py
--rw-rw-rw-   0        0        0     1519 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/provider/quao_provider.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.805750 quao-0.2.1/src/quao/util/
--rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/util/__init__.py
--rw-rw-rw-   0        0        0     2047 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/util/json_parser_util.py
--rw-rw-rw-   0        0        0     1288 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/util/response_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.704082 quao-0.2.1/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-06-13 10:13:32.000000 quao-0.2.1/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1480 2023-06-13 10:13:32.000000 quao-0.2.1/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 10:13:32.000000 quao-0.2.1/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      166 2023-06-13 10:13:32.000000 quao-0.2.1/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-13 10:13:32.000000 quao-0.2.1/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 09:44:35.018784 quao-0.2.2/
+-rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-06-14 09:44:35.017784 quao-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.2.2/README.md
+-rw-rw-rw-   0        0        0      916 2023-06-14 09:43:50.000000 quao-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 09:44:35.018784 quao-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 09:44:34.949785 quao-0.2.2/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:44:34.951789 quao-0.2.2/src/quao/
+-rw-rw-rw-   0        0        0      203 2023-06-14 09:11:58.000000 quao-0.2.2/src/quao/__init__.py
+-rw-rw-rw-   0        0        0     5614 2023-06-09 04:02:10.000000 quao-0.2.2/src/quao/backend.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:44:34.961786 quao-0.2.2/src/quao/config/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.2/src/quao/config/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-06-02 01:59:38.000000 quao-0.2.2/src/quao/config/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:44:34.962784 quao-0.2.2/src/quao/data/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.2/src/quao/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:44:34.965784 quao-0.2.2/src/quao/data/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.2/src/quao/data/job/__init__.py
+-rw-rw-rw-   0        0        0      801 2023-06-02 10:41:04.000000 quao-0.2.2/src/quao/data/job/job_response.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:44:34.968789 quao-0.2.2/src/quao/data/request/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.2/src/quao/data/request/__init__.py
+-rw-rw-rw-   0        0        0      566 2023-06-02 01:59:38.000000 quao-0.2.2/src/quao/data/request/request_data.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:44:34.979786 quao-0.2.2/src/quao/enum/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.2/src/quao/enum/__init__.py
+-rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.2.2/src/quao/enum/http_status.py
+-rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.2.2/src/quao/enum/job_status.py
+-rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.2.2/src/quao/enum/media_type.py
+-rw-rw-rw-   0        0        0      205 2023-06-13 03:37:41.000000 quao-0.2.2/src/quao/enum/processing_unit.py
+-rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.2.2/src/quao/enum/provider_type.py
+-rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.2.2/src/quao/enum/sdk.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:44:34.984790 quao-0.2.2/src/quao/factory/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.2/src/quao/factory/__init__.py
+-rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.2.2/src/quao/factory/device_factory.py
+-rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.2.2/src/quao/factory/provider_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:44:34.985783 quao-0.2.2/src/quao/model/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.2/src/quao/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:44:34.997785 quao-0.2.2/src/quao/model/device/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.2/src/quao/model/device/__init__.py
+-rw-rw-rw-   0        0        0     1540 2023-06-13 03:37:41.000000 quao-0.2.2/src/quao/model/device/aws_braket_device.py
+-rw-rw-rw-   0        0        0     3144 2023-06-13 03:37:41.000000 quao-0.2.2/src/quao/model/device/device.py
+-rw-rw-rw-   0        0        0     1014 2023-06-13 03:37:41.000000 quao-0.2.2/src/quao/model/device/ibm_cloud_device.py
+-rw-rw-rw-   0        0        0      794 2023-06-13 03:37:41.000000 quao-0.2.2/src/quao/model/device/ibm_quantum_device.py
+-rw-rw-rw-   0        0        0      778 2023-06-13 03:37:41.000000 quao-0.2.2/src/quao/model/device/qiskit_device.py
+-rw-rw-rw-   0        0        0     2635 2023-06-14 07:23:20.000000 quao-0.2.2/src/quao/model/device/quao_device.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:44:35.000787 quao-0.2.2/src/quao/model/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.2/src/quao/model/job/__init__.py
+-rw-rw-rw-   0        0        0     2693 2023-06-02 10:41:04.000000 quao-0.2.2/src/quao/model/job/qiskit_status.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:44:35.011783 quao-0.2.2/src/quao/model/provider/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.2/src/quao/model/provider/__init__.py
+-rw-rw-rw-   0        0        0     1257 2023-06-13 03:37:41.000000 quao-0.2.2/src/quao/model/provider/aws_braket_provider.py
+-rw-rw-rw-   0        0        0     1010 2023-06-13 03:37:41.000000 quao-0.2.2/src/quao/model/provider/ibm_cloud_provider.py
+-rw-rw-rw-   0        0        0      880 2023-06-13 03:37:41.000000 quao-0.2.2/src/quao/model/provider/ibm_quantum_provider.py
+-rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.2.2/src/quao/model/provider/provider.py
+-rw-rw-rw-   0        0        0     1455 2023-06-14 07:23:20.000000 quao-0.2.2/src/quao/model/provider/quao_provider.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:44:35.015785 quao-0.2.2/src/quao/util/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.2/src/quao/util/__init__.py
+-rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.2.2/src/quao/util/json_parser_util.py
+-rw-rw-rw-   0        0        0     1288 2023-06-02 10:41:04.000000 quao-0.2.2/src/quao/util/response_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:44:34.958784 quao-0.2.2/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-06-14 09:44:34.000000 quao-0.2.2/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1480 2023-06-14 09:44:34.000000 quao-0.2.2/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 09:44:34.000000 quao-0.2.2/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      166 2023-06-14 09:44:34.000000 quao-0.2.2/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-14 09:44:34.000000 quao-0.2.2/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.2.1/LICENSE` & `quao-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/PKG-INFO` & `quao-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.2.1
+Version: 0.2.2
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.2.1/README.md` & `quao-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/pyproject.toml` & `quao-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.2.1"
+version = "0.2.2"
 description = "Quao Library supporting Quao Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `quao-0.2.1/src/quao/backend.py` & `quao-0.2.2/src/quao/backend.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/src/quao/data/job/job_response.py` & `quao-0.2.2/src/quao/data/job/job_response.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/src/quao/data/request/request_data.py` & `quao-0.2.2/src/quao/data/request/request_data.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/src/quao/factory/device_factory.py` & `quao-0.2.2/src/quao/factory/device_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/src/quao/factory/provider_factory.py` & `quao-0.2.2/src/quao/factory/provider_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/src/quao/model/device/aws_braket_device.py` & `quao-0.2.2/src/quao/model/device/aws_braket_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/src/quao/model/device/device.py` & `quao-0.2.2/src/quao/model/device/device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/src/quao/model/device/ibm_cloud_device.py` & `quao-0.2.2/src/quao/model/device/ibm_cloud_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/src/quao/model/device/ibm_quantum_device.py` & `quao-0.2.2/src/quao/model/device/ibm_quantum_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/src/quao/model/device/qiskit_device.py` & `quao-0.2.2/src/quao/model/device/qiskit_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/src/quao/model/device/quao_device.py` & `quao-0.2.2/src/quao/model/device/quao_device.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
     QuaO Project quao_device.py Copyright © CITYNOW Co. Ltd. All rights reserved.
 """
 from qiskit import transpile
 from qiskit import QiskitError
 
 from ...enum.job_status import JobStatus
+from ...enum.processing_unit import ProcessingUnit
 from ...util.json_parser_util import JsonParserUtils
 from ...enum.sdk import Sdk
 from ..device.device import Device
 from ..provider.provider import Provider
 from ...config.logging_config import logging
 
 
@@ -16,17 +17,18 @@
     def __init__(self, provider: Provider, device_specification: str, sdk: str):
         super().__init__(provider, device_specification)
         self.sdk = sdk
 
     def _create_job(self, circuit, shots):
         logging.info('Create Quao job with {0} shots'.format(shots))
         if Sdk.QISKIT.value.__eq__(self.sdk):
+            self.device.set_options(device=ProcessingUnit.GPU.value, shots=shots)
             transpiled_circuit = transpile(circuits=circuit, backend=self.device)
 
-            return self.device.run(transpiled_circuit, shots=shots)
+            return self.device.run(transpiled_circuit)
 
         if Sdk.BRAKET.value.__eq__(self.sdk):
             return self.device.run(task_specification=circuit, shots=shots)
 
         raise Exception("Sdk not supported!")
 
     def _is_simulator(self) -> bool:
```

### Comparing `quao-0.2.1/src/quao/model/job/qiskit_status.py` & `quao-0.2.2/src/quao/model/job/qiskit_status.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/src/quao/model/provider/aws_braket_provider.py` & `quao-0.2.2/src/quao/model/provider/aws_braket_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/src/quao/model/provider/ibm_cloud_provider.py` & `quao-0.2.2/src/quao/model/provider/ibm_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/src/quao/model/provider/ibm_quantum_provider.py` & `quao-0.2.2/src/quao/model/provider/ibm_quantum_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/src/quao/model/provider/provider.py` & `quao-0.2.2/src/quao/model/provider/provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/src/quao/model/provider/quao_provider.py` & `quao-0.2.2/src/quao/model/provider/quao_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         providers = self.collect_providers()
 
         aer_device_names = set(map(self.__map_aer_backend_name, providers[0].backends()))
         aws_device_names = providers[1].registered_backends()
 
         if aer_device_names.__contains__(device_specification):
             backend = providers[0].get_backend(device_specification)
-            backend.set_options(device=ProcessingUnit.GPU.value)
+
             return backend
 
         if aws_device_names.__contains__(device_specification):
             return LocalSimulator(device_specification)
 
         raise Exception('Unsupported device')
```

### Comparing `quao-0.2.1/src/quao/util/json_parser_util.py` & `quao-0.2.2/src/quao/util/json_parser_util.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/src/quao/util/response_utils.py` & `quao-0.2.2/src/quao/util/response_utils.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.1/src/quao.egg-info/PKG-INFO` & `quao-0.2.2/src/quao.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.2.1
+Version: 0.2.2
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.2.1/src/quao.egg-info/SOURCES.txt` & `quao-0.2.2/src/quao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

