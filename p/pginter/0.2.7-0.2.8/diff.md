# Comparing `tmp/pginter-0.2.7.tar.gz` & `tmp/pginter-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pginter-0.2.7.tar", last modified: Wed Jun 14 11:04:03 2023, max compression
+gzip compressed data, was "pginter-0.2.8.tar", last modified: Wed Jun 14 11:18:20 2023, max compression
```

## Comparing `pginter-0.2.7.tar` & `pginter-0.2.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.092187 pginter-0.2.7/
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.2.7/LICENSE
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      115 2023-05-31 20:31:36.000000 pginter-0.2.7/MANIFEST.in
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-14 11:04:03.092187 pginter-0.2.7/PKG-INFO
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.2.7/README.md
--rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      116 2023-05-24 18:38:46.000000 pginter-0.2.7/pyproject.toml
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-06-14 11:04:03.092187 pginter-0.2.7/setup.cfg
--rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)     1021 2023-06-13 15:28:20.000000 pginter-0.2.7/setup.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.068853 pginter-0.2.7/src/
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.075520 pginter-0.2.7/src/pginter/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.2.7/src/pginter/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     8707 2023-06-01 19:29:58.000000 pginter-0.2.7/src/pginter/_pg_root.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.2.7/src/pginter/icon.png
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.078853 pginter-0.2.7/src/pginter/theme/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.2.7/src/pginter/theme/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3997 2023-05-25 23:31:05.000000 pginter-0.2.7/src/pginter/theme/_manager.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.078853 pginter-0.2.7/src/pginter/theme/themes/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      673 2023-06-01 19:26:32.000000 pginter-0.2.7/src/pginter/theme/themes/default.json
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.082186 pginter-0.2.7/src/pginter/types/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      335 2023-05-25 22:58:36.000000 pginter-0.2.7/src/pginter/types/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.2.7/src/pginter/types/_better_dict.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      455 2023-05-25 19:05:55.000000 pginter-0.2.7/src/pginter/types/_binds.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4227 2023-05-25 23:31:05.000000 pginter-0.2.7/src/pginter/types/_color.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      456 2023-05-25 23:31:05.000000 pginter-0.2.7/src/pginter/types/_constants.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      273 2023-05-14 20:36:55.000000 pginter-0.2.7/src/pginter/types/_geo_types.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      161 2023-05-25 15:16:09.000000 pginter-0.2.7/src/pginter/types/_notifications.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5384 2023-05-30 12:53:46.000000 pginter-0.2.7/src/pginter/types/_scheme.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     6528 2023-05-15 19:07:58.000000 pginter-0.2.7/src/pginter/types/_style.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4301 2023-05-25 23:22:37.000000 pginter-0.2.7/src/pginter/types/_tk_vars.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.088853 pginter-0.2.7/src/pginter/utils/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      123 2023-06-14 09:10:26.000000 pginter-0.2.7/src/pginter/utils/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      873 2023-06-14 11:03:08.000000 pginter-0.2.7/src/pginter/utils/_funcs.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3250 2023-06-14 11:03:08.000000 pginter-0.2.7/src/pginter/utils/_image_funcs.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.092187 pginter-0.2.7/src/pginter/widgets/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      197 2023-05-25 22:58:36.000000 pginter-0.2.7/src/pginter/widgets/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4982 2023-05-25 10:36:44.000000 pginter-0.2.7/src/pginter/widgets/_button.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    14178 2023-05-30 19:45:06.000000 pginter-0.2.7/src/pginter/widgets/_entry.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    25984 2023-06-14 09:10:26.000000 pginter-0.2.7/src/pginter/widgets/_frame.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26315 2023-06-01 18:54:30.000000 pginter-0.2.7/src/pginter/widgets/_geo_manager.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5961 2023-05-30 19:49:43.000000 pginter-0.2.7/src/pginter/widgets/_label.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.2.7/src/pginter/widgets/_supports_children.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1022 2023-05-24 20:39:09.000000 pginter-0.2.7/src/pginter/widgets/_surface_frame.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.075520 pginter-0.2.7/src/pginter.egg-info/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-14 11:04:03.000000 pginter-0.2.7/src/pginter.egg-info/PKG-INFO
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1062 2023-06-14 11:04:03.000000 pginter-0.2.7/src/pginter.egg-info/SOURCES.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-06-14 11:04:03.000000 pginter-0.2.7/src/pginter.egg-info/dependency_links.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       33 2023-06-14 11:04:03.000000 pginter-0.2.7/src/pginter.egg-info/requires.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-06-14 11:04:03.000000 pginter-0.2.7/src/pginter.egg-info/top_level.txt
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:20.009806 pginter-0.2.8/
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.2.8/LICENSE
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      115 2023-05-31 20:31:36.000000 pginter-0.2.8/MANIFEST.in
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-14 11:18:20.009806 pginter-0.2.8/PKG-INFO
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.2.8/README.md
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      116 2023-05-24 18:38:46.000000 pginter-0.2.8/pyproject.toml
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-06-14 11:18:20.009806 pginter-0.2.8/setup.cfg
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)     1021 2023-06-14 11:04:25.000000 pginter-0.2.8/setup.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:19.989806 pginter-0.2.8/src/
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:19.993139 pginter-0.2.8/src/pginter/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.2.8/src/pginter/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     8707 2023-06-01 19:29:58.000000 pginter-0.2.8/src/pginter/_pg_root.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.2.8/src/pginter/icon.png
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:19.996472 pginter-0.2.8/src/pginter/theme/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.2.8/src/pginter/theme/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3997 2023-05-25 23:31:05.000000 pginter-0.2.8/src/pginter/theme/_manager.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:19.996472 pginter-0.2.8/src/pginter/theme/themes/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      673 2023-06-01 19:26:32.000000 pginter-0.2.8/src/pginter/theme/themes/default.json
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:20.003139 pginter-0.2.8/src/pginter/types/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      335 2023-05-25 22:58:36.000000 pginter-0.2.8/src/pginter/types/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.2.8/src/pginter/types/_better_dict.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      455 2023-05-25 19:05:55.000000 pginter-0.2.8/src/pginter/types/_binds.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4227 2023-05-25 23:31:05.000000 pginter-0.2.8/src/pginter/types/_color.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      456 2023-05-25 23:31:05.000000 pginter-0.2.8/src/pginter/types/_constants.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      273 2023-05-14 20:36:55.000000 pginter-0.2.8/src/pginter/types/_geo_types.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      161 2023-05-25 15:16:09.000000 pginter-0.2.8/src/pginter/types/_notifications.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5384 2023-05-30 12:53:46.000000 pginter-0.2.8/src/pginter/types/_scheme.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     6528 2023-05-15 19:07:58.000000 pginter-0.2.8/src/pginter/types/_style.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4301 2023-05-25 23:22:37.000000 pginter-0.2.8/src/pginter/types/_tk_vars.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:20.003139 pginter-0.2.8/src/pginter/utils/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      123 2023-06-14 09:10:26.000000 pginter-0.2.8/src/pginter/utils/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      873 2023-06-14 11:03:08.000000 pginter-0.2.8/src/pginter/utils/_funcs.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3250 2023-06-14 11:03:08.000000 pginter-0.2.8/src/pginter/utils/_image_funcs.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:20.009806 pginter-0.2.8/src/pginter/widgets/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      197 2023-05-25 22:58:36.000000 pginter-0.2.8/src/pginter/widgets/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4982 2023-05-25 10:36:44.000000 pginter-0.2.8/src/pginter/widgets/_button.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    14178 2023-05-30 19:45:06.000000 pginter-0.2.8/src/pginter/widgets/_entry.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    25890 2023-06-14 11:15:42.000000 pginter-0.2.8/src/pginter/widgets/_frame.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26315 2023-06-01 18:54:30.000000 pginter-0.2.8/src/pginter/widgets/_geo_manager.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5961 2023-05-30 19:49:43.000000 pginter-0.2.8/src/pginter/widgets/_label.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.2.8/src/pginter/widgets/_supports_children.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1022 2023-05-24 20:39:09.000000 pginter-0.2.8/src/pginter/widgets/_surface_frame.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:18:19.996472 pginter-0.2.8/src/pginter.egg-info/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-14 11:18:19.000000 pginter-0.2.8/src/pginter.egg-info/PKG-INFO
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1062 2023-06-14 11:18:19.000000 pginter-0.2.8/src/pginter.egg-info/SOURCES.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-06-14 11:18:19.000000 pginter-0.2.8/src/pginter.egg-info/dependency_links.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       33 2023-06-14 11:18:19.000000 pginter-0.2.8/src/pginter.egg-info/requires.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-06-14 11:18:19.000000 pginter-0.2.8/src/pginter.egg-info/top_level.txt
```

### Comparing `pginter-0.2.7/LICENSE` & `pginter-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pginter-0.2.7/setup.py` & `pginter-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pginter",
-    version="0.2.7",
+    version="0.2.8",
     author="Nilusink",
     author_email="nilusink@protonmail.com",
     description="A python GUI interface, based on pygame",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nilusink/PgInter",
     # project_urls={
