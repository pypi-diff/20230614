# Comparing `tmp/imerit-ango-1.1.4.1.tar.gz` & `tmp/imerit-ango-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imerit-ango-1.1.4.1.tar", last modified: Tue Jun 13 06:40:05 2023, max compression
+gzip compressed data, was "imerit-ango-1.1.5.tar", last modified: Wed Jun 14 14:31:32 2023, max compression
```

## Comparing `imerit-ango-1.1.4.1.tar` & `imerit-ango-1.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-13 06:40:05.349372 imerit-ango-1.1.4.1/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1667 2023-06-13 06:40:05.349372 imerit-ango-1.1.4.1/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 imerit-ango-1.1.4.1/README.md
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-13 06:40:05.349372 imerit-ango-1.1.4.1/imerit_ango/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-12 07:14:27.000000 imerit-ango-1.1.4.1/imerit_ango/__init__.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-13 06:40:05.349372 imerit-ango-1.1.4.1/imerit_ango/models/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-12 07:14:27.000000 imerit-ango-1.1.4.1/imerit_ango/models/__init__.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-06-12 07:14:27.000000 imerit-ango-1.1.4.1/imerit_ango/models/enums.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5452 2023-06-12 07:14:27.000000 imerit-ango-1.1.4.1/imerit_ango/models/label_category.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-06-12 07:14:27.000000 imerit-ango-1.1.4.1/imerit_ango/plugin_logger.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5840 2023-06-13 06:32:14.000000 imerit-ango-1.1.4.1/imerit_ango/plugins.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)    14443 2023-06-12 07:14:27.000000 imerit-ango-1.1.4.1/imerit_ango/sdk.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-13 06:40:05.349372 imerit-ango-1.1.4.1/imerit_ango.egg-info/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1667 2023-06-13 06:40:05.000000 imerit-ango-1.1.4.1/imerit_ango.egg-info/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      383 2023-06-13 06:40:05.000000 imerit-ango-1.1.4.1/imerit_ango.egg-info/SOURCES.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-13 06:40:05.000000 imerit-ango-1.1.4.1/imerit_ango.egg-info/dependency_links.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      137 2023-06-13 06:40:05.000000 imerit-ango-1.1.4.1/imerit_ango.egg-info/requires.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       12 2023-06-13 06:40:05.000000 imerit-ango-1.1.4.1/imerit_ango.egg-info/top_level.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-13 06:40:05.349372 imerit-ango-1.1.4.1/setup.cfg
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      894 2023-06-13 06:40:02.000000 imerit-ango-1.1.4.1/setup.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-14 14:31:32.191470 imerit-ango-1.1.5/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1665 2023-06-14 14:31:32.191470 imerit-ango-1.1.5/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 imerit-ango-1.1.5/README.md
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-14 14:31:32.191470 imerit-ango-1.1.5/imerit_ango/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-14 14:11:28.000000 imerit-ango-1.1.5/imerit_ango/__init__.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-14 14:31:32.191470 imerit-ango-1.1.5/imerit_ango/models/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-14 14:11:28.000000 imerit-ango-1.1.5/imerit_ango/models/__init__.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-06-14 14:11:28.000000 imerit-ango-1.1.5/imerit_ango/models/enums.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5452 2023-06-14 14:11:28.000000 imerit-ango-1.1.5/imerit_ango/models/label_category.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-06-14 14:11:28.000000 imerit-ango-1.1.5/imerit_ango/plugin_logger.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5865 2023-06-14 14:31:13.000000 imerit-ango-1.1.5/imerit_ango/plugins.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)    14443 2023-06-14 14:11:28.000000 imerit-ango-1.1.5/imerit_ango/sdk.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-14 14:31:32.191470 imerit-ango-1.1.5/imerit_ango.egg-info/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1665 2023-06-14 14:31:32.000000 imerit-ango-1.1.5/imerit_ango.egg-info/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      383 2023-06-14 14:31:32.000000 imerit-ango-1.1.5/imerit_ango.egg-info/SOURCES.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-14 14:31:32.000000 imerit-ango-1.1.5/imerit_ango.egg-info/dependency_links.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      137 2023-06-14 14:31:32.000000 imerit-ango-1.1.5/imerit_ango.egg-info/requires.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       12 2023-06-14 14:31:32.000000 imerit-ango-1.1.5/imerit_ango.egg-info/top_level.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-14 14:31:32.191470 imerit-ango-1.1.5/setup.cfg
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      892 2023-06-14 14:31:26.000000 imerit-ango-1.1.5/setup.py
```

### Comparing `imerit-ango-1.1.4.1/PKG-INFO` & `imerit-ango-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imerit-ango
-Version: 1.1.4.1
+Version: 1.1.5
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: imerit_ango,ango-hub,imerit_ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `imerit-ango-1.1.4.1/README.md` & `imerit-ango-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `imerit-ango-1.1.4.1/imerit_ango/models/label_category.py` & `imerit-ango-1.1.5/imerit_ango/models/label_category.py`

 * *Files identical despite different names*

### Comparing `imerit-ango-1.1.4.1/imerit_ango/plugin_logger.py` & `imerit-ango-1.1.5/imerit_ango/plugin_logger.py`

 * *Files identical despite different names*

### Comparing `imerit-ango-1.1.4.1/imerit_ango/plugins.py` & `imerit-ango-1.1.5/imerit_ango/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import datetime
 import logging
