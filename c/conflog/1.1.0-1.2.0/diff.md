# Comparing `tmp/conflog-1.1.0.tar.gz` & `tmp/conflog-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conflog-1.1.0.tar", last modified: Wed Jun 14 02:02:31 2023, max compression
+gzip compressed data, was "conflog-1.2.0.tar", last modified: Wed Jun 14 06:51:52 2023, max compression
```

## Comparing `conflog-1.1.0.tar` & `conflog-1.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:02:31.727089 conflog-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-14 02:01:35.000000 conflog-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-14 02:02:31.723089 conflog-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-14 02:01:35.000000 conflog-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:02:31.723089 conflog-1.1.0/conflog/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:02:31.723089 conflog-1.1.0/conflog/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/handlers/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/handlers/stream_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:02:31.723089 conflog-1.1.0/conflog/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/loaders/environ_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/loaders/ini_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/loaders/json_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/loaders/xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/loaders/yaml_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:02:31.723089 conflog-1.1.0/conflog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-14 02:02:31.000000 conflog-1.1.0/conflog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-14 02:02:31.000000 conflog-1.1.0/conflog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 02:02:31.000000 conflog-1.1.0/conflog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 02:02:31.000000 conflog-1.1.0/conflog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 02:02:31.000000 conflog-1.1.0/conflog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 02:02:31.727089 conflog-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-14 02:01:35.000000 conflog-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:02:31.723089 conflog-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:02:31.723089 conflog-1.1.0/tests/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/handlers/test_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/handlers/test_stream_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:02:31.723089 conflog-1.1.0/tests/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/loaders/test_environ_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/loaders/test_ini_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/loaders/test_json_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/loaders/test_xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/loaders/test_yaml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/test_conflog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:52.871562 conflog-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-14 06:51:01.000000 conflog-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-14 06:51:52.871562 conflog-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-14 06:51:01.000000 conflog-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:52.863562 conflog-1.2.0/conflog/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:52.867562 conflog-1.2.0/conflog/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/handlers/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/handlers/stream_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:52.867562 conflog-1.2.0/conflog/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/loaders/environ_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/loaders/ini_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/loaders/json_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/loaders/xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-14 06:51:01.000000 conflog-1.2.0/conflog/loaders/yaml_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:52.867562 conflog-1.2.0/conflog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-14 06:51:52.000000 conflog-1.2.0/conflog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-14 06:51:52.000000 conflog-1.2.0/conflog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 06:51:52.000000 conflog-1.2.0/conflog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 06:51:52.000000 conflog-1.2.0/conflog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 06:51:52.000000 conflog-1.2.0/conflog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 06:51:52.871562 conflog-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-14 06:51:01.000000 conflog-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:52.867562 conflog-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:52.867562 conflog-1.2.0/tests/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/handlers/test_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/handlers/test_stream_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:52.871562 conflog-1.2.0/tests/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/loaders/test_environ_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/loaders/test_ini_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/loaders/test_json_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/loaders/test_xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/loaders/test_yaml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-14 06:51:01.000000 conflog-1.2.0/tests/test_conflog.py
```

### Comparing `conflog-1.1.0/LICENSE` & `conflog-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conflog-1.1.0/PKG-INFO` & `conflog-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conflog
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python logging setup via environment variables and configuration files
 Home-page: https://github.com/cliffano/pyconflog
 Author: Cliffano Subagio
 Author-email: cliffano@gmail.com
 Keywords: log,logger,logging,config,configuration,environment,envvar,ini,json,xml,yaml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `conflog-1.1.0/README.md` & `conflog-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `conflog-1.1.0/conflog/__init__.py` & `conflog-1.2.0/conflog/__init__.py`

 * *Files identical despite different names*

### Comparing `conflog-1.1.0/conflog/config.py` & `conflog-1.2.0/conflog/config.py`

 * *Files identical despite different names*

### Comparing `conflog-1.1.0/conflog/loaders/ini_loader.py` & `conflog-1.2.0/conflog/loaders/ini_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.1.0/conflog.egg-info/PKG-INFO` & `conflog-1.2.0/conflog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conflog
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python logging setup via environment variables and configuration files
 Home-page: https://github.com/cliffano/pyconflog
 Author: Cliffano Subagio
 Author-email: cliffano@gmail.com
 Keywords: log,logger,logging,config,configuration,environment,envvar,ini,json,xml,yaml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `conflog-1.1.0/conflog.egg-info/SOURCES.txt` & `conflog-1.2.0/conflog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conflog-1.1.0/setup.py` & `conflog-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `conflog-1.1.0/tests/handlers/test_file_handler.py` & `conflog-1.2.0/tests/handlers/test_file_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # pylint: disable=missing-module-docstring,missing-class-docstring,missing-function-docstring,duplicate-code,too-many-locals
 from unittest.mock import patch
 import unittest.mock
 import unittest
