# Comparing `tmp/pginter-0.2.8.tar.gz` & `tmp/pginter-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pginter-0.2.8.tar", last modified: Wed Jun 14 11:18:20 2023, max compression
+gzip compressed data, was "pginter-0.2.9.tar", last modified: Wed Jun 14 13:27:06 2023, max compression
```

## Comparing `pginter-0.2.8.tar` & `pginter-0.2.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:20.009806 pginter-0.2.8/
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.2.8/LICENSE
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      115 2023-05-31 20:31:36.000000 pginter-0.2.8/MANIFEST.in
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-14 11:18:20.009806 pginter-0.2.8/PKG-INFO
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.2.8/README.md
--rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      116 2023-05-24 18:38:46.000000 pginter-0.2.8/pyproject.toml
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-06-14 11:18:20.009806 pginter-0.2.8/setup.cfg
--rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)     1021 2023-06-14 11:04:25.000000 pginter-0.2.8/setup.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:19.989806 pginter-0.2.8/src/
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:19.993139 pginter-0.2.8/src/pginter/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.2.8/src/pginter/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     8707 2023-06-01 19:29:58.000000 pginter-0.2.8/src/pginter/_pg_root.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.2.8/src/pginter/icon.png
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:19.996472 pginter-0.2.8/src/pginter/theme/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.2.8/src/pginter/theme/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3997 2023-05-25 23:31:05.000000 pginter-0.2.8/src/pginter/theme/_manager.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:19.996472 pginter-0.2.8/src/pginter/theme/themes/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      673 2023-06-01 19:26:32.000000 pginter-0.2.8/src/pginter/theme/themes/default.json
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:20.003139 pginter-0.2.8/src/pginter/types/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      335 2023-05-25 22:58:36.000000 pginter-0.2.8/src/pginter/types/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.2.8/src/pginter/types/_better_dict.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      455 2023-05-25 19:05:55.000000 pginter-0.2.8/src/pginter/types/_binds.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4227 2023-05-25 23:31:05.000000 pginter-0.2.8/src/pginter/types/_color.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      456 2023-05-25 23:31:05.000000 pginter-0.2.8/src/pginter/types/_constants.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      273 2023-05-14 20:36:55.000000 pginter-0.2.8/src/pginter/types/_geo_types.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      161 2023-05-25 15:16:09.000000 pginter-0.2.8/src/pginter/types/_notifications.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5384 2023-05-30 12:53:46.000000 pginter-0.2.8/src/pginter/types/_scheme.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     6528 2023-05-15 19:07:58.000000 pginter-0.2.8/src/pginter/types/_style.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4301 2023-05-25 23:22:37.000000 pginter-0.2.8/src/pginter/types/_tk_vars.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:20.003139 pginter-0.2.8/src/pginter/utils/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      123 2023-06-14 09:10:26.000000 pginter-0.2.8/src/pginter/utils/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      873 2023-06-14 11:03:08.000000 pginter-0.2.8/src/pginter/utils/_funcs.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3250 2023-06-14 11:03:08.000000 pginter-0.2.8/src/pginter/utils/_image_funcs.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:20.009806 pginter-0.2.8/src/pginter/widgets/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      197 2023-05-25 22:58:36.000000 pginter-0.2.8/src/pginter/widgets/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4982 2023-05-25 10:36:44.000000 pginter-0.2.8/src/pginter/widgets/_button.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    14178 2023-05-30 19:45:06.000000 pginter-0.2.8/src/pginter/widgets/_entry.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    25890 2023-06-14 11:15:42.000000 pginter-0.2.8/src/pginter/widgets/_frame.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26315 2023-06-01 18:54:30.000000 pginter-0.2.8/src/pginter/widgets/_geo_manager.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5961 2023-05-30 19:49:43.000000 pginter-0.2.8/src/pginter/widgets/_label.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.2.8/src/pginter/widgets/_supports_children.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1022 2023-05-24 20:39:09.000000 pginter-0.2.8/src/pginter/widgets/_surface_frame.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:19.996472 pginter-0.2.8/src/pginter.egg-info/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-14 11:18:19.000000 pginter-0.2.8/src/pginter.egg-info/PKG-INFO
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1062 2023-06-14 11:18:19.000000 pginter-0.2.8/src/pginter.egg-info/SOURCES.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-06-14 11:18:19.000000 pginter-0.2.8/src/pginter.egg-info/dependency_links.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       33 2023-06-14 11:18:19.000000 pginter-0.2.8/src/pginter.egg-info/requires.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-06-14 11:18:19.000000 pginter-0.2.8/src/pginter.egg-info/top_level.txt
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 13:27:06.345321 pginter-0.2.9/
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.2.9/LICENSE
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      115 2023-05-31 20:31:36.000000 pginter-0.2.9/MANIFEST.in
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-14 13:27:06.345321 pginter-0.2.9/PKG-INFO
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.2.9/README.md
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      116 2023-05-24 18:38:46.000000 pginter-0.2.9/pyproject.toml
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-06-14 13:27:06.345321 pginter-0.2.9/setup.cfg
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)     1021 2023-06-14 11:18:53.000000 pginter-0.2.9/setup.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 13:27:06.335321 pginter-0.2.9/src/
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 13:27:06.338654 pginter-0.2.9/src/pginter/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.2.9/src/pginter/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     8972 2023-06-14 13:26:15.000000 pginter-0.2.9/src/pginter/_pg_root.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.2.9/src/pginter/icon.png
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 13:27:06.341988 pginter-0.2.9/src/pginter/theme/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.2.9/src/pginter/theme/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3997 2023-05-25 23:31:05.000000 pginter-0.2.9/src/pginter/theme/_manager.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 13:27:06.341988 pginter-0.2.9/src/pginter/theme/themes/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      673 2023-06-01 19:26:32.000000 pginter-0.2.9/src/pginter/theme/themes/default.json
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 13:27:06.345321 pginter-0.2.9/src/pginter/types/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      335 2023-05-25 22:58:36.000000 pginter-0.2.9/src/pginter/types/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.2.9/src/pginter/types/_better_dict.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      455 2023-05-25 19:05:55.000000 pginter-0.2.9/src/pginter/types/_binds.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4227 2023-05-25 23:31:05.000000 pginter-0.2.9/src/pginter/types/_color.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      456 2023-05-25 23:31:05.000000 pginter-0.2.9/src/pginter/types/_constants.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      317 2023-06-14 12:25:19.000000 pginter-0.2.9/src/pginter/types/_geo_types.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      161 2023-05-25 15:16:09.000000 pginter-0.2.9/src/pginter/types/_notifications.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5384 2023-05-30 12:53:46.000000 pginter-0.2.9/src/pginter/types/_scheme.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     6528 2023-05-15 19:07:58.000000 pginter-0.2.9/src/pginter/types/_style.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4301 2023-05-25 23:22:37.000000 pginter-0.2.9/src/pginter/types/_tk_vars.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 13:27:06.345321 pginter-0.2.9/src/pginter/utils/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      123 2023-06-14 09:10:26.000000 pginter-0.2.9/src/pginter/utils/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      873 2023-06-14 11:03:08.000000 pginter-0.2.9/src/pginter/utils/_funcs.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3250 2023-06-14 11:03:08.000000 pginter-0.2.9/src/pginter/utils/_image_funcs.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 13:27:06.345321 pginter-0.2.9/src/pginter/widgets/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      197 2023-05-25 22:58:36.000000 pginter-0.2.9/src/pginter/widgets/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4982 2023-05-25 10:36:44.000000 pginter-0.2.9/src/pginter/widgets/_button.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    14178 2023-05-30 19:45:06.000000 pginter-0.2.9/src/pginter/widgets/_entry.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26375 2023-06-14 13:26:15.000000 pginter-0.2.9/src/pginter/widgets/_frame.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26315 2023-06-14 13:21:30.000000 pginter-0.2.9/src/pginter/widgets/_geo_manager.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5961 2023-05-30 19:49:43.000000 pginter-0.2.9/src/pginter/widgets/_label.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.2.9/src/pginter/widgets/_supports_children.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1022 2023-05-24 20:39:09.000000 pginter-0.2.9/src/pginter/widgets/_surface_frame.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 13:27:06.338654 pginter-0.2.9/src/pginter.egg-info/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-14 13:27:06.000000 pginter-0.2.9/src/pginter.egg-info/PKG-INFO
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1062 2023-06-14 13:27:06.000000 pginter-0.2.9/src/pginter.egg-info/SOURCES.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-06-14 13:27:06.000000 pginter-0.2.9/src/pginter.egg-info/dependency_links.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       33 2023-06-14 13:27:06.000000 pginter-0.2.9/src/pginter.egg-info/requires.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-06-14 13:27:06.000000 pginter-0.2.9/src/pginter.egg-info/top_level.txt
```

### Comparing `pginter-0.2.8/LICENSE` & `pginter-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pginter-0.2.8/setup.py` & `pginter-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pginter",
-    version="0.2.8",
+    version="0.2.9",
     author="Nilusink",
     author_email="nilusink@protonmail.com",
     description="A python GUI interface, based on pygame",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nilusink/PgInter",
     # project_urls={
