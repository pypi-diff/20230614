# Comparing `tmp/data_collect-0.8.5.tar.gz` & `tmp/data_collect-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_collect-0.8.5.tar", last modified: Wed Jun 14 19:29:49 2023, max compression
+gzip compressed data, was "data_collect-0.8.6.tar", last modified: Wed Jun 14 19:39:43 2023, max compression
```

## Comparing `data_collect-0.8.5.tar` & `data_collect-0.8.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:29:49.952291 data_collect-0.8.5/
--rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:29:49.952385 data_collect-0.8.5/PKG-INFO
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:29:49.950629 data_collect-0.8.5/data_collect/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.5/data_collect/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)    12455 2023-06-14 19:28:58.000000 data_collect-0.8.5/data_collect/client.py
--rw-r--r--   0 jojo       (501) staff       (20)     1097 2023-04-11 15:51:48.000000 data_collect-0.8.5/data_collect/constants.py
--rw-r--r--   0 jojo       (501) staff       (20)      283 2023-04-11 15:51:48.000000 data_collect-0.8.5/data_collect/correlation_id.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:29:49.952105 data_collect-0.8.5/data_collect/data_types/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.5/data_collect/data_types/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:28:55.000000 data_collect-0.8.5/data_collect/data_types/blob.py
--rw-r--r--   0 jojo       (501) staff       (20)     3422 2023-06-14 19:28:53.000000 data_collect-0.8.5/data_collect/data_types/image.py
--rw-r--r--   0 jojo       (501) staff       (20)      388 2023-06-14 19:28:54.000000 data_collect-0.8.5/data_collect/data_types/text.py
--rw-r--r--   0 jojo       (501) staff       (20)     7430 2023-06-14 19:28:52.000000 data_collect-0.8.5/data_collect/logger.py
--rw-r--r--   0 jojo       (501) staff       (20)     5564 2023-05-08 13:37:11.000000 data_collect-0.8.5/data_collect/queue.py
--rw-r--r--   0 jojo       (501) staff       (20)      179 2023-04-12 08:56:34.000000 data_collect-0.8.5/data_collect/setup.py
--rw-r--r--   0 jojo       (501) staff       (20)     6629 2023-05-08 13:37:11.000000 data_collect-0.8.5/data_collect/thread.py
--rw-r--r--   0 jojo       (501) staff       (20)     1108 2023-04-11 15:51:48.000000 data_collect-0.8.5/data_collect/utils.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:29:49.951505 data_collect-0.8.5/data_collect.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:29:49.000000 data_collect-0.8.5/data_collect.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)      582 2023-06-14 19:29:49.000000 data_collect-0.8.5/data_collect.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-14 19:29:49.000000 data_collect-0.8.5/data_collect.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-14 19:29:49.000000 data_collect-0.8.5/data_collect.egg-info/not-zip-safe
--rw-r--r--   0 jojo       (501) staff       (20)       75 2023-06-14 19:29:49.000000 data_collect-0.8.5/data_collect.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)       13 2023-06-14 19:29:49.000000 data_collect-0.8.5/data_collect.egg-info/top_level.txt
--rw-r--r--   0 jojo       (501) staff       (20)      720 2023-06-14 19:29:49.952816 data_collect-0.8.5/setup.cfg
--rw-r--r--   0 jojo       (501) staff       (20)      179 2023-06-14 19:29:49.000000 data_collect-0.8.5/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:39:43.767450 data_collect-0.8.6/
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:39:43.767538 data_collect-0.8.6/PKG-INFO
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:39:43.766057 data_collect-0.8.6/data_collect/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.6/data_collect/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)    12455 2023-06-14 19:36:27.000000 data_collect-0.8.6/data_collect/client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1097 2023-04-11 15:51:48.000000 data_collect-0.8.6/data_collect/constants.py
+-rw-r--r--   0 jojo       (501) staff       (20)      283 2023-04-11 15:51:48.000000 data_collect-0.8.6/data_collect/correlation_id.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:39:43.767212 data_collect-0.8.6/data_collect/data_types/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.6/data_collect/data_types/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:39:18.000000 data_collect-0.8.6/data_collect/data_types/blob.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3426 2023-06-14 19:39:14.000000 data_collect-0.8.6/data_collect/data_types/image.py
+-rw-r--r--   0 jojo       (501) staff       (20)      388 2023-06-14 19:28:54.000000 data_collect-0.8.6/data_collect/data_types/text.py
+-rw-r--r--   0 jojo       (501) staff       (20)     7416 2023-06-14 19:39:04.000000 data_collect-0.8.6/data_collect/logger.py
+-rw-r--r--   0 jojo       (501) staff       (20)     5564 2023-05-08 13:37:11.000000 data_collect-0.8.6/data_collect/queue.py
+-rw-r--r--   0 jojo       (501) staff       (20)      179 2023-04-12 08:56:34.000000 data_collect-0.8.6/data_collect/setup.py
+-rw-r--r--   0 jojo       (501) staff       (20)     6629 2023-05-08 13:37:11.000000 data_collect-0.8.6/data_collect/thread.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1108 2023-04-11 15:51:48.000000 data_collect-0.8.6/data_collect/utils.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:39:43.766760 data_collect-0.8.6/data_collect.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:39:43.000000 data_collect-0.8.6/data_collect.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)      582 2023-06-14 19:39:43.000000 data_collect-0.8.6/data_collect.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-14 19:39:43.000000 data_collect-0.8.6/data_collect.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-14 19:39:43.000000 data_collect-0.8.6/data_collect.egg-info/not-zip-safe
+-rw-r--r--   0 jojo       (501) staff       (20)       75 2023-06-14 19:39:43.000000 data_collect-0.8.6/data_collect.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)       13 2023-06-14 19:39:43.000000 data_collect-0.8.6/data_collect.egg-info/top_level.txt
+-rw-r--r--   0 jojo       (501) staff       (20)      720 2023-06-14 19:39:43.767954 data_collect-0.8.6/setup.cfg
+-rw-r--r--   0 jojo       (501) staff       (20)      179 2023-06-14 19:39:43.000000 data_collect-0.8.6/setup.py
```

### Comparing `data_collect-0.8.5/PKG-INFO` & `data_collect-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_collect
-Version: 0.8.5
+Version: 0.8.6
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `data_collect-0.8.5/data_collect/client.py` & `data_collect-0.8.6/data_collect/client.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.5/data_collect/constants.py` & `data_collect-0.8.6/data_collect/constants.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.5/data_collect/data_types/blob.py` & `data_collect-0.8.6/data_collect/data_types/blob.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.5/data_collect/data_types/image.py` & `data_collect-0.8.6/data_collect/data_types/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def __init__(self,
                  data: Union[np.ndarray, PIL.Image.Image],
                  designation: str = '',
                  metadata=None
                  ) -> None:
         """
         :param data: image data
-        :param save_path: save_path
+        :param designation: designation
         :param metadata: metadata
         """
         super().__init__(data, designation, metadata)
 
     def covert_to_rgb(self):
         """
         covert to rgb
```

