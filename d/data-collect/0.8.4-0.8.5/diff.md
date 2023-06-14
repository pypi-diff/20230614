# Comparing `tmp/data_collect-0.8.4.tar.gz` & `tmp/data_collect-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_collect-0.8.4.tar", last modified: Tue Jun  6 18:06:20 2023, max compression
+gzip compressed data, was "data_collect-0.8.5.tar", last modified: Wed Jun 14 19:29:49 2023, max compression
```

## Comparing `data_collect-0.8.4.tar` & `data_collect-0.8.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-06 18:06:20.109643 data_collect-0.8.4/
--rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-06 18:06:20.109719 data_collect-0.8.4/PKG-INFO
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-06 18:06:20.108112 data_collect-0.8.4/data_collect/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.4/data_collect/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)    12320 2023-06-06 18:04:44.000000 data_collect-0.8.4/data_collect/client.py
--rw-r--r--   0 jojo       (501) staff       (20)     1097 2023-04-11 15:51:48.000000 data_collect-0.8.4/data_collect/constants.py
--rw-r--r--   0 jojo       (501) staff       (20)      283 2023-04-11 15:51:48.000000 data_collect-0.8.4/data_collect/correlation_id.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-06 18:06:20.109499 data_collect-0.8.4/data_collect/data_types/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.4/data_collect/data_types/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)      544 2023-04-11 15:51:48.000000 data_collect-0.8.4/data_collect/data_types/blob.py
--rw-r--r--   0 jojo       (501) staff       (20)     3438 2023-05-08 13:37:11.000000 data_collect-0.8.4/data_collect/data_types/image.py
--rw-r--r--   0 jojo       (501) staff       (20)      394 2023-04-11 15:51:48.000000 data_collect-0.8.4/data_collect/data_types/text.py
--rw-r--r--   0 jojo       (501) staff       (20)     7755 2023-06-06 18:04:24.000000 data_collect-0.8.4/data_collect/logger.py
--rw-r--r--   0 jojo       (501) staff       (20)     5564 2023-05-08 13:37:11.000000 data_collect-0.8.4/data_collect/queue.py
--rw-r--r--   0 jojo       (501) staff       (20)      179 2023-04-12 08:56:34.000000 data_collect-0.8.4/data_collect/setup.py
--rw-r--r--   0 jojo       (501) staff       (20)     6629 2023-05-08 13:37:11.000000 data_collect-0.8.4/data_collect/thread.py
--rw-r--r--   0 jojo       (501) staff       (20)     1108 2023-04-11 15:51:48.000000 data_collect-0.8.4/data_collect/utils.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-06 18:06:20.108930 data_collect-0.8.4/data_collect.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-06 18:06:20.000000 data_collect-0.8.4/data_collect.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)      582 2023-06-06 18:06:20.000000 data_collect-0.8.4/data_collect.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-06 18:06:20.000000 data_collect-0.8.4/data_collect.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-06 18:06:20.000000 data_collect-0.8.4/data_collect.egg-info/not-zip-safe
--rw-r--r--   0 jojo       (501) staff       (20)       75 2023-06-06 18:06:20.000000 data_collect-0.8.4/data_collect.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)       13 2023-06-06 18:06:20.000000 data_collect-0.8.4/data_collect.egg-info/top_level.txt
--rw-r--r--   0 jojo       (501) staff       (20)      720 2023-06-06 18:06:20.110112 data_collect-0.8.4/setup.cfg
--rw-r--r--   0 jojo       (501) staff       (20)      179 2023-06-06 18:06:19.000000 data_collect-0.8.4/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:29:49.952291 data_collect-0.8.5/
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:29:49.952385 data_collect-0.8.5/PKG-INFO
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:29:49.950629 data_collect-0.8.5/data_collect/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.5/data_collect/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)    12455 2023-06-14 19:28:58.000000 data_collect-0.8.5/data_collect/client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1097 2023-04-11 15:51:48.000000 data_collect-0.8.5/data_collect/constants.py
+-rw-r--r--   0 jojo       (501) staff       (20)      283 2023-04-11 15:51:48.000000 data_collect-0.8.5/data_collect/correlation_id.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:29:49.952105 data_collect-0.8.5/data_collect/data_types/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.5/data_collect/data_types/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:28:55.000000 data_collect-0.8.5/data_collect/data_types/blob.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3422 2023-06-14 19:28:53.000000 data_collect-0.8.5/data_collect/data_types/image.py
+-rw-r--r--   0 jojo       (501) staff       (20)      388 2023-06-14 19:28:54.000000 data_collect-0.8.5/data_collect/data_types/text.py
+-rw-r--r--   0 jojo       (501) staff       (20)     7430 2023-06-14 19:28:52.000000 data_collect-0.8.5/data_collect/logger.py
+-rw-r--r--   0 jojo       (501) staff       (20)     5564 2023-05-08 13:37:11.000000 data_collect-0.8.5/data_collect/queue.py
+-rw-r--r--   0 jojo       (501) staff       (20)      179 2023-04-12 08:56:34.000000 data_collect-0.8.5/data_collect/setup.py
+-rw-r--r--   0 jojo       (501) staff       (20)     6629 2023-05-08 13:37:11.000000 data_collect-0.8.5/data_collect/thread.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1108 2023-04-11 15:51:48.000000 data_collect-0.8.5/data_collect/utils.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:29:49.951505 data_collect-0.8.5/data_collect.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:29:49.000000 data_collect-0.8.5/data_collect.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)      582 2023-06-14 19:29:49.000000 data_collect-0.8.5/data_collect.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-14 19:29:49.000000 data_collect-0.8.5/data_collect.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-14 19:29:49.000000 data_collect-0.8.5/data_collect.egg-info/not-zip-safe
+-rw-r--r--   0 jojo       (501) staff       (20)       75 2023-06-14 19:29:49.000000 data_collect-0.8.5/data_collect.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)       13 2023-06-14 19:29:49.000000 data_collect-0.8.5/data_collect.egg-info/top_level.txt
+-rw-r--r--   0 jojo       (501) staff       (20)      720 2023-06-14 19:29:49.952816 data_collect-0.8.5/setup.cfg
+-rw-r--r--   0 jojo       (501) staff       (20)      179 2023-06-14 19:29:49.000000 data_collect-0.8.5/setup.py
```

### Comparing `data_collect-0.8.4/PKG-INFO` & `data_collect-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_collect
-Version: 0.8.4
+Version: 0.8.5
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `data_collect-0.8.4/data_collect/client.py` & `data_collect-0.8.5/data_collect/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         check is need print log
         :return:
         """
         return self.input_enable or \
             self.prediction_enable or \
             self.ground_truth_enable
 
-    def _gen_image_save_path(self, correlation_id: str, designation: str = '', metadata=None) -> str:
+    def gen_image_save_path(self, correlation_id: str, designation: str = '', metadata=None) -> str:
         """
         generate image tmp save dir as yyyy-MM-dd/hh
         :return:
         """
         # generate time directory
         if metadata is None:
             metadata = {}
@@ -197,15 +197,15 @@
         if image is not None and self.input_enable:
             self._log_image(correlation_id, image, designation)
 
         if blob is not None and self._is_data_capture_enable():
             self._log_blob(correlation_id, blob, designation)
 
         if self._is_data_capture_enable() and message is not None:
-            self._logger.log(correlation_id, message)
+            self._logger.log(message)
 
     def _load_env_setting_and_config(self, config: DataCollectConfig):
         """
         load env setting and config
         :param config:
         :return:
         """
@@ -278,29 +278,33 @@
                     - H x W x 3 (an RGB channel order is assumed)
                     - H x W x 4 (an RGBA channel order is assumed)
 
         :param correlation_id: Correlation ID of the image.
         :param image: Image to log.
         :param designation: Designation of the image.
         """
-        tmp_path = self._gen_image_save_path(correlation_id, designation, image.metadata)
-        self._image_logger.log(correlation_id, image, tmp_path)
+        if image.designation is None:
+            image.designation = self.gen_image_save_path(correlation_id, designation, image.metadata)
+        self._image_logger.log(image)
 
     def _log_blob(self, correlation_id: str, blob: WindmillBlob, designation: str = ''):
-        tmp_path = self._gen_blob_save_path(correlation_id, blob.metadata)
-        self._blob_logger.log(correlation_id, blob, tmp_path)
+        if blob.designation is None:
+            blob.designation = self.gen_blob_save_path(correlation_id, designation, blob.metadata)
+        self._blob_logger.log(blob)
 
-    def _gen_blob_save_path(self, correlation_id: str, metadata: Dict = None):
+    def gen_blob_save_path(self, correlation_id: str, designation: str = '', metadata=None) -> str:
         """
         generate blob save path
         :param correlation_id:
         :return:
         """
         time_tuple = time.localtime(int(time.time()))
-        dir_name = os.path.join(f"{self.blob_path}/{DEFAULT_CAPTURE_INPUT_DESIGNATION}",
+        if len(designation) == 0:
+            designation = DEFAULT_CAPTURE_INPUT_DESIGNATION
+        dir_name = os.path.join(f"{self.blob_path}/{designation}",
                                 time.strftime(TIME_DIRECTORY_FORMAT, time_tuple))
         if not os.path.exists(dir_name):
             os.makedirs(dir_name)
         content_type = metadata.get("content_type", "application/octet-stream") \
             if metadata is not None else "application/octet-stream"
         ext = mimetypes.guess_extension(content_type)
         extension = ext if ext is not None else "bin"
```

