# Comparing `tmp/cove_unified_logs-0.2.1.tar.gz` & `tmp/cove_unified_logs-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cove_unified_logs-0.2.1.tar", last modified: Wed Jun 14 07:48:56 2023, max compression
+gzip compressed data, was "cove_unified_logs-0.2.2.tar", last modified: Wed Jun 14 07:51:30 2023, max compression
```

## Comparing `cove_unified_logs-0.2.1.tar` & `cove_unified_logs-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-14 07:48:56.712096 cove_unified_logs-0.2.1/
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1076 2023-06-08 19:25:10.000000 cove_unified_logs-0.2.1/LICENSE
--rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-14 07:48:56.711976 cove_unified_logs-0.2.1/PKG-INFO
--rw-r--r--   0 sarvpriye   (502) staff       (20)     6452 2023-06-08 19:44:21.000000 cove_unified_logs-0.2.1/README.md
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-14 07:48:56.711230 cove_unified_logs-0.2.1/cove_unified_logs/
--rw-r--r--   0 sarvpriye   (502) staff       (20)       72 2023-06-08 20:52:43.000000 cove_unified_logs-0.2.1/cove_unified_logs/__init__.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     6059 2023-06-08 21:21:58.000000 cove_unified_logs-0.2.1/cove_unified_logs/cloud_logger.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     2204 2023-06-08 21:30:17.000000 cove_unified_logs-0.2.1/cove_unified_logs/console_logger.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     2289 2023-06-09 16:31:04.000000 cove_unified_logs-0.2.1/cove_unified_logs/log_consumer.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     2112 2023-06-08 20:15:13.000000 cove_unified_logs-0.2.1/cove_unified_logs/log_producer.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)      873 2023-06-09 13:01:22.000000 cove_unified_logs-0.2.1/cove_unified_logs/middleware.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)      247 2023-06-08 20:52:38.000000 cove_unified_logs-0.2.1/cove_unified_logs/singleton.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1791 2023-06-14 07:45:43.000000 cove_unified_logs-0.2.1/cove_unified_logs/unified_logger.py
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-14 07:48:56.711787 cove_unified_logs-0.2.1/cove_unified_logs.egg-info/
--rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-14 07:48:56.000000 cove_unified_logs-0.2.1/cove_unified_logs.egg-info/PKG-INFO
--rw-r--r--   0 sarvpriye   (502) staff       (20)      497 2023-06-14 07:48:56.000000 cove_unified_logs-0.2.1/cove_unified_logs.egg-info/SOURCES.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)        1 2023-06-14 07:48:56.000000 cove_unified_logs-0.2.1/cove_unified_logs.egg-info/dependency_links.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       31 2023-06-14 07:48:56.000000 cove_unified_logs-0.2.1/cove_unified_logs.egg-info/requires.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       18 2023-06-14 07:48:56.000000 cove_unified_logs-0.2.1/cove_unified_logs.egg-info/top_level.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       38 2023-06-14 07:48:56.712135 cove_unified_logs-0.2.1/setup.cfg
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1174 2023-06-14 07:48:39.000000 cove_unified_logs-0.2.1/setup.py
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-14 07:51:30.632881 cove_unified_logs-0.2.2/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1076 2023-06-08 19:25:10.000000 cove_unified_logs-0.2.2/LICENSE
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-14 07:51:30.632761 cove_unified_logs-0.2.2/PKG-INFO
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     6452 2023-06-08 19:44:21.000000 cove_unified_logs-0.2.2/README.md
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-14 07:51:30.631935 cove_unified_logs-0.2.2/cove_unified_logs/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       72 2023-06-08 20:52:43.000000 cove_unified_logs-0.2.2/cove_unified_logs/__init__.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     6059 2023-06-08 21:21:58.000000 cove_unified_logs-0.2.2/cove_unified_logs/cloud_logger.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     2204 2023-06-08 21:30:17.000000 cove_unified_logs-0.2.2/cove_unified_logs/console_logger.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     2289 2023-06-09 16:31:04.000000 cove_unified_logs-0.2.2/cove_unified_logs/log_consumer.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     2209 2023-06-14 07:51:18.000000 cove_unified_logs-0.2.2/cove_unified_logs/log_producer.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)      873 2023-06-09 13:01:22.000000 cove_unified_logs-0.2.2/cove_unified_logs/middleware.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)      247 2023-06-08 20:52:38.000000 cove_unified_logs-0.2.2/cove_unified_logs/singleton.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1791 2023-06-14 07:45:43.000000 cove_unified_logs-0.2.2/cove_unified_logs/unified_logger.py
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-14 07:51:30.632588 cove_unified_logs-0.2.2/cove_unified_logs.egg-info/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-14 07:51:30.000000 cove_unified_logs-0.2.2/cove_unified_logs.egg-info/PKG-INFO
+-rw-r--r--   0 sarvpriye   (502) staff       (20)      497 2023-06-14 07:51:30.000000 cove_unified_logs-0.2.2/cove_unified_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)        1 2023-06-14 07:51:30.000000 cove_unified_logs-0.2.2/cove_unified_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       31 2023-06-14 07:51:30.000000 cove_unified_logs-0.2.2/cove_unified_logs.egg-info/requires.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       18 2023-06-14 07:51:30.000000 cove_unified_logs-0.2.2/cove_unified_logs.egg-info/top_level.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       38 2023-06-14 07:51:30.632924 cove_unified_logs-0.2.2/setup.cfg
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1174 2023-06-14 07:51:28.000000 cove_unified_logs-0.2.2/setup.py
```

### Comparing `cove_unified_logs-0.2.1/LICENSE` & `cove_unified_logs-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.2.1/PKG-INFO` & `cove_unified_logs-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cove_unified_logs
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.
 Home-page: https://github.com/Cove-Identity/cove-unified-logs
 Author: Coveidentity Tech Private Limited
 Author-email: sarvpriye.soni@coveidentity.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cove_unified_logs-0.2.1/README.md` & `cove_unified_logs-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.2.1/cove_unified_logs/cloud_logger.py` & `cove_unified_logs-0.2.2/cove_unified_logs/cloud_logger.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.2.1/cove_unified_logs/console_logger.py` & `cove_unified_logs-0.2.2/cove_unified_logs/console_logger.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.2.1/cove_unified_logs/log_consumer.py` & `cove_unified_logs-0.2.2/cove_unified_logs/log_consumer.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.2.1/cove_unified_logs/log_producer.py` & `cove_unified_logs-0.2.2/cove_unified_logs/log_producer.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,7 +53,10 @@
         self.log('warning', message, **metadata)
 
     def error(self, message, **metadata):
         self.log('error', message, **metadata)
 
     def critical(self, message, **metadata):
         self.log('critical', message, **metadata)
+
+    def exception(self, message, **metadata):
+        self.log('exception', message, **metadata)
```

### Comparing `cove_unified_logs-0.2.1/cove_unified_logs/middleware.py` & `cove_unified_logs-0.2.2/cove_unified_logs/middleware.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.2.1/cove_unified_logs/unified_logger.py` & `cove_unified_logs-0.2.2/cove_unified_logs/unified_logger.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.2.1/cove_unified_logs.egg-info/PKG-INFO` & `cove_unified_logs-0.2.2/cove_unified_logs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cove-unified-logs
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.
 Home-page: https://github.com/Cove-Identity/cove-unified-logs
 Author: Coveidentity Tech Private Limited
 Author-email: sarvpriye.soni@coveidentity.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cove_unified_logs-0.2.1/setup.py` & `cove_unified_logs-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cove_unified_logs',
-    version='0.2.1',
+    version='0.2.2',
     description='A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Coveidentity Tech Private Limited',
     author_email='sarvpriye.soni@coveidentity.com',
     url='https://github.com/Cove-Identity/cove-unified-logs',
     packages=['cove_unified_logs'],
```

