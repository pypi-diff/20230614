# Comparing `tmp/extraneous_activity_delays-2.1.10.tar.gz` & `tmp/extraneous_activity_delays-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extraneous_activity_delays-2.1.10.tar", max compression
+gzip compressed data, was "extraneous_activity_delays-2.1.9.tar", max compression
```

## Comparing `extraneous_activity_delays-2.1.10.tar` & `extraneous_activity_delays-2.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11349 2023-06-14 11:44:18.368192 extraneous_activity_delays-2.1.10/LICENSE
--rw-r--r--   0        0        0     9404 2023-06-14 11:44:18.368192 extraneous_activity_delays-2.1.10/README.md
--rw-r--r--   0        0        0      554 2023-06-14 11:44:18.432191 extraneous_activity_delays-2.1.10/pyproject.toml
--rw-r--r--   0        0        0       64 2023-06-14 11:44:18.432191 extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/__init__.py
--rw-r--r--   0        0        0     6580 2023-06-14 11:44:18.432191 extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/config.py
--rw-r--r--   0        0        0    13561 2023-06-14 11:44:18.432191 extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/delay_discoverer.py
--rw-r--r--   0        0        0    16020 2023-06-14 11:44:18.432191 extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/enhance_with_delays.py
--rw-r--r--   0        0        0       53 2023-06-14 11:44:18.432191 extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/prosimos/__init__.py
--rw-r--r--   0        0        0     2358 2023-06-14 11:44:18.432191 extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/prosimos/simulation_model_enhancer.py
--rw-r--r--   0        0        0     2118 2023-06-14 11:44:18.432191 extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/prosimos/simulator.py
--rw-r--r--   0        0        0       53 2023-06-14 11:44:18.432191 extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/qbp/__init__.py
--rw-r--r--   0        0        0     4372 2023-06-14 11:44:18.432191 extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/qbp/simulation_model_enhancer.py
--rw-r--r--   0        0        0     1593 2023-06-14 11:44:18.432191 extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/qbp/simulator.py
--rw-r--r--   0        0        0       60 2023-06-14 11:44:18.432191 extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/utils/__init__.py
--rw-r--r--   0        0        0     3194 2023-06-14 11:44:18.432191 extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/utils/bpmn_enhancement.py
--rw-r--r--   0        0        0      810 2023-06-14 11:44:18.432191 extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/utils/file_manager.py
--rw-r--r--   0        0        0    10111 1970-01-01 00:00:00.000000 extraneous_activity_delays-2.1.10/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-10 11:11:52.365418 extraneous_activity_delays-2.1.9/LICENSE
+-rw-r--r--   0        0        0     9404 2023-05-24 10:39:33.962708 extraneous_activity_delays-2.1.9/README.md
+-rw-r--r--   0        0        0      553 2023-05-24 10:27:55.491113 extraneous_activity_delays-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-05-24 10:09:51.247101 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/__init__.py
+-rw-r--r--   0        0        0     6580 2023-05-24 10:36:04.338823 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/config.py
+-rw-r--r--   0        0        0    13561 2023-05-24 10:11:56.745400 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/delay_discoverer.py
+-rw-r--r--   0        0        0    16020 2023-05-24 10:11:56.759114 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/enhance_with_delays.py
+-rw-r--r--   0        0        0       53 2023-05-24 10:09:51.253732 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/prosimos/__init__.py
+-rw-r--r--   0        0        0     2358 2023-05-24 10:11:56.721128 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/prosimos/simulation_model_enhancer.py
+-rw-r--r--   0        0        0     2118 2023-05-24 10:11:56.715176 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/prosimos/simulator.py
+-rw-r--r--   0        0        0       53 2023-05-24 10:09:51.260582 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/qbp/__init__.py
+-rw-r--r--   0        0        0     4372 2023-05-24 10:11:56.729581 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/qbp/simulation_model_enhancer.py
+-rw-r--r--   0        0        0     1593 2023-05-24 10:11:56.717662 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/qbp/simulator.py
+-rw-r--r--   0        0        0       60 2023-05-24 10:09:51.266529 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/utils/__init__.py
+-rw-r--r--   0        0        0     3194 2023-05-24 10:11:56.736893 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/utils/bpmn_enhancement.py
+-rw-r--r--   0        0        0      810 2023-05-24 10:11:56.726632 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/utils/file_manager.py
+-rw-r--r--   0        0        0    10110 1970-01-01 00:00:00.000000 extraneous_activity_delays-2.1.9/PKG-INFO
```

### Comparing `extraneous_activity_delays-2.1.10/LICENSE` & `extraneous_activity_delays-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.10/README.md` & `extraneous_activity_delays-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.10/pyproject.toml` & `extraneous_activity_delays-2.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "extraneous-activity-delays"
-version = "2.1.10"
+version = "2.1.9"
 description = ""
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 prosimos = "^1.2.4"
```

### Comparing `extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/config.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/config.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/delay_discoverer.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/delay_discoverer.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/enhance_with_delays.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/enhance_with_delays.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/prosimos/simulation_model_enhancer.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/prosimos/simulation_model_enhancer.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/prosimos/simulator.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/prosimos/simulator.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/qbp/simulation_model_enhancer.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/qbp/simulation_model_enhancer.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/qbp/simulator.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/qbp/simulator.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/utils/bpmn_enhancement.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/utils/bpmn_enhancement.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.10/src/extraneous_activity_delays/utils/file_manager.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/utils/file_manager.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.10/PKG-INFO` & `extraneous_activity_delays-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extraneous-activity-delays
-Version: 2.1.10
+Version: 2.1.9
 Summary: 
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

