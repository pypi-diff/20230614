# Comparing `tmp/conflog-1.2.0.tar.gz` & `tmp/conflog-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conflog-1.2.0.tar", last modified: Wed Jun 14 06:51:52 2023, max compression
+gzip compressed data, was "conflog-1.3.0.tar", last modified: Wed Jun 14 09:39:16 2023, max compression
```

## Comparing `conflog-1.2.0.tar` & `conflog-1.3.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:52.871562 conflog-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-14 06:51:01.000000 conflog-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-14 06:51:52.871562 conflog-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-14 06:51:01.000000 conflog-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:52.863562 conflog-1.2.0/conflog/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:52.867562 conflog-1.2.0/conflog/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/handlers/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/handlers/stream_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:52.867562 conflog-1.2.0/conflog/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/loaders/environ_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/loaders/ini_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/loaders/json_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/loaders/xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/loaders/yaml_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:52.867562 conflog-1.2.0/conflog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-14 06:51:52.000000 conflog-1.2.0/conflog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-14 06:51:52.000000 conflog-1.2.0/conflog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 06:51:52.000000 conflog-1.2.0/conflog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 06:51:52.000000 conflog-1.2.0/conflog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 06:51:52.000000 conflog-1.2.0/conflog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 06:51:52.871562 conflog-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-14 06:51:01.000000 conflog-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:52.867562 conflog-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:52.867562 conflog-1.2.0/tests/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/handlers/test_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/handlers/test_stream_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:52.871562 conflog-1.2.0/tests/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/loaders/test_environ_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/loaders/test_ini_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/loaders/test_json_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/loaders/test_xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/loaders/test_yaml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/test_conflog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:39:16.901686 conflog-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-14 09:38:36.000000 conflog-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-14 09:39:16.901686 conflog-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-14 09:38:36.000000 conflog-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:39:16.897686 conflog-1.3.0/conflog/
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:39:16.897686 conflog-1.3.0/conflog/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/handlers/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/handlers/stream_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:39:16.901686 conflog-1.3.0/conflog/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/loaders/environ_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/loaders/ini_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/loaders/json_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/loaders/xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-14 09:38:36.000000 conflog-1.3.0/conflog/loaders/yaml_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:39:16.897686 conflog-1.3.0/conflog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-14 09:39:16.000000 conflog-1.3.0/conflog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-14 09:39:16.000000 conflog-1.3.0/conflog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:39:16.000000 conflog-1.3.0/conflog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 09:39:16.000000 conflog-1.3.0/conflog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 09:39:16.000000 conflog-1.3.0/conflog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:39:16.901686 conflog-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-14 09:38:36.000000 conflog-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:39:16.901686 conflog-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:39:16.901686 conflog-1.3.0/tests/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/handlers/test_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/handlers/test_stream_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:39:16.901686 conflog-1.3.0/tests/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/loaders/test_environ_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/loaders/test_ini_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/loaders/test_json_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/loaders/test_xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/loaders/test_yaml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-14 09:38:36.000000 conflog-1.3.0/tests/test_conflog.py
```

### Comparing `conflog-1.2.0/LICENSE` & `conflog-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conflog-1.2.0/PKG-INFO` & `conflog-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conflog
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python logging setup via environment variables and configuration files
 Home-page: https://github.com/cliffano/pyconflog
 Author: Cliffano Subagio
 Author-email: cliffano@gmail.com
 Keywords: log,logger,logging,config,configuration,environment,envvar,ini,json,xml,yaml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `conflog-1.2.0/README.md` & `conflog-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `conflog-1.2.0/conflog/__init__.py` & `conflog-1.3.0/conflog/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
         """
         logger = logging.getLogger(name)
         logger.propagate = False # prevent duplicate logging from parent propagation
         for handler in self.handlers:
             logger.addHandler(handler)
 
         logger = logging.LoggerAdapter(logger, self.extras)
+        logger.setLevel(self.config.get_level())
+
         return logger
 
     def close_logger_handlers(self, name):
         """Close logger handlers
         and clear the handlers from logger.
         """
         logger = logging.getLogger(name)
```

### Comparing `conflog-1.2.0/conflog/config.py` & `conflog-1.3.0/conflog/config.py`

 * *Files identical despite different names*

### Comparing `conflog-1.2.0/conflog/loaders/ini_loader.py` & `conflog-1.3.0/conflog/loaders/ini_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.2.0/conflog.egg-info/PKG-INFO` & `conflog-1.3.0/conflog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conflog
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python logging setup via environment variables and configuration files
 Home-page: https://github.com/cliffano/pyconflog
 Author: Cliffano Subagio
 Author-email: cliffano@gmail.com
 Keywords: log,logger,logging,config,configuration,environment,envvar,ini,json,xml,yaml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `conflog-1.2.0/conflog.egg-info/SOURCES.txt` & `conflog-1.3.0/conflog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conflog-1.2.0/setup.py` & `conflog-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `conflog-1.2.0/tests/handlers/test_file_handler.py` & `conflog-1.3.0/tests/handlers/test_file_handler.py`

 * *Files identical despite different names*

### Comparing `conflog-1.2.0/tests/handlers/test_stream_handler.py` & `conflog-1.3.0/tests/handlers/test_stream_handler.py`

 * *Files identical despite different names*

### Comparing `conflog-1.2.0/tests/loaders/test_environ_loader.py` & `conflog-1.3.0/tests/loaders/test_environ_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.2.0/tests/loaders/test_ini_loader.py` & `conflog-1.3.0/tests/loaders/test_ini_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.2.0/tests/loaders/test_json_loader.py` & `conflog-1.3.0/tests/loaders/test_json_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.2.0/tests/loaders/test_xml_loader.py` & `conflog-1.3.0/tests/loaders/test_xml_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.2.0/tests/loaders/test_yaml_loader.py` & `conflog-1.3.0/tests/loaders/test_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.2.0/tests/test_config.py` & `conflog-1.3.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `conflog-1.2.0/tests/test_conflog.py` & `conflog-1.3.0/tests/test_conflog.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 
         logger = conflog.get_logger('someloggername')
         func_get_logger.assert_called_with('someloggername')
         self.assertEqual(logger, mock_adapted_logger)
         self.assertFalse(mock_logger.propagate)
         mock_logger.addHandler.assert_any_call(mock_stream_handler)
         mock_logger.addHandler.assert_any_call(mock_file_handler)
+        mock_adapted_logger.setLevel.assert_called_once_with(logging.INFO)
 
         conflog.close_logger_handlers('someloggername')
         mock_stream_handler.close.assert_called_once_with()
         mock_file_handler.close.assert_called_once_with()
 
         config = conflog.get_config_properties()
         self.assertEqual(config, mock_config.conf)
```

