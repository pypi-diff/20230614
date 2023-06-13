# Comparing `tmp/airunner-1.9.4.tar.gz` & `tmp/airunner-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airunner-1.9.4.tar", last modified: Fri Apr 21 15:03:39 2023, max compression
+gzip compressed data, was "airunner-1.9.5.tar", last modified: Sun Apr 23 13:36:01 2023, max compression
```

## Comparing `airunner-1.9.4.tar` & `airunner-1.9.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:03:39.147076 airunner-1.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 15:03:26.000000 airunner-1.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-21 15:03:39.147076 airunner-1.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-21 15:03:26.000000 airunner-1.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 15:03:39.147076 airunner-1.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-21 15:03:26.000000 airunner-1.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:03:39.143076 airunner-1.9.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:03:39.147076 airunner-1.9.4/src/airunner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/balloon.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/history.py
--rw-r--r--   0 runner    (1001) docker     (123)    64664 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    32827 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/qtcanvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/runai_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/settingsmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:03:39.147076 airunner-1.9.4/src/airunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-21 15:03:39.000000 airunner-1.9.4/src/airunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-21 15:03:39.000000 airunner-1.9.4/src/airunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 15:03:39.000000 airunner-1.9.4/src/airunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 15:03:39.000000 airunner-1.9.4/src/airunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 15:03:39.000000 airunner-1.9.4/src/airunner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:36:01.596524 airunner-1.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 13:35:50.000000 airunner-1.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-23 13:36:01.596524 airunner-1.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-23 13:35:50.000000 airunner-1.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 13:36:01.596524 airunner-1.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-23 13:35:50.000000 airunner-1.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:36:01.592524 airunner-1.9.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:36:01.592524 airunner-1.9.5/src/airunner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/balloon.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64713 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32883 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/qtcanvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/runai_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/settingsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:36:01.596524 airunner-1.9.5/src/airunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-23 13:36:01.000000 airunner-1.9.5/src/airunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-23 13:36:01.000000 airunner-1.9.5/src/airunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 13:36:01.000000 airunner-1.9.5/src/airunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 13:36:01.000000 airunner-1.9.5/src/airunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 13:36:01.000000 airunner-1.9.5/src/airunner.egg-info/top_level.txt
```

### Comparing `airunner-1.9.4/LICENSE` & `airunner-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `airunner-1.9.4/PKG-INFO` & `airunner-1.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airunner
-Version: 1.9.4
+Version: 1.9.5
 Summary: A Stable Diffusion GUI
 Home-page: https://github.com/Capsize-Games/airunner
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `airunner-1.9.4/README.md` & `airunner-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `airunner-1.9.4/setup.py` & `airunner-1.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='airunner',
-    version="1.9.4",
+    version="1.9.5",
     author="Capsize LLC",
     description="A Stable Diffusion GUI",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="ai, chatbot, chat, ai",
     license="AGPL-3.0",
     author_email="contact@capsize.gg",
```

### Comparing `airunner-1.9.4/src/airunner/balloon.py` & `airunner-1.9.5/src/airunner/balloon.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.4/src/airunner/extensions.py` & `airunner-1.9.5/src/airunner/extensions.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.4/src/airunner/filters.py` & `airunner-1.9.5/src/airunner/filters.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.4/src/airunner/main.py` & `airunner-1.9.5/src/airunner/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1068,15 +1068,16 @@
         if data["action"] == "txt2vid":
             return self.video_handler(data)
 
         self.stop_progress_bar(data["action"])
         if nsfw_content_detected and self.settings_manager.settings.nsfw_filter.get():
             self.message_handler("NSFW content detected, try again.", error=True)
         else:
-            self.canvas.add_layer()
+            if data["action"] != "outpaint":
+                self.canvas.add_layer()
             self.canvas.image_handler(image, data)
             self.message_handler("")
             self.show_layers()
 
     def update_canvas_color(self, color):
         self.window.canvas_container.setStyleSheet(f"background-color: {color};")
         self.window.canvas_container.setAutoFillBackground(True)
```

### Comparing `airunner-1.9.4/src/airunner/qtcanvas.py` & `airunner-1.9.5/src/airunner/qtcanvas.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,16 @@
         self.parent.history.add_event(history_event)
         self.image_root_point = image_root_point
         self.image_pivot_point = image_pivot_point
         self.current_layer.images = [ImageData(image_pivot_point, processed_image)]
 
     def handle_outpaint(self, outpaint_box_rect, outpainted_image, action):
         if len(self.current_layer.images) == 0:
-            return outpainted_image, self.image_root_point, self.image_pivot_point
+            point = QPoint(outpaint_box_rect.x(), outpaint_box_rect.y())
+            return outpainted_image, self.image_root_point, point
 
         # make a copy of the current canvas image
         existing_image_copy = self.current_layer.images[0].image.copy()
         width = existing_image_copy.width
         height = existing_image_copy.height
         working_width = self.settings_manager.settings.working_width.get()
         working_height = self.settings_manager.settings.working_height.get()
```

### Comparing `airunner-1.9.4/src/airunner/runai_client.py` & `airunner-1.9.5/src/airunner/runai_client.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.4/src/airunner/settingsmanager.py` & `airunner-1.9.5/src/airunner/settingsmanager.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.4/src/airunner/utils.py` & `airunner-1.9.5/src/airunner/utils.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.4/src/airunner.egg-info/PKG-INFO` & `airunner-1.9.5/src/airunner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airunner
-Version: 1.9.4
+Version: 1.9.5
 Summary: A Stable Diffusion GUI
 Home-page: https://github.com/Capsize-Games/airunner
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

