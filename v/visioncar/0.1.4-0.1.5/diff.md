# Comparing `tmp/visioncar-0.1.4.tar.gz` & `tmp/visioncar-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visioncar-0.1.4.tar", last modified: Wed Jun 14 13:31:21 2023, max compression
+gzip compressed data, was "visioncar-0.1.5.tar", last modified: Wed Jun 14 14:36:46 2023, max compression
```

## Comparing `visioncar-0.1.4.tar` & `visioncar-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sh7dm     (1000) sh7dm     (1000)        0 2023-06-14 13:31:21.975375 visioncar-0.1.4/
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)     1077 2023-06-12 09:08:41.000000 visioncar-0.1.4/LICENSE
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       52 2023-06-12 09:08:41.000000 visioncar-0.1.4/MANIFEST.in
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      447 2023-06-14 13:31:21.976375 visioncar-0.1.4/PKG-INFO
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       78 2023-06-12 09:08:41.000000 visioncar-0.1.4/README.md
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       98 2023-06-12 09:08:41.000000 visioncar-0.1.4/pyproject.toml
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      112 2023-06-14 13:31:21.976375 visioncar-0.1.4/setup.cfg
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      848 2023-06-12 09:08:41.000000 visioncar-0.1.4/setup.py
-drwxr-xr-x   0 sh7dm     (1000) sh7dm     (1000)        0 2023-06-14 13:31:21.973375 visioncar-0.1.4/src/
-drwxr-xr-x   0 sh7dm     (1000) sh7dm     (1000)        0 2023-06-14 13:31:21.975375 visioncar-0.1.4/src/visioncar/
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       52 2023-06-12 09:08:41.000000 visioncar-0.1.4/src/visioncar/__init__.py
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)     3264 2023-06-12 09:08:41.000000 visioncar-0.1.4/src/visioncar/__main__.py
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)    17305 2023-06-14 13:29:22.000000 visioncar-0.1.4/src/visioncar/visioncar.py
-drwxr-xr-x   0 sh7dm     (1000) sh7dm     (1000)        0 2023-06-14 13:31:21.975375 visioncar-0.1.4/src/visioncar.egg-info/
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      447 2023-06-14 13:31:21.000000 visioncar-0.1.4/src/visioncar.egg-info/PKG-INFO
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      366 2023-06-14 13:31:21.000000 visioncar-0.1.4/src/visioncar.egg-info/SOURCES.txt
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)        1 2023-06-14 13:31:21.000000 visioncar-0.1.4/src/visioncar.egg-info/dependency_links.txt
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       49 2023-06-14 13:31:21.000000 visioncar-0.1.4/src/visioncar.egg-info/entry_points.txt
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       43 2023-06-14 13:31:21.000000 visioncar-0.1.4/src/visioncar.egg-info/requires.txt
--rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       10 2023-06-14 13:31:21.000000 visioncar-0.1.4/src/visioncar.egg-info/top_level.txt
+drwxr-xr-x   0 sh7dm     (1000) sh7dm     (1000)        0 2023-06-14 14:36:46.381747 visioncar-0.1.5/
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)     1077 2023-06-12 09:08:41.000000 visioncar-0.1.5/LICENSE
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       52 2023-06-12 09:08:41.000000 visioncar-0.1.5/MANIFEST.in
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      638 2023-06-14 14:36:46.381747 visioncar-0.1.5/PKG-INFO
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      269 2023-06-14 13:37:42.000000 visioncar-0.1.5/README.md
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       98 2023-06-12 09:08:41.000000 visioncar-0.1.5/pyproject.toml
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      112 2023-06-14 14:36:46.382747 visioncar-0.1.5/setup.cfg
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      848 2023-06-12 09:08:41.000000 visioncar-0.1.5/setup.py
+drwxr-xr-x   0 sh7dm     (1000) sh7dm     (1000)        0 2023-06-14 14:36:46.379747 visioncar-0.1.5/src/
+drwxr-xr-x   0 sh7dm     (1000) sh7dm     (1000)        0 2023-06-14 14:36:46.380747 visioncar-0.1.5/src/visioncar/
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       52 2023-06-14 13:37:46.000000 visioncar-0.1.5/src/visioncar/__init__.py
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)     2564 2023-06-14 14:26:22.000000 visioncar-0.1.5/src/visioncar/__main__.py
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)    18624 2023-06-14 14:26:16.000000 visioncar-0.1.5/src/visioncar/visioncar.py
+drwxr-xr-x   0 sh7dm     (1000) sh7dm     (1000)        0 2023-06-14 14:36:46.381747 visioncar-0.1.5/src/visioncar.egg-info/
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      638 2023-06-14 14:36:46.000000 visioncar-0.1.5/src/visioncar.egg-info/PKG-INFO
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)      366 2023-06-14 14:36:46.000000 visioncar-0.1.5/src/visioncar.egg-info/SOURCES.txt
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)        1 2023-06-14 14:36:46.000000 visioncar-0.1.5/src/visioncar.egg-info/dependency_links.txt
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       49 2023-06-14 14:36:46.000000 visioncar-0.1.5/src/visioncar.egg-info/entry_points.txt
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       43 2023-06-14 14:36:46.000000 visioncar-0.1.5/src/visioncar.egg-info/requires.txt
+-rw-r--r--   0 sh7dm     (1000) sh7dm     (1000)       10 2023-06-14 14:36:46.000000 visioncar-0.1.5/src/visioncar.egg-info/top_level.txt
```

### Comparing `visioncar-0.1.4/LICENSE` & `visioncar-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `visioncar-0.1.4/setup.py` & `visioncar-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `visioncar-0.1.4/src/visioncar/__main__.py` & `visioncar-0.1.5/src/visioncar/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -67,58 +67,25 @@
 
 def _quit():
     robot.close()
     if not args.novideo:
         cv2.destroyAllWindows()
     exit(0)
 
