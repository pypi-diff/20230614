# Comparing `tmp/visioncar-0.1.5.tar.gz` & `tmp/visioncar-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visioncar-0.1.5.tar", last modified: Wed Jun 14 14:36:46 2023, max compression
+gzip compressed data, was "visioncar-0.1.6.tar", last modified: Wed Jun 14 16:57:22 2023, max compression
```

## Comparing `visioncar-0.1.5.tar` & `visioncar-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sh7dm     (1000) sh7dm     (1000)        0 2023-06-14 14:36:46.381747 visioncar-0.1.5/
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)     1077 2023-06-12 09:08:41.000000 visioncar-0.1.5/LICENSE
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       52 2023-06-12 09:08:41.000000 visioncar-0.1.5/MANIFEST.in
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      638 2023-06-14 14:36:46.381747 visioncar-0.1.5/PKG-INFO
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      269 2023-06-14 13:37:42.000000 visioncar-0.1.5/README.md
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       98 2023-06-12 09:08:41.000000 visioncar-0.1.5/pyproject.toml
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      112 2023-06-14 14:36:46.382747 visioncar-0.1.5/setup.cfg
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      848 2023-06-12 09:08:41.000000 visioncar-0.1.5/setup.py
-drwxr-xr-x   0 sh7dm     (1000) sh7dm     (1000)        0 2023-06-14 14:36:46.379747 visioncar-0.1.5/src/
-drwxr-xr-x   0 sh7dm     (1000) sh7dm     (1000)        0 2023-06-14 14:36:46.380747 visioncar-0.1.5/src/visioncar/
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       52 2023-06-14 13:37:46.000000 visioncar-0.1.5/src/visioncar/__init__.py
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)     2564 2023-06-14 14:26:22.000000 visioncar-0.1.5/src/visioncar/__main__.py
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)    18624 2023-06-14 14:26:16.000000 visioncar-0.1.5/src/visioncar/visioncar.py
-drwxr-xr-x   0 sh7dm     (1000) sh7dm     (1000)        0 2023-06-14 14:36:46.381747 visioncar-0.1.5/src/visioncar.egg-info/
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      638 2023-06-14 14:36:46.000000 visioncar-0.1.5/src/visioncar.egg-info/PKG-INFO
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      366 2023-06-14 14:36:46.000000 visioncar-0.1.5/src/visioncar.egg-info/SOURCES.txt
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)        1 2023-06-14 14:36:46.000000 visioncar-0.1.5/src/visioncar.egg-info/dependency_links.txt
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       49 2023-06-14 14:36:46.000000 visioncar-0.1.5/src/visioncar.egg-info/entry_points.txt
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       43 2023-06-14 14:36:46.000000 visioncar-0.1.5/src/visioncar.egg-info/requires.txt
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       10 2023-06-14 14:36:46.000000 visioncar-0.1.5/src/visioncar.egg-info/top_level.txt
+drwxr-xr-x   0 sh7dm     (1000) sh7dm     (1000)        0 2023-06-14 16:57:22.405486 visioncar-0.1.6/
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)     1077 2023-06-12 09:08:41.000000 visioncar-0.1.6/LICENSE
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       52 2023-06-12 09:08:41.000000 visioncar-0.1.6/MANIFEST.in
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      638 2023-06-14 16:57:22.405486 visioncar-0.1.6/PKG-INFO
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      269 2023-06-14 13:37:42.000000 visioncar-0.1.6/README.md
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       98 2023-06-12 09:08:41.000000 visioncar-0.1.6/pyproject.toml
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      112 2023-06-14 16:57:22.405486 visioncar-0.1.6/setup.cfg
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      848 2023-06-12 09:08:41.000000 visioncar-0.1.6/setup.py
+drwxr-xr-x   0 sh7dm     (1000) sh7dm     (1000)        0 2023-06-14 16:57:22.402486 visioncar-0.1.6/src/
+drwxr-xr-x   0 sh7dm     (1000) sh7dm     (1000)        0 2023-06-14 16:57:22.404486 visioncar-0.1.6/src/visioncar/
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       52 2023-06-14 16:54:02.000000 visioncar-0.1.6/src/visioncar/__init__.py
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)     2564 2023-06-14 14:26:22.000000 visioncar-0.1.6/src/visioncar/__main__.py
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)    18725 2023-06-14 16:51:24.000000 visioncar-0.1.6/src/visioncar/visioncar.py
+drwxr-xr-x   0 sh7dm     (1000) sh7dm     (1000)        0 2023-06-14 16:57:22.405486 visioncar-0.1.6/src/visioncar.egg-info/
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      638 2023-06-14 16:57:22.000000 visioncar-0.1.6/src/visioncar.egg-info/PKG-INFO
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      366 2023-06-14 16:57:22.000000 visioncar-0.1.6/src/visioncar.egg-info/SOURCES.txt
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)        1 2023-06-14 16:57:22.000000 visioncar-0.1.6/src/visioncar.egg-info/dependency_links.txt
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       49 2023-06-14 16:57:22.000000 visioncar-0.1.6/src/visioncar.egg-info/entry_points.txt
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       43 2023-06-14 16:57:22.000000 visioncar-0.1.6/src/visioncar.egg-info/requires.txt
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       10 2023-06-14 16:57:22.000000 visioncar-0.1.6/src/visioncar.egg-info/top_level.txt
```

### Comparing `visioncar-0.1.5/LICENSE` & `visioncar-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `visioncar-0.1.5/PKG-INFO` & `visioncar-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visioncar
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python library for controlling ESP32 robot
 Author: VisionCar team
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `visioncar-0.1.5/setup.py` & `visioncar-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `visioncar-0.1.5/src/visioncar/__main__.py` & `visioncar-0.1.6/src/visioncar/__main__.py`

 * *Files identical despite different names*