### Comparing `data_collect-0.8.5/data_collect/logger.py` & `data_collect-0.8.6/data_collect/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,20 +110,20 @@
         while True:
             item = queue.get()
             if item == "EOF":
                 break
             executor.submit(self._save, *item)
         executor.shutdown()
 
-    def log(self, image: WindmillImage = None):
+    def log(self, image: WindmillImage):
         """
         put params to queue
         """
         self._set_thread()
-        self._queue.put((image))
+        self._queue.put([image])
 
     def close(self):
         """ Signal to the Save Threads that they should be closed and cleanly shutdown
         the saver """
         self._queue.put("EOF")
         super().close()
 
@@ -156,23 +156,23 @@
         while True:
             item = queue.get()
             if item == "EOF":
                 break
             executor.submit(self._save, *item)
         executor.shutdown()
 
-    def log(self, blob: WindmillBlob = None):
+    def log(self, blob: WindmillBlob):
         """main save function
 
         Args:
             designation (str): _description_
             blob (WindmillBlob, optional): _description_. Defaults to None.
         """
         self._set_thread()
-        self._queue.put((blob))
+        self._queue.put([blob])
 
     def close(self):
         """ Signal to the Save Threads that they should be closed and cleanly shutdown
         the saver """
         self._queue.put("EOF")
         super().close()
```

### Comparing `data_collect-0.8.5/data_collect/queue.py` & `data_collect-0.8.6/data_collect/queue.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.5/data_collect/thread.py` & `data_collect-0.8.6/data_collect/thread.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.5/data_collect/utils.py` & `data_collect-0.8.6/data_collect/utils.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.5/data_collect.egg-info/PKG-INFO` & `data_collect-0.8.6/data_collect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-collect
-Version: 0.8.5
+Version: 0.8.6
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `data_collect-0.8.5/data_collect.egg-info/SOURCES.txt` & `data_collect-0.8.6/data_collect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.5/setup.cfg` & `data_collect-0.8.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = data_collect
 author = zhoubohan
 author_email = zhoubohan.pro@gmail.com
-version = 0.8.5
+version = 0.8.6
 description = project descriptions here
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://github.com/FlyTOmeLight
 license = MIT
 classifier = 
 	Programming Language :: Python
```

