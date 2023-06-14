# Comparing `tmp/UC2 REST-0.2.0.8.tar.gz` & `tmp/UC2 REST-0.2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UC2 REST-0.2.0.8.tar", last modified: Tue Mar 14 07:30:12 2023, max compression
+gzip compressed data, was "UC2 REST-0.2.0.9.tar", last modified: Fri Mar 24 08:35:41 2023, max compression
```

## Comparing `UC2 REST-0.2.0.8.tar` & `UC2 REST-0.2.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 07:30:12.013702 UC2 REST-0.2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-03-14 07:30:12.013702 UC2 REST-0.2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10455 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 07:30:12.013702 UC2 REST-0.2.0.8/UC2_REST.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-03-14 07:30:12.000000 UC2 REST-0.2.0.8/UC2_REST.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-14 07:30:12.000000 UC2 REST-0.2.0.8/UC2_REST.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 07:30:12.000000 UC2 REST-0.2.0.8/UC2_REST.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 07:30:11.000000 UC2 REST-0.2.0.8/UC2_REST.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-14 07:30:12.000000 UC2 REST-0.2.0.8/UC2_REST.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-14 07:30:12.000000 UC2 REST-0.2.0.8/UC2_REST.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 07:30:12.013702 UC2 REST-0.2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 07:30:12.013702 UC2 REST-0.2.0.8/uc2rest/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5548 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/UC2Client.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-14 07:29:59.000000 UC2 REST-0.2.0.8/uc2rest/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/analog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/config_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/digitalout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/galvo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/home.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/laser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/ledmatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    18614 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/motor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/mserial.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/slm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11709 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-03-14 07:29:58.000000 UC2 REST-0.2.0.8/uc2rest/wifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 08:35:41.877601 UC2 REST-0.2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-03-24 08:35:41.877601 UC2 REST-0.2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10455 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 08:35:41.873601 UC2 REST-0.2.0.9/UC2_REST.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-03-24 08:35:41.000000 UC2 REST-0.2.0.9/UC2_REST.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-24 08:35:41.000000 UC2 REST-0.2.0.9/UC2_REST.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 08:35:41.000000 UC2 REST-0.2.0.9/UC2_REST.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 08:35:41.000000 UC2 REST-0.2.0.9/UC2_REST.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-24 08:35:41.000000 UC2 REST-0.2.0.9/UC2_REST.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-24 08:35:41.000000 UC2 REST-0.2.0.9/UC2_REST.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 08:35:41.877601 UC2 REST-0.2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 08:35:41.877601 UC2 REST-0.2.0.9/uc2rest/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5682 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/UC2Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-24 08:35:27.000000 UC2 REST-0.2.0.9/uc2rest/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/analog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/config_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/digitalout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/galvo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/home.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/laser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/ledmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18229 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/motor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/mserial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/slm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11709 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-03-24 08:35:25.000000 UC2 REST-0.2.0.9/uc2rest/wifi.py
```

### Comparing `UC2 REST-0.2.0.8/PKG-INFO` & `UC2 REST-0.2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UC2 REST
-Version: 0.2.0.8
+Version: 0.2.0.9
 Summary: This pacage will help you to drive the ESP32-driven microscopy control modules from UC2
 Home-page: https://github.com/openUC2/UC2-REST
 Author: Benedict Diederich
 Author-email: benedictdied@gmail.com
 License: GPL v3
 Keywords: UC2REST API to control ESP32-driven microscopy control boards
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: UC2 REST Version: 0.2.0.8 Summary: This pacage will
+Metadata-Version: 2.1 Name: UC2 REST Version: 0.2.0.9 Summary: This pacage will
 help you to drive the ESP32-driven microscopy control modules from UC2 Home-
 page: https://github.com/openUC2/UC2-REST Author: Benedict Diederich Author-
 email: benedictdied@gmail.com License: GPL v3 Keywords: UC2REST API to control
 ESP32-driven microscopy control boards Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3.7 Requires-Python: >=3.7 Description-Content-Type:
 text/markdown License-File: LICENSE