+import os
+import sys
 import time
 from io import BytesIO
 from typing import Callable, Tuple
 import queue
 import requests
 import socketio
 from apscheduler.schedulers.background import BackgroundScheduler
@@ -19,17 +21,17 @@
 
 class Plugin(socketio.ClientNamespace):
 
     def __init__(self, id: str, secret: str, callback: Callable):
         super().__init__('/plugin')
         self.id = id
         self.secret = secret
-        scheduler = BackgroundScheduler()
-        scheduler.add_job(self.heartbeat, 'interval', seconds=60)
-        scheduler.start()
+        self.scheduler = BackgroundScheduler()
+        self.scheduler.add_job(self.heartbeat, 'interval', seconds=5)
+        self.scheduler.start()
         self.logger = logging.getLogger()
         self.callback = callback
         self.loop = asyncio.get_event_loop()
 
     def on_connect(self):
         self.heartbeat()
         self.logger.warning("Connected")
@@ -38,15 +40,15 @@
         self.logger.warning("Disconnected")
 
     def heartbeat(self):
         try:
             self.emit('heartbeat', {"id": self.id, "secret": self.secret})
         except Exception as e:
             self.logger.fatal(e)
-            quit()
+            os._exit(1)
         self.logger.info("Heartbeat at %s" % str(time.time()))
 
     def on_plugin(self, data):
         data["logger"] = self._get_logger(data)
         data["batches"] = data.get('tags', [])
         response = {
             "response": self.callback(**data),
@@ -130,15 +132,15 @@
         if not workflow:
             return super().on_plugin(data)
         self.queue.put(data)
 
     def start(self):
         tasks = [self.work() for i in range(self.concurrency)]
         future = asyncio.gather(*tasks)
-        asyncio.get_event_loop().run_until_complete(future)
+        self.loop.run_until_complete(future)
 
 
 class FileExplorerPlugin(Plugin):
     def __init__(self, id: str, secret: str, callback: Callable):
         super().__init__(id, secret, callback)
```

### Comparing `imerit-ango-1.1.4.1/imerit_ango/sdk.py` & `imerit-ango-1.1.5/imerit_ango/sdk.py`

 * *Files identical despite different names*

### Comparing `imerit-ango-1.1.4.1/imerit_ango.egg-info/PKG-INFO` & `imerit-ango-1.1.5/imerit_ango.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imerit-ango
-Version: 1.1.4.1
+Version: 1.1.5
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: imerit_ango,ango-hub,imerit_ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `imerit-ango-1.1.4.1/setup.py` & `imerit-ango-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="imerit-ango",
-    version="1.1.4.1",
+    version="1.1.5",
     author="Faruk Karakaya",
     author_email="<faruk@ango.ai>",
     description="Ango-Hub SDK",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