+import logging
 from conflog.handlers.file_handler import init
 
 class TestFileHandler(unittest.TestCase):
 
     @patch('logging.FileHandler.__new__')
     @patch('logging.Formatter.__new__')
     def test_init( # pylint: disable=unused-argument
             self,
             func_formatter,
             func_file_handler):
 
         mock_config = unittest.mock.Mock()
         mock_config.get_datefmt.return_value = '%d-%b-%y %H:%M:%S'
+        mock_config.get_level.return_value = logging.INFO
         mock_config.get_format.return_value = '%(asctime)s --> '\
                                               '%(name)s - %(levelname)s - %(message)s'
         mock_config.get_filename.return_value = 'conflog.log'
         mock_config.get_filemode.return_value = 'w'
 
         mock_formatter = unittest.mock.Mock()
         func_formatter.return_value = mock_formatter
 
         mock_file_handler = unittest.mock.Mock()
         func_file_handler.return_value = mock_file_handler
 
         result = init(mock_config)
         self.assertEqual(result, mock_file_handler)
         mock_file_handler.setFormatter.assert_called_once_with(mock_formatter)
+        mock_file_handler.setLevel.assert_called_once_with(logging.INFO)
```

### Comparing `conflog-1.1.0/tests/handlers/test_stream_handler.py` & `conflog-1.2.0/tests/handlers/test_stream_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # pylint: disable=missing-module-docstring,missing-class-docstring,missing-function-docstring,duplicate-code,too-many-locals
 from unittest.mock import patch
 import unittest.mock
 import unittest
+import logging
 from conflog.handlers.stream_handler import init
 
 class TestStreamHandler(unittest.TestCase):
 
     @patch('logging.StreamHandler.__new__')
     @patch('logging.Formatter.__new__')
     def test_init( # pylint: disable=unused-argument
             self,
             func_formatter,
             func_stream_handler):
 
         mock_config = unittest.mock.Mock()
         mock_config.get_datefmt.return_value = '%d-%b-%y %H:%M:%S'
+        mock_config.get_level.return_value = logging.INFO
         mock_config.get_format.return_value = '%(asctime)s --> '\
                                               '%(name)s - %(levelname)s - %(message)s'
 
         mock_formatter = unittest.mock.Mock()
         func_formatter.return_value = mock_formatter
 
         mock_stream_handler = unittest.mock.Mock()
         func_stream_handler.return_value = mock_stream_handler
 
         result = init(mock_config)
         self.assertEqual(result, mock_stream_handler)
         mock_stream_handler.setFormatter.assert_called_once_with(mock_formatter)
+        mock_stream_handler.setLevel.assert_called_once_with(logging.INFO)
```

### Comparing `conflog-1.1.0/tests/loaders/test_environ_loader.py` & `conflog-1.2.0/tests/loaders/test_environ_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.1.0/tests/loaders/test_ini_loader.py` & `conflog-1.2.0/tests/loaders/test_ini_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.1.0/tests/loaders/test_json_loader.py` & `conflog-1.2.0/tests/loaders/test_json_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.1.0/tests/loaders/test_xml_loader.py` & `conflog-1.2.0/tests/loaders/test_xml_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.1.0/tests/loaders/test_yaml_loader.py` & `conflog-1.2.0/tests/loaders/test_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.1.0/tests/test_config.py` & `conflog-1.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `conflog-1.1.0/tests/test_conflog.py` & `conflog-1.2.0/tests/test_conflog.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,17 @@
 
         mock_config.get_handlers.return_value = ['stream', 'file']
         mock_config.get_datefmt.return_value = '%d-%b-%y %H:%M:%S'
         mock_config.get_level.return_value = logging.INFO
 
         conflog = Conflog(conf_files=['somefile.ini', 'somefile.json'])
         mock_stream_handler.setFormatter.assert_called_once_with(mock_formatter)
+        mock_stream_handler.setLevel.assert_called_once_with(logging.INFO)
         mock_file_handler.setFormatter.assert_called_once_with(mock_formatter)
+        mock_file_handler.setLevel.assert_called_once_with(logging.INFO)
         func_basic_config.assert_called_once_with(
             datefmt='%d-%b-%y %H:%M:%S',
             level=logging.INFO,
         )
 
         logger = conflog.get_logger('someloggername')
         func_get_logger.assert_called_with('someloggername')
```

