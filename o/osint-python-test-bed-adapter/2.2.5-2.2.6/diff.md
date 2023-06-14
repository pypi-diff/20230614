# Comparing `tmp/osint-python-test-bed-adapter-2.2.5.tar.gz` & `tmp/osint-python-test-bed-adapter-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-test-bed-adapter-2.2.5.tar", last modified: Fri Jun  9 13:41:43 2023, max compression
+gzip compressed data, was "osint-python-test-bed-adapter-2.2.6.tar", last modified: Wed Jun 14 11:05:03 2023, max compression
```

## Comparing `osint-python-test-bed-adapter-2.2.5.tar` & `osint-python-test-bed-adapter-2.2.6.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-09 13:41:43.337409 osint-python-test-bed-adapter-2.2.5/
--rw-r--r--   0 erik      (1000) erik      (1000)     1064 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/LICENSE
--rw-r--r--   0 erik      (1000) erik      (1000)     1873 2023-06-09 13:41:43.337409 osint-python-test-bed-adapter-2.2.5/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)     1409 2023-06-09 13:23:45.000000 osint-python-test-bed-adapter-2.2.5/README.md
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-09 13:41:43.317409 osint-python-test-bed-adapter-2.2.5/osint_python_test_bed_adapter.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)     1873 2023-06-09 13:41:43.000000 osint-python-test-bed-adapter-2.2.5/osint_python_test_bed_adapter.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      703 2023-06-09 13:41:43.000000 osint-python-test-bed-adapter-2.2.5/osint_python_test_bed_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-06-09 13:41:43.000000 osint-python-test-bed-adapter-2.2.5/osint_python_test_bed_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       39 2023-06-09 13:41:43.000000 osint-python-test-bed-adapter-2.2.5/osint_python_test_bed_adapter.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       17 2023-06-09 13:41:43.000000 osint-python-test-bed-adapter-2.2.5/osint_python_test_bed_adapter.egg-info/top_level.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       38 2023-06-09 13:41:43.337409 osint-python-test-bed-adapter-2.2.5/setup.cfg
--rw-r--r--   0 erik      (1000) erik      (1000)      758 2023-06-09 13:39:37.000000 osint-python-test-bed-adapter-2.2.5/setup.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-09 13:41:43.317409 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/
--rw-r--r--   0 erik      (1000) erik      (1000)     1361 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-09 13:41:43.327409 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/
--rw-r--r--   0 erik      (1000) erik      (1000)       68 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2246 2023-06-09 13:19:07.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/consumer_manager.py
--rw-r--r--   0 erik      (1000) erik      (1000)     1660 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/heartbeat_manager.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2999 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/log_manager.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2122 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/producer_manager.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-09 13:41:43.327409 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/options/
--rw-r--r--   0 erik      (1000) erik      (1000)       31 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/options/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     3486 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/options/test_bed_options.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-09 13:41:43.337409 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/utils/
--rw-r--r--   0 erik      (1000) erik      (1000)       22 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/utils/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)      598 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/utils/helpers.py
--rw-r--r--   0 erik      (1000) erik      (1000)     1005 2023-06-09 13:18:42.000000 osint-python-test-bed-adapter-2.2.5/test_bed_adapter/utils/key.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-14 11:05:03.211362 osint-python-test-bed-adapter-2.2.6/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.2.6/LICENSE
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3592 2023-06-14 11:05:03.211362 osint-python-test-bed-adapter-2.2.6/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3165 2023-06-13 08:56:50.000000 osint-python-test-bed-adapter-2.2.6/README.md
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-14 11:05:03.208029 osint-python-test-bed-adapter-2.2.6/osint_python_test_bed_adapter.egg-info/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3592 2023-06-14 11:05:03.000000 osint-python-test-bed-adapter-2.2.6/osint_python_test_bed_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      782 2023-06-14 11:05:03.000000 osint-python-test-bed-adapter-2.2.6/osint_python_test_bed_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-06-14 11:05:03.000000 osint-python-test-bed-adapter-2.2.6/osint_python_test_bed_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       39 2023-06-14 11:05:03.000000 osint-python-test-bed-adapter-2.2.6/osint_python_test_bed_adapter.egg-info/requires.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       17 2023-06-14 11:05:03.000000 osint-python-test-bed-adapter-2.2.6/osint_python_test_bed_adapter.egg-info/top_level.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-06-14 11:05:03.211362 osint-python-test-bed-adapter-2.2.6/setup.cfg
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      758 2023-06-14 10:59:52.000000 osint-python-test-bed-adapter-2.2.6/setup.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-14 11:05:03.208029 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1361 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/__init__.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-14 11:05:03.211362 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       68 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2481 2023-06-14 11:02:28.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/consumer_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1660 2023-03-16 17:49:08.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/heartbeat_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2999 2023-06-07 19:48:38.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/log_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2122 2023-04-06 23:32:08.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/producer_manager.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-14 11:05:03.211362 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/options/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       31 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/options/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3486 2023-06-01 22:28:40.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/options/test_bed_options.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-14 11:05:03.211362 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/services/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-14 11:55:32.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/services/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2065 2023-03-14 12:17:24.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/services/http_server.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-14 11:05:03.211362 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/utils/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       22 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/utils/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      598 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/utils/helpers.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1005 2023-03-16 17:51:41.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/utils/key.py
```

### Comparing `osint-python-test-bed-adapter-2.2.5/LICENSE` & `osint-python-test-bed-adapter-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.5/osint_python_test_bed_adapter.egg-info/SOURCES.txt` & `osint-python-test-bed-adapter-2.2.6/osint_python_test_bed_adapter.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,10 +10,12 @@
 test_bed_adapter/kafka/__init__.py
 test_bed_adapter/kafka/consumer_manager.py
 test_bed_adapter/kafka/heartbeat_manager.py
 test_bed_adapter/kafka/log_manager.py
 test_bed_adapter/kafka/producer_manager.py
 test_bed_adapter/options/__init__.py
 test_bed_adapter/options/test_bed_options.py