```

### Comparing `UC2 REST-0.2.0.8/README.md` & `UC2 REST-0.2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.8/UC2_REST.egg-info/PKG-INFO` & `UC2 REST-0.2.0.9/UC2_REST.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UC2-REST
-Version: 0.2.0.8
+Version: 0.2.0.9
 Summary: This pacage will help you to drive the ESP32-driven microscopy control modules from UC2
 Home-page: https://github.com/openUC2/UC2-REST
 Author: Benedict Diederich
 Author-email: benedictdied@gmail.com
 License: GPL v3
 Keywords: UC2REST API to control ESP32-driven microscopy control boards
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: UC2-REST Version: 0.2.0.8 Summary: This pacage will
+Metadata-Version: 2.1 Name: UC2-REST Version: 0.2.0.9 Summary: This pacage will
 help you to drive the ESP32-driven microscopy control modules from UC2 Home-
 page: https://github.com/openUC2/UC2-REST Author: Benedict Diederich Author-
 email: benedictdied@gmail.com License: GPL v3 Keywords: UC2REST API to control
 ESP32-driven microscopy control boards Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3.7 Requires-Python: >=3.7 Description-Content-Type:
 text/markdown License-File: LICENSE
```

### Comparing `UC2 REST-0.2.0.8/UC2_REST.egg-info/SOURCES.txt` & `UC2 REST-0.2.0.9/UC2_REST.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.8/setup.py` & `UC2 REST-0.2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.8/uc2rest/UC2Client.py` & `UC2 REST-0.2.0.9/uc2rest/UC2Client.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,7 +168,11 @@
             return r.json()
         elif self.is_serial:
             self.serial.get_json(path)
             return self.serial.read_json()
         else:
             self.logger.error("No ESP32 device is connected - check IP or Serial port!")
             return None
+
+    def setDebugging(self, debug=False):
+        self.logger.debug(f"Setting debugging to {debug}")
+        self.serial.DEBUG = debug
```

### Comparing `UC2 REST-0.2.0.8/uc2rest/analog.py` & `UC2 REST-0.2.0.9/uc2rest/analog.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.8/uc2rest/camera.py` & `UC2 REST-0.2.0.9/uc2rest/camera.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.8/uc2rest/config.py` & `UC2 REST-0.2.0.9/uc2rest/config.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.8/uc2rest/config_.py` & `UC2 REST-0.2.0.9/uc2rest/config_.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.8/uc2rest/digitalout.py` & `UC2 REST-0.2.0.9/uc2rest/digitalout.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.8/uc2rest/galvo.py` & `UC2 REST-0.2.0.9/uc2rest/galvo.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.8/uc2rest/home.py` & `UC2 REST-0.2.0.9/uc2rest/home.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.8/uc2rest/laser.py` & `UC2 REST-0.2.0.9/uc2rest/laser.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.8/uc2rest/ledmatrix.py` & `UC2 REST-0.2.0.9/uc2rest/ledmatrix.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import json
 import time 
-gTimeout = 0.1
+gTimeout = 1
 class LedMatrix(object):
     def __init__(self, parent, NLeds=64):
         #TOOD: This is for the LED matrix only!
         self.NLeds = NLeds
         #assuming we have a square grid!
         self.Nx = self.Ny = int(np.sqrt(NLeds))
         
@@ -13,33 +13,34 @@
         self.ledpattern = np.zeros((self.NLeds, 3))
         
         # this is a istance of the _parent32Client class
         self._parent = parent
         self.timeout = 1
         self.intensity = (255,255,255)
         
-        self.ledArrayMode = {
+        self.ledArrayModes = {
             "array": 0,
             "full": 1,
             "single": 2,
             "off": 3,
             "left": 4,
             "right": 5,
             "top": 6,
             "bottom": 7,
             "multi": 8}
-            
+
+        self.currentLedArrayMode = "full"            
             
     
     '''
     ##############################################################################################################################
     LED ARRAY
     ##############################################################################################################################
     '''
-    def send_LEDMatrix_array(self, led_pattern, is_blocking = False, timeout=gTimeout):
+    def send_LEDMatrix_array(self, led_pattern, getReturn = True, timeout=gTimeout):
         '''
         Send an LED array pattern e.g. an RGB Matrix: led_pattern=np.zeros((3,8,8))
         '''
         path = '/ledarr_act'
         # if we have a 2d pattern => flatten
         if len(led_pattern.shape)==3:
             led_pattern=np.reshape(led_pattern, (np.prod(led_pattern.shape[0:2]),led_pattern.shape[2])) 
@@ -53,21 +54,23 @@
                 "g": int(led_pattern[i,1]),
                 "b": int(led_pattern[i,2])                        
             })
 
         payload = {
             "task":path,
             "led": {
-                "LEDArrMode": self.ledArrayMode["array"],
+                "LEDArrMode": self.ledArrayModes["array"],
                 "led_array": pattern_list
             }
         }
         #self._parent.logger.debug("Setting LED Pattern (array) ")
