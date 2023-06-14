# Comparing `tmp/cove_unified_logs-0.2.0.tar.gz` & `tmp/cove_unified_logs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cove_unified_logs-0.2.0.tar", last modified: Fri Jun  9 13:24:09 2023, max compression
+gzip compressed data, was "cove_unified_logs-0.2.1.tar", last modified: Wed Jun 14 07:48:56 2023, max compression
```

## Comparing `cove_unified_logs-0.2.0.tar` & `cove_unified_logs-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-09 13:24:09.932532 cove_unified_logs-0.2.0/
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1076 2023-06-08 19:25:10.000000 cove_unified_logs-0.2.0/LICENSE
--rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-09 13:24:09.932396 cove_unified_logs-0.2.0/PKG-INFO
--rw-r--r--   0 sarvpriye   (502) staff       (20)     6452 2023-06-08 19:44:21.000000 cove_unified_logs-0.2.0/README.md
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-09 13:24:09.931486 cove_unified_logs-0.2.0/cove_unified_logs/
--rw-r--r--   0 sarvpriye   (502) staff       (20)       72 2023-06-08 20:52:43.000000 cove_unified_logs-0.2.0/cove_unified_logs/__init__.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     6059 2023-06-08 21:21:58.000000 cove_unified_logs-0.2.0/cove_unified_logs/cloud_logger.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     2204 2023-06-08 21:30:17.000000 cove_unified_logs-0.2.0/cove_unified_logs/console_logger.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     2219 2023-06-08 19:37:52.000000 cove_unified_logs-0.2.0/cove_unified_logs/log_consumer.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     2112 2023-06-08 20:15:13.000000 cove_unified_logs-0.2.0/cove_unified_logs/log_producer.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)      873 2023-06-09 13:01:22.000000 cove_unified_logs-0.2.0/cove_unified_logs/middleware.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)      247 2023-06-08 20:52:38.000000 cove_unified_logs-0.2.0/cove_unified_logs/singleton.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1609 2023-06-09 13:21:31.000000 cove_unified_logs-0.2.0/cove_unified_logs/unified_logger.py
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-09 13:24:09.932208 cove_unified_logs-0.2.0/cove_unified_logs.egg-info/
--rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-09 13:24:09.000000 cove_unified_logs-0.2.0/cove_unified_logs.egg-info/PKG-INFO
--rw-r--r--   0 sarvpriye   (502) staff       (20)      497 2023-06-09 13:24:09.000000 cove_unified_logs-0.2.0/cove_unified_logs.egg-info/SOURCES.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)        1 2023-06-09 13:24:09.000000 cove_unified_logs-0.2.0/cove_unified_logs.egg-info/dependency_links.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       31 2023-06-09 13:24:09.000000 cove_unified_logs-0.2.0/cove_unified_logs.egg-info/requires.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       18 2023-06-09 13:24:09.000000 cove_unified_logs-0.2.0/cove_unified_logs.egg-info/top_level.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       38 2023-06-09 13:24:09.932575 cove_unified_logs-0.2.0/setup.cfg
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1174 2023-06-09 13:24:04.000000 cove_unified_logs-0.2.0/setup.py
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-14 07:48:56.712096 cove_unified_logs-0.2.1/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1076 2023-06-08 19:25:10.000000 cove_unified_logs-0.2.1/LICENSE
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-14 07:48:56.711976 cove_unified_logs-0.2.1/PKG-INFO
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     6452 2023-06-08 19:44:21.000000 cove_unified_logs-0.2.1/README.md
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-14 07:48:56.711230 cove_unified_logs-0.2.1/cove_unified_logs/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       72 2023-06-08 20:52:43.000000 cove_unified_logs-0.2.1/cove_unified_logs/__init__.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     6059 2023-06-08 21:21:58.000000 cove_unified_logs-0.2.1/cove_unified_logs/cloud_logger.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     2204 2023-06-08 21:30:17.000000 cove_unified_logs-0.2.1/cove_unified_logs/console_logger.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     2289 2023-06-09 16:31:04.000000 cove_unified_logs-0.2.1/cove_unified_logs/log_consumer.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     2112 2023-06-08 20:15:13.000000 cove_unified_logs-0.2.1/cove_unified_logs/log_producer.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)      873 2023-06-09 13:01:22.000000 cove_unified_logs-0.2.1/cove_unified_logs/middleware.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)      247 2023-06-08 20:52:38.000000 cove_unified_logs-0.2.1/cove_unified_logs/singleton.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1791 2023-06-14 07:45:43.000000 cove_unified_logs-0.2.1/cove_unified_logs/unified_logger.py
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-14 07:48:56.711787 cove_unified_logs-0.2.1/cove_unified_logs.egg-info/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-14 07:48:56.000000 cove_unified_logs-0.2.1/cove_unified_logs.egg-info/PKG-INFO
+-rw-r--r--   0 sarvpriye   (502) staff       (20)      497 2023-06-14 07:48:56.000000 cove_unified_logs-0.2.1/cove_unified_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)        1 2023-06-14 07:48:56.000000 cove_unified_logs-0.2.1/cove_unified_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       31 2023-06-14 07:48:56.000000 cove_unified_logs-0.2.1/cove_unified_logs.egg-info/requires.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       18 2023-06-14 07:48:56.000000 cove_unified_logs-0.2.1/cove_unified_logs.egg-info/top_level.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       38 2023-06-14 07:48:56.712135 cove_unified_logs-0.2.1/setup.cfg
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1174 2023-06-14 07:48:39.000000 cove_unified_logs-0.2.1/setup.py
```

### Comparing `cove_unified_logs-0.2.0/LICENSE` & `cove_unified_logs-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.2.0/PKG-INFO` & `cove_unified_logs-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cove_unified_logs
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.
 Home-page: https://github.com/Cove-Identity/cove-unified-logs
 Author: Coveidentity Tech Private Limited
 Author-email: sarvpriye.soni@coveidentity.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cove_unified_logs-0.2.0/README.md` & `cove_unified_logs-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.2.0/cove_unified_logs/cloud_logger.py` & `cove_unified_logs-0.2.1/cove_unified_logs/cloud_logger.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.2.0/cove_unified_logs/console_logger.py` & `cove_unified_logs-0.2.1/cove_unified_logs/console_logger.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.2.0/cove_unified_logs/log_consumer.py` & `cove_unified_logs-0.2.1/cove_unified_logs/log_consumer.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 
 
 class LogConsumer:
     def __init__(self, channel='logs', cloud_logger=None):
         redis_host = os.getenv('REDIS_HOST', 'localhost')
         redis_port = int(os.getenv('REDIS_PORT', 6379))
         redis_password = os.getenv('REDIS_PASSWORD', None)