### Comparing `data_collect-0.8.4/data_collect/constants.py` & `data_collect-0.8.5/data_collect/constants.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.4/data_collect/data_types/image.py` & `data_collect-0.8.5/data_collect/data_types/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 
 from .blob import Blob
 
 
 class Image(Blob):
     def __init__(self,
                  data: Union[np.ndarray, PIL.Image.Image],
-                 correlation_id: str = '',
+                 designation: str = '',
                  metadata=None
                  ) -> None:
         """
         :param data: image data
-        :param correlation_id: correlation id
+        :param save_path: save_path
         :param metadata: metadata
         """
-        super().__init__(data, correlation_id, metadata)
+        super().__init__(data, designation, metadata)
 
     def covert_to_rgb(self):
         """
         covert to rgb
         """
         self.data = np.asarray(self.data)
         # pillow image mode P covert to RGB 需要特别处理
```

### Comparing `data_collect-0.8.4/data_collect/logger.py` & `data_collect-0.8.5/data_collect/logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,20 +36,20 @@
         from data_collect.thread import MultiThread
         self._thread = MultiThread(self._process,
                                    self._queue,
                                    name=self.__class__.__name__,
                                    thread_count=1)
         self._thread.start()
 
-    def log(self, correlation_id: str, **kwargs):
+    def log(self, **kwargs):
         """ Log 
 
         Parameters
         ----------
-        correlation_id: str
+        designation: str
             The symbol of the log record
         """
         raise NotImplementedError
 
     def _process(self, queue):
         """ IO process to be run in a thread. get data from queue and save to disk.
 
@@ -73,35 +73,34 @@
     """
     图片日志类
     """
 
     def __init__(self, config: Dict = None):
         super().__init__(config)
 
-    def _save(self, designation: str, image: WindmillImage):
+    def _save(self, image: WindmillImage):
         """
         保存图片
         :param designation:
         :param image:
         :return:
         """
         try:
             if image.is_bytes():
-                with open(designation, "wb") as f:
+                with open(image.designation, "wb") as f:
                     f.write(image.data)
             else:
                 if "PIL" in sys.modules and image.is_pillow_image():
                     image.covert_to_rgb()
                 elif "numpy" in sys.modules and image.is_numpy_array():
                     image.covert_cv_image()
-                cv2.imwrite(designation, image.data)
+                cv2.imwrite(image.designation, image.data)
         except Exception as e:
             print(f"save image error: {e}")
         del image
-        del designation
 
     def _process(self, queue):
         """ Saves images from the save queue to the given params inside a thread.
 
         Parameters
         ----------
         queue: queue.Queue()
