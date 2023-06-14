# Comparing `tmp/cellworld-0.0.98.tar.gz` & `tmp/cellworld-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellworld-0.0.98.tar", last modified: Fri Jul 15 13:36:39 2022, max compression
+gzip compressed data, was "cellworld-0.0.99.tar", last modified: Fri Jul 15 13:41:21 2022, max compression
```

## Comparing `cellworld-0.0.98.tar` & `cellworld-0.0.99.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-07-15 13:36:39.278599 cellworld-0.0.98/
--rwxrwxrwx   0 german    (1000) german    (1000)      190 2022-07-15 13:36:39.276610 cellworld-0.0.98/PKG-INFO
-drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-07-15 13:36:39.206052 cellworld-0.0.98/cellworld/
--rwxrwxrwx   0 german    (1000) german    (1000)      283 2022-07-15 13:36:37.000000 cellworld-0.0.98/cellworld/__init__.py
--rwxrwxrwx   0 german    (1000) german    (1000)     4512 2022-07-15 13:36:37.000000 cellworld-0.0.98/cellworld/agent_markers.py
--rwxrwxrwx   0 german    (1000) german    (1000)     1779 2022-07-15 13:36:37.000000 cellworld-0.0.98/cellworld/capture.py
--rwxrwxrwx   0 german    (1000) german    (1000)     3178 2022-07-15 13:36:37.000000 cellworld-0.0.98/cellworld/cell.py
--rwxrwxrwx   0 german    (1000) german    (1000)     1110 2022-07-15 13:36:37.000000 cellworld-0.0.98/cellworld/coordinates.py
--rwxrwxrwx   0 german    (1000) german    (1000)     8933 2022-07-15 13:36:37.000000 cellworld-0.0.98/cellworld/display.py
--rwxrwxrwx   0 german    (1000) german    (1000)    13008 2022-07-15 13:36:37.000000 cellworld-0.0.98/cellworld/experiment.py
--rwxrwxrwx   0 german    (1000) german    (1000)     1864 2022-07-15 13:36:37.000000 cellworld-0.0.98/cellworld/graph.py
--rwxrwxrwx   0 german    (1000) german    (1000)     3297 2022-07-15 13:36:37.000000 cellworld-0.0.98/cellworld/location.py
--rwxrwxrwx   0 german    (1000) german    (1000)     5661 2022-07-15 13:36:37.000000 cellworld-0.0.98/cellworld/shape.py
--rwxrwxrwx   0 german    (1000) german    (1000)     3143 2022-07-15 13:36:37.000000 cellworld-0.0.98/cellworld/util.py
--rwxrwxrwx   0 german    (1000) german    (1000)     1607 2022-07-15 13:36:37.000000 cellworld-0.0.98/cellworld/visibility.py
--rwxrwxrwx   0 german    (1000) german    (1000)    13422 2022-07-15 13:36:37.000000 cellworld-0.0.98/cellworld/world.py
-drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-07-15 13:36:39.265313 cellworld-0.0.98/cellworld.egg-info/
--rwxrwxrwx   0 german    (1000) german    (1000)      190 2022-07-15 13:36:38.000000 cellworld-0.0.98/cellworld.egg-info/PKG-INFO
--rwxrwxrwx   0 german    (1000) german    (1000)      483 2022-07-15 13:36:39.000000 cellworld-0.0.98/cellworld.egg-info/SOURCES.txt
--rwxrwxrwx   0 german    (1000) german    (1000)        1 2022-07-15 13:36:38.000000 cellworld-0.0.98/cellworld.egg-info/dependency_links.txt
--rwxrwxrwx   0 german    (1000) german    (1000)        1 2022-07-15 13:36:38.000000 cellworld-0.0.98/cellworld.egg-info/not-zip-safe
--rwxrwxrwx   0 german    (1000) german    (1000)       48 2022-07-15 13:36:38.000000 cellworld-0.0.98/cellworld.egg-info/requires.txt
--rwxrwxrwx   0 german    (1000) german    (1000)       10 2022-07-15 13:36:38.000000 cellworld-0.0.98/cellworld.egg-info/top_level.txt
--rwxrwxrwx   0 german    (1000) german    (1000)       38 2022-07-15 13:36:39.278599 cellworld-0.0.98/setup.cfg
--rwxrwxrwx   0 german    (1000) german    (1000)      334 2022-07-15 13:36:37.000000 cellworld-0.0.98/setup.py
+drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-07-15 13:41:21.571910 cellworld-0.0.99/
+-rwxrwxrwx   0 german    (1000) german    (1000)      190 2022-07-15 13:41:21.569917 cellworld-0.0.99/PKG-INFO
+drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-07-15 13:41:21.500696 cellworld-0.0.99/cellworld/
+-rwxrwxrwx   0 german    (1000) german    (1000)      283 2022-07-15 13:41:20.000000 cellworld-0.0.99/cellworld/__init__.py
+-rwxrwxrwx   0 german    (1000) german    (1000)     4512 2022-07-15 13:41:20.000000 cellworld-0.0.99/cellworld/agent_markers.py
+-rwxrwxrwx   0 german    (1000) german    (1000)     1779 2022-07-15 13:41:20.000000 cellworld-0.0.99/cellworld/capture.py
+-rwxrwxrwx   0 german    (1000) german    (1000)     3178 2022-07-15 13:41:20.000000 cellworld-0.0.99/cellworld/cell.py
+-rwxrwxrwx   0 german    (1000) german    (1000)     1110 2022-07-15 13:41:20.000000 cellworld-0.0.99/cellworld/coordinates.py
+-rwxrwxrwx   0 german    (1000) german    (1000)     8933 2022-07-15 13:41:20.000000 cellworld-0.0.99/cellworld/display.py
+-rwxrwxrwx   0 german    (1000) german    (1000)    13193 2022-07-15 13:41:20.000000 cellworld-0.0.99/cellworld/experiment.py
+-rwxrwxrwx   0 german    (1000) german    (1000)     1864 2022-07-15 13:41:20.000000 cellworld-0.0.99/cellworld/graph.py
+-rwxrwxrwx   0 german    (1000) german    (1000)     3297 2022-07-15 13:41:20.000000 cellworld-0.0.99/cellworld/location.py
+-rwxrwxrwx   0 german    (1000) german    (1000)     5661 2022-07-15 13:41:20.000000 cellworld-0.0.99/cellworld/shape.py
+-rwxrwxrwx   0 german    (1000) german    (1000)     3143 2022-07-15 13:41:20.000000 cellworld-0.0.99/cellworld/util.py
+-rwxrwxrwx   0 german    (1000) german    (1000)     1607 2022-07-15 13:41:20.000000 cellworld-0.0.99/cellworld/visibility.py
+-rwxrwxrwx   0 german    (1000) german    (1000)    13422 2022-07-15 13:41:20.000000 cellworld-0.0.99/cellworld/world.py
+drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-07-15 13:41:21.558921 cellworld-0.0.99/cellworld.egg-info/
+-rwxrwxrwx   0 german    (1000) german    (1000)      190 2022-07-15 13:41:20.000000 cellworld-0.0.99/cellworld.egg-info/PKG-INFO
+-rwxrwxrwx   0 german    (1000) german    (1000)      483 2022-07-15 13:41:21.000000 cellworld-0.0.99/cellworld.egg-info/SOURCES.txt
+-rwxrwxrwx   0 german    (1000) german    (1000)        1 2022-07-15 13:41:21.000000 cellworld-0.0.99/cellworld.egg-info/dependency_links.txt
+-rwxrwxrwx   0 german    (1000) german    (1000)        1 2022-07-15 13:41:20.000000 cellworld-0.0.99/cellworld.egg-info/not-zip-safe
+-rwxrwxrwx   0 german    (1000) german    (1000)       48 2022-07-15 13:41:21.000000 cellworld-0.0.99/cellworld.egg-info/requires.txt
+-rwxrwxrwx   0 german    (1000) german    (1000)       10 2022-07-15 13:41:21.000000 cellworld-0.0.99/cellworld.egg-info/top_level.txt
+-rwxrwxrwx   0 german    (1000) german    (1000)       38 2022-07-15 13:41:21.571910 cellworld-0.0.99/setup.cfg
+-rwxrwxrwx   0 german    (1000) german    (1000)      334 2022-07-15 13:41:20.000000 cellworld-0.0.99/setup.py
```

### Comparing `cellworld-0.0.98/cellworld/agent_markers.py` & `cellworld-0.0.99/cellworld/agent_markers.py`

 * *Files identical despite different names*

### Comparing `cellworld-0.0.98/cellworld/capture.py` & `cellworld-0.0.99/cellworld/capture.py`

 * *Files identical despite different names*

### Comparing `cellworld-0.0.98/cellworld/cell.py` & `cellworld-0.0.99/cellworld/cell.py`

 * *Files identical despite different names*

### Comparing `cellworld-0.0.98/cellworld/coordinates.py` & `cellworld-0.0.99/cellworld/coordinates.py`

 * *Files identical despite different names*

### Comparing `cellworld-0.0.98/cellworld/display.py` & `cellworld-0.0.99/cellworld/display.py`

 * *Files identical despite different names*

### Comparing `cellworld-0.0.98/cellworld/experiment.py` & `cellworld-0.0.99/cellworld/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                 time_dif = s.time_stamp - last_time_stamp[s.agent_name]
                 velocity = s.location.dist(last_locations[s.agent_name]) / time_dif
                 velocities[s.agent_name].append(velocity)
             last_locations[s.agent_name] = s.location
             last_time_stamp[s.agent_name] = s.time_stamp
         return velocities
 