```

### Comparing `pginter-0.2.7/src/pginter/_pg_root.py` & `pginter-0.2.8/src/pginter/_pg_root.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.7/src/pginter/icon.png` & `pginter-0.2.8/src/pginter/icon.png`

 * *Files identical despite different names*

### Comparing `pginter-0.2.7/src/pginter/theme/_manager.py` & `pginter-0.2.8/src/pginter/theme/_manager.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.7/src/pginter/theme/themes/default.json` & `pginter-0.2.8/src/pginter/theme/themes/default.json`

 * *Files identical despite different names*

### Comparing `pginter-0.2.7/src/pginter/types/_color.py` & `pginter-0.2.8/src/pginter/types/_color.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.7/src/pginter/types/_scheme.py` & `pginter-0.2.8/src/pginter/types/_scheme.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.7/src/pginter/types/_style.py` & `pginter-0.2.8/src/pginter/types/_style.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.7/src/pginter/types/_tk_vars.py` & `pginter-0.2.8/src/pginter/types/_tk_vars.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.7/src/pginter/utils/_funcs.py` & `pginter-0.2.8/src/pginter/utils/_funcs.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.7/src/pginter/utils/_image_funcs.py` & `pginter-0.2.8/src/pginter/utils/_image_funcs.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.7/src/pginter/widgets/_button.py` & `pginter-0.2.8/src/pginter/widgets/_button.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.7/src/pginter/widgets/_entry.py` & `pginter-0.2.8/src/pginter/widgets/_entry.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.7/src/pginter/widgets/_frame.py` & `pginter-0.2.8/src/pginter/widgets/_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -504,33 +504,29 @@
             image_width, image_height = self._image.size
 
             # try to reserve aspect angle
             if hasattr(self, "debug_this"):
                 print("size: ", width, height)
 
             if width <= 0 < height:
+                print("w0")
                 width = int((image_width / image_height) * height)
 
             if height <= 0 < width:
+                print("h0")
                 height = int((image_height / image_width) * width)
 
             # if no with or height has yet been set, clone the
             # original image's size
             if width <= 0:
                 width = image_width
 
             if height <= 0:
                 height = image_height
 
-            if width >= self._width:
-                self.width = width
-
-            if height >= self._height:
-                self.height = height
-
             # center image
             pos = (
                 self.assigned_width / 2 - width / 2,
                 self.assigned_height / 2 - height / 2
             )
 
             pos = (
```

### Comparing `pginter-0.2.7/src/pginter/widgets/_geo_manager.py` & `pginter-0.2.8/src/pginter/widgets/_geo_manager.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.7/src/pginter/widgets/_label.py` & `pginter-0.2.8/src/pginter/widgets/_label.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.7/src/pginter/widgets/_surface_frame.py` & `pginter-0.2.8/src/pginter/widgets/_surface_frame.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.7/src/pginter.egg-info/SOURCES.txt` & `pginter-0.2.8/src/pginter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