-        r = self._parent.post_json(path, payload, getReturn=is_blocking, timeout=timeout)
-        
+        r = self._parent.post_json(path, payload, getReturn=getReturn, timeout=timeout)
+        if not getReturn or timeout==0:
+            r = {"success": 1}
+        self.currentLedArrayMode = "array"            
         return r
 
     def send_LEDMatrix_full(self, intensity = (255,255,255), getReturn=True, timeout=gTimeout):
         '''
         set all LEDs with te same RGB value: intensity=(255,255,255)
         '''
         #{"task": "/ledarr_act","led": {"LEDArrMode": 1,"led_array": [{"b": 255,"g": 255,"r": 255}]}}
@@ -75,58 +78,67 @@
         payload = {
             "task":path,
             "led": {
                 "led_array":[{
                     "r": int(intensity[0]),
                     "g": int(intensity[1]),
                     "b": int(intensity[2])}],
-                "LEDArrMode": self.ledArrayMode["full"]
+                "LEDArrMode": self.ledArrayModes["full"]
             }
         }
         
         #self._parent.logger.debug("Setting LED Pattern (full): "+ str(intensity))
         r = self._parent.post_json(path, payload, getReturn=getReturn, timeout=timeout)
+        if not getReturn or timeout==0:
+            r = {"success": 1}
+        self.currentLedArrayMode = "full"            
         return r
 
-    def send_LEDMatrix_special(self, pattern="left", intensity = (255,255,255),timeout=gTimeout):
+    def send_LEDMatrix_special(self, pattern="left", intensity = (255,255,255), getReturn = True, timeout=gTimeout):
         '''
         set all LEDs inside a certain pattern (e.g. left half) with the same RGB value: intensity=(255,255,255), rest 0
         '''
         path = '/ledarr_act'
         payload = {
             "task":path,
             "led": {
             "r": int(intensity[0]),
             "g": int(intensity[1]),
             "b": int(intensity[2]),
-            "LEDArrMode": self.ledArrayMode[pattern]
+            "LEDArrMode": self.ledArrayModes[pattern]
             }
         }
         self._parent.logger.debug("Setting LED Pattern (full): "+ str(intensity))
         r = self._parent.post_json(path, payload, getReturn=True, timeout=timeout)
+        if not getReturn or timeout==0:
+            r = {"success": 1}
+        self.currentLedArrayMode = "special"            
         return r
 
-    def send_LEDMatrix_single(self, indexled=0, intensity=(255,255,255), timeout=gTimeout):
+    def send_LEDMatrix_single(self, indexled=0, intensity=(255,255,255), getReturn = True, timeout=gTimeout):
         '''
         update only a single LED with a colour:  indexled=0, intensity=(255,255,255)
         '''
         path = '/ledarr_act'
         payload = {
             "task":path,
             "led": {
-                "LEDArrMode": self.ledArrayMode["single"],
+                "LEDArrMode": self.ledArrayModes["single"],
                 "led_array": [{
                     "id": indexled,
                     "r": int(intensity[0]),
                     "g": int(intensity[1]),
                     "b": int(intensity[2])}]
             }
         }
         self._parent.logger.debug("Setting LED Pattern (single) ")
-        r = self._parent.post_json(path, payload, getReturn=True, timeout=timeout)
+        r = self._parent.post_json(path, payload, getReturn=getReturn, timeout=timeout)
+        if not getReturn or timeout==0:
+            r = {"success": 1}
+        self.currentLedArrayMode = "single"            
         return r
 
 
     def get_LEDMatrix(self, timeout=gTimeout):
         '''
         get information about pinnumber and number of leds
         '''
