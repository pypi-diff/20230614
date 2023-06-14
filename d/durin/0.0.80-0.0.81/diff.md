# Comparing `tmp/durin-0.0.80.tar.gz` & `tmp/durin-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "durin-0.0.80.tar", last modified: Mon May 22 11:52:44 2023, max compression
+gzip compressed data, was "durin-0.0.81.tar", last modified: Thu Jun  1 14:41:51 2023, max compression
```

## Comparing `durin-0.0.80.tar` & `durin-0.0.81.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:44.428178 durin-0.0.80/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-22 11:52:35.000000 durin-0.0.80/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-22 11:52:44.428178 durin-0.0.80/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2683 2023-05-22 11:52:35.000000 durin-0.0.80/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:44.424178 durin-0.0.80/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-05-22 11:52:35.000000 durin-0.0.80/bin/durin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:44.424178 durin-0.0.80/durin/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-22 11:52:35.000000 durin-0.0.80/durin/Profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-22 11:52:35.000000 durin-0.0.80/durin/Read_profilers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-05-22 11:52:35.000000 durin-0.0.80/durin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-05-22 11:52:35.000000 durin-0.0.80/durin/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-05-22 11:52:35.000000 durin-0.0.80/durin/actuator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4148 2023-05-22 11:52:35.000000 durin-0.0.80/durin/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:44.424178 durin-0.0.80/durin/controller/
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-05-22 11:52:35.000000 durin-0.0.80/durin/controller/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-05-22 11:52:35.000000 durin-0.0.80/durin/controller/dvs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4307 2023-05-22 11:52:35.000000 durin-0.0.80/durin/controller/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:44.424178 durin-0.0.80/durin/controller/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:35.000000 durin-0.0.80/durin/controller/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-05-22 11:52:35.000000 durin-0.0.80/durin/controller/test/test_stream.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4694 2023-05-22 11:52:35.000000 durin-0.0.80/durin/durin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   181742 2023-05-22 11:52:35.000000 durin-0.0.80/durin/durin_birdseye.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-05-22 11:52:35.000000 durin-0.0.80/durin/dvs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:44.428178 durin-0.0.80/durin/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/CPU_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/braitenberg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2631 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/commands.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1448 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/dashboard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:44.428178 durin-0.0.80/durin/io/
--rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-05-22 11:52:35.000000 durin-0.0.80/durin/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-22 11:52:35.000000 durin-0.0.80/durin/io/command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-05-22 11:52:35.000000 durin-0.0.80/durin/io/gamepad.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6181 2023-05-22 11:52:35.000000 durin-0.0.80/durin/io/network.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-05-22 11:52:35.000000 durin-0.0.80/durin/io/ringbuffer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-05-22 11:52:35.000000 durin-0.0.80/durin/io/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-05-22 11:52:35.000000 durin-0.0.80/durin/io/schema.capnp
--rwxr-xr-x   0 runner    (1001) docker     (123)     7102 2023-05-22 11:52:35.000000 durin-0.0.80/durin/sensor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14773 2023-05-22 11:52:35.000000 durin-0.0.80/durin/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:44.424178 durin-0.0.80/durin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-22 11:52:44.000000 durin-0.0.80/durin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-22 11:52:44.000000 durin-0.0.80/durin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 11:52:44.000000 durin-0.0.80/durin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-22 11:52:44.000000 durin-0.0.80/durin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 11:52:44.000000 durin-0.0.80/durin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 11:52:44.428178 durin-0.0.80/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-05-22 11:52:35.000000 durin-0.0.80/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:50.996440 durin-0.0.81/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 14:41:40.000000 durin-0.0.81/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-01 14:41:50.996440 durin-0.0.81/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2683 2023-06-01 14:41:40.000000 durin-0.0.81/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:50.992439 durin-0.0.81/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-06-01 14:41:40.000000 durin-0.0.81/bin/durin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:50.996440 durin-0.0.81/durin/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-01 14:41:40.000000 durin-0.0.81/durin/Profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-01 14:41:40.000000 durin-0.0.81/durin/Read_profilers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-06-01 14:41:40.000000 durin-0.0.81/durin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-06-01 14:41:40.000000 durin-0.0.81/durin/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-06-01 14:41:40.000000 durin-0.0.81/durin/actuator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4148 2023-06-01 14:41:40.000000 durin-0.0.81/durin/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:50.996440 durin-0.0.81/durin/controller/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-06-01 14:41:40.000000 durin-0.0.81/durin/controller/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-06-01 14:41:40.000000 durin-0.0.81/durin/controller/dvs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4307 2023-06-01 14:41:40.000000 durin-0.0.81/durin/controller/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:50.996440 durin-0.0.81/durin/controller/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:40.000000 durin-0.0.81/durin/controller/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-06-01 14:41:40.000000 durin-0.0.81/durin/controller/test/test_stream.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4694 2023-06-01 14:41:40.000000 durin-0.0.81/durin/durin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   181742 2023-06-01 14:41:40.000000 durin-0.0.81/durin/durin_birdseye.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-06-01 14:41:40.000000 durin-0.0.81/durin/dvs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:50.996440 durin-0.0.81/durin/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-01 14:41:40.000000 durin-0.0.81/durin/examples/CPU_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:40.000000 durin-0.0.81/durin/examples/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-06-01 14:41:40.000000 durin-0.0.81/durin/examples/braitenberg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2631 2023-06-01 14:41:40.000000 durin-0.0.81/durin/examples/commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1448 2023-06-01 14:41:40.000000 durin-0.0.81/durin/examples/dashboard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-06-01 14:41:40.000000 durin-0.0.81/durin/examples/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-01 14:41:40.000000 durin-0.0.81/durin/examples/plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-06-01 14:41:40.000000 durin-0.0.81/durin/examples/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-01 14:41:40.000000 durin-0.0.81/durin/examples/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:50.996440 durin-0.0.81/durin/io/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-06-01 14:41:40.000000 durin-0.0.81/durin/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-01 14:41:40.000000 durin-0.0.81/durin/io/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1418 2023-06-01 14:41:40.000000 durin-0.0.81/durin/io/gamepad.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6181 2023-06-01 14:41:40.000000 durin-0.0.81/durin/io/network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-01 14:41:40.000000 durin-0.0.81/durin/io/ringbuffer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-06-01 14:41:40.000000 durin-0.0.81/durin/io/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-06-01 14:41:40.000000 durin-0.0.81/durin/io/schema.capnp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7102 2023-06-01 14:41:40.000000 durin-0.0.81/durin/sensor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14991 2023-06-01 14:41:40.000000 durin-0.0.81/durin/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:41:50.996440 durin-0.0.81/durin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-01 14:41:50.000000 durin-0.0.81/durin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-01 14:41:50.000000 durin-0.0.81/durin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:41:50.000000 durin-0.0.81/durin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-01 14:41:50.000000 durin-0.0.81/durin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 14:41:50.000000 durin-0.0.81/durin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:41:50.996440 durin-0.0.81/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-06-01 14:41:40.000000 durin-0.0.81/setup.py
```

### Comparing `durin-0.0.80/PKG-INFO` & `durin-0.0.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durin
-Version: 0.0.80
+Version: 0.0.81
 Summary: Python control interface for the Durin robot
 Maintainer: Jens E. Pedersen
 Maintainer-email: jeped@kth.se
 License: LGPLv3
 Description-Content-Type: text/markdown
 Provides-Extra: aestream