@@ -111,23 +110,20 @@
         while True:
             item = queue.get()
             if item == "EOF":
                 break
             executor.submit(self._save, *item)
         executor.shutdown()
 
-    def log(self,
-            correlation_id: str,
-            image: WindmillImage = None,
-            designation: str = ''):
+    def log(self, image: WindmillImage = None):
         """
         put params to queue
         """
         self._set_thread()
-        self._queue.put((designation, image))
+        self._queue.put((image))
 
     def close(self):
         """ Signal to the Save Threads that they should be closed and cleanly shutdown
         the saver """
         self._queue.put("EOF")
         super().close()
 
@@ -136,21 +132,23 @@
     """
     二进制文件类
     """
 
     def __init__(self, config: Dict = None):
         super().__init__(config)
 
-    def _save(self, designation, file_bytes):
+    def _save(self, blob: WindmillBlob):
         try:
-            with open(designation, "wb") as f:
-                f.write(file_bytes)
+            with open(blob.designation, "wb") as f:
+                f.write(blob.data)
         except Exception as e:
             print(f"save blob error: {e}")
-            
+        
+        del blob
+        
     def _process(self, queue):
         """ Saves blob from the save queue to the given params inside a thread.
 
         Parameters
         ----------
         queue: queue.Queue()
         """
