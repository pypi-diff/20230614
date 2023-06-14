# Comparing `tmp/mykit-2.0.1.tar.gz` & `tmp/mykit-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-cbqrps87/mykit-2.0.1.tar", last modified: Wed Jun 14 05:33:06 2023, max compression
+gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-87idpf5o/mykit-2.0.2.tar", last modified: Wed Jun 14 07:07:29 2023, max compression
```

## Comparing `mykit-2.0.1.tar` & `mykit-2.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-14 05:32:48.000000 mykit-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-14 05:33:06.000000 mykit-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-14 05:32:48.000000 mykit-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit/app/
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/app/_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/app/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/app/button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit/app/complex/
--rw-r--r--   0 runner    (1001) docker     (123)    20724 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/app/complex/biplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    15893 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/app/complex/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/app/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    27050 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/app/slider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit/kit/
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit/kit/fast_visualizations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit/kit/fast_visualizations/static/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/fast_visualizations/static/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/ffmpeg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit/kit/keycrate/
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/keycrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit/kit/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/neuralnet/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/neuralnet/genetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-14 05:32:48.000000 mykit-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-14 05:33:06.000000 mykit-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-14 05:32:48.000000 mykit-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-14 07:07:05.000000 mykit-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-14 07:07:29.000000 mykit-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-14 07:07:05.000000 mykit-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/app/_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/app/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/app/button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit/app/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)    20724 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/app/complex/biplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16684 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/app/complex/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/app/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27007 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/app/slider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit/kit/fast_visualizations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit/kit/fast_visualizations/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/fast_visualizations/static/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/ffmpeg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit/kit/keycrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/keycrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit/kit/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/neuralnet/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/neuralnet/genetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-14 07:07:05.000000 mykit-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-14 07:07:29.000000 mykit-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-14 07:07:05.000000 mykit-2.0.2/setup.py
```

### Comparing `mykit-2.0.1/LICENSE` & `mykit-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-2.0.1/PKG-INFO` & `mykit-2.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: report bugs, https://github.com/nvfp/mykit/issues
@@ -58,14 +58,17 @@
 ## FAQ
 
 - 
 
 
 ## Changelog
 
+- 2.0.2 (June 14, 2023):
+    - finished updating all type hints
+    - Added visibility functionality to `/app/complex/plot.py`
 - 2.0.1 (June 14, 2023):
     - Updated all type hints to make them work on Python 3.8 and 3.9
     - Added visibility functionality to `/app/complex/biplot.py`
 - 2.0.0 (June 13, 2023):
     - Breaking changes:
         - New mechanism for app: `/app/__init__.py`
         - Moved: `/kit/graph/graph2d.py` -> `/app/complex/plot.py`
```

### Comparing `mykit-2.0.1/README.md` & `mykit-2.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 ## FAQ
 
 - 
 
 
 ## Changelog
 
+- 2.0.2 (June 14, 2023):
+    - finished updating all type hints
+    - Added visibility functionality to `/app/complex/plot.py`
 - 2.0.1 (June 14, 2023):
     - Updated all type hints to make them work on Python 3.8 and 3.9
     - Added visibility functionality to `/app/complex/biplot.py`
 - 2.0.0 (June 13, 2023):
     - Breaking changes:
         - New mechanism for app: `/app/__init__.py`
         - Moved: `/kit/graph/graph2d.py` -> `/app/complex/plot.py`
```

### Comparing `mykit-2.0.1/mykit/__main__.py` & `mykit-2.0.2/mykit/__main__.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.1/mykit/app/__init__.py` & `mykit-2.0.2/mykit/app/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import tkinter as _tk
-import typing as _typing
+from typing import (
+    Callable as _Callable,
+    List as _List
+)
 
 from mykit.app._runtime import Runtime as _Rt
 from mykit.app.button import Button as _Button
 from mykit.app.label import Label as _Label
 from mykit.app.slider import _Slider
 
 
@@ -45,15 +48,15 @@
         self._left_mouse_hold = []
         self._left_mouse_release = []
 
         self._setup = None
         self._teardown = None
         ## </runtime>
 
-    def listen(self, to: str, do: _typing.Callable[[_tk.Event], None]):
+    def listen(self, to: str, do: _Callable[[_tk.Event], None]):
         """
         Add event listener.
 
         ---
 
         ## Params
         - `to`: `Literal["left-mouse-press", "left-mouse-hold", "left-mouse-release"]`
@@ -67,18 +70,18 @@
         elif to == 'left-mouse-hold':
             self._left_mouse_hold.append(do)
         elif to == 'left-mouse-release':
             self._left_mouse_release.append(do)
         else:
             ValueError(f'Invalid event: {repr(to)}.')
 
-    def setup(self, funcs: list[_typing.Callable[[], None]]):
+    def setup(self, funcs: _List[_Callable[[], None]]):
         self._setup = funcs
 
-    def teardown(self, funcs: list[_typing.Callable[[], None]]):
+    def teardown(self, funcs: _List[_Callable[[], None]]):
         self._teardown = funcs
 
     def run(self):
         
         ## <listeners>
 
         def left_mouse_press(e):
```

### Comparing `mykit-2.0.1/mykit/app/button.py` & `mykit-2.0.2/mykit/app/button.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 import random as _random
-import typing as _typing
+from typing import (
+    Callable as _Callable,
+    Dict as _Dict,
+    List as _List,
+    Literal as _Literal,
+    Optional as _Optional,
+    Tuple as _Tuple,
+    Union as _Union
+)
 
 from mykit.app._runtime import Runtime as _Rt
 
 
 class Button(_Rt):
 
-    buttons: dict[str, 'Button'] = {}
-    button_tags: dict[str, list['Button']] = {}
+    buttons: _Dict[str, 'Button'] = {}
+    button_tags: _Dict[str, _List['Button']] = {}
 
     def __init__(
         self,
         x: int = 0,
         y: int = 0,
-        fn: _typing.Callable[[], None] | None = None,
+        fn: _Optional[_Callable[[], None]] = None,
         label: str = '',
-        label_font: str | tuple[str, int] = 'Verdana 8',
-        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
+        label_font: _Union[str, _Tuple[str, int]] = 'Verdana 8',
+        anchor: _Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
         width: int = 100,
         height: int = 18,
         locked: bool = False,
         visible: bool = True,
 
         color_btn_normal: str = '#464646',
         color_btn_hover: str = '#5a5a5a',
         color_btn_press: str = '#6e6e6e',
         color_btn_locked: str = '#282828',
         color_bd_normal: str = '#6e6e6e',
         color_bd_locked: str = '#282828',
         color_lbl_normal: str = '#fafbfa',
         color_lbl_locked: str = '#050505',
 
-        id: str | None = None,
-        tags: str | list[str] | None = None,
+        id: _Optional[str] = None,
+        tags: _Optional[_Union[str, _List[str]]] = None,
     ) -> None:
         """
         ## Params
         - `x` and `y` is the position of the `anchor` (not the center of the button)
         - `color_btn_normal`: button's color
         - `color_bd_normal`: button's border color
         - `color_lbl_normal`: button's label color
