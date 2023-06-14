# Comparing `tmp/conflog-1.0.1.tar.gz` & `tmp/conflog-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conflog-1.0.1.tar", last modified: Thu Jun  8 05:41:19 2023, max compression
+gzip compressed data, was "conflog-1.1.0.tar", last modified: Wed Jun 14 02:02:31 2023, max compression
```

## Comparing `conflog-1.0.1.tar` & `conflog-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:41:19.042632 conflog-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-08 05:40:30.000000 conflog-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-06-08 05:41:19.042632 conflog-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-08 05:40:30.000000 conflog-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:41:19.038632 conflog-1.0.1/conflog/
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-08 05:40:30.000000 conflog-1.0.1/conflog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-08 05:40:30.000000 conflog-1.0.1/conflog/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:41:19.042632 conflog-1.0.1/conflog/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 05:40:30.000000 conflog-1.0.1/conflog/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-08 05:40:30.000000 conflog-1.0.1/conflog/handlers/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-08 05:40:30.000000 conflog-1.0.1/conflog/handlers/stream_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:41:19.042632 conflog-1.0.1/conflog/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-08 05:40:30.000000 conflog-1.0.1/conflog/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-08 05:40:30.000000 conflog-1.0.1/conflog/loaders/environ_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-08 05:40:30.000000 conflog-1.0.1/conflog/loaders/ini_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-08 05:40:30.000000 conflog-1.0.1/conflog/loaders/json_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-08 05:40:30.000000 conflog-1.0.1/conflog/loaders/xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-08 05:40:30.000000 conflog-1.0.1/conflog/loaders/yaml_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:41:19.038632 conflog-1.0.1/conflog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-06-08 05:41:18.000000 conflog-1.0.1/conflog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-08 05:41:18.000000 conflog-1.0.1/conflog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:41:18.000000 conflog-1.0.1/conflog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 05:41:18.000000 conflog-1.0.1/conflog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 05:41:19.042632 conflog-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-08 05:40:30.000000 conflog-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:41:19.042632 conflog-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 05:40:30.000000 conflog-1.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:41:19.042632 conflog-1.0.1/tests/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 05:40:30.000000 conflog-1.0.1/tests/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-08 05:40:30.000000 conflog-1.0.1/tests/handlers/test_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-08 05:40:30.000000 conflog-1.0.1/tests/handlers/test_stream_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:41:19.042632 conflog-1.0.1/tests/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 05:40:30.000000 conflog-1.0.1/tests/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-08 05:40:30.000000 conflog-1.0.1/tests/loaders/test_environ_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-08 05:40:30.000000 conflog-1.0.1/tests/loaders/test_ini_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-08 05:40:30.000000 conflog-1.0.1/tests/loaders/test_json_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-08 05:40:30.000000 conflog-1.0.1/tests/loaders/test_xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-08 05:40:30.000000 conflog-1.0.1/tests/loaders/test_yaml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-06-08 05:40:30.000000 conflog-1.0.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-08 05:40:30.000000 conflog-1.0.1/tests/test_conflog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:02:31.727089 conflog-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-14 02:01:35.000000 conflog-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-14 02:02:31.723089 conflog-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-14 02:01:35.000000 conflog-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:02:31.723089 conflog-1.1.0/conflog/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:02:31.723089 conflog-1.1.0/conflog/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/handlers/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/handlers/stream_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:02:31.723089 conflog-1.1.0/conflog/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/loaders/environ_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/loaders/ini_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/loaders/json_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/loaders/xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-14 02:01:35.000000 conflog-1.1.0/conflog/loaders/yaml_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:02:31.723089 conflog-1.1.0/conflog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-14 02:02:31.000000 conflog-1.1.0/conflog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-14 02:02:31.000000 conflog-1.1.0/conflog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 02:02:31.000000 conflog-1.1.0/conflog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 02:02:31.000000 conflog-1.1.0/conflog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 02:02:31.000000 conflog-1.1.0/conflog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 02:02:31.727089 conflog-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-14 02:01:35.000000 conflog-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:02:31.723089 conflog-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:02:31.723089 conflog-1.1.0/tests/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/handlers/test_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/handlers/test_stream_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:02:31.723089 conflog-1.1.0/tests/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/loaders/test_environ_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/loaders/test_ini_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/loaders/test_json_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/loaders/test_xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/loaders/test_yaml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-14 02:01:35.000000 conflog-1.1.0/tests/test_conflog.py
```

### Comparing `conflog-1.0.1/LICENSE` & `conflog-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conflog-1.0.1/PKG-INFO` & `conflog-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conflog
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python logging setup via environment variables and configuration files
 Home-page: https://github.com/cliffano/pyconflog
 Author: Cliffano Subagio
 Author-email: cliffano@gmail.com
 Keywords: log,logger,logging,config,configuration,environment,envvar,ini,json,xml,yaml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img align="right" src="https://raw.github.com/cliffano/pyconflog/main/avatar.jpg" alt="Avatar"/>
 
 [![Build Status](https://github.com/cliffano/pyconflog/workflows/CI/badge.svg)](https://github.com/cliffano/pyconflog/actions?query=workflow%3ACI)
 [![Vulnerabilities Status](https://snyk.io/test/github/cliffano/pyconflog/badge.svg)](https://snyk.io/test/github/cliffano/pyconflog)
-[![Published Version](https://img.shields.io/pypi/v/pyconflog.svg)](https://pypi.python.org/pypi/pyconflog)
+[![Published Version](https://img.shields.io/pypi/v/conflog.svg)](https://pypi.python.org/pypi/conflog)
 <br/>
 
 Pyconflog
 ---------
 
 Pyconflog library provides Python logging setup via environment variables and configuration files.
```

### Comparing `conflog-1.0.1/README.md` & `conflog-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <img align="right" src="https://raw.github.com/cliffano/pyconflog/main/avatar.jpg" alt="Avatar"/>
 
 [![Build Status](https://github.com/cliffano/pyconflog/workflows/CI/badge.svg)](https://github.com/cliffano/pyconflog/actions?query=workflow%3ACI)
 [![Vulnerabilities Status](https://snyk.io/test/github/cliffano/pyconflog/badge.svg)](https://snyk.io/test/github/cliffano/pyconflog)
-[![Published Version](https://img.shields.io/pypi/v/pyconflog.svg)](https://pypi.python.org/pypi/pyconflog)
+[![Published Version](https://img.shields.io/pypi/v/conflog.svg)](https://pypi.python.org/pypi/conflog)
 <br/>
 
 Pyconflog
 ---------
 
 Pyconflog library provides Python logging setup via environment variables and configuration files.
```

### Comparing `conflog-1.0.1/conflog/__init__.py` & `conflog-1.1.0/conflog/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,25 +21,25 @@
     def __init__(self, conf_files=None):
         """Initialise Python logging with configuration from conf_files.
         """
 
         if isinstance(conf_files, str):
             conf_files = [conf_files]
 
-        config = Config(conf_files=conf_files)
-        handlers = config.get_handlers()
-        datefmt = config.get_datefmt()
-        level = config.get_level()
-        self.extras = config.get_extras()
+        self.config = Config(conf_files=conf_files)
+        handlers = self.config.get_handlers()
+        datefmt = self.config.get_datefmt()
+        level = self.config.get_level()
+        self.extras = self.config.get_extras()
 
         self.handlers = []
         if 'stream' in handlers:
-            self.handlers.append(init_stream_handler(config))
+            self.handlers.append(init_stream_handler(self.config))
         if 'file' in handlers:
-            self.handlers.append(init_file_handler(config))
+            self.handlers.append(init_file_handler(self.config))
 
         logging.basicConfig(
             datefmt=datefmt,
             level=level
         )
 
     def get_logger(self, name):
@@ -58,7 +58,12 @@
         """Close logger handlers
         and clear the handlers from logger.
         """
         logger = logging.getLogger(name)
         for handler in logger.handlers:
             handler.close()
         logger.handlers.clear()
+
+    def get_config_properties(self):
+        """Get the configuration properties dictionary.
+        """
+        return self.config.conf
```

### Comparing `conflog-1.0.1/conflog/config.py` & `conflog-1.1.0/conflog/config.py`

 * *Files identical despite different names*

### Comparing `conflog-1.0.1/conflog/loaders/ini_loader.py` & `conflog-1.1.0/conflog/loaders/ini_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.0.1/conflog.egg-info/PKG-INFO` & `conflog-1.1.0/conflog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conflog
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python logging setup via environment variables and configuration files
 Home-page: https://github.com/cliffano/pyconflog
 Author: Cliffano Subagio
 Author-email: cliffano@gmail.com
 Keywords: log,logger,logging,config,configuration,environment,envvar,ini,json,xml,yaml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img align="right" src="https://raw.github.com/cliffano/pyconflog/main/avatar.jpg" alt="Avatar"/>
 
 [![Build Status](https://github.com/cliffano/pyconflog/workflows/CI/badge.svg)](https://github.com/cliffano/pyconflog/actions?query=workflow%3ACI)
 [![Vulnerabilities Status](https://snyk.io/test/github/cliffano/pyconflog/badge.svg)](https://snyk.io/test/github/cliffano/pyconflog)
-[![Published Version](https://img.shields.io/pypi/v/pyconflog.svg)](https://pypi.python.org/pypi/pyconflog)
+[![Published Version](https://img.shields.io/pypi/v/conflog.svg)](https://pypi.python.org/pypi/conflog)
 <br/>
 
 Pyconflog
 ---------
 
 Pyconflog library provides Python logging setup via environment variables and configuration files.
```

### Comparing `conflog-1.0.1/conflog.egg-info/SOURCES.txt` & `conflog-1.1.0/conflog.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 conflog/__init__.py
 conflog/config.py
 conflog.egg-info/PKG-INFO
 conflog.egg-info/SOURCES.txt
 conflog.egg-info/dependency_links.txt
+conflog.egg-info/requires.txt
 conflog.egg-info/top_level.txt
 conflog/handlers/__init__.py
 conflog/handlers/file_handler.py
 conflog/handlers/stream_handler.py
 conflog/loaders/__init__.py
 conflog/loaders/environ_loader.py
 conflog/loaders/ini_loader.py
```

### Comparing `conflog-1.0.1/setup.py` & `conflog-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,9 +26,10 @@
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.8',
     install_requires=[
+        'PyYAML==6.0'
     ],
 )
```

### Comparing `conflog-1.0.1/tests/handlers/test_file_handler.py` & `conflog-1.1.0/tests/handlers/test_file_handler.py`

 * *Files identical despite different names*

### Comparing `conflog-1.0.1/tests/handlers/test_stream_handler.py` & `conflog-1.1.0/tests/handlers/test_stream_handler.py`

 * *Files identical despite different names*

### Comparing `conflog-1.0.1/tests/loaders/test_environ_loader.py` & `conflog-1.1.0/tests/loaders/test_environ_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.0.1/tests/loaders/test_ini_loader.py` & `conflog-1.1.0/tests/loaders/test_ini_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.0.1/tests/loaders/test_json_loader.py` & `conflog-1.1.0/tests/loaders/test_json_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.0.1/tests/loaders/test_xml_loader.py` & `conflog-1.1.0/tests/loaders/test_xml_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.0.1/tests/loaders/test_yaml_loader.py` & `conflog-1.1.0/tests/loaders/test_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.0.1/tests/test_config.py` & `conflog-1.1.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `conflog-1.0.1/tests/test_conflog.py` & `conflog-1.1.0/tests/test_conflog.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,7 +57,10 @@
         self.assertFalse(mock_logger.propagate)
         mock_logger.addHandler.assert_any_call(mock_stream_handler)
         mock_logger.addHandler.assert_any_call(mock_file_handler)
 
         conflog.close_logger_handlers('someloggername')
         mock_stream_handler.close.assert_called_once_with()
         mock_file_handler.close.assert_called_once_with()
+
+        config = conflog.get_config_properties()
+        self.assertEqual(config, mock_config.conf)
```