```

### Comparing `pginter-0.2.8/src/pginter/_pg_root.py` & `pginter-0.2.9/src/pginter/_pg_root.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     _theme: ThemeManager = ...
     __background: pg.Surface = ...
     layout_params: BetterDict = ...
     _min_size: tuple[int, int] = ...
     _bg_configured: bool = False
     _mouse_pos: tuple[int, int] = ...
     _max_framerate: int = ...
+    _requires_recalc: bool = True
 
     __timeouts: list[_TimeoutCandidate]
     _last_it_call: float
     _tpool: Pool
 
     show_wireframe: bool = False
 
@@ -182,14 +183,17 @@
         """
         match event:
             case ThemeManager.NotifyEvent.theme_reload:
                 # the theme has been reloaded
                 if not self._bg_configured:
                     self._bg = self.theme.root.bg.rgba
 
+            case GeoNotes.RequireRecalc:
+                self._requires_recalc = True
+
     # pygame stuff
     def _event_handler(self) -> None:
         """
         handle the events raised by pygame
         """
         for event in pg.event.get():
             match event.type:
@@ -206,15 +210,16 @@
                 case pg.KEYUP:
                     if self._focus_item is not None:
                         self._focus_item.notify(
                             KeyboardNotifyEvent.key_up,
                             event
                         )
 
-                # case pg.VIDEORESIZE:  # window size changed
+                case pg.VIDEORESIZE:  # window size changed
+                    self._requires_recalc = True
                 #     width, height = event.size
                 #
                 #     print("updating size: ", (width, height), "\t", self._min_size)
                 #
                 #     width = max([width, self._min_size[0]])
                 #     height = max([height, self._min_size[1]])
                 #
@@ -254,21 +259,24 @@
                 self._tpool.submit(curr_func)
                 self.__timeouts.remove(to)
 
     def update(self) -> None:
         """
         update the screen
         """
-        self.__background.fill(self._bg)
+        if self._requires_recalc:
+            self._requires_recalc = False
+
+            self.__background.fill(self._bg)
 
-        self.calculate_geometry()
-        for child, params in self._child_params:
-            child.draw(self.__background)
+            self.calculate_geometry()
+            for child, params in self._child_params:
+                child.draw(self.__background)
 
-        pg.display.flip()
+            pg.display.flip()
 
     def mainloop(self):
         """
         run the windows main loop
         """
         while self._running:
             self.update_idletasks()
```

### Comparing `pginter-0.2.8/src/pginter/icon.png` & `pginter-0.2.9/src/pginter/icon.png`

 * *Files identical despite different names*

### Comparing `pginter-0.2.8/src/pginter/theme/_manager.py` & `pginter-0.2.9/src/pginter/theme/_manager.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.8/src/pginter/theme/themes/default.json` & `pginter-0.2.9/src/pginter/theme/themes/default.json`

 * *Files identical despite different names*

### Comparing `pginter-0.2.8/src/pginter/types/_color.py` & `pginter-0.2.9/src/pginter/types/_color.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.8/src/pginter/types/_scheme.py` & `pginter-0.2.9/src/pginter/types/_scheme.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.8/src/pginter/types/_style.py` & `pginter-0.2.9/src/pginter/types/_style.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.8/src/pginter/types/_tk_vars.py` & `pginter-0.2.9/src/pginter/types/_tk_vars.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.8/src/pginter/utils/_funcs.py` & `pginter-0.2.9/src/pginter/utils/_funcs.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.8/src/pginter/utils/_image_funcs.py` & `pginter-0.2.9/src/pginter/utils/_image_funcs.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.8/src/pginter/widgets/_button.py` & `pginter-0.2.9/src/pginter/widgets/_button.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.8/src/pginter/widgets/_entry.py` & `pginter-0.2.9/src/pginter/widgets/_entry.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.8/src/pginter/widgets/_frame.py` & `pginter-0.2.9/src/pginter/widgets/_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     _focused: bool = False
     _binds: list[_Bind]
     style: Style = ...
     hover_style: Style = ...
     active_style: Style = ...
     _x: int = -1
     _y: int = -1
+    _last_size: tuple[int, int] = ...
 
     _image: Image.Image
 
     show_wireframe: bool = False
 
     def __init__(
             self,
@@ -422,14 +423,18 @@
     def get_position(self) -> tuple[int, int]:
         return self._x, self._y
 
     def draw(self, surface: pg.Surface) -> None:
         """
         draw the frame
         """
+        if hasattr(self, "debug_this"):
+            print("draw")
+        requires_recalc = False
+
         current_style = self.style
 
         if self.is_hover:
             current_style = self.style.overwrite(self.hover_style)
 
         if self.is_active:
             current_style = self.style.overwrite(self.hover_style).overwrite(
@@ -448,14 +453,23 @@
         if current_style.width is not ...:
             self.width = current_style.width
 
         else:
             self.unset_width()
 
         width, height = self.get_size()
+        if self._last_size is not ...:
+            if self._last_size[0] != width \
+                    or self._last_size[1] != height:
+                requires_recalc = True
+
+        else:
+            requires_recalc = True
+
+        self._last_size = (width, height)
 
         # check if the frame even exists
         if width <= 0 or height <= 0:
             # since the image doesn't affect the calculate_size function,
             # try to set the frames size through this piece of sh- code
             if self._image is not ...:
                 width, height = self.get_size()
@@ -478,14 +492,15 @@
 
                 if width > self._width:
                     self.width = width
 
                 if height > self._height:
                     self.height = height
 
+            self.root.notify(GeoNotes.RequireRecalc)
             return
 
         _surface = pg.Surface((width, height), pg.SRCALPHA)
 
         # draw the frame
         r_rect = pg.Rect((0, 0, width, height))
 
@@ -504,19 +519,17 @@
             image_width, image_height = self._image.size
 
             # try to reserve aspect angle
             if hasattr(self, "debug_this"):
                 print("size: ", width, height)
 
             if width <= 0 < height:
-                print("w0")
                 width = int((image_width / image_height) * height)
 
             if height <= 0 < width:
-                print("h0")
                 height = int((image_height / image_width) * width)
 
             # if no with or height has yet been set, clone the
             # original image's size
             if width <= 0:
                 width = image_width
 
@@ -629,14 +642,17 @@
                     w_text,
                     (
                         (self._x + width / 2) - w_text.get_width() / 2,
                         self._y
                     )
                 )
 
+        if requires_recalc:
+            self.root.notify(GeoNotes.RequireRecalc)
+
     def place(
             self,
             x: int,
             y: int,
     ) -> None:
         """
         place the frame in a parent container
```

### Comparing `pginter-0.2.8/src/pginter/widgets/_geo_manager.py` & `pginter-0.2.9/src/pginter/widgets/_geo_manager.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.8/src/pginter/widgets/_label.py` & `pginter-0.2.9/src/pginter/widgets/_label.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.8/src/pginter/widgets/_surface_frame.py` & `pginter-0.2.9/src/pginter/widgets/_surface_frame.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.8/src/pginter.egg-info/SOURCES.txt` & `pginter-0.2.9/src/pginter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