@@ -243,46 +251,46 @@
 
     @staticmethod
     def set_visibility_all(visible: bool, /):
         for button in Button.buttons.values():
             button.set_visibility(visible)
 
 
-    def set_label(self, label: str | None, /):
+    def set_label(self, label: _Optional[str], /):
         """
         If `label = None`, the default label (the one assigned
         when the instance was created) will be used.
         """
 
         if label is None:
             label = self.default_label
 
         if self.label != label:
             self.label = label
             self._redraw()
 
     @staticmethod
-    def set_label_by_id(id: str, label: str | None, /):
+    def set_label_by_id(id: str, label: _Optional[str], /):
         Button.buttons[id].set_label(label)
 
 
-    def set_fn(self, fn: _typing.Callable[[], None], /):
+    def set_fn(self, fn: _Callable[[], None], /):
         if self.fn is not fn:
             self.fn = fn
 
     @staticmethod
-    def set_fn_by_id(id: str, fn: _typing.Callable[[], None], /):
+    def set_fn_by_id(id: str, fn: _Callable[[], None], /):
         Button.buttons[id].set_fn(fn)
 
 
     def get_anchor_loc(
         self,
-        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'],
+        anchor: _Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'],
         /
-    ) -> tuple[int, int]:
+    ) -> _Tuple[int, int]:
         """To get the button's center coordinate, use `anchor='center'`"""
 
         W = self.width
         H = self.height
 
         ## get the coordinates for the center (X, Y)
         if self.anchor == 'center':