-_video_ready = False
-
-def video_cap(robot):
-    global _video_ready
-    global _console
-
-    while True:
-        if robot.closing:
-            break
-
-        try:
-            frame = robot.capture()
-            if not len(frame):
-                continue
-
-            cv2.imshow('Video', frame)
-            _video_ready = True
-        except Exception as e:
-            print('Capture error: ' + str(e))
-            _quit()
-
-        if cv2.waitKey(1) == 27:
-            _quit()
-
-if not args.novideo:
-    robot.open_camera()
-    threading.Thread(target=video_cap, args=(robot,)).start()
-
 if not args.nocommand:
     robot.open_control()
 
     if not robot.set_speed(30):
         if not robot.set_speed(30):
             print("Failed to set initial speed")
             _quit()
 
 # Unrelated to control socket, can be called anyway
 robot.set_control("led_intensity", 0)
-
-# Wait for CV warnings
-_started = time.time()
-while time.time() < _started + 5:
-    if _video_ready or args.novideo:
-        break
+robot.show_video()
 
 import code
 
 # Work around readline only available on UNIX
 try:
     import readline
 except:
```

### Comparing `visioncar-0.1.4/src/visioncar/visioncar.py` & `visioncar-0.1.5/src/visioncar/visioncar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from zeroconf import Zeroconf
+from zeroconf.asyncio import AsyncZeroconf
 import requests
 import threading
 import time
 import itertools
 import os
 import asyncio
 import simplejpeg
@@ -114,14 +114,17 @@
         self.count = itertools.count()
         self.queue = {}
         self.tx_queue = []
         self.vbatt = None
         self.als = None
         self.path = None
         self.verbose = False
+        # Video window
+        self._video_open = False
+        self.video_thread = None
 
     def from_zeroconf(http_info, mjpeg_info, ctl_info):
         h = None
         m = None
         ca = None
         cp = None
 
@@ -149,30 +152,31 @@
         return Robot(h, ma, mp, ca, cp)
 
     def discover(hostname):
         """
         Takes robot hostname used to find in on network using Zeroconf
         :return: A new Robot instance
         """
-        zeroconf = Zeroconf()
+        zc = AsyncZeroconf()
+        loop = asyncio.new_event_loop()
 
         http_info = None
         mjpeg_info = None
         ctl_info = None
 
         try:
-            http_info = zeroconf.get_service_info(
-                TYPE_HTTP, hostname + '.' + TYPE_HTTP)
-            mjpeg_info = zeroconf.get_service_info(
-                TYPE_MJPEG, hostname + '.' + TYPE_MJPEG)
-            ctl_info = zeroconf.get_service_info(
-                TYPE_CTL, hostname + '.' + TYPE_CTL)
-
+            http_info = loop.run_until_complete(zc.async_get_service_info(
+                TYPE_HTTP, hostname + '.' + TYPE_HTTP))
+            mjpeg_info = loop.run_until_complete(zc.async_get_service_info(
+                TYPE_MJPEG, hostname + '.' + TYPE_MJPEG))
+            ctl_info = loop.run_until_complete(zc.async_get_service_info(
+                TYPE_CTL, hostname + '.' + TYPE_CTL))
         finally:
-            zeroconf.close()
+            loop.run_until_complete(zc.async_close())
+            loop.close()
 
         if not (http_info and mjpeg_info and ctl_info):
             print(f"Device {hostname} unavailable")
             return None
 
         return Robot.from_zeroconf(http_info, mjpeg_info, ctl_info)
 
@@ -341,14 +345,17 @@
             return True
 
     def open_camera(self):
         """
         Start the robot camera
         :return:
         """
+        if camera_thread:
+            return
+
         loop = asyncio.new_event_loop()
         connect = loop.create_datagram_endpoint(
             lambda: CameraProtocol(self, loop),
             remote_addr=(self.mjpeg_addr, self.mjpeg_port))
         loop.run_until_complete(connect)
         self.camera_loop = loop
         self.camera_thread = threading.Thread(target=loop.run_forever)
@@ -550,7 +557,46 @@
         ret = self.submit("wsping;", 3)
         end = time.time()
         if not ret or not "wsping" in ret:
             print("Ping error: " + str(ret))
             return -1
 
         return (end - start) * 1000
+
+    def _video_worker(_self):
+        while True:
+            if _self.closing:
+                return
+
+            try:
+                frame = _self.capture()
+                if not len(frame):
+                    continue
+
+                cv2.imshow('Video', frame)
+                _self._video_open = True
+            except Exception as e:
+                print('Capture error: ' + str(e))
+                return
+
+            if cv2.waitKey(1) == 27:
+                return
+
+    def show_video(self, timeout = 5):
+        """
+        Open a video streaming window
+        :return: True if opened successfully
+        """
+        if self.video_thread:
+            return True
+
+        self.open_camera()
+        time.sleep(0.5)
+        self.video_thread = threading.Thread(target=self._video_worker, args=(self,))
+        self.video_thread.start()
+
+        started = time.time()
+        while time.time() < started + 5:
+            if self._video_open:
+                return True
+
+        return False
```

