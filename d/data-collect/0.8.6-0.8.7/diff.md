# Comparing `tmp/data_collect-0.8.6.tar.gz` & `tmp/data_collect-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_collect-0.8.6.tar", last modified: Wed Jun 14 19:39:43 2023, max compression
+gzip compressed data, was "data_collect-0.8.7.tar", last modified: Wed Jun 14 19:46:33 2023, max compression
```

## Comparing `data_collect-0.8.6.tar` & `data_collect-0.8.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:39:43.767450 data_collect-0.8.6/
--rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:39:43.767538 data_collect-0.8.6/PKG-INFO
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:39:43.766057 data_collect-0.8.6/data_collect/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.6/data_collect/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)    12455 2023-06-14 19:36:27.000000 data_collect-0.8.6/data_collect/client.py
--rw-r--r--   0 jojo       (501) staff       (20)     1097 2023-04-11 15:51:48.000000 data_collect-0.8.6/data_collect/constants.py
--rw-r--r--   0 jojo       (501) staff       (20)      283 2023-04-11 15:51:48.000000 data_collect-0.8.6/data_collect/correlation_id.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:39:43.767212 data_collect-0.8.6/data_collect/data_types/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.6/data_collect/data_types/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:39:18.000000 data_collect-0.8.6/data_collect/data_types/blob.py
--rw-r--r--   0 jojo       (501) staff       (20)     3426 2023-06-14 19:39:14.000000 data_collect-0.8.6/data_collect/data_types/image.py
--rw-r--r--   0 jojo       (501) staff       (20)      388 2023-06-14 19:28:54.000000 data_collect-0.8.6/data_collect/data_types/text.py
--rw-r--r--   0 jojo       (501) staff       (20)     7416 2023-06-14 19:39:04.000000 data_collect-0.8.6/data_collect/logger.py
--rw-r--r--   0 jojo       (501) staff       (20)     5564 2023-05-08 13:37:11.000000 data_collect-0.8.6/data_collect/queue.py
--rw-r--r--   0 jojo       (501) staff       (20)      179 2023-04-12 08:56:34.000000 data_collect-0.8.6/data_collect/setup.py
--rw-r--r--   0 jojo       (501) staff       (20)     6629 2023-05-08 13:37:11.000000 data_collect-0.8.6/data_collect/thread.py
--rw-r--r--   0 jojo       (501) staff       (20)     1108 2023-04-11 15:51:48.000000 data_collect-0.8.6/data_collect/utils.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:39:43.766760 data_collect-0.8.6/data_collect.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:39:43.000000 data_collect-0.8.6/data_collect.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)      582 2023-06-14 19:39:43.000000 data_collect-0.8.6/data_collect.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-14 19:39:43.000000 data_collect-0.8.6/data_collect.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-14 19:39:43.000000 data_collect-0.8.6/data_collect.egg-info/not-zip-safe
--rw-r--r--   0 jojo       (501) staff       (20)       75 2023-06-14 19:39:43.000000 data_collect-0.8.6/data_collect.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)       13 2023-06-14 19:39:43.000000 data_collect-0.8.6/data_collect.egg-info/top_level.txt
--rw-r--r--   0 jojo       (501) staff       (20)      720 2023-06-14 19:39:43.767954 data_collect-0.8.6/setup.cfg
--rw-r--r--   0 jojo       (501) staff       (20)      179 2023-06-14 19:39:43.000000 data_collect-0.8.6/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:46:33.517897 data_collect-0.8.7/
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:46:33.517991 data_collect-0.8.7/PKG-INFO
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:46:33.515792 data_collect-0.8.7/data_collect/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.7/data_collect/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)    12648 2023-06-14 19:46:12.000000 data_collect-0.8.7/data_collect/client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1097 2023-04-11 15:51:48.000000 data_collect-0.8.7/data_collect/constants.py
+-rw-r--r--   0 jojo       (501) staff       (20)      283 2023-04-11 15:51:48.000000 data_collect-0.8.7/data_collect/correlation_id.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:46:33.517606 data_collect-0.8.7/data_collect/data_types/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.7/data_collect/data_types/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:41:14.000000 data_collect-0.8.7/data_collect/data_types/blob.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3426 2023-06-14 19:39:14.000000 data_collect-0.8.7/data_collect/data_types/image.py
+-rw-r--r--   0 jojo       (501) staff       (20)      388 2023-06-14 19:28:54.000000 data_collect-0.8.7/data_collect/data_types/text.py
+-rw-r--r--   0 jojo       (501) staff       (20)     7416 2023-06-14 19:39:04.000000 data_collect-0.8.7/data_collect/logger.py
+-rw-r--r--   0 jojo       (501) staff       (20)     5564 2023-05-08 13:37:11.000000 data_collect-0.8.7/data_collect/queue.py
+-rw-r--r--   0 jojo       (501) staff       (20)      179 2023-04-12 08:56:34.000000 data_collect-0.8.7/data_collect/setup.py
+-rw-r--r--   0 jojo       (501) staff       (20)     6629 2023-05-08 13:37:11.000000 data_collect-0.8.7/data_collect/thread.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1108 2023-04-11 15:51:48.000000 data_collect-0.8.7/data_collect/utils.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:46:33.516601 data_collect-0.8.7/data_collect.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:46:33.000000 data_collect-0.8.7/data_collect.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)      582 2023-06-14 19:46:33.000000 data_collect-0.8.7/data_collect.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-14 19:46:33.000000 data_collect-0.8.7/data_collect.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-14 19:46:33.000000 data_collect-0.8.7/data_collect.egg-info/not-zip-safe
+-rw-r--r--   0 jojo       (501) staff       (20)       75 2023-06-14 19:46:33.000000 data_collect-0.8.7/data_collect.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)       13 2023-06-14 19:46:33.000000 data_collect-0.8.7/data_collect.egg-info/top_level.txt
+-rw-r--r--   0 jojo       (501) staff       (20)      720 2023-06-14 19:46:33.518445 data_collect-0.8.7/setup.cfg
+-rw-r--r--   0 jojo       (501) staff       (20)      179 2023-06-14 19:46:32.000000 data_collect-0.8.7/setup.py
```

### Comparing `data_collect-0.8.6/PKG-INFO` & `data_collect-0.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_collect
-Version: 0.8.6
+Version: 0.8.7
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `data_collect-0.8.6/data_collect/client.py` & `data_collect-0.8.7/data_collect/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 
     def log(self,
             correlation_id: str,
             logline: Dict[str, Any] = None,
             designation: str = '',
             text: Sequence = None,
             time_series: Sequence = None,
+            file_paths: Union[Dict, List, str] = None,
             image: WindmillImage = None,
             blob: Union[WindmillText, WindmillBlob] = None,
             prediction: Union[Dict, List, str] = None,
             ground_truth: Union[Dict, List] = None,
             config: DataCollectConfig = None,
             ):
         """
@@ -195,15 +196,18 @@
             message['ground_truth'] = ground_truth if isinstance(ground_truth, str) else json.dumps(ground_truth,
                                                                                                     cls=NpEncoder)
         if image is not None and self.input_enable:
             self._log_image(correlation_id, image, designation)
 
         if blob is not None and self._is_data_capture_enable():
             self._log_blob(correlation_id, blob, designation)
-
+        
+        if file_paths is not None and self._is_data_capture_enable():
+            message['file_paths'] = file_paths
+            
         if self._is_data_capture_enable() and message is not None:
             self._logger.log(message)
 
     def _load_env_setting_and_config(self, config: DataCollectConfig):
         """
         load env setting and config
         :param config:
```

