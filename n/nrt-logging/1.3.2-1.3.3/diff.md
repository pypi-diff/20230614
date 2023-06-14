# Comparing `tmp/nrt-logging-1.3.2.tar.gz` & `tmp/nrt-logging-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrt-logging-1.3.2.tar", last modified: Sat Dec 10 22:25:57 2022, max compression
+gzip compressed data, was "nrt-logging-1.3.3.tar", last modified: Wed Jun 14 06:33:30 2023, max compression
```

## Comparing `nrt-logging-1.3.2.tar` & `nrt-logging-1.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-12-10 22:25:57.950848 nrt-logging-1.3.2/
--rw-rw-rw-   0        0        0     1088 2022-11-23 08:09:14.000000 nrt-logging-1.3.2/LICENSE.md
--rw-rw-rw-   0        0        0     7767 2022-12-10 22:25:57.947854 nrt-logging-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     6769 2022-11-23 08:09:14.000000 nrt-logging-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2022-12-10 22:25:57.927663 nrt-logging-1.3.2/nrt_logging/
--rw-rw-rw-   0        0        0      298 2022-12-04 20:21:20.000000 nrt-logging-1.3.2/nrt_logging/__init__.py
--rw-rw-rw-   0        0        0    14373 2022-11-23 08:09:14.000000 nrt-logging-1.3.2/nrt_logging/config.py
--rw-rw-rw-   0        0        0      237 2022-11-23 08:09:14.000000 nrt-logging-1.3.2/nrt_logging/exceptions.py
--rw-rw-rw-   0        0        0     1851 2022-11-23 08:09:14.000000 nrt-logging-1.3.2/nrt_logging/log_format.py
--rw-rw-rw-   0        0        0      990 2022-11-23 08:09:14.000000 nrt-logging-1.3.2/nrt_logging/log_level.py
--rw-rw-rw-   0        0        0     5905 2022-11-26 09:18:33.000000 nrt-logging-1.3.2/nrt_logging/logger.py
--rw-rw-rw-   0        0        0    11456 2022-11-26 18:50:22.000000 nrt-logging-1.3.2/nrt_logging/logger_manager.py
--rw-rw-rw-   0        0        0    45309 2022-12-10 22:13:13.000000 nrt-logging-1.3.2/nrt_logging/logger_stream_handlers.py
-drwxrwxrwx   0        0        0        0 2022-12-10 22:25:57.945845 nrt-logging-1.3.2/nrt_logging.egg-info/
--rw-rw-rw-   0        0        0     7767 2022-12-10 22:25:57.000000 nrt-logging-1.3.2/nrt_logging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2022-12-10 22:25:57.000000 nrt-logging-1.3.2/nrt_logging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-10 22:25:57.000000 nrt-logging-1.3.2/nrt_logging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2022-12-10 22:25:57.000000 nrt-logging-1.3.2/nrt_logging.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-12-10 22:25:57.000000 nrt-logging-1.3.2/nrt_logging.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      983 2022-12-10 22:13:17.000000 nrt-logging-1.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       31 2022-11-23 08:09:14.000000 nrt-logging-1.3.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-12-10 22:25:57.950848 nrt-logging-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1236 2022-11-23 08:09:14.000000 nrt-logging-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:33:30.202990 nrt-logging-1.3.3/
+-rw-rw-rw-   0        0        0     1088 2022-11-23 08:09:14.000000 nrt-logging-1.3.3/LICENSE.md
+-rw-rw-rw-   0        0        0     7760 2023-06-14 06:33:30.202990 nrt-logging-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6762 2023-06-14 06:13:12.000000 nrt-logging-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 06:33:30.196476 nrt-logging-1.3.3/nrt_logging/
+-rw-rw-rw-   0        0        0      298 2023-06-14 06:13:43.000000 nrt-logging-1.3.3/nrt_logging/__init__.py
+-rw-rw-rw-   0        0        0    14373 2022-11-23 08:09:14.000000 nrt-logging-1.3.3/nrt_logging/config.py
+-rw-rw-rw-   0        0        0      237 2022-11-23 08:09:14.000000 nrt-logging-1.3.3/nrt_logging/exceptions.py
+-rw-rw-rw-   0        0        0     1851 2022-11-23 08:09:14.000000 nrt-logging-1.3.3/nrt_logging/log_format.py
+-rw-rw-rw-   0        0        0      990 2022-11-23 08:09:14.000000 nrt-logging-1.3.3/nrt_logging/log_level.py
+-rw-rw-rw-   0        0        0     5905 2022-11-26 09:18:33.000000 nrt-logging-1.3.3/nrt_logging/logger.py
+-rw-rw-rw-   0        0        0    11456 2022-11-26 18:50:22.000000 nrt-logging-1.3.3/nrt_logging/logger_manager.py
+-rw-rw-rw-   0        0        0    45309 2022-12-10 22:13:13.000000 nrt-logging-1.3.3/nrt_logging/logger_stream_handlers.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:33:30.201990 nrt-logging-1.3.3/nrt_logging.egg-info/
+-rw-rw-rw-   0        0        0     7760 2023-06-14 06:33:30.000000 nrt-logging-1.3.3/nrt_logging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-06-14 06:33:30.000000 nrt-logging-1.3.3/nrt_logging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 06:33:30.000000 nrt-logging-1.3.3/nrt_logging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-14 06:33:30.000000 nrt-logging-1.3.3/nrt_logging.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-14 06:33:30.000000 nrt-logging-1.3.3/nrt_logging.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      983 2023-06-14 06:14:10.000000 nrt-logging-1.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       31 2022-11-23 08:09:14.000000 nrt-logging-1.3.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 06:33:30.202990 nrt-logging-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1236 2022-11-23 08:09:14.000000 nrt-logging-1.3.3/setup.py
```

### Comparing `nrt-logging-1.3.2/LICENSE.md` & `nrt-logging-1.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nrt-logging-1.3.2/PKG-INFO` & `nrt-logging-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrt-logging
-Version: 1.3.2
+Version: 1.3.3
 Summary: Hierarchical logging in yaml format
 Home-page: https://github.com/etuzon/Python-NRT-Logging
 Author: Eyal Tuzon
 Author-email: Eyal Tuzon <eyal.tuzon.dev@gmail.com>
 Project-URL: Homepage, https://github.com/etuzon/Python-NRT-Logging
 Project-URL: Bug Tracker, https://github.com/etuzon/Python-NRT-Logging/issues
 Project-URL: documentation, https://github.com/etuzon/Python-NRT-Logging/wiki
