# Comparing `tmp/graphdisplay-0.4.8.tar.gz` & `tmp/graphdisplay-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphdisplay-0.4.8.tar", last modified: Sat Jun 10 19:41:49 2023, max compression
+gzip compressed data, was "graphdisplay-0.4.9.tar", last modified: Wed Jun 14 21:35:01 2023, max compression
```

## Comparing `graphdisplay-0.4.8.tar` & `graphdisplay-0.4.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-10 19:41:49.916483 graphdisplay-0.4.8/
--rw-rw-r--   0 beto      (1000) beto      (1000)     1067 2023-05-06 20:46:34.000000 graphdisplay-0.4.8/LICENSE
--rw-rw-r--   0 beto      (1000) beto      (1000)     7953 2023-06-10 19:41:49.916483 graphdisplay-0.4.8/PKG-INFO
--rw-rw-r--   0 beto      (1000) beto      (1000)     7299 2023-06-10 18:55:10.000000 graphdisplay-0.4.8/README.md
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-10 19:41:49.912483 graphdisplay-0.4.8/graphdisplay/
--rw-rw-r--   0 beto      (1000) beto      (1000)     1344 2023-06-10 19:16:02.000000 graphdisplay-0.4.8/graphdisplay/__init__.py
--rw-rw-r--   0 beto      (1000) beto      (1000)     2309 2023-06-08 08:28:47.000000 graphdisplay-0.4.8/graphdisplay/about_win_manager.py
--rw-rw-r--   0 beto      (1000) beto      (1000)     5079 2023-06-10 19:41:48.000000 graphdisplay-0.4.8/graphdisplay/general_config.py
--rw-rw-r--   0 beto      (1000) beto      (1000)    38219 2023-06-10 18:55:10.000000 graphdisplay-0.4.8/graphdisplay/graphdisplay.py
--rw-rw-r--   0 beto      (1000) beto      (1000)    11353 2023-06-10 18:55:10.000000 graphdisplay-0.4.8/graphdisplay/graphdisplay.pyi
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-10 19:41:49.916483 graphdisplay-0.4.8/graphdisplay/graphs/
--rw-rw-r--   0 beto      (1000) beto      (1000)       24 2023-05-14 22:04:49.000000 graphdisplay-0.4.8/graphdisplay/graphs/__init__.py
--rw-rw-r--   0 beto      (1000) beto      (1000)    22482 2023-06-07 15:32:37.000000 graphdisplay-0.4.8/graphdisplay/graphs/graph.py
--rw-rw-r--   0 beto      (1000) beto      (1000)    12198 2023-06-10 18:55:10.000000 graphdisplay-0.4.8/graphdisplay/json_manager.py
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-10 19:41:49.916483 graphdisplay-0.4.8/graphdisplay/store/
--rw-rw-r--   0 beto      (1000) beto      (1000)        0 2023-05-06 20:46:34.000000 graphdisplay-0.4.8/graphdisplay/store/__init__.py
--rw-rw-r--   0 beto      (1000) beto      (1000)    18712 2023-06-08 08:22:05.000000 graphdisplay-0.4.8/graphdisplay/tools_win_manager.py
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-10 19:41:49.916483 graphdisplay-0.4.8/graphdisplay/trees/
--rw-rw-r--   0 beto      (1000) beto      (1000)       87 2023-05-14 22:04:49.000000 graphdisplay-0.4.8/graphdisplay/trees/__init__.py
--rw-rw-r--   0 beto      (1000) beto      (1000)     3524 2023-05-14 22:04:49.000000 graphdisplay-0.4.8/graphdisplay/trees/auto_balance_tree.py
--rw-rw-r--   0 beto      (1000) beto      (1000)     3068 2023-06-10 19:31:00.000000 graphdisplay-0.4.8/graphdisplay/trees/binary_search_tree.py
--rw-rw-r--   0 beto      (1000) beto      (1000)     6026 2023-05-28 11:58:14.000000 graphdisplay-0.4.8/graphdisplay/trees/binary_tree.py
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-10 19:41:49.912483 graphdisplay-0.4.8/graphdisplay.egg-info/
--rw-rw-r--   0 beto      (1000) beto      (1000)     7953 2023-06-10 19:41:49.000000 graphdisplay-0.4.8/graphdisplay.egg-info/PKG-INFO
--rw-rw-r--   0 beto      (1000) beto      (1000)      620 2023-06-10 19:41:49.000000 graphdisplay-0.4.8/graphdisplay.egg-info/SOURCES.txt
--rw-rw-r--   0 beto      (1000) beto      (1000)        1 2023-06-10 19:41:49.000000 graphdisplay-0.4.8/graphdisplay.egg-info/dependency_links.txt
--rw-rw-r--   0 beto      (1000) beto      (1000)       13 2023-06-10 19:41:49.000000 graphdisplay-0.4.8/graphdisplay.egg-info/top_level.txt
--rw-rw-r--   0 beto      (1000) beto      (1000)       38 2023-06-10 19:41:49.916483 graphdisplay-0.4.8/setup.cfg
--rw-rw-r--   0 beto      (1000) beto      (1000)     1763 2023-06-10 19:40:18.000000 graphdisplay-0.4.8/setup.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-14 21:35:01.773776 graphdisplay-0.4.9/
+-rw-rw-r--   0 beto      (1000) beto      (1000)     1067 2023-05-06 20:46:34.000000 graphdisplay-0.4.9/LICENSE
+-rw-rw-r--   0 beto      (1000) beto      (1000)     7953 2023-06-14 21:35:01.773776 graphdisplay-0.4.9/PKG-INFO
+-rw-rw-r--   0 beto      (1000) beto      (1000)     7299 2023-06-10 18:55:10.000000 graphdisplay-0.4.9/README.md
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-14 21:35:01.769776 graphdisplay-0.4.9/graphdisplay/
+-rw-rw-r--   0 beto      (1000) beto      (1000)     1370 2023-06-14 20:35:00.000000 graphdisplay-0.4.9/graphdisplay/__init__.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     2309 2023-06-08 08:28:47.000000 graphdisplay-0.4.9/graphdisplay/about_win_manager.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     5254 2023-06-14 21:34:11.000000 graphdisplay-0.4.9/graphdisplay/general_config.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)    40927 2023-06-14 21:21:25.000000 graphdisplay-0.4.9/graphdisplay/graphdisplay.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)    11452 2023-06-14 20:49:52.000000 graphdisplay-0.4.9/graphdisplay/graphdisplay.pyi
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-14 21:35:01.769776 graphdisplay-0.4.9/graphdisplay/graphs/
+-rw-rw-r--   0 beto      (1000) beto      (1000)       24 2023-05-14 22:04:49.000000 graphdisplay-0.4.9/graphdisplay/graphs/__init__.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)    22482 2023-06-07 15:32:37.000000 graphdisplay-0.4.9/graphdisplay/graphs/graph.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)    12198 2023-06-10 18:55:10.000000 graphdisplay-0.4.9/graphdisplay/json_manager.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-14 21:35:01.773776 graphdisplay-0.4.9/graphdisplay/store/
+-rw-rw-r--   0 beto      (1000) beto      (1000)        0 2023-05-06 20:46:34.000000 graphdisplay-0.4.9/graphdisplay/store/__init__.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)    18712 2023-06-08 08:22:05.000000 graphdisplay-0.4.9/graphdisplay/tools_win_manager.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-14 21:35:01.773776 graphdisplay-0.4.9/graphdisplay/trees/
+-rw-rw-r--   0 beto      (1000) beto      (1000)       87 2023-05-14 22:04:49.000000 graphdisplay-0.4.9/graphdisplay/trees/__init__.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     3524 2023-05-14 22:04:49.000000 graphdisplay-0.4.9/graphdisplay/trees/auto_balance_tree.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     3068 2023-06-14 14:48:26.000000 graphdisplay-0.4.9/graphdisplay/trees/binary_search_tree.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     6026 2023-06-14 14:48:26.000000 graphdisplay-0.4.9/graphdisplay/trees/binary_tree.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-14 21:35:01.769776 graphdisplay-0.4.9/graphdisplay.egg-info/
+-rw-rw-r--   0 beto      (1000) beto      (1000)     7953 2023-06-14 21:35:01.000000 graphdisplay-0.4.9/graphdisplay.egg-info/PKG-INFO
+-rw-rw-r--   0 beto      (1000) beto      (1000)      620 2023-06-14 21:35:01.000000 graphdisplay-0.4.9/graphdisplay.egg-info/SOURCES.txt
+-rw-rw-r--   0 beto      (1000) beto      (1000)        1 2023-06-14 21:35:01.000000 graphdisplay-0.4.9/graphdisplay.egg-info/dependency_links.txt
+-rw-rw-r--   0 beto      (1000) beto      (1000)       13 2023-06-14 21:35:01.000000 graphdisplay-0.4.9/graphdisplay.egg-info/top_level.txt
+-rw-rw-r--   0 beto      (1000) beto      (1000)       38 2023-06-14 21:35:01.773776 graphdisplay-0.4.9/setup.cfg
+-rw-rw-r--   0 beto      (1000) beto      (1000)     1384 2023-06-14 21:34:11.000000 graphdisplay-0.4.9/setup.py
```

### Comparing `graphdisplay-0.4.8/LICENSE` & `graphdisplay-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.8/PKG-INFO` & `graphdisplay-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdisplay
-Version: 0.4.8
+Version: 0.4.9
 Summary: Librería para representar grafos visualmente
 Home-page: https://github.com/seniorbeto
 Author: Alberto Penas Díaz (@seniorbeto)
 Author-email: albertopenasdiaz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `graphdisplay-0.4.8/README.md` & `graphdisplay-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.8/graphdisplay/__init__.py` & `graphdisplay-0.4.9/graphdisplay/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 DESCRIPTION:
+------------
 graphdisplay is a Python package for easy visualization of graphs and trees. It is built on top of the tkinter module,
 and is designed to be easy to use and integrate into your own projects. It also includes graph and tree data structures
 implementation based on the official Data Structures and Algorithms course at Carlos III University of Madrid.
 
 It is an open source project fully developed by Alberto Penas Díaz, used under a MIT license at: https://github.com/seniorbeto/graphdisplay
 
 USE EXAMPLES:
-
+-------------
 1.->
     from graphdisplay import GraphGUI, Graph
 
     labels = ['A', 'B', 'C', 'D', 'E']
     g = Graph(labels)
 
     # Now, we add the edges
```