```

### Comparing `durin-0.0.80/README.md` & `durin-0.0.81/README.md`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/actuator.py` & `durin-0.0.81/durin/actuator.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/cli.py` & `durin-0.0.81/durin/cli.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/controller/server.py` & `durin-0.0.81/durin/controller/server.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/controller/test/test_stream.py` & `durin-0.0.81/durin/controller/test/test_stream.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/durin.py` & `durin-0.0.81/durin/durin.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/durin_birdseye.jpg` & `durin-0.0.81/durin/durin_birdseye.jpg`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/examples/braitenberg.py` & `durin-0.0.81/durin/examples/braitenberg.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/examples/commands.py` & `durin-0.0.81/durin/examples/commands.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/examples/dashboard.py` & `durin-0.0.81/durin/examples/dashboard.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/examples/main.py` & `durin-0.0.81/durin/examples/main.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/examples/plot.py` & `durin-0.0.81/durin/examples/plot.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/examples/record.py` & `durin-0.0.81/durin/examples/record.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/examples/stats.py` & `durin-0.0.81/durin/examples/stats.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/io/__init__.py` & `durin-0.0.81/durin/io/__init__.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/io/command.py` & `durin-0.0.81/durin/io/command.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/io/gamepad.py` & `durin-0.0.81/durin/io/gamepad.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 class Gamepad(RunnableProducer):
     def __init__(self, timeout: float = 0.05):
         context = multiprocessing.get_context("spawn")
         self.queue = context.Queue(maxsize=1)
         self.timeout = timeout
         self.values = multiprocessing.Array("f", 3)