-    def get_stops(self, distance_threshold: float = 0.01, stop_time: float = 0.5):
+    def get_stops_steps(self, distance_threshold: float = 0.01, stop_time: float = 0.5):
         stops = []
         future = 0
         for current in range(len(self)):
             if current <= future:
                 continue
             future = current
             last_future = future
@@ -132,20 +132,23 @@
                     future = last_future
                     break
                 last_future = future
                 future += 1
             if future == len(self):
                 break
             if self[current].time_stamp + stop_time < self[future].time_stamp:
-                stops.append((self[current].frame, self[future].frame))
+                stops.append((self[current], self[future]))
             else:
                 future = 0
         return stops
 
-    def get_filtered_velocities(self, complementary: float=None, outliers: float=None) -> {}:
+    def get_stops(self, distance_threshold: float = 0.01, stop_time: float = 0.5):
+        return [(b.frame, e.frame) for b, e in self.get_stops_steps(distance_threshold, stop_time)]
+
+    def get_filtered_velocities(self, complementary: float = None, outliers: float = None) -> {}:
         avs = self.get_velocities()
         for agent_name in avs:
             if outliers:
                 avs[agent_name] = avs[agent_name].outliers_filter(outliers)
             if complementary:
                 avs[agent_name] = avs[agent_name].complementary_filter(complementary)
         return avs
```

### Comparing `cellworld-0.0.98/cellworld/graph.py` & `cellworld-0.0.99/cellworld/graph.py`

 * *Files identical despite different names*

### Comparing `cellworld-0.0.98/cellworld/location.py` & `cellworld-0.0.99/cellworld/location.py`

 * *Files identical despite different names*

### Comparing `cellworld-0.0.98/cellworld/shape.py` & `cellworld-0.0.99/cellworld/shape.py`

 * *Files identical despite different names*

### Comparing `cellworld-0.0.98/cellworld/util.py` & `cellworld-0.0.99/cellworld/util.py`

 * *Files identical despite different names*

### Comparing `cellworld-0.0.98/cellworld/visibility.py` & `cellworld-0.0.99/cellworld/visibility.py`

 * *Files identical despite different names*

### Comparing `cellworld-0.0.98/cellworld/world.py` & `cellworld-0.0.99/cellworld/world.py`

 * *Files identical despite different names*