+        redis_db = os.getenv('REDIS_DB', 0)
         try:
             if redis_password is not None:
-                self.redis = redis.Redis(host=redis_host, port=redis_port, password=redis_password)
+                self.redis = redis.Redis(host=redis_host, port=redis_port, password=redis_password, db=redis_db)
             else:
-                self.redis = redis.Redis(host=redis_host, port=redis_port)
+                self.redis = redis.Redis(host=redis_host, port=redis_port, db=redis_db)
             self.pubsub = self.redis.pubsub()
             self.pubsub.subscribe(channel)
             self.cloud_logger = cloud_logger
         except Exception as e:
             logging.error(f"Failed to initialize LogConsumer: {str(e)}")
             raise
```

### Comparing `cove_unified_logs-0.2.0/cove_unified_logs/log_producer.py` & `cove_unified_logs-0.2.1/cove_unified_logs/log_producer.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.2.0/cove_unified_logs/middleware.py` & `cove_unified_logs-0.2.1/cove_unified_logs/middleware.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.2.0/cove_unified_logs/unified_logger.py` & `cove_unified_logs-0.2.1/cove_unified_logs/unified_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,7 +38,11 @@
     def error(self, message, **metadata):
         if self.log_level in ('debug', 'info', 'warning', 'error'):
             self._log('error', message, **metadata)
 
     def critical(self, message, **metadata):
         if self.log_level in ('debug', 'info', 'warning', 'error', 'critical'):
             self._log('critical', message, **metadata)
+
+    def exception(self, message, **metadata):
+        if self.log_level in ('debug', 'info', 'warning', 'error', 'critical'):
+            self._log('exception', message, **metadata)
```

### Comparing `cove_unified_logs-0.2.0/cove_unified_logs.egg-info/PKG-INFO` & `cove_unified_logs-0.2.1/cove_unified_logs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cove-unified-logs
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.
 Home-page: https://github.com/Cove-Identity/cove-unified-logs
 Author: Coveidentity Tech Private Limited
 Author-email: sarvpriye.soni@coveidentity.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cove_unified_logs-0.2.0/setup.py` & `cove_unified_logs-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cove_unified_logs',
-    version='0.2.0',
+    version='0.2.1',
     description='A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Coveidentity Tech Private Limited',
     author_email='sarvpriye.soni@coveidentity.com',
     url='https://github.com/Cove-Identity/cove-unified-logs',
     packages=['cove_unified_logs'],
```