@@ -158,27 +156,23 @@
         while True:
             item = queue.get()
             if item == "EOF":
                 break
             executor.submit(self._save, *item)
         executor.shutdown()
 
-    def log(self,
-            correlation_id: str,
-            blob: WindmillBlob = None,
-            designation: str = ''):
+    def log(self, blob: WindmillBlob = None):
         """main save function
 
         Args:
-            correlation_id (str): _description_
+            designation (str): _description_
             blob (WindmillBlob, optional): _description_. Defaults to None.
-            designation (str, optional): _description_. Defaults to ''.
         """
         self._set_thread()
-        self._queue.put((designation, blob.data))
+        self._queue.put((blob))
 
     def close(self):
         """ Signal to the Save Threads that they should be closed and cleanly shutdown
         the saver """
         self._queue.put("EOF")
         super().close()
 
@@ -228,15 +222,15 @@
             return int(self._rotation[:-2]) * 1024
         if self._rotation.endswith('MB'):
             return int(self._rotation[:-2]) * 1024 * 1024
         if self._rotation.endswith('GB'):
             return int(self._rotation[:-2]) * 1024 * 1024 * 1024
         return int(self._rotation)
 
-    def log(self, correlation_id: str, message=None):
+    def log(self, message):
         """main save function
 
         Args:
             correlation_id (str): _description_
             message (_type_, optional): _description_. Defaults to None.
         """
         if isinstance(message, dict):
```

### Comparing `data_collect-0.8.4/data_collect/queue.py` & `data_collect-0.8.5/data_collect/queue.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.4/data_collect/thread.py` & `data_collect-0.8.5/data_collect/thread.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.4/data_collect/utils.py` & `data_collect-0.8.5/data_collect/utils.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.4/data_collect.egg-info/PKG-INFO` & `data_collect-0.8.5/data_collect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-collect
-Version: 0.8.4
+Version: 0.8.5
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `data_collect-0.8.4/data_collect.egg-info/SOURCES.txt` & `data_collect-0.8.5/data_collect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.4/setup.cfg` & `data_collect-0.8.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = data_collect
 author = zhoubohan
 author_email = zhoubohan.pro@gmail.com
-version = 0.8.4
+version = 0.8.5
 description = project descriptions here
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://github.com/FlyTOmeLight
 license = MIT
 classifier = 
 	Programming Language :: Python
```