@@ -240,9 +240,9 @@
 
 
 CONFIG_FILE_PATH = './config/config1.yaml'
 
 logger_manager.set_config(file_path=CONFIG_FILE_PATH)
 ```
 
-Wiki: https://github.com/etuzon/Python-NRT-Logging/wiki
+Wiki: https://github.com/etuzon/nrt-logging/wiki
```

### Comparing `nrt-logging-1.3.2/README.md` & `nrt-logging-1.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -219,9 +219,9 @@
 
 
 CONFIG_FILE_PATH = './config/config1.yaml'
 
 logger_manager.set_config(file_path=CONFIG_FILE_PATH)
 ```
 
-Wiki: https://github.com/etuzon/Python-NRT-Logging/wiki
+Wiki: https://github.com/etuzon/nrt-logging/wiki
```

### Comparing `nrt-logging-1.3.2/nrt_logging/config.py` & `nrt-logging-1.3.3/nrt_logging/config.py`

 * *Files identical despite different names*

### Comparing `nrt-logging-1.3.2/nrt_logging/log_format.py` & `nrt-logging-1.3.3/nrt_logging/log_format.py`

 * *Files identical despite different names*

### Comparing `nrt-logging-1.3.2/nrt_logging/log_level.py` & `nrt-logging-1.3.3/nrt_logging/log_level.py`

 * *Files identical despite different names*

### Comparing `nrt-logging-1.3.2/nrt_logging/logger.py` & `nrt-logging-1.3.3/nrt_logging/logger.py`

 * *Files identical despite different names*

### Comparing `nrt-logging-1.3.2/nrt_logging/logger_manager.py` & `nrt-logging-1.3.3/nrt_logging/logger_manager.py`

 * *Files identical despite different names*

### Comparing `nrt-logging-1.3.2/nrt_logging/logger_stream_handlers.py` & `nrt-logging-1.3.3/nrt_logging/logger_stream_handlers.py`

 * *Files identical despite different names*

### Comparing `nrt-logging-1.3.2/nrt_logging.egg-info/PKG-INFO` & `nrt-logging-1.3.3/nrt_logging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrt-logging
-Version: 1.3.2
+Version: 1.3.3
 Summary: Hierarchical logging in yaml format
 Home-page: https://github.com/etuzon/Python-NRT-Logging
 Author: Eyal Tuzon
 Author-email: Eyal Tuzon <eyal.tuzon.dev@gmail.com>
 Project-URL: Homepage, https://github.com/etuzon/Python-NRT-Logging
 Project-URL: Bug Tracker, https://github.com/etuzon/Python-NRT-Logging/issues
 Project-URL: documentation, https://github.com/etuzon/Python-NRT-Logging/wiki
@@ -240,9 +240,9 @@
 
 
 CONFIG_FILE_PATH = './config/config1.yaml'
 
 logger_manager.set_config(file_path=CONFIG_FILE_PATH)
 ```
 
-Wiki: https://github.com/etuzon/Python-NRT-Logging/wiki
+Wiki: https://github.com/etuzon/nrt-logging/wiki
```

### Comparing `nrt-logging-1.3.2/pyproject.toml` & `nrt-logging-1.3.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name='nrt-logging'
-version='1.3.2'
+version='1.3.3'
 authors=[
 { name='Eyal Tuzon', email='eyal.tuzon.dev@gmail.com' },
 ]
 description='Hierarchical logging in yaml format'
 keywords=[
 'python', 'python3', 'python-3', 'logging', 'logger', 'log', 'loggers',
 'hierarchical', 'logging-library', 'logging-framework', 'hierarchy', 'yaml',
```

### Comparing `nrt-logging-1.3.2/setup.py` & `nrt-logging-1.3.3/setup.py`

 * *Files identical despite different names*