@@ -156,24 +168,29 @@
         if intensity is not None:
             self.intensity = intensity
         intensity2display = np.array(self.intensity)*np.array(state)
         self.send_LEDMatrix_full(intensity = intensity2display, timeout=self.timeout)
         self.ledpattern = state*np.ones((self.NLeds, 3))
         return self.ledpattern
     
-    def setIntensity(self, intensity):
+    def setIntensity(self, intensity, getReturn=True):
         self.intensity = intensity
-        self.setPattern()
+        self.setPattern(getReturn=getReturn)
     
-    def setPattern(self, ledpattern=None):
+    def setPattern(self, getReturn=True, ledpattern=None):
         # sends pattern with proper intensity
         if ledpattern is not None:
             self.ledpattern = ledpattern
         pattern2send = (self.ledpattern>=1)*self.intensity
-        self.send_LEDMatrix_array(pattern2send, timeout=self.timeout)
+        if np.sum(self.ledpattern, 0)[0]==self.ledpattern.shape[0]:
+            # turn on all - faster! 
+            self.send_LEDMatrix_full(pattern2send[0,:], getReturn=getReturn, timeout=self.timeout)
+        else:
+            # set individual pattern - slower
+            self.send_LEDMatrix_array(pattern2send, getReturn=getReturn, timeout=self.timeout)
         return self.ledpattern
     
     def getPattern(self):
         return self.ledpattern
         
     def set_led(self, colour=(0,0,0)):
         payload = {
```

### Comparing `UC2 REST-0.2.0.8/uc2rest/modules.py` & `UC2 REST-0.2.0.9/uc2rest/modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     def get_modules(self, timeout=1):
         # returns a list of available modules that are set or not set in the ESP
         path = '/modules_get'
         
         payload = {
             "task": path,
             }
-        r = self._parent.post_json(path, payload)
+        r = self._parent.post_json(path, payload)["modules"]
         
         return r
 
     def set_modules(self, modules, timeout=1):
         path = '/modules_set'
         
         payload = {
```

### Comparing `UC2 REST-0.2.0.8/uc2rest/motor.py` & `UC2 REST-0.2.0.9/uc2rest/motor.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,24 +80,24 @@
             axis = 2
         if axis == "Z":
             axis = 3
         if axis == "T" or axis == "A":
             axis = 0
         return axis
 
-    def move_x(self, steps=100, speed=1000, is_blocking=False, is_absolute=False, is_enabled=True, timeout=gTIMEOUT):
+    def move_x(self, steps=0, speed=1000, is_blocking=False, is_absolute=False, is_enabled=True, timeout=gTIMEOUT):
         return self.move_axis_by_name(axis="X", steps=steps, speed=speed, is_blocking=is_blocking, is_absolute=is_absolute, is_enabled=is_enabled, timeout=timeout)
 
-    def move_y(self, steps=100, speed=1000, is_blocking=False, is_absolute=False, is_enabled=True, timeout=gTIMEOUT):
+    def move_y(self, steps=0, speed=1000, is_blocking=False, is_absolute=False, is_enabled=True, timeout=gTIMEOUT):
         return self.move_axis_by_name(axis="Y", steps=steps, speed=speed, is_blocking=is_blocking, is_absolute=is_absolute, is_enabled=is_enabled, timeout=timeout)
 
-    def move_z(self, steps=100, speed=1000, is_blocking=False, is_absolute=False, is_enabled=True, timeout=gTIMEOUT):
+    def move_z(self, steps=0, speed=1000, is_blocking=False, is_absolute=False, is_enabled=True, timeout=gTIMEOUT):
         return self.move_axis_by_name(axis="Z", steps=steps, speed=speed, is_blocking=is_blocking, is_absolute=is_absolute, is_enabled=is_enabled, timeout=timeout)
 
-    def move_t(self, steps=100, speed=1000, is_blocking=False, is_absolute=False, is_enabled=True, timeout=gTIMEOUT):
+    def move_t(self, steps=0, speed=1000, is_blocking=False, is_absolute=False, is_enabled=True, timeout=gTIMEOUT):
         return self.move_axis_by_name(axis="T", steps=steps, speed=speed, is_blocking=is_blocking, is_absolute=is_absolute, is_enabled=is_enabled, timeout=timeout)
 
     def move_xyz(self, steps=(0,0,0), speed=(1000,1000,1000), is_blocking=False, is_absolute=False, is_enabled=True, timeout=gTIMEOUT):
         if len(speed)!= 3:
             speed = (speed,speed,speed)
 
         # motor axis is 1,2,3,0 => X,Y,Z,T # FIXME: Hardcoded
@@ -277,15 +277,16 @@
         motorPropList = []
         for iMotor in range(4):
             if isAbsoluteArray[iMotor] or abs(steps[iMotor])>0:
                 motorProp = { "stepperid": self.motorAxisOrder[iMotor],
                              "position": np.int(steps[iMotor]),
                              "speed": speed[iMotor],
                              "isabs": isAbsoluteArray[iMotor],
-                             "isaccel":0}
+                             "isaccel":0, 
+                             "isen": is_enabled}
                 motorPropList.append(motorProp)
 
         path = "/motor_act"
         payload = {
             "task":path,
             "motor":
             {
@@ -425,49 +426,35 @@
         try:
             for index, istepper in enumerate(r["motor"]["steppers"]):
                 _position[istepper["stepperid"]]=istepper["position"]*_physicalStepSizes[self.motorAxisOrder[index]]
         except Exception as e: self._parent.logger.error(e)
         return _position
 
     def set_position(self, axis=1, position=0, timeout=1):
-        self._parent.logger.error("set_position is deprecated. Use set_motor_currentPosition instead.")
+
         '''
-        path = "/motor_set"
+        {"task":"/home_act",  "setpos": {"steppers": [{"stepperid":1, "posval": 0}]}}
+        '''
+        path = "/home_act"
         if axis=="X": axis=1
         if axis=="Y": axis=2
         if axis=="Z": axis=3
 
         payload = {
-            "task":path,
-            "axis":axis,
-            "currentposition": position
-        }
+            "task": path,
+            "setpos":{
+                "steppers": [
+                {
+                 "stepperid": axis,
+                 "posval": int(position)
+                 }]
+            }}
         r = self._parent.post_json(path, payload, timeout=timeout)
 
         return r
-        '''
-        return False
-
-    def set_motors(self, settingsdict, isBlocking=True, timeout=1):
-        path = "/motor_set"
-        payload = settingsdict
-        payload["task"] = path
-
-        # send command
-        r = self._parent.post_json(path, payload, timeout=1)
-
-        # wait until job has been done
-        time0=time.time()
-        if isBlocking:
-            while self.isBusy((0,0,0,0)):
-                time.sleep(0.1)
-                if time.time()-time0>timeout:
-                    break
-
-        return r
 
 
     def get_motor(self, axis=1, timeout=1):
         path = "/motor_get"
         payload = {
             "task":path,
         }
```

### Comparing `UC2 REST-0.2.0.8/uc2rest/mserial.py` & `UC2 REST-0.2.0.9/uc2rest/mserial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import serial
 import serial.tools.list_ports
 import time
 import json
 
-T_SERIAL_WARMUP = 5 # the time to wait for the serial to warm up
+T_SERIAL_WARMUP = 2 # the time to wait for the serial to warm up
 
 class Serial(object):
     
     def __init__(self, port, baudrate, timeout=1, identity="UC2_Feather", parent=None, DEBUG=False):
         self.serialport = port
         self.baudrate = baudrate
         self.timeout = timeout
```

### Comparing `UC2 REST-0.2.0.8/uc2rest/pid.py` & `UC2 REST-0.2.0.9/uc2rest/pid.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.8/uc2rest/slm.py` & `UC2 REST-0.2.0.9/uc2rest/slm.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.8/uc2rest/state.py` & `UC2 REST-0.2.0.9/uc2rest/state.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.8/uc2rest/updater.py` & `UC2 REST-0.2.0.9/uc2rest/updater.py`

 * *Files identical despite different names*

### Comparing `UC2 REST-0.2.0.8/uc2rest/wifi.py` & `UC2 REST-0.2.0.9/uc2rest/wifi.py`

 * *Files identical despite different names*