### Comparing `graphdisplay-0.4.8/graphdisplay/about_win_manager.py` & `graphdisplay-0.4.9/graphdisplay/about_win_manager.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.8/graphdisplay/general_config.py` & `graphdisplay-0.4.9/graphdisplay/general_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,24 @@
-VERSION = '0.4.8'
+VERSION = '0.4.9'
+# Every 'int' value is in pixels
 DEFAULT_SCR_WIDTH = 600
 DEFAULT_SCR_HEIGHT = 600
 DEFAULT_NODE_RADIUS = 25
 DEFAULT_THEME = 'BROWN'
 BUTTON_HEIGHT = 30
 BUTTON_WIDTH = 60
 XMARGEN = 7
 YMARGEN = 7
+
+# For overlapped edges
+MIN_EDGE_SEPARATION = 80
+MAX_EDGE_SEPARATION = 220
+SEPARATION_RATIO = 5500 # In pixels
+SEPARATION_LABEL_RATIO = 3000
+
 THEMES = {
     "BROWN":{
         "BUTTON_COLOR": "#ede4cc",
         "SELECTED_VERTEX_COLOR": "#c2baa7",
         "VERTEX_COLOR": "#e3d7c5",
         "BACKGROUND_CANVAS_COLOR": "#c7b9a5",
         "FRAME_COLOR": "#87715f",
```

### Comparing `graphdisplay-0.4.8/graphdisplay/graphdisplay.py` & `graphdisplay-0.4.9/graphdisplay/graphdisplay.py`

 * *Files 5% similar despite different names*

```diff
@@ -685,15 +685,15 @@
                  text_color: str = "black"):
 
         if type(canvas) != tk.Canvas:
             raise TypeError("canvas must be a tkinter canvas object")
         if type(start) != Node or type(end) != Node:
             raise TypeError("start and end must be Node objects")
 
-        self.__canvas = canvas
+        self.__canvas: tk.Canvas = canvas
         self.overlapped = overlapped
         self.__start_node = start
         self.__end_node = end
         self.__weight = weight
         self.__window_color = window_color
         self.__text_color = text_color
         self.__start = self.__calculate_start(start, end)
@@ -706,63 +706,122 @@
 
     def __str__(self):
         return 'Edge: ' + str(self.__start_node.id) + ' -> ' + str(self.__end_node.id)
 
     def update_position(self) -> None:
         """Updates the position of the edge by recalculating the start and end node position"""
         self.__recalculate()
-        self.__canvas.coords(self.line, self.__start[0], self.__start[1], self.__end[0], self.__end[1])
+        if not self.overlapped:
+            self.__canvas.coords(self.line, self.__start[0], self.__start[1], self.__end[0], self.__end[1])
+        else:
+            new_displacement = self.__get_displacement()
+            self.__canvas.coords(self.line, self.__start[0],
+                                 self.__start[1],
+                                 new_displacement[0],
+                                 new_displacement[1],
+                                 self.__end[0],
+                                 self.__end[1])
         if self.__weight:
             if not self.overlapped:
                 self.__canvas.coords(self.window, (self.__start[0] + self.__end[0]) // 2, (self.__start[1] + self.__end[1]) // 2)
             else:
-                self.__canvas.coords(self.window, self.__start[0] * 0.2 + self.__end[0] * 0.8, self.__start[1] * 0.2 + self.__end[1] * 0.8)
+                self.__canvas.coords(self.window, new_displacement[2], new_displacement[3])
 
     def terminate(self) -> None:
-        """Deletes the edge from the canvas and removes it from the asociated edges of the start and end nodes"""
+        """Deletes the edge from the canvas and removes it from the associated edges of the start and end nodes"""
         self.__canvas.delete(self.line)
         if self.__weight:
             self.__canvas.delete(self.window)
 
         if self in self.__end_node.associated_edges_IN:
             self.__end_node.associated_edges_IN.remove(self)
         if self in self.__start_node.associated_edges_OUT:
             self.__start_node.associated_edges_OUT.remove(self)
 
     def show(self) -> None:
         """Displays the edge in the canvas"""
-        self.line = self.__canvas.create_line(self.__start[0],
-                                            self.__start[1],
-                                            self.__end[0],
-                                            self.__end[1],
-                                            arrow=tk.LAST,
-                                            width=1.5)
+        # Line creation
+        if not self.overlapped:
+            self.line = self.__canvas.create_line(self.__start[0],
+                                                  self.__start[1],
+                                                  self.__end[0],
+                                                  self.__end[1],
+                                                  arrow=tk.LAST,
+                                                  arrowshape=(10, 12, 5),
+                                                  width=1.5)
+        else:
+            displacement = self.__get_displacement()
+            self.line = self.__canvas.create_line(self.__start[0],
+                                                  self.__start[1],
+
+                                                  displacement[0],
+                                                  displacement[1],
+
+                                                  self.__end[0],
+                                                  self.__end[1],
+                                                  arrow=tk.LAST,
+                                                  width=1.5,
+                                                  arrowshape=(10, 12, 5),
+                                                  smooth=True,
+                                                  splinesteps=100)
+
         if self.__weight:
             if not self.overlapped:
                 self.window = self.__canvas.create_window((self.__start[0] + self.__end[0]) // 2,
                                                         (self.__start[1] + self.__end[1]) // 2,
                                                         window=tk.Label(self.__canvas,
                                                                         bg=self.__window_color,
                                                                         text=str(self.__weight),
                                                                         font=("Arial", 13),
                                                                         fg=self.__text_color))
             else:
-                self.window = self.__canvas.create_window((self.__start[0] * 0.2 + self.__end[0] * 0.8),
-                                                        (self.__start[1] * 0.2 + self.__end[1] * 0.8),
+                self.window = self.__canvas.create_window(displacement[2],
+                                                        displacement[3],
                                                         window=tk.Label(self.__canvas,
                                                                         bg=self.__window_color,
                                                                         text=str(self.__weight),
                                                                         font=("Arial", 13),
                                                                         fg=self.__text_color))
 
     def __recalculate(self) -> None:
         """Recalculates the start and end position of the edge"""
         self.__start = self.__calculate_start(self.__start_node, self.__end_node)
         self.__end = self.__calculate_end(self.__start_node, self.__end_node)
 
+    def __get_displacement(self) -> tuple:
+        """
+        When an edge is overlapped, it calculates de displacement of the arrow by calculating the middle
+        point between the start and end nodes and then, calculating the angle between the line that connects
+        the start and end nodes and the horizontal line.
+        """
+        center_start = (self.__start_node.pos_x + self.__start_node.radius, self.__start_node.pos_y + self.__start_node.radius)
+        center_end = (self.__end_node.pos_x + self.__end_node.radius, self.__end_node.pos_y + self.__end_node.radius)
+
+        x1 = center_start[0]
+        y1 = center_start[1]
+        x2 = center_end[0]
+        y2 = center_end[1]
+
+        distance = min(max(math.sqrt((x2 - x1) ** 2 + (y2 - y1) ** 2) / 2, MIN_EDGE_SEPARATION), MAX_EDGE_SEPARATION)
+
+        x = x2 - x1
+        y = y2 - y1
+        edge_angle = math.atan2(y, x)
+
+        mid_point_x = (x1 + x2) // 2
+        mid_point_y = (y1 + y2) // 2
+        displacement_x = mid_point_x + math.sin(edge_angle) * SEPARATION_RATIO/distance
+        displacement_y = mid_point_y - math.cos(edge_angle) * SEPARATION_RATIO/distance
+
+        label_position_x = mid_point_x + math.sin(edge_angle) * SEPARATION_LABEL_RATIO/distance
+        label_position_y = mid_point_y - math.cos(edge_angle) * SEPARATION_LABEL_RATIO/distance
+
+        return displacement_x, displacement_y, label_position_x, label_position_y
+
+
     def __calculate_start(self, start: Node, end: Node) -> tuple:
         """
         It calculates the initial position of the arrow that connects the nodes "start" and "end"
         :param start: Node
         :param end: Node
         :return: tuple with the initial position of the arrow
         """
@@ -775,15 +834,15 @@
         y2 = center_end[1]
 
         x = x2 - x1
         y = y2 - y1
         edge_angle = math.atan2(y, x) * (180.0 / math.pi)
         x = math.cos(math.radians(edge_angle)) * start.radius
         y = math.sin(math.radians(edge_angle)) * start.radius
-        return (center_start[0] + int(x), center_start[1] + int(y))
+        return center_start[0] + int(x), center_start[1] + int(y)
 
     def __calculate_end(self, start: Node, end: Node) -> tuple:
         """
         It calculates the final position of the arrow that connects the nodes "start" and "end"
         :param start: Node
         :param end: Node
         :return: tuple with the final position of the arrow
@@ -797,15 +856,15 @@
         y2 = center_end[1]
 
         x = x2 - x1
         y = y2 - y1
         edge_angle = math.atan2(y, x) * (180.0 / math.pi)
         x = math.cos(math.radians(edge_angle)) * end.radius
         y = math.sin(math.radians(edge_angle)) * end.radius
-        return  (center_end[0] - int(x), center_end[1] - int(y))
+        return  center_end[0] - int(x), center_end[1] - int(y)
 
     @property
     def start_node(self):
         return self.__start_node
 
     @property
     def end_node(self):
```

### Comparing `graphdisplay-0.4.8/graphdisplay/graphdisplay.pyi` & `graphdisplay-0.4.9/graphdisplay/graphdisplay.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Coding: utf-8
 """
 DESCRIPTION:
+------------
 graphdisplay is a Python package for easy visualization of graphs and trees. It is built on top of the tkinter module,
 and is designed to be easy to use and integrate into your own projects. It also includes graph and tree data structures
 implementation based on the official Data Structures and Algorithms course at Carlos III University of Madrid.
 
 It is an open source project fully developed by Alberto Penas Díaz, used under a MIT license at: https://github.com/seniorbeto/graphdisplay
 
 USE EXAMPLES:
-
+-------------
 1.->
     from graphdisplay import GraphGUI, Graph
 
     labels = ['A', 'B', 'C', 'D', 'E']
     g = Graph(labels)
 
     # Now, we add the edges
@@ -83,15 +84,15 @@
         runs normally.
 
     Returns
     -------
     GraphGUI.__GraphGUI : Any
         The GraphGUI object.
     """
-    def __new__(cls, graph: Any) -> None:...
+    def __new__(cls: type, graph: Any) -> None:...
     def __getattr__(self, name: Any) -> Any: ...
     def __setattr__(self, name: Any, value: Any) -> None: ...
     @staticmethod
     def _generate(graph: Any, instance: int) -> GraphGUI.__GraphGUI: ...
 
     class __GraphGUI:
         """
@@ -297,9 +298,10 @@
                  text_color: str = "black") -> None:
         ...
     def __str__(self)-> str: ...
     def update_position(self) -> None: ...
     def terminate(self) -> None: ...
     def show(self) -> None: ...
     def __recalculate(self) -> None: ...
+    def __get_displacement(self) -> tuple[int, int, int, int]: ...
     def __calculate_start(self, start: Node, end: Node) -> tuple[int, int]: ...
     def __calculate_end(self, start: Node, end: Node) -> tuple[int, int]: ...
```

### Comparing `graphdisplay-0.4.8/graphdisplay/graphs/graph.py` & `graphdisplay-0.4.9/graphdisplay/graphs/graph.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.8/graphdisplay/json_manager.py` & `graphdisplay-0.4.9/graphdisplay/json_manager.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.8/graphdisplay/tools_win_manager.py` & `graphdisplay-0.4.9/graphdisplay/tools_win_manager.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.8/graphdisplay/trees/auto_balance_tree.py` & `graphdisplay-0.4.9/graphdisplay/trees/auto_balance_tree.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.8/graphdisplay/trees/binary_search_tree.py` & `graphdisplay-0.4.9/graphdisplay/trees/binary_search_tree.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.8/graphdisplay/trees/binary_tree.py` & `graphdisplay-0.4.9/graphdisplay/trees/binary_tree.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.8/graphdisplay.egg-info/PKG-INFO` & `graphdisplay-0.4.9/graphdisplay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdisplay
-Version: 0.4.8
+Version: 0.4.9
 Summary: Librería para representar grafos visualmente
 Home-page: https://github.com/seniorbeto
 Author: Alberto Penas Díaz (@seniorbeto)
 Author-email: albertopenasdiaz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `graphdisplay-0.4.8/graphdisplay.egg-info/SOURCES.txt` & `graphdisplay-0.4.9/graphdisplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.8/setup.py` & `graphdisplay-0.4.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,28 +17,14 @@
 LONG_DESC_TYPE = "text/markdown"
 
 
 INSTALL_REQUIRES = [
       'tk==0.1.1'
       ]
 
-path = os.getcwd()
-try:
-    if os.path.exists(os.path.join(path, "permanent.json")):
-        os.remove(os.path.join(path, "permanent.json"))
-except FileNotFoundError:
-    pass
-
-store_path = os.path.join(path, "graphdisplay/store/")
-
-for file in os.listdir(store_path):
-    if file.endswith(".json"):
-        removing = os.path.join(store_path, file)
-        os.remove(removing)
-
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type=LONG_DESC_TYPE,
     author=AUTHOR,
```