+test_bed_adapter/services/__init__.py
+test_bed_adapter/services/http_server.py
 test_bed_adapter/utils/__init__.py
 test_bed_adapter/utils/helpers.py
 test_bed_adapter/utils/key.py
```

### Comparing `osint-python-test-bed-adapter-2.2.5/setup.py` & `osint-python-test-bed-adapter-2.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="osint-python-test-bed-adapter",
-    version="2.2.5",
+    version="2.2.6",
     author="TimovdK",
     author_email="timo_kuil@hotmail.com",
     description="Python adapter for Kafka",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-adapter",
     include_package_data=True,
```

### Comparing `osint-python-test-bed-adapter-2.2.5/test_bed_adapter/__init__.py` & `osint-python-test-bed-adapter-2.2.6/test_bed_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/consumer_manager.py` & `osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/consumer_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from confluent_kafka import DeserializingConsumer, TopicPartition
+import time
+
+from confluent_kafka import DeserializingConsumer
 from confluent_kafka.schema_registry import SchemaRegistryClient
 from confluent_kafka.schema_registry.avro import AvroDeserializer
-import time
 
 from ..options.test_bed_options import TestBedOptions
 
 
-class ConsumerManager():
+class ConsumerManager:
     def __init__(self, options: TestBedOptions, kafka_topic, handle_message, run):
         self.options = options
         self.handle_message = handle_message
         self.run = run
 
         sr_conf = {'url': self.options.schema_registry}
         schema_registry_client = SchemaRegistryClient(sr_conf)
@@ -22,15 +23,24 @@
         consumer_conf = {'bootstrap.servers': self.options.kafka_host,
                          'key.deserializer': self.avro_deserializer,
                          'value.deserializer': self.avro_deserializer,
                          'group.id': self.options.consumer_group,
                          'message.max.bytes': self.options.message_max_bytes,
                          'auto.offset.reset': self.options.offset_type}
         self.consumer = DeserializingConsumer(consumer_conf)
-        self.consumer.subscribe([kafka_topic])
+
+        def on_assign(c, ps):
+            for p in ps:
+                p.offset = 0
+            c.assign(ps)
+
+        if self.options.offset_type == 'earliest':
+            self.consumer.subscribe([kafka_topic], on_assign=on_assign)
+        else:
+            self.consumer.subscribe([kafka_topic])
 
     def listen(self):
         _start_time = time.time()
         _latest_message = None
 
         # Ignore messages for a period of time
         while True and self.options.ignore_timeout:
```

### Comparing `osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/heartbeat_manager.py` & `osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/heartbeat_manager.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/log_manager.py` & `osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/log_manager.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.5/test_bed_adapter/kafka/producer_manager.py` & `osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/producer_manager.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.5/test_bed_adapter/options/test_bed_options.py` & `osint-python-test-bed-adapter-2.2.6/test_bed_adapter/options/test_bed_options.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.5/test_bed_adapter/utils/helpers.py` & `osint-python-test-bed-adapter-2.2.6/test_bed_adapter/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.5/test_bed_adapter/utils/key.py` & `osint-python-test-bed-adapter-2.2.6/test_bed_adapter/utils/key.py`

 * *Files identical despite different names*