-        self.tau = 0.99
 
         super().__init__(self.queue, self.values)
 
     @staticmethod
     def norm(x):
         if x == 0:
             return int(x)
```

### Comparing `durin-0.0.80/durin/io/network.py` & `durin-0.0.81/durin/io/network.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/io/ringbuffer.py` & `durin-0.0.81/durin/io/ringbuffer.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/io/runnable.py` & `durin-0.0.81/durin/io/runnable.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/io/schema.capnp` & `durin-0.0.81/durin/io/schema.capnp`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/sensor.py` & `durin-0.0.81/durin/sensor.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/durin/ui.py` & `durin-0.0.81/durin/ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,16 +77,16 @@
         self.a = 0 # Just for debugging. Delete soon!
 
         self.set_frequency()
         self(EnableTofStatus(True))
 
         pygame.init()
         self.clock = pygame.time.Clock()
-        self.font = pygame.font.SysFont(None, 22)
-        self.big_font = pygame.font.SysFont(None, 34)
+        self.font = pygame.font.SysFont(None, 40)
+        self.big_font = pygame.font.SysFont(None, 60)
 
 
         # Set up the display
         # Get screen size
         info = pygame.display.Info()
         self.screen_width, self.screen_height = info.current_w, info.current_h-50
 
@@ -132,15 +132,19 @@
         keys = pygame.key.get_pressed()
 
         # Gamepad
         if not self.gamepad.queue.empty():
             x, y, r = self.gamepad.queue.get()
             self.horizontal = x
             self.vertical = y
-            self.rot = r
+            self.rot = -r
+        # else:
+        #     self.horizontal = self.horizontal - 0.1 * self.horizontal
+        #     self.vertical = self.vertical - 0.1 * self.vertical
+        #     self.rot = self.rot - 0.1 * self.rot
 
         for event in pygame.event.get():
             if event.type == pygame.QUIT or (event.type == pygame.KEYDOWN and event.key == pygame.K_ESCAPE):
                 return False
 
             # Keyboard
             elif event.type == pygame.KEYDOWN:
@@ -274,17 +278,17 @@
 
 
         # Update Durin position ######################
         for m in range(3):
             self.render_text(str(obs.position[m]), (POSITION_PLACEMENT[0]+2*m*d, POSITION_PLACEMENT[1]+2*d))
 
         # Update movement commands ################
-        self.render_text(str(self.horizontal),(MV_CMD_PLACEMENT[0],MV_CMD_PLACEMENT[1]+2*d))
-        self.render_text(str(self.vertical),(MV_CMD_PLACEMENT[0]+2*d,MV_CMD_PLACEMENT[1]+2*d))
-        self.render_text(str(self.rot),(MV_CMD_PLACEMENT[0]+4*d,MV_CMD_PLACEMENT[1]+2*d))
+        self.render_text(f"{self.horizontal:.0f}",(MV_CMD_PLACEMENT[0],MV_CMD_PLACEMENT[1]+2*d))
+        self.render_text(f"{self.vertical:.0f}",(MV_CMD_PLACEMENT[0]+2*d,MV_CMD_PLACEMENT[1]+2*d))
+        self.render_text(f"{self.rot:.0f}",(MV_CMD_PLACEMENT[0]+4*d,MV_CMD_PLACEMENT[1]+2*d))
 
         self.render_static_texts()
 
         # Just for debugging.
         self.a += 1
         #self.render_text("Time step (for debugging): " + str(self.a),(UWB_PLACEMENT[0],UWB_PLACEMENT[1]+10*d))
```

### Comparing `durin-0.0.80/durin.egg-info/PKG-INFO` & `durin-0.0.81/durin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durin
-Version: 0.0.80
+Version: 0.0.81
 Summary: Python control interface for the Durin robot
 Maintainer: Jens E. Pedersen
 Maintainer-email: jeped@kth.se
 License: LGPLv3
 Description-Content-Type: text/markdown
 Provides-Extra: aestream
```

### Comparing `durin-0.0.80/durin.egg-info/SOURCES.txt` & `durin-0.0.81/durin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `durin-0.0.80/setup.py` & `durin-0.0.81/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = fp.read().split("\n")
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 setup(
     name="durin",
-    version="0.0.80",
+    version="0.0.81",
     install_requires=requirements,
     packages=find_packages(),
     license="LGPLv3",
     maintainer="Jens E. Pedersen",
     maintainer_email="jeped@kth.se",
     extras_require={"aestream": ["aestream"]},
     scripts=["bin/durin"],
```