### Comparing `visioncar-0.1.5/src/visioncar/visioncar.py` & `visioncar-0.1.6/src/visioncar/visioncar.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import requests
 import threading
 import time
 import itertools
 import os
 import asyncio
 import simplejpeg
+import cv2
 
 TYPE_HTTP = '_ctl-http._tcp.local.'
 TYPE_MJPEG = '_mjpeg._udp.local.'
 TYPE_CTL = '_control-socket._udp.local.'
 
 class RobotProtocol:
 
@@ -57,15 +58,15 @@
             self.robot.in_buf = data
         else:
             self.robot.in_buf += data
 
         # JPEG file end, try parsing frame, swap if OK
         if n >= 2 and data[n - 2] == 0xff and data[n - 1] == 0xd9:
             try:
-                recv = simplejpeg.decode_jpeg(self.robot.in_buf, colorspace = "BGR")
+                recv = simplejpeg.decode_jpeg(self.robot.in_buf, colorspace = self.robot.colorspace)
                 if not len(recv):
                     if self.robot.verbose:
                         print("Frame is empty")
                     return
                 self.robot.fb = recv
                 ts = time.time()
                 self.robot.frametime = ts - self.robot.frame_ts
@@ -117,14 +118,15 @@
         self.vbatt = None
         self.als = None
         self.path = None
         self.verbose = False
         # Video window
         self._video_open = False
         self.video_thread = None
+        self.colorspace = "BGR"
 
     def from_zeroconf(http_info, mjpeg_info, ctl_info):
         h = None
         m = None
         ca = None
         cp = None
 
@@ -153,29 +155,30 @@
 
     def discover(hostname):
         """
         Takes robot hostname used to find in on network using Zeroconf
         :return: A new Robot instance
         """
         zc = AsyncZeroconf()
-        loop = asyncio.new_event_loop()
+        loop = asyncio.get_event_loop()
 
         http_info = None
         mjpeg_info = None
         ctl_info = None
 
         try:
             http_info = loop.run_until_complete(zc.async_get_service_info(
                 TYPE_HTTP, hostname + '.' + TYPE_HTTP))
             mjpeg_info = loop.run_until_complete(zc.async_get_service_info(
                 TYPE_MJPEG, hostname + '.' + TYPE_MJPEG))
             ctl_info = loop.run_until_complete(zc.async_get_service_info(
                 TYPE_CTL, hostname + '.' + TYPE_CTL))
         finally:
-            loop.run_until_complete(zc.async_close())
+            # For some reason, this can be very slow
+            # loop.run_until_complete(zc.async_close())
             loop.close()
 
         if not (http_info and mjpeg_info and ctl_info):
             print(f"Device {hostname} unavailable")
             return None
 
         return Robot.from_zeroconf(http_info, mjpeg_info, ctl_info)
@@ -345,15 +348,15 @@
             return True
 
     def open_camera(self):
         """
         Start the robot camera
         :return:
         """
-        if camera_thread:
+        if self.camera_thread:
             return
 
         loop = asyncio.new_event_loop()
         connect = loop.create_datagram_endpoint(
             lambda: CameraProtocol(self, loop),
             remote_addr=(self.mjpeg_addr, self.mjpeg_port))
         loop.run_until_complete(connect)
@@ -558,26 +561,26 @@
         end = time.time()
         if not ret or not "wsping" in ret:
             print("Ping error: " + str(ret))
             return -1
 
         return (end - start) * 1000
 
-    def _video_worker(_self):
+    def _video_worker(self):
         while True:
-            if _self.closing:
+            if self.closing:
                 return
 
             try:
-                frame = _self.capture()
+                frame = self.capture()
                 if not len(frame):
                     continue
 
                 cv2.imshow('Video', frame)
-                _self._video_open = True
+                self._video_open = True
             except Exception as e:
                 print('Capture error: ' + str(e))
                 return
 
             if cv2.waitKey(1) == 27:
                 return
 
@@ -587,15 +590,15 @@
         :return: True if opened successfully
         """
         if self.video_thread:
             return True
 
         self.open_camera()
         time.sleep(0.5)
-        self.video_thread = threading.Thread(target=self._video_worker, args=(self,))
+        self.video_thread = threading.Thread(target=self._video_worker)
         self.video_thread.start()
 
         started = time.time()
         while time.time() < started + 5:
             if self._video_open:
                 return True
```

### Comparing `visioncar-0.1.5/src/visioncar.egg-info/PKG-INFO` & `visioncar-0.1.6/src/visioncar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visioncar
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python library for controlling ESP32 robot
 Author: VisionCar team
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