@@ -334,41 +342,41 @@
             return (X-W/2, Y-H/2)
         else:
             raise ValueError(f'Invalid anchor value: {repr(anchor)}')
 
     @staticmethod
     def get_anchor_loc_by_id(
         id: str,
-        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'],
+        anchor: _Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'],
         /
-    ) -> tuple[int, int]:
+    ) -> _Tuple[int, int]:
         return Button.buttons[id].get_anchor_loc(anchor)
 
 
     def move(
         self,
         x: int,
         y: int,
         /,
-        anchor: _typing.Optional[_typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
+        anchor: _Optional[_Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
     ) -> None:
         """If `anchor = None`, the current anchor will be used."""
         self.x = x
         self.y = y
         if anchor is not None:
             self.anchor = anchor
         self._redraw()
 
     @staticmethod
     def move_by_id(
         id: str,
         x: int,
         y: int,
         /,
-        anchor: _typing.Optional[_typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
+        anchor: _Optional[_Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
     ) -> None:
         Button.buttons[id].move(x, y, anchor)
 
 
     def align(
         self,
         target: 'Button',
```

### Comparing `mykit-2.0.1/mykit/app/complex/biplot.py` & `mykit-2.0.2/mykit/app/complex/biplot.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.1/mykit/app/complex/plot.py` & `mykit-2.0.2/mykit/app/complex/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import random as _random
-import typing as _typing
+from typing import (
+    Dict as _Dict,
+    List as _List,
+    Optional as _Optional,
+    Tuple as _Tuple,
+    Union as _Union
+)
 
 from mykit.app._runtime import Runtime as _Rt
 
 
 class Plot(_Rt):
 
-    plots: dict[str, 'Plot'] = {}
-    plot_tags: dict[str, list['Plot']] = {}
+    plots: _Dict[str, 'Plot'] = {}
+    plot_tags: _Dict[str, _List['Plot']] = {}
 
     def __init__(
         self,
-        points: list[tuple[float, float]],
+        points: _List[_Tuple[float, float]],
         /,
-        xmin: _typing.Optional[float] = None,
-        xmax: _typing.Optional[float] = None,
-        ymin: _typing.Optional[float] = None,
-        ymax: _typing.Optional[float] = None,
+        xmin: _Optional[float] = None,
+        xmax: _Optional[float] = None,
+        ymin: _Optional[float] = None,
+        ymax: _Optional[float] = None,
 
         width: int = 300,
         height: int = 200,
         tl_x: int = 0,
         tl_y: int = 0,
 
         pad_x: float = 0.03,
@@ -35,45 +41,47 @@
 
         grid_color: str = '#555',
         axes_color: str = '#ccc',
         axes_label_color: str = '#ccc',
 
         title: str = '',
         title_color: str = '#fff',
-        title_font: str | tuple = ('Arial Bold', 15),
+        title_font: _Union[str, tuple] = ('Arial Bold', 15),
 
         x_axis_label: str = '',
         x_axis_label_shift: int = 15,
-        x_axis_label_font: str | tuple = ('Arial Bold', 12),
+        x_axis_label_font: _Union[str, tuple] = ('Arial Bold', 12),
         y_axis_label: str = '',
         y_axis_label_shift: int = 15,
-        y_axis_label_font: str | tuple = ('Arial Bold', 12),
+        y_axis_label_font: _Union[str, tuple] = ('Arial Bold', 12),
 
         tick_x_prefix: str = '',
         tick_x_suffix: str = '',
         tick_x_shift: int = 0,
-        tick_x_font: str | tuple = 'Consolas 9',
+        tick_x_font: _Union[str, tuple] = 'Consolas 9',
         tick_x_prec: int = 1,
         tick_y_prefix: str = '',
         tick_y_suffix: str = '',
         tick_y_shift: int = 0,
-        tick_y_font: str | tuple = 'Consolas 9',
+        tick_y_font: _Union[str, tuple] = 'Consolas 9',
         tick_y_prec: int = 1,
         tick_color: str = '#ccc',
 
         plot_color: str = '#7f7',
         plot_thick: int = 1,  # line width
 
         show_points: bool = False,
         points_rad: int = 7,
         points_color: str = '#a77',
         points_border: str = '#eee',
 
-        id: str | None = None,
-        tags: str | list[str] | None = None,
+        visible: bool = True,
+
+        id: _Optional[str] = None,
+        tags: _Optional[_Union[str, _List[str]]] = None,
     ):
         """
         To display this graph, there should be a minimum of 2 pairs of points in `points`.
 
         ---
 
         ## Params
@@ -137,14 +145,16 @@
         self.plot_thick = plot_thick
 
         self.show_points = show_points
         self.points_rad = points_rad
         self.points_color = points_color
         self.points_border = points_border
 
+        self.visibile = visible
+
         ## `self.id`: to make sure that we can modify a specific instance without affecting the others
         if id is None:
             self.id = _random.randint(-10000, 10000)
             while self.id in Plot.plots:
                 self.id = _random.randint(-10000, 10000)
         else:
             self.id = id
@@ -340,15 +350,15 @@
             for x, y in coords:
                 Plot.page.create_oval(
                     x-self.points_rad/2, y-self.points_rad/2,
                     x+self.points_rad/2, y+self.points_rad/2,
                     fill=self.points_color, outline=self.points_border, width=1, tags=f'Plot_{self.id}'
                 )
     
-    def redraw_plot(self, points: list[tuple[float, float]], /) -> None:
+    def redraw_plot(self, points: _List[_Tuple[float, float]], /) -> None:
         """
         Redraws the plot and updates the tick labels with a new set of given `points`.
         """
 
         self.points = points
 
         ## The code below is duplicated from `_redraw`. While it may seem redundant,
@@ -431,27 +441,27 @@
             coords.append((X, Y))
         Plot.page.create_line(
             coords,
             fill=self.plot_color, width=self.plot_thick,
             tags=(f'Plot_{self.id}', f'Plot_{self.id}_plot')
         )
 
-    def shift_plot(self, new_points: list[tuple[float, float]], /) -> None:
+    def shift_plot(self, new_points: _List[_Tuple[float, float]], /) -> None:
         """
         Shifts the plot by inserting `new_points` and removing the leftmost points.
         For example, if 2 pairs are inserted, 2 leftmost pairs will be removed.
         Make sure that the new x values are always greater than the rightmost x value.
         For instance, if the current rightmost x is 100, the new x values
         should follow a sequence like 100, 101, 102.
         """
         n_new = len(new_points)
         points = self.points[n_new:] + new_points
         self.redraw_plot(points)
 
-    def add_point(self, point: tuple[float, float], max: int | None = None):
+    def add_point(self, point: _Tuple[float, float], max: _Optional[int] = None):
         """
         Adding the new point to the current plot.
         If a max value is specified (e.g., max=100), and the total number of points
         exceeds 100, the plot will shift by inserting the new point and removing
         the leftmost point. If max is not specified, the point will simply be added.
         """
 
@@ -461,8 +471,28 @@
             points.append(point)
             self.redraw_plot(points)
         else:
             if len(points) < max:
                 points.append(point)
                 self.redraw_plot(points)
             else:
-                self.shift_plot([point])
+                self.shift_plot([point])
+
+    
+    def set_visibility(self, visible: bool, /):
+        if self.visible is not visible:
+            self.visible = visible
+            self._redraw()
+
+    @staticmethod
+    def set_visibility_by_id(id: str, visible: bool, /):
+        Plot.plots[id].set_visibility(visible)
+
+    @staticmethod
+    def set_visibility_by_tag(tag: str, visible: bool, /):
+        for plot in Plot.plot_tags[tag]:
+            plot.set_visibility(visible)
+
+    @staticmethod
+    def set_visibility_all(visible: bool, /):
+        for plot in Plot.plots.values():
+            plot.set_visibility(visible)
```

### Comparing `mykit-2.0.1/mykit/app/label.py` & `mykit-2.0.2/mykit/app/label.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 import random as _random
 import tkinter as _tk
-import typing as _typing
+from typing import (
+    Callable as _Callable,
+    Dict as _Dict,
+    List as _List,
+    Literal as _Literal,
+    Optional as _Optional,
+    Tuple as _Tuple,
+    Union as _Union
+)
 
 
 class Label:
 
-    labels: dict[str, 'Label'] = {}
-    label_tags: dict[str, list['Label']] = {}
+    labels: _Dict[str, 'Label'] = {}
+    label_tags: _Dict[str, _List['Label']] = {}
 
     def __init__(
         self,
         x: int = 0,
         y: int = 0,
         text: str = '',
-        font: str | tuple[str, int] = 'Verdana 10',
+        font: _Union[str, _Tuple[str, int]] = 'Verdana 10',
         justify: str = 'left',
-        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
+        anchor: _Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
         fg: str = '#ccc',
         bg: str = '#111',
         bd: str = '#555',
         bd_width: int = 0,
         wraplength: int = 1000,
         padx: int = 0,
         pady: int = 0,
         visible: bool = True,
 
-        id: str | None = None,
-        tags: str | list[str] | None = None,
+        id: _Optional[str] = None,
+        tags: _Optional[_Union[str, _List[str]]] = None,
     ):
         """
         `x`: the x-position for the `anchor` argument, not the center of the label
         `y`: the y-position for the `anchor` argument, not the center of the label
         """
 
         self.x = x  # reminder: this is the x-position for the `anchor` argument, not the center of the label
@@ -76,36 +84,36 @@
                 if tag in Label.label_tags:
                     Label.label_tags[tag].append(self)
                 else:
                     Label.label_tags[tag] = [self]
         ## <tags>
 
 
-    def set_text(self, text: str | None, /):
+    def set_text(self, text: _Optional[str], /):
         """if None -> set default text."""
 
         if text is None:
             text = self.default_text
 
         if text != self.text:
             self.text = text
             self.label.configure(text=text)
 
     @staticmethod
-    def set_text_by_id(id: str, text: str | None, /):
+    def set_text_by_id(id: str, text: _Optional[str], /):
         Label.labels[id].set_text(text)
 
 
-    def set_font(self, font: str | tuple[str, int], /):
+    def set_font(self, font: _Union[str, _Tuple[str, int]], /):
         if font != self.font:
             self.font = font
             self.label.configure(font=font)
 
     @staticmethod
-    def set_font_by_id(id: str, font: str | tuple[str, int], /):
+    def set_font_by_id(id: str, font: _Union[str, _Tuple[str, int]], /):
         Label.labels[id].set_font(font)
 
 
     def set_fg(self, fg: str, /):
         if fg != self.fg:
             self.fg = fg
             self.label.configure(fg=fg)
@@ -149,15 +157,15 @@
         return self.label.winfo_reqheight()
 
     @staticmethod
     def get_height_by_id(id: str, /) -> int:
         return Label.labels[id].get_height()
 
 
-    def get_anchor_loc(self, anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'], /) -> tuple[int, int]:
+    def get_anchor_loc(self, anchor: _Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'], /) -> _Tuple[int, int]:
         """To get the center of the label coordinates, use `anchor='center'`"""
 
         W = self.get_width()
         H = self.get_height()
 
         ## get the coordinates for the center (X, Y)
         if self.anchor == 'center':
@@ -207,34 +215,40 @@
             return (X-W/2, Y)
         elif anchor == 'nw':
             return (X-W/2, Y-H/2)
         else:
             raise ValueError(f'Invalid anchor value: {repr(anchor)}')
 
     @staticmethod
-    def get_anchor_loc_by_id(id: str, anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'], /) -> tuple[int, int]:
+    def get_anchor_loc_by_id(id: str, anchor: _Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'], /) -> _Tuple[int, int]:
         return Label.labels[id].get_anchor_loc(anchor)
 
     
-    def move(self, x: int, y: int, /, anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] | None = None) -> None:
+    def move(
+            self,
+            x: int,
+            y: int,
+            /,
+            anchor: _Optional[_Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
+    ) -> None:
         """If `anchor = None`, the current anchor will be used."""
         self.x = x
         self.y = y
         if anchor is not None:
             self.anchor = anchor
         # self.label.place(x=x, y=y, anchor=anchor)  # reminder: don't do this because `anchor` could be `None`
         self.label.place(x=x, y=y, anchor=self.anchor)
 
     @staticmethod
     def move_by_id(
         id: str,
         x: int,
         y: int,
         /,
-        anchor: _typing.Optional[_typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
+        anchor: _Optional[_Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
     ) -> None:
         Label.labels[id].move(x, y, anchor)
 
 
     def align(
         self,
         target: 'Label',
```

### Comparing `mykit-2.0.1/mykit/app/slider.py` & `mykit-2.0.2/mykit/app/slider.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 import random as _random
-import tkinter as _tk
-import typing as _typing
+from typing import (
+    Callable as _Callable,
+    Dict as _Dict,
+    List as _List,
+    Literal as _Literal,
+    Optional as _Optional,
+    Tuple as _Tuple,
+    Union as _Union
+)
 
 from mykit.app._runtime import Runtime as _Rt
 from mykit.kit.utils import minmax_normalization as _norm
 
 
 class _Slider(_Rt):
 
-    sliders: dict[str, '_Slider'] = {}
-    slider_tags: dict[str, list['_Slider']] = {}  # note that the horizontal and vertical sliders store the tags together
+    sliders: _Dict[str, '_Slider'] = {}
+    slider_tags: _Dict[str, _List['_Slider']] = {}  # note that the horizontal and vertical sliders store the tags together
 
     def __init__(
         self,
         min: float = 0,
         max: float = 1,
-        step: _typing.Optional[float] = None,
-        init: _typing.Optional[float] = None,
-        fn: _typing.Optional[_typing.Callable[[], None]] = None,
+        step: _Optional[float] = None,
+        init: _Optional[float] = None,
+        fn: _Optional[_Callable[[], None]] = None,
 
         x: int = 0,
         y: int = 0,
-        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
+        anchor: _Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
         tolerance: float = 0.25,
         
-        label: _typing.Optional[str] = None,
+        label: _Optional[str] = None,
         label_fg: str = '#ccc',
-        label_font: str | tuple[str, int] = 'Verdana 9',
+        label_font: _Union[str, _Tuple[str, int]] = 'Verdana 9',
         show_label_box: bool = False,
-        label_box_color: _typing.Optional[str] = None,
-        label_box_width: _typing.Optional[int] = None,
-        label_box_height: _typing.Optional[int] = None,
+        label_box_color: _Optional[str] = None,
+        label_box_width: _Optional[int] = None,
+        label_box_height: _Optional[int] = None,
         label_y_shift: int = -15,
 
         show_value: bool = True,
         value_fg: str = '#ccc',
-        value_font: str | tuple[str, int] = 'Consolas 9',
+        value_font: _Union[str, _Tuple[str, int]] = 'Consolas 9',
         value_prefix: str = '',
         value_suffix: str = '',
         show_value_box: bool = False,
-        value_box_color: _typing.Optional[str] = None,
-        value_box_width: _typing.Optional[int] = None,
-        value_box_height: _typing.Optional[int] = None,
+        value_box_color: _Optional[str] = None,
+        value_box_width: _Optional[int] = None,
+        value_box_height: _Optional[int] = None,
 
         rod_len: int = 200,
         rod_thick: int = 3,
         btn_r: int = 5,
         color_rod_normal: str = '#4b4b4b',
         color_rod_locked: str = '#2d2d2d',
         color_btn_normal: str = '#555555',
@@ -54,16 +61,16 @@
         color_btn_hover: str = '#696969',
         color_btn_bd_normal: str = '#f5f5f5',
         color_btn_bd_locked: str = '#373737',
 
         locked: bool = False,
         visible: bool = True,
 
-        id: str | None = None,
-        tags: str | list[str] | None = None,
+        id: _Optional[str] = None,
+        tags: _Optional[_Union[str, _List[str]]] = None,
     ) -> None:
         """
         ## Params
         - `x` and `y` is the position of the `anchor` (not the center of the button)
         - `tolerance`: to determine how closely the cursor needs to be to the slider's step values for it to move to a new value
 
         ## Docs
@@ -215,15 +222,15 @@
     
     @staticmethod
     def set_visibility_all(visible: bool, /) -> None:
         for slider in _Slider.sliders.values():
             slider.set_visibility(visible)
 
 
-    def set_value(self, value: int | None, /) -> None:
+    def set_value(self, value: _Optional[int], /) -> None:
         """if `None` -> default value."""
 
         if value is None:
             value = self.init
 
         if value < self.min:
             value = self.min
@@ -231,39 +238,39 @@
             value = self.max
 
         if value != self.value:
             self.value = value
             self._redraw()
     
     @staticmethod
-    def set_value_by_id(id: str, value: int | None, /) -> None:
+    def set_value_by_id(id: str, value: _Optional[int], /) -> None:
         _Slider.sliders[id].set_value(value)
 
     @staticmethod
-    def set_value_by_tag(tag: str, value: int | None, /) -> None:
+    def set_value_by_tag(tag: str, value: _Optional[int], /) -> None:
         for slider in _Slider.slider_tags[tag]:
             slider.set_value(value)
 
     @staticmethod
-    def set_value_all(value: int | None, /) -> None:
+    def set_value_all(value: _Optional[int], /) -> None:
         """To reset the value of all sliders, use `value = None`."""
         for slider in _Slider.sliders.values():
             slider.set_value(value)
 
 
     @staticmethod
     def get_value_by_id(id: str, /) -> None:
         return _Slider.sliders[id].value
     
 
     def get_anchor_loc(
         self,
-        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'],
+        anchor: _Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'],
         /
-    ) -> tuple[int, int]:
+    ) -> _Tuple[int, int]:
         """To get the slider-rod's center coordinate, use `anchor='center'`"""
 
         W = self.width
         H = self.height
 
         ## get the coordinates for the center (X, Y)
         if self.anchor == 'center':
@@ -315,41 +322,41 @@
             return (X-W/2, Y-H/2)
         else:
             raise ValueError(f'Invalid anchor value: {repr(anchor)}')
 
     @staticmethod
     def get_anchor_loc_by_id(
         id: str,
-        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'],
+        anchor: _Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'],
         /
-    ) -> tuple[int, int]:
+    ) -> _Tuple[int, int]:
         return _Slider.sliders[id].get_anchor_loc(anchor)
 
 
     def move(
         self,
         x: int,
         y: int,
         /,
-        anchor: _typing.Optional[_typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
+        anchor: _Optional[_Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
     ) -> None:
         """If `anchor = None`, the current anchor will be used."""
         self.x = x
         self.y = y
         if anchor is not None:
             self.anchor = anchor
         self._redraw()
 
     @staticmethod
     def move_by_id(
         id: str,
         x: int,
         y: int,
         /,
-        anchor: _typing.Optional[_typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
+        anchor: _Optional[_Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
     ) -> None:
         _Slider.sliders[id].move(x, y, anchor)
 
 
     def align(
         self,
         target: '_Slider',
@@ -405,41 +412,41 @@
 
 class Slider(_Slider):
 
     def __init__(
         self,
         min: float = 0,
         max: float = 1,
-        step: _typing.Optional[float] = None,
-        init: _typing.Optional[float] = None,
-        fn: _typing.Optional[_typing.Callable[[], None]] = None,
+        step: _Optional[float] = None,
+        init: _Optional[float] = None,
+        fn: _Optional[_Callable[[], None]] = None,
 
         x: int = 0,
         y: int = 0,
-        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
+        anchor: _Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
         tolerance: float = 0.25,
         
-        label: _typing.Optional[str] = None,
+        label: _Optional[str] = None,
         label_fg: str = '#ccc',
-        label_font: str | tuple[str, int] = 'Verdana 9',
+        label_font: _Union[str, _Tuple[str, int]] = 'Verdana 9',
         show_label_box: bool = False,
-        label_box_color: _typing.Optional[str] = None,
-        label_box_width: _typing.Optional[int] = None,
-        label_box_height: _typing.Optional[int] = None,
+        label_box_color: _Optional[str] = None,
+        label_box_width: _Optional[int] = None,
+        label_box_height: _Optional[int] = None,
         label_y_shift: int = -15,
 
         show_value: bool = True,
         value_fg: str = '#ccc',
-        value_font: str | tuple[str, int] = 'Consolas 9',
+        value_font: _Union[str, _Tuple[str, int]] = 'Consolas 9',
         value_prefix: str = '',
         value_suffix: str = '',
         show_value_box: bool = False,
-        value_box_color: _typing.Optional[str] = None,
-        value_box_width: _typing.Optional[int] = None,
-        value_box_height: _typing.Optional[int] = None,
+        value_box_color: _Optional[str] = None,
+        value_box_width: _Optional[int] = None,
+        value_box_height: _Optional[int] = None,
         value_box_x_shift: int = 25,  # extra arg. reminder: this parameter has a different argument name for horizontal and vertical sliders
 
         rod_len: int = 200,
         rod_thick: int = 3,
         btn_r: int = 5,
         color_rod_normal: str = '#4b4b4b',
         color_rod_locked: str = '#2d2d2d',
@@ -449,16 +456,16 @@
         color_btn_hover: str = '#696969',
         color_btn_bd_normal: str = '#f5f5f5',
         color_btn_bd_locked: str = '#373737',
 
         locked: bool = False,
         visible: bool = True,
 
-        id: str | None = None,
-        tags: str | list[str] | None = None,
+        id: _Optional[str] = None,
+        tags: _Optional[_Union[str, _List[str]]] = None,
     ) -> None:
 
         super().__init__(
             min, max, step, init, fn,
             x, y, anchor, tolerance,
             label, label_fg, label_font, show_label_box, label_box_color, label_box_width, label_box_height, label_y_shift,
             show_value, value_fg, value_font, value_prefix, value_suffix, show_value_box, value_box_color, value_box_width, value_box_height,
@@ -613,41 +620,41 @@
 
 class VSlider(_Slider):
 
     def __init__(
         self,
         min: float = 0,
         max: float = 1,
-        step: _typing.Optional[float] = None,
-        init: _typing.Optional[float] = None,
-        fn: _typing.Optional[_typing.Callable[[], None]] = None,
+        step: _Optional[float] = None,
+        init: _Optional[float] = None,
+        fn: _Optional[_Callable[[], None]] = None,
 
         x: int = 0,
         y: int = 0,
-        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
+        anchor: _Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
         tolerance: float = 0.25,
         
-        label: _typing.Optional[str] = None,
+        label: _Optional[str] = None,
         label_fg: str = '#ccc',
-        label_font: str | tuple[str, int] = 'Verdana 9',
+        label_font: _Union[str, _Tuple[str, int]] = 'Verdana 9',
         show_label_box: bool = False,
-        label_box_color: _typing.Optional[str] = None,
-        label_box_width: _typing.Optional[int] = None,
-        label_box_height: _typing.Optional[int] = None,
+        label_box_color: _Optional[str] = None,
+        label_box_width: _Optional[int] = None,
+        label_box_height: _Optional[int] = None,
         label_y_shift: int = -15,
 
         show_value: bool = True,
         value_fg: str = '#ccc',
-        value_font: str | tuple[str, int] = 'Consolas 9',
+        value_font: _Union[str, _Tuple[str, int]] = 'Consolas 9',
         value_prefix: str = '',
         value_suffix: str = '',
         show_value_box: bool = False,
-        value_box_color: _typing.Optional[str] = None,
-        value_box_width: _typing.Optional[int] = None,
-        value_box_height: _typing.Optional[int] = None,
+        value_box_color: _Optional[str] = None,
+        value_box_width: _Optional[int] = None,
+        value_box_height: _Optional[int] = None,
         value_box_y_shift: int = 15,  # extra arg. reminder: this parameter has a different argument name for horizontal and vertical sliders
 
         rod_len: int = 200,
         rod_thick: int = 3,
         btn_r: int = 5,
         color_rod_normal: str = '#4b4b4b',
         color_rod_locked: str = '#2d2d2d',
@@ -657,16 +664,16 @@
         color_btn_hover: str = '#696969',
         color_btn_bd_normal: str = '#f5f5f5',
         color_btn_bd_locked: str = '#373737',
 
         locked: bool = False,
         visible: bool = True,
 
-        id: str | None = None,
-        tags: str | list[str] | None = None,
+        id: _Optional[str] = None,
+        tags: _Optional[_Union[str, _List[str]]] = None,
     ) -> None:
 
         super().__init__(
             min, max, step, init, fn,
             x, y, anchor, tolerance,
             label, label_fg, label_font, show_label_box, label_box_color, label_box_width, label_box_height, label_y_shift,
             show_value, value_fg, value_font, value_prefix, value_suffix, show_value_box, value_box_color, value_box_width, value_box_height,
```

### Comparing `mykit-2.0.1/mykit/kit/color.py` & `mykit-2.0.2/mykit/kit/color.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.1/mykit/kit/fast_visualizations/static/plot.py` & `mykit-2.0.2/mykit/kit/fast_visualizations/static/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.1/mykit/kit/ffmpeg.py` & `mykit-2.0.2/mykit/kit/ffmpeg.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import re as _re
 import subprocess as _sp
+from typing import (
+    List as _List,
+    Tuple as _Tuple,
+    Union as _Union
+)
 
 
-def get_resolution(input_path: str, ffprobe_path: str) -> tuple[int, int]:
+def get_resolution(input_path: str, ffprobe_path: str) -> _Tuple[int, int]:
     """
     image/video resolution.
 
     `input_path`: absolute path to the input file
     `ffprobe_path`: absolute path to ffprobe executable
 
     return: `(width, height)`
@@ -77,15 +82,15 @@
         ],
         stderr=_sp.STDOUT, text=True
     )
     res = _re.match(r'^(?P<dur>\d+(?:\.\d+)?)', stdout)
     return float(res.group('dur'))
 
 
-def get_vid_fps(file: str, ffprobe: str, /, *, do_round: bool = False) -> int | float:
+def get_vid_fps(file: str, ffprobe: str, /, *, do_round: bool = False) -> _Union[int, float]:
     """
     Video fps (average frame rate).
 
     `file`: full path to the input file
     `ffprobe`: ffprobe.exe full path
     `do_round`: round the fps to the nearest integer
     """
@@ -103,15 +108,15 @@
     fps = eval(res.group('fps'), {})
     if do_round:
         return round(fps)
     else:
         return fps
 
 
-def gen_dyn_vol(__timestamp: list[tuple[float, float]], /, precision: float = 0.0001, vol_round: int = 2) -> str:
+def gen_dyn_vol(__timestamp: _List[_Tuple[float, float]], /, precision: float = 0.0001, vol_round: int = 2) -> str:
     """
     Generate a dynamic volume (with linear interpolation) filter.
 
     ---
 
     ## params
     - `precision`: Lower values indicate better quality with fewer artifacts.
```

### Comparing `mykit-2.0.1/mykit/kit/keycrate/__init__.py` & `mykit-2.0.2/mykit/kit/keycrate/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 import re as _re
-import typing as _typing
+from typing import (
+    Any as _Any,
+    List as _List,
+    NoReturn as _NoReturn,
+    Optional as _Optional
+)
 
 from mykit.kit.path import open_file as _open_file
 from mykit.kit.utils import is_valid_var_name as _is_valid_var_name
 
 
 class KeyCrate:
     """
@@ -13,16 +18,16 @@
 
     def __init__(
         self,
         file_pth: str,
         /,
         key_is_var: bool = False,
         eval_value: bool = False,
-        only_keys: _typing.Optional[list[str]] = None,
-        need_keys: _typing.Optional[list[str]] = None
+        only_keys: _Optional[_List[str]] = None,
+        need_keys: _Optional[_List[str]] = None
     ) -> None:
         """
         Storing key-value pairs (key: value) in the .txt file `file_pth`.
         Access the value using either the class-like way (`kc.key`)
         or the dictionary-like way (`kc['key']`).
 
         ---
@@ -55,19 +60,19 @@
         self._kc__eval_value = eval_value
         self._kc__only_keys = only_keys
         self._kc__need_keys = need_keys
 
         ## init
         self.parse()
 
-    def __getattr__(self, __name: str, __default: _typing.Any = None, /) -> _typing.NoReturn:
+    def __getattr__(self, __name: str, __default: _Any = None, /) -> _NoReturn:
         """This method is called when attribute `__name` is not found"""
         raise AttributeError(f'KeyCrate file {repr(self._kc__file_pth)} does not have key {repr(__name)}.')
 
-    def __getitem__(self, __key: str, /) -> _typing.Any:
+    def __getitem__(self, __key: str, /) -> _Any:
         """
         To access the keys in a dictionary-like way (e.g., `kc['key1']`),
         it is commonly used for keys that are not variable names (e.g., `kc['full name']`).
         """
         return getattr(self, __key)
 
     def _read(self) -> str:
```

### Comparing `mykit-2.0.1/mykit/kit/math.py` & `mykit-2.0.2/mykit/kit/math.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.1/mykit/kit/neuralnet/dense.py` & `mykit-2.0.2/mykit/kit/neuralnet/dense.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import numpy as _np
 import random as _random
-import typing as _typing
+from typing import (
+    Callable as _Callable,
+    List as _List,
+    Optional as _Optional,
+    Tuple as _Tuple
+)
 
 from mykit.kit.math import relu as _ReLU
 
 
 class DenseNN:
     """Also known as fully connected neural networks"""
 
     def __init__(
         self,
-        sizes: list[int],
-        hidden_act_fn: _typing.Callable[[_np.ndarray, bool], _np.ndarray] = _ReLU,
-        output_act_fn: _typing.Callable[[_np.ndarray, bool], _np.ndarray] = _ReLU,
-        load_weights_and_biases: tuple[list[_np.ndarray], list[_np.ndarray]] | None = None,
+        sizes: _List[int],
+        hidden_act_fn: _Callable[[_np.ndarray, bool], _np.ndarray] = _ReLU,
+        output_act_fn: _Callable[[_np.ndarray, bool], _np.ndarray] = _ReLU,
+        load_weights_and_biases: _Optional[_Tuple[_List[_np.ndarray], _List[_np.ndarray]]] = None,
     ) -> None:
         """
         The network uses normalized Xavier weight initialization and cross-entropy loss function.
 
         ---
 
         `load_weights_and_biases`: Pre-loaded weights and biases decoded by `decode` method. `None` for a new network.
@@ -94,15 +99,15 @@
         ## Params
         `inputs`: Input array with shape `(n, 1)`.
             Example: `np.array([[i1], [i2], [i3], ...])`
         `outputs`: Desired output array with shape `(m, 1)`.
             Example: `np.array([[o1], [o2], [o3], ...])`
 
         ## Returns
-        `tuple[dgw, dgb]`: Gradients of weights and biases as lists.
+        `Tuple[dgw, dgb]`: Gradients of weights and biases as lists.
         """
 
         self.feedforward(inputs)
 
         ## gradient delta
         dgw = [_np.zeros(w.shape) for w in self.weights]
         dgb = [_np.zeros(b.shape) for b in self.biases]
@@ -116,15 +121,15 @@
         for l in range(2, self.n_layer):
             delta = _np.dot(self.weights[-l + 1].transpose(), delta)*self.hidden_act_fn(self.z_values[-l], derivative=True)
             dgw[-l] = _np.dot(delta, self.a_values[-l - 1].transpose())
             dgb[-l] = delta
 
         return (dgw, dgb)
 
-    def _tuning(self, samples: list[tuple[_np.ndarray, _np.ndarray]], k1: float, k2: float) -> None:
+    def _tuning(self, samples: _List[_Tuple[_np.ndarray, _np.ndarray]], k1: float, k2: float) -> None:
         """
         Update weights and biases.
 
         ---
         
         ## Params
             - `samples`: A list of input-output pairs used for updating the model
@@ -152,15 +157,15 @@
         self.biases = [
             b - k2*_gb
             for b, _gb in zip(self.biases, gb)
         ]
 
     def train(
         self,
-        training_data: list[tuple[_np.ndarray, _np.ndarray]],
+        training_data: _List[_Tuple[_np.ndarray, _np.ndarray]],
         sample_size: int,
         n_epoch: int,
         learning_rate: float = 0.005,
         regularization: float = 0.001
     ) -> None:
         """
         Trains the model using gradient descent with regularization.
@@ -199,12 +204,12 @@
         encoded_data = {
             'weights': [w.tolist() for w in self.weights],
             'biases': [b.tolist() for b in self.biases]
         }
         return encoded_data
 
     @staticmethod
-    def decode(encoded_data: dict) -> tuple[list[_np.ndarray], list[_np.ndarray]]:
+    def decode(encoded_data: dict) -> _Tuple[_List[_np.ndarray], _List[_np.ndarray]]:
         """Decode the weights and biases from what is encoded by the `encode` method."""
         weights = [_np.array(w) for w in encoded_data['weights']]
         biases = [_np.array(b) for b in encoded_data['biases']]
         return weights, biases
```

### Comparing `mykit-2.0.1/mykit/kit/neuralnet/genetic.py` & `mykit-2.0.2/mykit/kit/neuralnet/genetic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 import random as _random
 import numpy as _np
-import typing as _typing
+from typing import (
+    Callable as _Callable,
+    Dict as _Dict,
+    List as _List,
+    Optional as _Optional,
+    Tuple as _Tuple
+)
 
 from mykit.kit.neuralnet.dense import DenseNN as _DenseNN
 
 
 class GeneticNN:
 
     def __init__(
         self,
-        layer_sizes: list[int],
-        hidden_act: _typing.Callable[[_np.ndarray, bool], _np.ndarray],
-        output_act: _typing.Callable[[_np.ndarray, bool], _np.ndarray],
+        layer_sizes: _List[int],
+        hidden_act: _Callable[[_np.ndarray, bool], _np.ndarray],
+        output_act: _Callable[[_np.ndarray, bool], _np.ndarray],
 
         population_size: int,
         crossover_threshold: float = 0.001,
         mutation1_rate: float = 0.85,
         mutation2_rate: float = 0.99,
-        mutation2_range: tuple[float, float] = (0.1, 2.5),
+        mutation2_range: _Tuple[float, float] = (0.1, 2.5),
         n_new: int = 0,
         init_score: float = 0,
         
-        load_wnb: tuple[list[_np.ndarray], list[_np.ndarray]] | None = None,
+        load_wnb: _Optional[_Tuple[_List[_np.ndarray], _List[_np.ndarray]]] = None,
     ) -> None:
         """
         Genetic neural network using dense neural network.
 
         ---
 
         ## Params
@@ -56,15 +62,15 @@
         self.crossover_threshold = crossover_threshold
         self.mutation1_rate = mutation1_rate
         self.mutation2_rate = mutation2_rate
         self.mutation2_range = mutation2_range
         self.n_new = n_new
         self.init_score = init_score
 
-        self.population: dict[_DenseNN, float] = {}
+        self.population: _Dict[_DenseNN, float] = {}
         for _ in range(population_size):
 
             if load_wnb is None:
                 wnb = None
             else:
                 w = [w.copy() for w in load_wnb[0]]
                 b = [b.copy() for b in load_wnb[1]]
@@ -72,16 +78,16 @@
 
             nn = _DenseNN(layer_sizes, hidden_act, output_act, wnb)
             self.population[nn] = init_score
 
 
         ## runtime
 
-        self.the_parent: tuple[_DenseNN, _DenseNN] = None  # to store the parent that produced the current generation (after executing `keep_elites()`)
-        self.prev: dict[_DenseNN, float] = {}  # to store the previous generation
+        self.the_parent: _Tuple[_DenseNN, _DenseNN] = None  # to store the parent that produced the current generation (after executing `keep_elites()`)
+        self.prev: _Dict[_DenseNN, float] = {}  # to store the previous generation
 
 
     def set_score(self, individual: _DenseNN, score: float, /) -> None:
         self.population[individual] = score
 
     def get_score(self, individual: _DenseNN, /) -> float:
         return self.population[individual]
```

### Comparing `mykit-2.0.1/mykit/kit/noise.py` & `mykit-2.0.2/mykit/kit/noise.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import math as _math
 import random as _random
 import time as _time
+from typing import (
+    List as _List,
+    Tuple as _Tuple
+)
 
 
 def _non_periodic_fn(__x: float, /, a: float = 1, b: float = 1, c: float = 1, d: float = 1, e: float = 1, f: float = 1, g: float = 1):
     """
     proven non-periodic.
     ref: https://stackoverflow.com/questions/8798771/perlin-noise-for-1d
 
@@ -15,16 +19,16 @@
     return a*(b*_math.sin(c*__x) + d*_math.sin(e*_math.pi*__x) + f*_math.sin(g*_math.e*__x))
 
 def random_sine_noise(
     seed: float,
     nsample: int,
     ymin: int,
     ymax: int,
-    params: tuple = (1, 1, 1, 1, 1, 1, 1)
-) -> list[tuple[float, float]]:
+    params: _Tuple = (1, 1, 1, 1, 1, 1, 1)
+) -> _List[_Tuple[float, float]]:
 
     _random.seed(seed)
     shift = _random.randint(-1000000000, 1000000000)
 
     points = []
     for x in range(nsample):
         x += shift
```

### Comparing `mykit-2.0.1/mykit/kit/path.py` & `mykit-2.0.2/mykit/kit/path.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import json as _json
 import os as _os
 import subprocess as _sp
 import sys as _sys
-import typing as _typing
+from typing import (
+    Any as _Any
+)
 
 
 class SafeJSON:
     """Secure JSON read/write operations, ensuring data integrity during writing and rewriting."""
 
     @staticmethod
-    def write(__pth: str, __obj: _typing.Any, /, do_log: bool = True) -> None:
+    def write(__pth: str, __obj: _Any, /, do_log: bool = True) -> None:
 
         ## normalize the path and perform some validations
         pth_norm = _os.path.normpath(__pth)
         if not pth_norm.lower().endswith('.json'):
             raise AssertionError(f'Not a JSON file: {repr(__pth)}.')
         if not _os.path.isdir(_os.path.dirname(pth_norm)):
             raise NotADirectoryError(f'The directory does not exist: {repr(__pth)}.')
@@ -23,29 +25,29 @@
         with open(pth_norm, 'w') as fp:
             _json.dump(__obj, fp)
         
         if do_log:
             print(f'INFO: Json written: {repr(__pth)}.')
 
     @staticmethod
-    def read(__pth: str, /) -> _typing.Any:
+    def read(__pth: str, /) -> _Any:
 
         ## normalize the path and perform some validations
         pth_norm = _os.path.normpath(__pth)
         if not pth_norm.lower().endswith('.json'):
             raise AssertionError(f'Not a JSON file: {repr(__pth)}.')
         if not _os.path.isfile(pth_norm):
             raise FileNotFoundError(f'Not a file: {repr(__pth)}.')
 
         with open(pth_norm, 'r') as fp:
             out = _json.load(fp)
         return out
 
     @staticmethod
-    def rewrite(__pth: str, __obj: _typing.Any, /, do_log: bool = True) -> None:
+    def rewrite(__pth: str, __obj: _Any, /, do_log: bool = True) -> None:
 
         ## normalize the path and perform some validations
         pth_norm = _os.path.normpath(__pth)
         if not pth_norm.lower().endswith('.json'):
             raise AssertionError(f'Not a JSON file: {repr(__pth)}.')
         if not _os.path.isfile(pth_norm):
             raise FileNotFoundError(f'Not a file: {repr(__pth)}.')
```

### Comparing `mykit-2.0.1/mykit/kit/time.py` & `mykit-2.0.2/mykit/kit/time.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.1/mykit/kit/utils.py` & `mykit-2.0.2/mykit/kit/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import datetime as _datetime
 import keyword as _keyword
 import random as _random
+from typing import (
+    Tuple as _Tuple
+)
 
 
 def randfloat(__low: float, __high: float, __prec: int = 2, /) -> float:
     """
     This function follows `random.uniform` behaviors.
     `__prec`: float precision (>= 0); if `__low` at 2 decimal point (`0.25`), `__prec` should at least `2`.
     `__prec` normally max at 15-18 (depends on system).
@@ -13,15 +16,15 @@
     ## can't use below because each end only half probability-dense
     # return round(_random.uniform(__low, __high), __prec)
 
     k = pow(10, __prec)
     return _random.randint(round(__low*k), round(__high*k)) / k
 
 
-def randrange(low: float, high: float, len: float, /, pad: float = 0.1, prec: int = 3) -> tuple[float, float]:
+def randrange(low: float, high: float, len: float, /, pad: float = 0.1, prec: int = 3) -> _Tuple[float, float]:
     """
     if `low = 0, high = 1` -> include both `0` and `1`.
     if `low = 0, high = 1, pad = 0.1` -> include both `0.1` and `0.9`.
 
     `pad`: should `0 <= pad < 0.5`
     """
```

### Comparing `mykit-2.0.1/mykit.egg-info/PKG-INFO` & `mykit-2.0.2/mykit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: report bugs, https://github.com/nvfp/mykit/issues
@@ -58,14 +58,17 @@
 ## FAQ
 
 - 
 
 
 ## Changelog
 
+- 2.0.2 (June 14, 2023):
+    - finished updating all type hints
+    - Added visibility functionality to `/app/complex/plot.py`
 - 2.0.1 (June 14, 2023):
     - Updated all type hints to make them work on Python 3.8 and 3.9
     - Added visibility functionality to `/app/complex/biplot.py`
 - 2.0.0 (June 13, 2023):
     - Breaking changes:
         - New mechanism for app: `/app/__init__.py`
         - Moved: `/kit/graph/graph2d.py` -> `/app/complex/plot.py`
```

### Comparing `mykit-2.0.1/mykit.egg-info/SOURCES.txt` & `mykit-2.0.2/mykit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mykit-2.0.1/pyproject.toml` & `mykit-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mykit"
-version = "2.0.1"
+version = "2.0.2"
 description = "Python utility library"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

