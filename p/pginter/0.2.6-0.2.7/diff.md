# Comparing `tmp/pginter-0.2.6.tar.gz` & `tmp/pginter-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pginter-0.2.6.tar", last modified: Tue Jun 13 15:28:01 2023, max compression
+gzip compressed data, was "pginter-0.2.7.tar", last modified: Wed Jun 14 11:04:03 2023, max compression
```

## Comparing `pginter-0.2.6.tar` & `pginter-0.2.7.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.828294 pginter-0.2.6/
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.2.6/LICENSE
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      115 2023-05-31 20:31:36.000000 pginter-0.2.6/MANIFEST.in
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-13 15:28:01.824960 pginter-0.2.6/PKG-INFO
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.2.6/README.md
--rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      116 2023-05-24 18:38:46.000000 pginter-0.2.6/pyproject.toml
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-06-13 15:28:01.828294 pginter-0.2.6/setup.cfg
--rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)     1021 2023-06-13 14:30:14.000000 pginter-0.2.6/setup.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.818293 pginter-0.2.6/src/
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.821627 pginter-0.2.6/src/pginter/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.2.6/src/pginter/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     8707 2023-06-01 19:29:58.000000 pginter-0.2.6/src/pginter/_pg_root.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.2.6/src/pginter/icon.png
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.821627 pginter-0.2.6/src/pginter/theme/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.2.6/src/pginter/theme/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3997 2023-05-25 23:31:05.000000 pginter-0.2.6/src/pginter/theme/_manager.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.821627 pginter-0.2.6/src/pginter/theme/themes/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      673 2023-06-01 19:26:32.000000 pginter-0.2.6/src/pginter/theme/themes/default.json
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.824960 pginter-0.2.6/src/pginter/types/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      335 2023-05-25 22:58:36.000000 pginter-0.2.6/src/pginter/types/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.2.6/src/pginter/types/_better_dict.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      455 2023-05-25 19:05:55.000000 pginter-0.2.6/src/pginter/types/_binds.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4227 2023-05-25 23:31:05.000000 pginter-0.2.6/src/pginter/types/_color.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      456 2023-05-25 23:31:05.000000 pginter-0.2.6/src/pginter/types/_constants.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      273 2023-05-14 20:36:55.000000 pginter-0.2.6/src/pginter/types/_geo_types.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      161 2023-05-25 15:16:09.000000 pginter-0.2.6/src/pginter/types/_notifications.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5384 2023-05-30 12:53:46.000000 pginter-0.2.6/src/pginter/types/_scheme.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     6528 2023-05-15 19:07:58.000000 pginter-0.2.6/src/pginter/types/_style.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4301 2023-05-25 23:22:37.000000 pginter-0.2.6/src/pginter/types/_tk_vars.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.824960 pginter-0.2.6/src/pginter/utils/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       63 2023-06-13 15:26:29.000000 pginter-0.2.6/src/pginter/utils/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1486 2023-06-13 15:27:29.000000 pginter-0.2.6/src/pginter/utils/_funcs.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.824960 pginter-0.2.6/src/pginter/widgets/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      197 2023-05-25 22:58:36.000000 pginter-0.2.6/src/pginter/widgets/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4982 2023-05-25 10:36:44.000000 pginter-0.2.6/src/pginter/widgets/_button.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    14178 2023-05-30 19:45:06.000000 pginter-0.2.6/src/pginter/widgets/_entry.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    28606 2023-06-13 15:27:29.000000 pginter-0.2.6/src/pginter/widgets/_frame.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26315 2023-06-01 18:54:30.000000 pginter-0.2.6/src/pginter/widgets/_geo_manager.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5961 2023-05-30 19:49:43.000000 pginter-0.2.6/src/pginter/widgets/_label.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.2.6/src/pginter/widgets/_supports_children.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1022 2023-05-24 20:39:09.000000 pginter-0.2.6/src/pginter/widgets/_surface_frame.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.821627 pginter-0.2.6/src/pginter.egg-info/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-13 15:28:01.000000 pginter-0.2.6/src/pginter.egg-info/PKG-INFO
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1028 2023-06-13 15:28:01.000000 pginter-0.2.6/src/pginter.egg-info/SOURCES.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-06-13 15:28:01.000000 pginter-0.2.6/src/pginter.egg-info/dependency_links.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       33 2023-06-13 15:28:01.000000 pginter-0.2.6/src/pginter.egg-info/requires.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-06-13 15:28:01.000000 pginter-0.2.6/src/pginter.egg-info/top_level.txt
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.092187 pginter-0.2.7/
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.2.7/LICENSE
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      115 2023-05-31 20:31:36.000000 pginter-0.2.7/MANIFEST.in
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-14 11:04:03.092187 pginter-0.2.7/PKG-INFO
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.2.7/README.md
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      116 2023-05-24 18:38:46.000000 pginter-0.2.7/pyproject.toml
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-06-14 11:04:03.092187 pginter-0.2.7/setup.cfg
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)     1021 2023-06-13 15:28:20.000000 pginter-0.2.7/setup.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.068853 pginter-0.2.7/src/
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.075520 pginter-0.2.7/src/pginter/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.2.7/src/pginter/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     8707 2023-06-01 19:29:58.000000 pginter-0.2.7/src/pginter/_pg_root.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.2.7/src/pginter/icon.png
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.078853 pginter-0.2.7/src/pginter/theme/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.2.7/src/pginter/theme/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3997 2023-05-25 23:31:05.000000 pginter-0.2.7/src/pginter/theme/_manager.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.078853 pginter-0.2.7/src/pginter/theme/themes/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      673 2023-06-01 19:26:32.000000 pginter-0.2.7/src/pginter/theme/themes/default.json
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.082186 pginter-0.2.7/src/pginter/types/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      335 2023-05-25 22:58:36.000000 pginter-0.2.7/src/pginter/types/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.2.7/src/pginter/types/_better_dict.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      455 2023-05-25 19:05:55.000000 pginter-0.2.7/src/pginter/types/_binds.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4227 2023-05-25 23:31:05.000000 pginter-0.2.7/src/pginter/types/_color.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      456 2023-05-25 23:31:05.000000 pginter-0.2.7/src/pginter/types/_constants.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      273 2023-05-14 20:36:55.000000 pginter-0.2.7/src/pginter/types/_geo_types.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      161 2023-05-25 15:16:09.000000 pginter-0.2.7/src/pginter/types/_notifications.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5384 2023-05-30 12:53:46.000000 pginter-0.2.7/src/pginter/types/_scheme.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     6528 2023-05-15 19:07:58.000000 pginter-0.2.7/src/pginter/types/_style.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4301 2023-05-25 23:22:37.000000 pginter-0.2.7/src/pginter/types/_tk_vars.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.088853 pginter-0.2.7/src/pginter/utils/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      123 2023-06-14 09:10:26.000000 pginter-0.2.7/src/pginter/utils/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      873 2023-06-14 11:03:08.000000 pginter-0.2.7/src/pginter/utils/_funcs.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3250 2023-06-14 11:03:08.000000 pginter-0.2.7/src/pginter/utils/_image_funcs.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.092187 pginter-0.2.7/src/pginter/widgets/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      197 2023-05-25 22:58:36.000000 pginter-0.2.7/src/pginter/widgets/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4982 2023-05-25 10:36:44.000000 pginter-0.2.7/src/pginter/widgets/_button.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    14178 2023-05-30 19:45:06.000000 pginter-0.2.7/src/pginter/widgets/_entry.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    25984 2023-06-14 09:10:26.000000 pginter-0.2.7/src/pginter/widgets/_frame.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26315 2023-06-01 18:54:30.000000 pginter-0.2.7/src/pginter/widgets/_geo_manager.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5961 2023-05-30 19:49:43.000000 pginter-0.2.7/src/pginter/widgets/_label.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.2.7/src/pginter/widgets/_supports_children.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1022 2023-05-24 20:39:09.000000 pginter-0.2.7/src/pginter/widgets/_surface_frame.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-14 11:04:03.075520 pginter-0.2.7/src/pginter.egg-info/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-14 11:04:03.000000 pginter-0.2.7/src/pginter.egg-info/PKG-INFO
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1062 2023-06-14 11:04:03.000000 pginter-0.2.7/src/pginter.egg-info/SOURCES.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-06-14 11:04:03.000000 pginter-0.2.7/src/pginter.egg-info/dependency_links.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       33 2023-06-14 11:04:03.000000 pginter-0.2.7/src/pginter.egg-info/requires.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-06-14 11:04:03.000000 pginter-0.2.7/src/pginter.egg-info/top_level.txt
```

### Comparing `pginter-0.2.6/LICENSE` & `pginter-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pginter-0.2.6/setup.py` & `pginter-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pginter",
-    version="0.2.6",
+    version="0.2.7",
     author="Nilusink",
     author_email="nilusink@protonmail.com",
     description="A python GUI interface, based on pygame",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nilusink/PgInter",
     # project_urls={