### Comparing `data_collect-0.8.6/data_collect/constants.py` & `data_collect-0.8.7/data_collect/constants.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.6/data_collect/data_types/blob.py` & `data_collect-0.8.7/data_collect/data_types/blob.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.6/data_collect/data_types/image.py` & `data_collect-0.8.7/data_collect/data_types/image.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.6/data_collect/logger.py` & `data_collect-0.8.7/data_collect/logger.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.6/data_collect/queue.py` & `data_collect-0.8.7/data_collect/queue.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.6/data_collect/thread.py` & `data_collect-0.8.7/data_collect/thread.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.6/data_collect/utils.py` & `data_collect-0.8.7/data_collect/utils.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.6/data_collect.egg-info/PKG-INFO` & `data_collect-0.8.7/data_collect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-collect
-Version: 0.8.6
+Version: 0.8.7
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `data_collect-0.8.6/data_collect.egg-info/SOURCES.txt` & `data_collect-0.8.7/data_collect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.6/setup.cfg` & `data_collect-0.8.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = data_collect
 author = zhoubohan
 author_email = zhoubohan.pro@gmail.com
-version = 0.8.6
+version = 0.8.7
 description = project descriptions here
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://github.com/FlyTOmeLight
 license = MIT
 classifier = 
 	Programming Language :: Python
```