```

### Comparing `pginter-0.2.6/src/pginter/_pg_root.py` & `pginter-0.2.7/src/pginter/_pg_root.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.6/src/pginter/icon.png` & `pginter-0.2.7/src/pginter/icon.png`

 * *Files identical despite different names*

### Comparing `pginter-0.2.6/src/pginter/theme/_manager.py` & `pginter-0.2.7/src/pginter/theme/_manager.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.6/src/pginter/theme/themes/default.json` & `pginter-0.2.7/src/pginter/theme/themes/default.json`

 * *Files identical despite different names*

### Comparing `pginter-0.2.6/src/pginter/types/_color.py` & `pginter-0.2.7/src/pginter/types/_color.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.6/src/pginter/types/_scheme.py` & `pginter-0.2.7/src/pginter/types/_scheme.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.6/src/pginter/types/_style.py` & `pginter-0.2.7/src/pginter/types/_style.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.6/src/pginter/types/_tk_vars.py` & `pginter-0.2.7/src/pginter/types/_tk_vars.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.6/src/pginter/widgets/_button.py` & `pginter-0.2.7/src/pginter/widgets/_button.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.6/src/pginter/widgets/_entry.py` & `pginter-0.2.7/src/pginter/widgets/_entry.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.6/src/pginter/widgets/_frame.py` & `pginter-0.2.7/src/pginter/widgets/_frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 04. February 2023
 
 Frame - the base widget
 
 Author:
 Nilusink
 """
+from ..utils import add_corners, pil_image_to_surface
 from ._geo_manager import GeometryManager
 from concurrent.futures import Future
 from ..theme import ThemeManager
-from ..utils import merge_alphas
 from ..types import *
 import typing as tp
 import pygame as pg
 
 # try importing pil. The user shouldn't be forced to install pil, but
 # will get an error if they try to use the image widget without having it
 # installed
@@ -30,69 +30,14 @@
 if tp.TYPE_CHECKING:
     from .._pg_root import PgRoot
 
 
 RES_T = tp.TypeVar("RES_T")
 
 
-# utility functions
-def add_corners(
-        im: Image,
-        ulr: int,
-        urr: int,
-        llr: int,
-        lrr: int
-) -> Image:
-    """
-    adds corners to an image
-
-    :param im: input image
-    :param ulr: upper left radius
-    :param urr: upper right radius
-    :param llr: lower left radius
-    :param lrr: lower right radius
-    :returns: the converted image
-    """
-    alpha = Image.new('L', im.size, 255)
-    w, h = im.size
-
-    # upper left corner
-    ulc = Image.new("L", (ulr * 2, ulr * 2), 0)
-    draw = ImageDraw.Draw(ulc)
-    draw.ellipse((0, 0, ulr * 2 - 1, ulr * 2 - 1), fill=255)
-    ulc = ulc.crop((0, 0, ulr, urr))
-    alpha.paste(ulc, (0, 0))
-
-    # upper right corner
-    urc = Image.new("L", (urr * 2, urr * 2), 0)
-    draw = ImageDraw.Draw(urc)
-    draw.ellipse((0, 0, urr * 2 - 1, urr * 2 - 1), fill=255)
-    urc = urc.crop((urr, 0, 2 * urr, urr))
-    alpha.paste(urc, (w - urr, 0))
-
-    # lower left radius
-    llc = Image.new("L", (llr * 2, llr * 2), 0)
-    draw = ImageDraw.Draw(llc)
-    draw.ellipse((0, 0, llr * 2 - 1, llr * 2 - 1), fill=255)
-    llc = llc.crop((0, llr, llr, llr * 2))
-    alpha.paste(llc, (0, h - llr))
-
-    # lower right radius
-    lrc = Image.new("L", (lrr * 2, lrr * 2), 0)
-    draw = ImageDraw.Draw(lrc)
-    draw.ellipse((0, 0, lrr * 2 - 1, lrr * 2 - 1), fill=255)
-    lrc = lrc.crop((lrr, lrr, lrr * 2, lrr * 2))
-    alpha.paste(lrc, (w - lrr, h - lrr))
-
-    # apply the corner radius, keeping the image's alpha (if already present)
-    *_, ia = im.split()  # extract alpha channel from image
-    im.putalpha(merge_alphas(alpha, ia, min))
-    return im
-
-
 def display_configurify(key: str) -> str:
     """
     convert a Frame init key to it's corresponding DisplayConfig key
     """
     replaces = [
         ("bg_color", "bg"),
         ("border_bottom_left_radius", "blr"),
@@ -104,25 +49,14 @@
     for init, config in replaces:
         if key == init:
             return config
 
     return key
 
 
-def pil_image_to_surface(pil_image):
-    """
-    helper function for converting pillow images to pygame images
-    """
-    return pg.image.fromstring(
-        pil_image.tobytes(),
-        pil_image.size,
-        pil_image.mode
-    ).convert_alpha()
-
-
 class _Bind(tp.TypedDict):
     id: int
     event: FrameBind
     function: tp.Callable[[tp.Any], tp.Any | None]
 
 
 class Frame(GeometryManager):
@@ -457,27 +391,14 @@
     ) -> None:
         """
         gets called by another class
         """
         match event:
             case ThemeManager.NotifyEvent.theme_reload:
                 print("theme changed")
-                # the theme has been reloaded
-                # if not self._display_config_configured.bg:
-                #     if isinstance(self.__parent, Frame) and self.__parent._display_config["bg"] == self.theme.frame.bg1:
-                #         self._display_config.bg = self.theme.frame.bg2
-                #
-                #     else:
-                #         self._display_config.bg = self.theme.frame.bg1
-                #
-                # if not self._display_config_configured.border_color:
-                #     self._display_config.border_color = self.theme.frame.border
-                #
-                # if not self._display_config_configured.border_radius:
-                #     self._display_config.border_radius = self.theme.frame.border_radius
 
             case Style.NotifyEvent.property_change:
                 print(f"style changed: {info}, new value: {self.style[info]}")
 
                 if info in ("padding", "margin"):
                     self.layout_params[info] = self.style[info]
```

### Comparing `pginter-0.2.6/src/pginter/widgets/_geo_manager.py` & `pginter-0.2.7/src/pginter/widgets/_geo_manager.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.6/src/pginter/widgets/_label.py` & `pginter-0.2.7/src/pginter/widgets/_label.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.6/src/pginter/widgets/_surface_frame.py` & `pginter-0.2.7/src/pginter/widgets/_surface_frame.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.6/src/pginter.egg-info/SOURCES.txt` & `pginter-0.2.7/src/pginter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 src/pginter/types/_geo_types.py
 src/pginter/types/_notifications.py
 src/pginter/types/_scheme.py
 src/pginter/types/_style.py
 src/pginter/types/_tk_vars.py
 src/pginter/utils/__init__.py
 src/pginter/utils/_funcs.py
+src/pginter/utils/_image_funcs.py
 src/pginter/widgets/__init__.py
 src/pginter/widgets/_button.py
 src/pginter/widgets/_entry.py
 src/pginter/widgets/_frame.py
 src/pginter/widgets/_geo_manager.py
 src/pginter/widgets/_label.py
 src/pginter/widgets/_supports_children.py
```

