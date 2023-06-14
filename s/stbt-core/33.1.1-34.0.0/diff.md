# Comparing `tmp/stbt_core-33.1.1.tar.gz` & `tmp/stbt_core-34.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stbt_core-33.1.1.tar", last modified: Thu Mar 23 11:06:59 2023, max compression
+gzip compressed data, was "stbt_core-34.0.0.tar", last modified: Wed Jun 14 10:55:22 2023, max compression
```

## Comparing `stbt_core-33.1.1.tar` & `stbt_core-34.0.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2023-03-23 11:06:59.210695 stbt_core-33.1.1/
--rw-r--r--   0 drothlis  (1000) drothlis  (1000)    24486 2019-05-20 14:19:36.000000 stbt_core-33.1.1/LICENSE
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      345 2022-07-08 07:29:17.000000 stbt_core-33.1.1/MANIFEST.in
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1821 2023-03-23 11:06:59.210695 stbt_core-33.1.1/PKG-INFO
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1572 2022-07-16 09:25:43.000000 stbt_core-33.1.1/README.md
-drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2023-03-23 11:06:59.206694 stbt_core-33.1.1/_stbt/
--rw-r--r--   0 drothlis  (1000) drothlis  (1000)        0 2020-12-14 13:13:00.000000 stbt_core-33.1.1/_stbt/__init__.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    32123 2023-03-23 10:24:36.000000 stbt_core-33.1.1/_stbt/android.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     5279 2022-11-15 16:58:36.000000 stbt_core-33.1.1/_stbt/black.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     6097 2023-02-02 16:29:48.000000 stbt_core-33.1.1/_stbt/config.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1693 2022-07-16 09:25:43.000000 stbt_core-33.1.1/_stbt/cv2_compat.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    11072 2022-11-15 16:58:36.000000 stbt_core-33.1.1/_stbt/diff.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    10314 2022-11-15 16:58:36.000000 stbt_core-33.1.1/_stbt/frameobject.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     9110 2022-11-15 16:58:36.000000 stbt_core-33.1.1/_stbt/grid.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    14278 2022-11-15 16:58:36.000000 stbt_core-33.1.1/_stbt/imgproc_cache.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    23899 2023-03-23 10:24:19.000000 stbt_core-33.1.1/_stbt/imgutils.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    36093 2023-02-02 16:28:47.000000 stbt_core-33.1.1/_stbt/keyboard.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    11204 2022-11-15 16:58:36.000000 stbt_core-33.1.1/_stbt/logging.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    11304 2022-11-15 16:58:36.000000 stbt_core-33.1.1/_stbt/mask.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    41413 2022-11-15 16:58:36.000000 stbt_core-33.1.1/_stbt/match.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     8462 2023-02-02 16:26:55.000000 stbt_core-33.1.1/_stbt/motion.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     4701 2022-11-15 16:58:36.000000 stbt_core-33.1.1/_stbt/multipress.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    30799 2022-11-15 16:58:36.000000 stbt_core-33.1.1/_stbt/ocr.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     3218 2022-11-15 16:58:36.000000 stbt_core-33.1.1/_stbt/precondition.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    11457 2022-10-13 08:33:40.000000 stbt_core-33.1.1/_stbt/pylint_plugin.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      925 2022-07-16 09:25:43.000000 stbt_core-33.1.1/_stbt/stbt.conf
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    13470 2023-02-02 16:26:55.000000 stbt_core-33.1.1/_stbt/transition.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    18113 2022-11-22 09:53:49.000000 stbt_core-33.1.1/_stbt/types.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     3566 2022-07-16 09:25:43.000000 stbt_core-33.1.1/_stbt/utils.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     6539 2022-11-15 16:58:36.000000 stbt_core-33.1.1/_stbt/wait.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       38 2023-03-23 11:06:59.210695 stbt_core-33.1.1/setup.cfg
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     2282 2023-03-23 11:02:42.000000 stbt_core-33.1.1/setup.py
-drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2023-03-23 11:06:59.206694 stbt_core-33.1.1/stbt_core/
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    11048 2022-11-15 16:58:36.000000 stbt_core-33.1.1/stbt_core/__init__.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      132 2022-07-16 09:25:43.000000 stbt_core-33.1.1/stbt_core/pylint_plugin.py
-drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2023-03-23 11:06:59.206694 stbt_core-33.1.1/stbt_core.egg-info/
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1821 2023-03-23 11:06:59.000000 stbt_core-33.1.1/stbt_core.egg-info/PKG-INFO
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      665 2023-03-23 11:06:59.000000 stbt_core-33.1.1/stbt_core.egg-info/SOURCES.txt
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)        1 2023-03-23 11:06:59.000000 stbt_core-33.1.1/stbt_core.egg-info/dependency_links.txt
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      145 2023-03-23 11:06:59.000000 stbt_core-33.1.1/stbt_core.egg-info/requires.txt
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       16 2023-03-23 11:06:59.000000 stbt_core-33.1.1/stbt_core.egg-info/top_level.txt
+drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2023-06-14 10:55:22.226771 stbt_core-34.0.0/
+-rw-r--r--   0 drothlis  (1000) drothlis  (1000)    24486 2019-05-20 14:19:36.000000 stbt_core-34.0.0/LICENSE
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      321 2023-06-14 10:43:47.000000 stbt_core-34.0.0/MANIFEST.in
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1821 2023-06-14 10:55:22.226771 stbt_core-34.0.0/PKG-INFO
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1572 2022-07-16 09:25:43.000000 stbt_core-34.0.0/README.md
+drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2023-06-14 10:55:22.226771 stbt_core-34.0.0/_stbt/
+-rw-r--r--   0 drothlis  (1000) drothlis  (1000)        0 2020-12-14 13:13:00.000000 stbt_core-34.0.0/_stbt/__init__.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    32123 2023-05-17 07:16:04.000000 stbt_core-34.0.0/_stbt/android.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     5279 2022-11-15 16:58:36.000000 stbt_core-34.0.0/_stbt/black.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     6108 2023-05-17 07:16:04.000000 stbt_core-34.0.0/_stbt/config.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1693 2022-07-16 09:25:43.000000 stbt_core-34.0.0/_stbt/cv2_compat.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    13982 2023-06-14 10:43:47.000000 stbt_core-34.0.0/_stbt/diff.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    10314 2022-11-15 16:58:36.000000 stbt_core-34.0.0/_stbt/frameobject.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     9110 2022-11-15 16:58:36.000000 stbt_core-34.0.0/_stbt/grid.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    14278 2022-11-15 16:58:36.000000 stbt_core-34.0.0/_stbt/imgproc_cache.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    23914 2023-05-17 07:16:04.000000 stbt_core-34.0.0/_stbt/imgutils.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    36093 2023-05-16 14:20:10.000000 stbt_core-34.0.0/_stbt/keyboard.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     3142 2023-06-14 10:43:47.000000 stbt_core-34.0.0/_stbt/libstbt.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    11281 2023-05-24 09:43:38.000000 stbt_core-34.0.0/_stbt/logging.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    12136 2023-05-24 09:43:42.000000 stbt_core-34.0.0/_stbt/mask.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    42474 2023-06-14 10:43:47.000000 stbt_core-34.0.0/_stbt/match.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    10381 2023-05-24 09:43:42.000000 stbt_core-34.0.0/_stbt/motion.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     4701 2022-11-15 16:58:36.000000 stbt_core-34.0.0/_stbt/multipress.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    30799 2022-11-15 16:58:36.000000 stbt_core-34.0.0/_stbt/ocr.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     3218 2022-11-15 16:58:36.000000 stbt_core-34.0.0/_stbt/precondition.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    11457 2022-10-13 08:33:40.000000 stbt_core-34.0.0/_stbt/pylint_plugin.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     5664 2023-06-14 10:43:47.000000 stbt_core-34.0.0/_stbt/sqdiff.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      923 2023-05-17 09:12:41.000000 stbt_core-34.0.0/_stbt/stbt.conf
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    14854 2023-05-24 09:43:42.000000 stbt_core-34.0.0/_stbt/transition.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    18342 2023-05-24 09:43:42.000000 stbt_core-34.0.0/_stbt/types.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     3566 2023-05-10 07:04:11.000000 stbt_core-34.0.0/_stbt/utils.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     6691 2023-05-17 07:46:48.000000 stbt_core-34.0.0/_stbt/wait.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       38 2023-06-14 10:55:22.226771 stbt_core-34.0.0/setup.cfg
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     2282 2023-06-14 10:44:15.000000 stbt_core-34.0.0/setup.py
+drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2023-06-14 10:55:22.226771 stbt_core-34.0.0/stbt_core/
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    11038 2023-05-24 09:43:42.000000 stbt_core-34.0.0/stbt_core/__init__.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      132 2022-07-16 09:25:43.000000 stbt_core-34.0.0/stbt_core/pylint_plugin.py
+drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2023-06-14 10:55:22.226771 stbt_core-34.0.0/stbt_core.egg-info/
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1821 2023-06-14 10:55:22.000000 stbt_core-34.0.0/stbt_core.egg-info/PKG-INFO
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      698 2023-06-14 10:55:22.000000 stbt_core-34.0.0/stbt_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)        1 2023-06-14 10:55:22.000000 stbt_core-34.0.0/stbt_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      145 2023-06-14 10:55:22.000000 stbt_core-34.0.0/stbt_core.egg-info/requires.txt
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       16 2023-06-14 10:55:22.000000 stbt_core-34.0.0/stbt_core.egg-info/top_level.txt
```

### Comparing `stbt_core-33.1.1/LICENSE` & `stbt_core-34.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stbt_core-33.1.1/PKG-INFO` & `stbt_core-34.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stbt_core
-Version: 33.1.1
+Version: 34.0.0
 Summary: Automated GUI testing for Set-Top Boxes
 Home-page: https://stb-tester.com
 Author: Stb-tester.com Ltd.
 Author-email: support@stb-tester.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,15 @@
 Provides-Extra: ocr
 License-File: LICENSE
 
 # Stb-tester open-source APIs (stbt_core)
 
 **Automated User Interface Testing for Set-Top Boxes & Smart TVs**
 
-* Copyright © 2013-2022 Stb-tester.com Ltd,
+* Copyright © 2013-2023 Stb-tester.com Ltd,
   2012-2014 YouView TV Ltd. and other contributors.
 * License: LGPL v2.1 or (at your option) any later version (see [LICENSE]).
 
 This package contains the `stbt_core` open-source Python APIs that you can use
 in test-scripts written for running on the [Stb-tester Platform]. The primary
 purpose of this package is to make the `stbt_core` library easy to install
 locally for IDE linting & autocompletion.
```

### Comparing `stbt_core-33.1.1/README.md` & `stbt_core-34.0.0/README.md`

 * *Files identical despite different names*

### Comparing `stbt_core-33.1.1/_stbt/android.py` & `stbt_core-34.0.0/_stbt/android.py`

 * *Files identical despite different names*

### Comparing `stbt_core-33.1.1/_stbt/black.py` & `stbt_core-34.0.0/_stbt/black.py`

 * *Files identical despite different names*

### Comparing `stbt_core-33.1.1/_stbt/config.py` & `stbt_core-34.0.0/_stbt/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,17 +131,17 @@
 def _config_init(force=False):
     global _config
     if force or not _config:
         config_files = [_find_file('stbt.conf')]
         try:
             # Host-wide config, e.g. /etc/stbt/stbt.conf (see `Makefile`).
             from .vars import sysconfdir
-            config_files.append(os.path.join(sysconfdir, 'stbt/stbt.conf'))
         except ImportError:
-            pass
+            sysconfdir = "/etc"
+        config_files.append(os.path.join(sysconfdir, 'stbt/stbt.conf'))
 
         # User config: ~/.config/stbt/stbt.conf, as per freedesktop's base
         # directory specification:
         config_files.append('%s/stbt/stbt.conf' % xdg_config_dir())
 
         # Config files specific to the test suite / test run,
         # with the one at the beginning taking precedence:
```

### Comparing `stbt_core-33.1.1/_stbt/cv2_compat.py` & `stbt_core-34.0.0/_stbt/cv2_compat.py`

 * *Files identical despite different names*

### Comparing `stbt_core-33.1.1/_stbt/diff.py` & `stbt_core-34.0.0/_stbt/logging.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,330 +1,356 @@
-from __future__ import annotations
+import argparse
+import itertools
+import logging
+import os
+import sys
+from collections import namedtuple, OrderedDict
+from contextlib import contextmanager
+from textwrap import dedent
 
-from typing import Optional
+from .config import get_config
+from .types import Region
+from .utils import mkdir_p
 
-import cv2
-import numpy
 
-from .imgutils import (
-    Frame, FrameT, crop, _frame_repr, _image_region, pixel_bounding_box)
-from .logging import ddebug, ImageLogger
-from .mask import load_mask, MaskTypes
-from .types import Region, SizeT
+_debug_level = None
 
+# Running in a Jupyter Notebook:
+_jupyter_logging_enabled = "JPY_PARENT_PID" in os.environ
 
-class MotionResult():
-    """The result from `detect_motion` and `wait_for_motion`.
+logger = logging.getLogger("stbt")
+trace_logger = logging.getLogger("stbt.trace")
 
-    :ivar float time: The time at which the video-frame was captured, in
-        seconds since 1970-01-01T00:00Z. This timestamp can be compared with
-        system time (``time.time()``).
 
-    :ivar bool motion: True if motion was found. This is the same as evaluating
-        ``MotionResult`` as a bool. That is, ``if result:`` will behave the
-        same as ``if result.motion:``.
+def init_logger():
+    if logger.handlers:
+        logger.warning("stbt logger already initialised", stack_info=True)
+        return
+    handler = logging.StreamHandler(sys.stderr)
+    handler.setFormatter(
+        logging.Formatter("%(levelname)s:%(name)s:%(message)s"))
+    logger.addHandler(handler)
+    logger.setLevel(logging.DEBUG)
+    logger.propagate = False
 
-    :ivar Region region: Bounding box where the motion was found, or ``None``
-        if no motion was found.
 
-    :ivar Frame frame: The video frame in which motion was (or wasn't) found.
-    """
-    _fields = ("time", "motion", "region", "frame")
+def debug(msg: str, *args, **kwargs):
+    """Print the given string to stderr if stbt run `--verbose` was given."""
+    if get_debug_level() > 0:
+        logger.debug(msg, *args, **kwargs)
 
-    def __init__(self, time: float, motion: bool, region: Region, frame: Frame):
-        self.time: float = time
-        self.motion: bool = motion
-        self.region: Region = region
-        self.frame: Frame = frame
-
-    def __bool__(self) -> bool:
-        return self.motion
-
-    def __nonzero__(self) -> bool:
-        return self.__bool__()
-
-    def __repr__(self) -> str:
-        return (
-            "MotionResult(time=%s, motion=%r, region=%r, frame=%s)" % (
-                "None" if self.time is None else "%.3f" % self.time,
-                self.motion, self.region, _frame_repr(self.frame)))
-
-
-class FrameDiffer():
-    """Interface for different algorithms for diffing frames in a sequence.
-
-    Say you have a sequence of frames A, B, C. Typically you will compare frame
-    A against B, and then frame B against C. This is a class (not a function)
-    so that you can remember work you've done on frame B, so that you don't
-    repeat that work when you need to compare against frame C.
-    """
-    def diff(self, frame: FrameT):
-        raise NotImplementedError(
-            "%s.diff is not implemented" % self.__class__.__name__)
-
-
-class BGRDiff(FrameDiffer):
-    """Compares 2 frames by calculating the color distance between them.
-
-    The algorithm is a simple euclidean distance between each pair of
-    corresponding pixels in the 2 frames. The color difference is then
-    binarized using the specified threshold: Values greater than the threshold
-    are counted as differences (that is, motion). Then, an "erode" operation
-    removes differences that are only 1 pixel wide or high. If any differences
-    remain, the 2 frames are considered different.
 
-    This is the default diffing algorithm for `find_selection_from_background`
-    and `ocr`'s `text_color`.
-    """
+def ddebug(s):
+    """Extra verbose debug for stbt developers, not end users"""
+    if get_debug_level() > 1:
+        trace_logger.debug(s)
 
-    def __init__(
-        self,
-        initial_frame: FrameT,
-        mask: MaskTypes = Region.ALL,
-        min_size: Optional[SizeT] = None,
-        threshold: float = 25,
-        erode: bool = True,
-    ):
-        self.prev_frame = initial_frame
-        self.min_size = min_size
-        self.threshold = threshold
-
-        self.mask_, self.region = load_mask(mask).to_array(
-            _image_region(initial_frame))
-
-        if isinstance(erode, numpy.ndarray):  # For power users
-            kernel = erode
-        elif erode:
-            kernel = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (3, 3))
-        else:
-            kernel = None
-        self.kernel = kernel
 
-    def diff(self, frame: FrameT) -> MotionResult:
-        imglog = ImageLogger("BGRDiff", region=self.region,
-                             min_size=self.min_size, threshold=self.threshold)
-        imglog.imwrite("source", frame)
-        imglog.imwrite("previous_frame", self.prev_frame)
-
-        mask_pixels = self.mask_
-        cframe = crop(frame, self.region)
-        cprev = crop(self.prev_frame, self.region)
-
-        sqd = numpy.subtract(cframe, cprev, dtype=numpy.int32)
-        sqd = (sqd[:, :, 0] ** 2 +
-               sqd[:, :, 1] ** 2 +
-               sqd[:, :, 2] ** 2)
-        sqd = sqd.reshape(sqd.shape + (1,))
-
-        if imglog.enabled:
-            normalised = numpy.sqrt(sqd / 3)
-            if mask_pixels is None:
-                imglog.imwrite("sqd", normalised)
-            else:
-                imglog.imwrite("sqd",
-                               normalised.astype(numpy.uint8) & mask_pixels)
+def warn(msg: str, *args, **kwargs):
+    logger.warning(msg, *args, **kwargs)
 
-        d = sqd >= (self.threshold ** 2) * 3
-        if mask_pixels is not None:
-            d = numpy.logical_and(d, mask_pixels)  # pylint:disable=assignment-from-no-return
-            imglog.imwrite("mask", mask_pixels)
-        d = d.astype(numpy.uint8)
-        if imglog.enabled:
-            imglog.imwrite("thresholded", d * 255)
-
-        if self.kernel is not None:
-            d = cv2.morphologyEx(d, cv2.MORPH_OPEN, self.kernel)
-            if imglog.enabled:
-                imglog.imwrite("eroded", d * 255)
-
-        out_region = pixel_bounding_box(d)
-        if out_region:
-            # Undo crop:
-            out_region = out_region.translate(self.region)
-
-        motion = bool(out_region and (
-            self.min_size is None or
-            (out_region.width >= self.min_size[0] and
-             out_region.height >= self.min_size[1])))
-
-        if motion:
-            # Only update the comparison frame if it's different to the previous
-            # one.  This makes `detect_motion` more sensitive to slow motion
-            # because the differences between frames 1 and 2 might be small and
-            # the differences between frames 2 and 3 might be small but we'd see
-            # the difference by looking between 1 and 3.
-            self.prev_frame = frame
-
-        result = MotionResult(getattr(frame, "time", None), motion,
-                              out_region, frame)
-        ddebug(str(result))
-        imglog.html(BGRDIFF_HTML, result=result)
-        return result
-
-
-BGRDIFF_HTML = """\
-    <h4>
-      BGRDiff:
-      {{ "Found" if result.motion else "Didn't find" }} differences
-    </h4>
-
-    {{ annotated_image(result) }}
-
-    <h5>Result:</h5>
-    <pre><code>{{ result | escape }}</code></pre>
-
-    {% if result.region and not result.motion %}
-    <p>Found motion <code>{{ result.region | escape }}</code> smaller than
-    min_size <code>{{ min_size | escape }}</code>.</p>
-    {% endif %}
-
-    <h5>Previous frame:</h5>
-    <img src="previous_frame.png" />
 
-    <h5>Differences:</h5>
-    <img src="sqd.png" />
+def get_debug_level():
+    global _debug_level
+    if _debug_level is None:
+        _debug_level = get_config('global', 'verbose', type_=int)
+    return _debug_level
 
-    {% if "mask" in images %}
-    <h5>Mask:</h5>
-    <img src="mask.png" />
-    {% endif %}
 
-    <h5>Differences above threshold ({{threshold}}):</h5>
-    <img src="thresholded.png" />
+@contextmanager
+def scoped_debug_level(level):
+    global _debug_level
+    oldlevel = _debug_level
+    _debug_level = level
+    try:
+        yield
+    finally:
+        _debug_level = oldlevel
 
-    {% if "eroded" in images %}
-    <h5>Eroded:</h5>
-    <img src="eroded.png" />
-    {% endif %}
-"""
 
+def argparser_add_verbose_argument(argparser):
+    class IncreaseDebugLevel(argparse.Action):
+        num_calls = 0
 
-class GrayscaleDiff(FrameDiffer):
-    """Compares 2 frames by converting them to grayscale, calculating
-    pixel-wise absolute differences, and ignoring differences below a
-    threshold.
+        def __call__(self, parser, namespace, values, option_string=None):
+            global _debug_level
+            self.num_calls += 1
+            _debug_level = self.num_calls
+            setattr(namespace, self.dest, _debug_level)
 
-    This is the default diffing algorithm for `wait_for_motion` and
-    `press_and_wait`.
-    """
+    argparser.add_argument(
+        '-v', '--verbose', action=IncreaseDebugLevel, nargs=0,
+        default=get_debug_level(),  # for stbt-run arguments dump
+        help='Enable debug output (specify twice to enable detailed '
+             'dumps to ./stbt-debug directory)')
 
-    def __init__(
-        self,
-        initial_frame: FrameT,
-        mask: MaskTypes = Region.ALL,
-        min_size: Optional[SizeT] = None,
-        threshold: float = 0.84,
-        erode: bool = True,
-    ):
-        self.prev_frame = initial_frame
-        self.min_size = min_size
-        self.threshold = threshold
-
-        self.mask_, self.region = load_mask(mask).to_array(
-            _image_region(initial_frame))
-
-        if isinstance(erode, numpy.ndarray):  # For power users
-            kernel = erode
-        elif erode:
-            kernel = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (3, 3))
-        else:
-            kernel = None
-        self.kernel = kernel
 
-        self.prev_frame_gray = self.gray(initial_frame)
+def imshow(img, regions=None):
+    """Displays the image in a Jupyter Notebook Notebook.
 
-    def gray(self, frame: FrameT):
-        return cv2.cvtColor(crop(frame, self.region), cv2.COLOR_BGR2GRAY)
+    You can only call this if you're already inside a Jupyter Notebook.
+    """
+    if "JPY_PARENT_PID" not in os.environ:
+        raise RuntimeError(
+            "_stbt.logging.imshow can only be run inside a Jupyter Notebook")
+
+    import cv2
+
+    if regions:
+        from _stbt.imgutils import load_image
+        img = load_image(img)
+        for r in regions:
+            cv2.rectangle(img, (r.x, r.y), (r.right, r.bottom), (32, 0, 255))
+
+    from IPython.core.display import Image, display
+    if isinstance(img, str):
+        display(Image(img))
+    else:
+        _, data = cv2.imencode(".png", img)
+        display(Image(data=bytes(data.data), format="png"))
 
-    def diff(self, frame: FrameT) -> MotionResult:
-        frame_gray = self.gray(frame)
-
-        imglog = ImageLogger("GrayscaleDiff", region=self.region,
-                             min_size=self.min_size,
-                             threshold=self.threshold)
-        imglog.imwrite("source", frame)
-        imglog.imwrite("gray", frame_gray)
-        imglog.imwrite("previous_frame_gray", self.prev_frame_gray)
-
-        absdiff = cv2.absdiff(self.prev_frame_gray, frame_gray)
-        imglog.imwrite("absdiff", absdiff)
-
-        if self.mask_ is not None:
-            absdiff = cv2.bitwise_and(absdiff, self.mask_)
-            imglog.imwrite("mask", self.mask_)
-            imglog.imwrite("absdiff_masked", absdiff)
-
-        _, thresholded = cv2.threshold(
-            absdiff, int((1 - self.threshold) * 255), 255,
-            cv2.THRESH_BINARY)
-        imglog.imwrite("absdiff_threshold", thresholded)
-        if self.kernel is not None:
-            thresholded = cv2.morphologyEx(
-                thresholded, cv2.MORPH_OPEN, self.kernel)
-            imglog.imwrite("absdiff_threshold_erode", thresholded)
-
-        out_region = pixel_bounding_box(thresholded)
-        if out_region:
-            # Undo crop:
-            out_region = out_region.translate(self.region)
-
-        motion = bool(out_region and (
-            self.min_size is None or
-            (out_region.width >= self.min_size[0] and
-             out_region.height >= self.min_size[1])))
-
-        if motion:
-            # Only update the comparison frame if it's different to the previous
-            # one.  This makes `detect_motion` more sensitive to slow motion
-            # because the differences between frames 1 and 2 might be small and
-            # the differences between frames 2 and 3 might be small but we'd see
-            # the difference by looking between 1 and 3.
-            self.prev_frame = frame
-            self.prev_frame_gray = frame_gray
-
-        result = MotionResult(getattr(frame, "time", None), motion,
-                              out_region, frame)
-        ddebug(str(result))
-        imglog.html(GRAYSCALEDIFF_HTML, result=result)
-        return result
-
-
-GRAYSCALEDIFF_HTML = """\
-    <h4>
-      GrayscaleDiff:
-      {{ "Found" if result.motion else "Didn't find" }} differences
-    </h4>
-
-    {{ annotated_image(result) }}
-
-    <h5>Result:</h5>
-    <pre><code>{{ result | escape }}</code></pre>
-
-    {% if result.region and not result.motion %}
-    <p>Found motion <code>{{ result.region | escape }}</code> smaller than
-    min_size <code>{{ min_size | escape }}</code>.</p>
-    {% endif %}
 
-    <h5>ROI Gray:</h5>
-    <img src="gray.png" />
+class ImageLogger():
+    """Log intermediate images used in image processing (such as `match`).
 
-    <h5>Previous frame ROI Gray:</h5>
-    <img src="previous_frame_gray.png" />
+    Create a new ImageLogger instance for each frame of video.
+    """
+    _frame_number = itertools.count(1)
 
-    <h5>Absolute difference:</h5>
-    <img src="absdiff.png" />
+    def __init__(self, name, **kwargs):
+        self.jupyter = _jupyter_logging_enabled
+        self.enabled = get_debug_level() > 1 or self.jupyter
+        if not self.enabled:
+            return
+
+        self.name = name
+        self.frame_number = next(ImageLogger._frame_number)
+
+        try:
+            outdir = os.path.join("stbt-debug", "%05d" % self.frame_number)
+            mkdir_p(outdir)
+            self.outdir = outdir
+        except OSError:
+            warn("Failed to create directory '%s'; won't save debug images."
+                 % outdir)
+            self.enabled = False
+            return
+
+        self.images = OrderedDict()
+        self.data = {}
+        for k, v in kwargs.items():
+            self.data[k] = v
+
+    def set(self, **kwargs):
+        if not self.enabled:
+            return
+        for k, v in kwargs.items():
+            self.data[k] = v
+
+    def append(self, **kwargs):
+        if not self.enabled:
+            return
+        for k, v in kwargs.items():
+            if k not in self.data:
+                self.data[k] = []
+            self.data[k].append(v)
+
+    def imwrite(self, name, image, regions=None, colours=None, scale=1):
+        import cv2
+        import numpy
+        if not self.enabled:
+            return
+        if image is None:
+            return
+        if name in self.images:
+            raise ValueError("Image for name '%s' already logged" % name)
+        if image is None:
+            return
+        if image.dtype == numpy.float32:
+            # Scale `cv2.matchTemplate` heatmap output in range
+            # [0.0, 1.0] to visible grayscale range [0, 255].
+            image = cv2.convertScaleAbs(image, alpha=255.0 / scale)
+        else:
+            image = image.copy()
+        self.images[name] = image
+        if regions is None:
+            regions = []
+        elif not isinstance(regions, list):
+            regions = [regions]
+        if colours is None:
+            colours = []
+        elif not isinstance(colours, list):
+            colours = [colours]
+        for region, colour in zip(regions, colours):
+            cv2.rectangle(
+                image, (region.x, region.y), (region.right, region.bottom),
+                colour, thickness=1)
+
+        cv2.imwrite(os.path.join(self.outdir, name + ".png"), image)
+
+    def html(self, template, **kwargs):
+        if not self.enabled:
+            return
+
+        try:
+            import jinja2
+        except ImportError:
+            warn(
+                "Not generating html view of the image-processing debug images "
+                "because python 'jinja2' module is not installed.")
+            return
+
+        template_kwargs = self.data.copy()
+        template_kwargs["images"] = self.images
+        template_kwargs.update(kwargs)
+
+        index_html = os.path.join(self.outdir, "index.html")
+        with open(index_html, "w", encoding="utf-8") as f:
+            f.write(jinja2.Template(_INDEX_HTML_HEADER)
+                    .render(frame_number=self.frame_number,
+                            jupyter=self.jupyter))
+            f.write(jinja2.Template(dedent(template.lstrip("\n")))
+                    .render(annotated_image=self._draw_annotated_image,
+                            draw=self._draw,
+                            jupyter=self.jupyter,
+                            **template_kwargs))
+            f.write(jinja2.Template(_INDEX_HTML_FOOTER)
+                    .render())
+
+        if self.jupyter:
+            from IPython.display import display, IFrame
+            display(IFrame(src=index_html, width=974, height=600))
+
+    def _draw(self, region, source_size, css_class, title=None):
+        import jinja2
+
+        if region is None:
+            return ""
+
+        if isinstance(css_class, bool):
+            if css_class:
+                css_class = "matched"
+            else:
+                css_class = "nomatch"
 
-    {% if "mask" in images %}
-    <h5>Mask:</h5>
-    <img src="mask.png" />
-    <h5>Absolute difference – masked:</h5>
-    <img src="absdiff_masked.png" />
+        return jinja2.Template(dedent("""\
+            <div class="region {{css_class}}"
+                 style="left: {{region.x / image.width * 100}}%;
+                        top: {{region.y / image.height * 100}}%;
+                        width: {{region.width / image.width * 100}}%;
+                        height: {{region.height / image.height * 100}}%"
+                 {% if title %}
+                 title="{{ title | escape }}"
+                 {% endif %}
+                 ></div>
+            """)) \
+            .render(css_class=css_class,
+                    image=source_size,
+                    region=region,
+                    title=title)
+
+    def _draw_annotated_image(self, regions=None, source_name="source"):
+        import jinja2
+
+        s = self.images[source_name].shape
+        source_size = Region(0, 0, s[1], s[0])
+
+        _regions = []
+        if "region" in self.data:
+            _regions.append((Region.intersect(self.data["region"], source_size),
+                             "source_region", None))
+
+        if regions is None:
+            regions = []
+        elif not isinstance(regions, list):
+            regions = [regions]
+        for r in regions:
+            if isinstance(r, Region):
+                _regions.append((r, True, None))
+            elif hasattr(r, "region"):  # e.g. MotionResult
+                _regions.append((r.region, bool(r), None))
+            elif isinstance(r, tuple) and len(r) == 3:
+                _regions.append(r)
+            else:
+                warn("ImageLogger._draw_annotated_image: Expected Region, "
+                     "Match/MotionResult, or 3-tuple (region, css_class, title)"
+                     "; got %r" % (r,))
+
+        return jinja2.Template(dedent("""\
+            <div class="annotated_image">
+              <img src="{{source_name}}.png">
+              {% for region, css_class, title in regions %}
+              {{ draw(region, source_size, css_class, title) }}
+              {% endfor %}
+            </div>
+        """)).render(
+            draw=self._draw,
+            regions=_regions,
+            source_name=source_name,
+            source_size=source_size,
+        )
+
+
+_INDEX_HTML_HEADER = dedent("""\
+    <!DOCTYPE html>
+    <html lang='en'>
+    <head>
+    <meta charset="utf-8"/>
+    <link href="https://stb-tester.com/assets/bootstrap-3.3.2.min.css" rel="stylesheet">
+    <style>
+        a.nav { margin: 10px; }
+        a.nav.pull-left { margin-left: 0; }
+        a.nav.pull-right { margin-right: 0; }
+        h5 { margin-top: 40px; }
+        .annotated_image { position: relative; display: inline-block; }
+        .annotated_image img { max-width: 100%; }
+        .region { position: absolute; }
+        .source_region { outline: 2px solid #8080ff; }
+        .region.matched { outline: 2px solid #ff0020; }
+        .region.nomatch { outline: 2px solid #ffff20; }
+
+        /* match */
+        .table th { font-weight: normal; background-color: #eee; }
+        img.thumb {
+            vertical-align: middle; max-width: 150px; max-height: 36px;
+            padding: 1px; border: 1px solid #ccc; }
+        .table td { vertical-align: middle; }
+    </style>
+    </head>
+    <body>
+    <div class="container-fluid">
+    {% if not jupyter %}
+    {%   if frame_number > 1 %}
+    <a href="../{{ "%05d" % (frame_number - 1) }}/index.html"
+       class="nav pull-left">«prev</a>
+    {%   endif %}
+    <a href="../{{ "%05d" % (frame_number + 1) }}/index.html"
+       class="nav pull-right">next»</a>
     {% endif %}
+    """)
 
-    <h5>Binarized (threshold={{threshold}}):</h5>
-    <img src="absdiff_threshold.png" />
+_INDEX_HTML_FOOTER = dedent("""\
 
-    {% if "eroded" in images %}
-    <h5>Eroded:</h5>
-    <img src="absdiff_threshold_erode.png" />
-    {% endif %}
-"""
+    </div>
+    </body>
+    </html>
+""")
+
+
+def draw_on(frame, *args, **kwargs):
+    draw_sink_ref = getattr(frame, '_draw_sink', None)
+    if not draw_sink_ref:
+        return
+    draw_sink = draw_sink_ref()
+    if not draw_sink:
+        return
+    draw_sink.draw(*args, **kwargs)
+
+
+class _Annotation(namedtuple("_Annotation", "time region label colour")):
+    MATCHED = (32, 0, 255)  # Red
+    NO_MATCH = (32, 255, 255)  # Yellow
+
+    @staticmethod
+    def from_result(result, label=""):
+        colour = _Annotation.MATCHED if result else _Annotation.NO_MATCH
+        return _Annotation(result.time, result.region, label, colour)
```

### Comparing `stbt_core-33.1.1/_stbt/frameobject.py` & `stbt_core-34.0.0/_stbt/frameobject.py`

 * *Files identical despite different names*

### Comparing `stbt_core-33.1.1/_stbt/grid.py` & `stbt_core-34.0.0/_stbt/grid.py`

 * *Files identical despite different names*

### Comparing `stbt_core-33.1.1/_stbt/imgproc_cache.py` & `stbt_core-34.0.0/_stbt/imgproc_cache.py`

 * *Files identical despite different names*

### Comparing `stbt_core-33.1.1/_stbt/imgutils.py` & `stbt_core-34.0.0/_stbt/imgutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,14 +418,19 @@
         filename = obj.filename
         absolute_filename = obj.absolute_filename
         img = _convert_color(obj, color_channels, absolute_filename)
     elif isinstance(obj, numpy.ndarray):
         filename = None
         absolute_filename = None
         img = _convert_color(obj, color_channels, absolute_filename)
+        if img.shape[2] == 4:
+            # Normalise transparency channel to either 0 or 255, for stbt.match
+            img = img.copy()
+            chan = img[:, :, 3]
+            chan[chan < 255] = 0
     elif isinstance(filename, str):
         absolute_filename = find_file(filename)
         img = _imread(absolute_filename, color_channels)
     else:
         raise TypeError("load_image requires a filename or Image")
 
     if not isinstance(img, Image):
@@ -607,46 +612,43 @@
 
     :rtype: str
     :returns: Absolute filename.
     :raises: `FileNotFoundError` if the file can't be found.
 
     Added in v33.
     """
-    if os.path.isabs(filename) and os.path.isfile(filename):
-        return filename
+    if os.path.isabs(filename):
+        if os.path.isfile(filename):
+            return filename
 
-    # Start searching from the first parent stack-frame that is outside of
-    # the _stbt installation directory (this file's directory).
-    _stbt_dir = os.path.abspath(os.path.dirname(__file__))
-    caller = inspect.currentframe()
-    try:
-        caller = caller.f_back  # skip this frame (find_file)
-        while caller:
-            caller_dir = os.path.abspath(
-                os.path.dirname(inspect.getframeinfo(caller).filename))
-            if not caller_dir.startswith(_stbt_dir):
+    else:
+        caller = inspect.currentframe()
+        try:
+            caller = caller.f_back  # skip this frame (find_file)
+            while caller:
+                caller_dir = os.path.abspath(
+                    os.path.dirname(inspect.getframeinfo(caller).filename))
                 caller_path = os.path.join(caller_dir, filename)
                 if os.path.isfile(caller_path):
                     ddebug("Resolved relative path %r to %r" % (
                         filename, caller_path))
                     return caller_path
-            caller = caller.f_back
-    finally:
-        # Avoid circular references between stack frame objects and themselves
-        # for more deterministic GC.  See
-        # https://docs.python.org/3.6/library/inspect.html#the-interpreter-stack
-        # for more information.
-        del caller
-
-    # Fall back to image from cwd, to allow loading an image saved previously
-    # during the same test-run.
-    if os.path.isfile(filename):
-        abspath = os.path.abspath(filename)
-        ddebug("Resolved relative path %r to %r" % (filename, abspath))
-        return abspath
+                caller = caller.f_back
+        finally:
+            # Avoid circular references between stack frame objects and
+            # themselves for more deterministic GC. See
+            # https://docs.python.org/3.10/library/inspect.html#the-interpreter-stack
+            del caller
+
+        # Fall back to image from cwd, to allow loading an image saved
+        # previously during the same test-run.
+        if os.path.isfile(filename):
+            abspath = os.path.abspath(filename)
+            ddebug("Resolved relative path %r to %r" % (filename, abspath))
+            return abspath
 
     raise FileNotFoundError(errno.ENOENT, "No such file", filename)
 
 
 def limit_time(frames, duration_secs):
     """
     Adapts a frame iterator such that it will return EOS after `duration_secs`
```

### Comparing `stbt_core-33.1.1/_stbt/keyboard.py` & `stbt_core-34.0.0/_stbt/keyboard.py`

 * *Files identical despite different names*

### Comparing `stbt_core-33.1.1/_stbt/mask.py` & `stbt_core-34.0.0/_stbt/mask.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from functools import lru_cache
-from typing import Optional, Tuple, Union
+from typing import Optional, Tuple, TypeAlias, Union
 
 import cv2
 import numpy
 
 from .imgutils import (
-    _convert_color, crop, find_file, Image, load_image, pixel_bounding_box,
-    _relative_filename)
+    _convert_color, crop, find_file, Image, ImageT, _image_region, load_image,
+    pixel_bounding_box, _relative_filename)
+from .logging import logger
 from .types import Region
 
 try:
     from _stbt.xxhash import Xxhash64
 except ImportError:
     Xxhash64 = None
 
 
-MaskTypes = Union[str, numpy.ndarray, "Mask", Region, None]
+MaskTypes: TypeAlias = Union[str, numpy.ndarray, "Mask", Region, None]
 
 
 def load_mask(mask: MaskTypes) -> Mask:
     """Used to load a mask from disk, or to create a mask from a `Region`.
 
     A mask is a black & white image (the same size as the video-frame) that
     specifies which parts of the frame to process: White pixels select the area
@@ -98,14 +99,33 @@
         elif m is None:  # Region.intersect can return None for "no region"
             self._region = Region.ALL
             self._invert = not invert
         else:
             raise TypeError("Expected filename, Image, Mask, or Region. "
                             f"Got {m!r}")
 
+    @staticmethod
+    def from_alpha_channel(image: ImageT) -> Mask:
+        """Create a mask from the alpha channel of an image.
+
+        :type image: string or `numpy.ndarray`
+        :param image:
+          An image with an alpha (transparency) channel. This can be the
+          filename of a png file on disk, or an image previously loaded with
+          `stbt.load_image`.
+
+          Filenames should be relative paths. See `stbt.load_image` for the
+          path lookup algorithm.
+        """
+        image = load_image(image)
+        if image.shape[2] == 4:
+            return Mask(image[:, :, 3])
+        else:
+            return Mask(_image_region(image))
+
     def __eq__(self, o):
         if isinstance(o, Region):
             return self.__eq__(Mask(o))
         if not isinstance(o, Mask):
             return False
         if self._array is not None:
             return numpy.array_equal(self._array, o._array)
@@ -241,14 +261,16 @@
             bounding_box = None
         else:
             bounding_box = region
     elif mask._region is not None and not mask._invert:
         bounding_box = Region.intersect(region, mask._region)
     else:
         bounding_box = pixel_bounding_box(array)
+        if bounding_box is None:
+            logger.warning("%r is an empty Region", mask)
 
     if bounding_box is None:
         raise ValueError("%r doesn't overlap with the frame's %r"
                          % (mask, region))
 
     if array is not None:
         array = crop(array, bounding_box)
```

### Comparing `stbt_core-33.1.1/_stbt/match.py` & `stbt_core-34.0.0/_stbt/match.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,26 +16,22 @@
 import cv2
 import numpy
 
 from . import cv2_compat
 from .config import ConfigurationError, get_config
 from .imgproc_cache import memoize_iterator
 from .imgutils import (
-    crop, FrameT, _frame_repr, ImageT, _image_region, limit_time, load_image,
-    _validate_region)
+    Frame, crop, FrameT, _frame_repr, ImageT, _image_region, limit_time,
+    load_image, _validate_region)
 from .logging import (_Annotation, ddebug, debug, draw_on, get_debug_level,
                       ImageLogger)
+from .sqdiff import sqdiff
 from .types import Position, Region, UITestFailure
 from .utils import to_unicode
 
-try:
-    from .sqdiff import sqdiff
-except ImportError:
-    sqdiff = None
-
 
 class MatchMethod(enum.Enum):
     """An enum. See `MatchParameters` for documentation of these values."""
 
     SQDIFF = "sqdiff"
     SQDIFF_NORMED = "sqdiff-normed"
     CCORR_NORMED = "ccorr-normed"
@@ -326,47 +322,79 @@
             yield result
         else:
             if not any_matches:
                 debug("No match found. Closest match: %s" % str(result))
             break
 
 
+def _norm_frame(frame: "FrameT"):
+    """Normalise single channel images to shape (h, w, 3) rather than (h, w) or
+    (h, w, 1).  match has the invariant that it behaves the same as if you'd
+    run `frame = cv2.cvtColor(frame, cv2.COLOR_GRAY2BGR)` first.
+
+    We fiddle with the strides of the numpy array to avoid copying the data.
+    """
+    if not isinstance(frame, numpy.ndarray):
+        raise TypeError(
+            "Expected numpy.ndarray, got %r" % (type(frame).__name__,))
+    if frame.dtype != numpy.uint8:
+        raise TypeError(
+            "Expected numpy.ndarray of uint8, got %r" % (frame.dtype,))
+    frame = frame.view()
+    if frame.ndim == 2:
+        frame.shape = frame.shape + (1,)
+    if frame.ndim != 3:
+        raise ValueError(
+            "Invalid shape for frame: %r. Shape must have 2 or 3 elements" %
+            (frame.shape,))
+    if frame.shape[2] not in (1, 3):
+        raise ValueError(
+            "Invalid shape for frame: %r. Shape must have 1 or 3 channels" %
+            (frame.shape,))
+    if frame.shape[2] == 1:
+        frame = numpy.lib.stride_tricks.as_strided(
+            frame, frame.shape[:2] + (3,), frame.strides[:2] + (0,),
+            subok=True, writeable=False)
+    return frame
+
+
+def test_norm_frame():
+    frame = Frame(
+        numpy.random.randint(256, size=(5, 5, 1), dtype=numpy.uint8), time=56)
+    normed = _norm_frame(frame)
+    assert normed.shape == (5, 5, 3)
+    assert isinstance(normed, Frame)
+    assert normed.time == 56
+    assert numpy.all(normed[:, :, 0] == normed[:, :, 1])
+    assert numpy.all(normed[:, :, 0] == normed[:, :, 2])
+
+
 def _match_all(image, frame, match_parameters, region):
     """
     Generator that yields a sequence of zero or more truthy MatchResults,
     followed by a falsey MatchResult.
     """
     if match_parameters is None:
         match_parameters = MatchParameters()
 
     if frame is None:
         from stbt_core import get_frame
         frame = get_frame()
 
-    # Normalise single channel images to shape (h, w, 1) rather than just (h, w)
-    frame = frame.view()
-    if len(frame.shape) == 2:
-        frame.shape = frame.shape + (1,)
-    if len(frame.shape) != 3:
-        raise ValueError(
-            "Invalid shape for frame: %r. Shape must have 2 or 3 elements" %
-            (frame.shape,))
+    # Normalise single channel images to shape (h, w, 3) rather than just (h, w)
+    frame = _norm_frame(frame)
 
-    t = load_image(image, color_channels={1: 1, 3: (3, 4)}[frame.shape[2]])
+    t = load_image(image, color_channels=(3, 4))
 
     if any(frame.shape[x] < t.shape[x] for x in (0, 1)):
         raise ValueError("Frame %r must be larger than reference image %r"
                          % (frame.shape, t.shape))
     if any(t.shape[x] < 1 for x in (0, 1)):
         raise ValueError("Reference image %r must contain some data"
                          % (t.shape,))
-    if (frame.shape[2], t.shape[2]) not in [(1, 1), (3, 3), (3, 4)]:
-        raise ValueError(
-            "Frame %r and reference image %r must have the same number of "
-            "channels" % (frame.shape, t.shape))
 
     if t.shape[2] == 4:
         if cv2_compat.version < [3, 0, 0]:
             raise ValueError(
                 "Reference image %s has alpha channel, but transparency "
                 "support requires OpenCV 3.0 or greater (you have %s)."
                 % (t.relative_filename, cv2_compat.version))
@@ -553,16 +581,15 @@
     }[match_parameters.match_method]
 
     levels = get_config("match", "pyramid_levels", type_=int)
     if levels <= 0:
         raise ConfigurationError("'match.pyramid_levels' must be > 0")
 
     if (match_parameters.match_method == MatchMethod.SQDIFF and
-            template.shape[:2] == image.shape[:2] and
-            sqdiff is not None):
+            template.shape[:2] == image.shape[:2]):
         # Fast-path: image and template are the same size, skip pyramid, FFT,
         # etc.  This is particularly useful for full-image matching.
         ddebug("stbt-match: frame and template sizes match: Using fast-path")
         imglog.set(fast_path=True)
         s, n = sqdiff(template, image)
         if n == 0:
             certainty = 1
```

### Comparing `stbt_core-33.1.1/_stbt/motion.py` & `stbt_core-34.0.0/_stbt/motion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
 import warnings
 from collections import deque
 from typing import Iterator, Optional
 
 from .config import ConfigurationError, get_config
-from .diff import FrameDiffer, GrayscaleDiff, MotionResult
-from .imgutils import limit_time, FrameT
+from .diff import BGRDiff, Differ, MotionResult
+from .imgutils import _image_region, limit_time, FrameT
 from .logging import debug, draw_on
 from .mask import MaskTypes
 from .types import Region, UITestFailure
 
 
 def detect_motion(
     timeout_secs: float = 10,
-    noise_threshold: Optional[float] = None,
+    noise_threshold: Optional[int] = None,
     mask: MaskTypes = Region.ALL,
     region: Region = Region.ALL,
     frames: Iterator[FrameT] = None,
 ) -> Iterator[MotionResult]:
     """Generator that yields a sequence of one `MotionResult` for each frame
     processed from the device-under-test's video stream.
 
@@ -35,21 +35,20 @@
     :param timeout_secs:
         A timeout in seconds. After this timeout the iterator will be exhausted.
         Thas is, a ``for`` loop like ``for m in detect_motion(timeout_secs=10)``
         will terminate after 10 seconds. If ``timeout_secs`` is ``None`` then
         the iterator will yield frames forever. Note that you can stop
         iterating (for example with ``break``) at any time.
 
-    :param float noise_threshold:
-        The amount of noise to ignore. This is only useful with noisy analogue
-        video sources. Valid values range from 0 (all differences are
-        considered noise; a value of 0 will never report motion) to 1.0 (any
-        difference is considered motion).
+    :param int noise_threshold:
+        The difference in pixel intensity to ignore. Valid values range from 0
+        (any difference is considered motion) to 255 (which would never report
+        motion).
 
-        This defaults to 0.84. You can override the global default value by
+        This defaults to 25. You can override the global default value by
         setting ``noise_threshold`` in the ``[motion]`` section of
         :ref:`.stbt.conf`.
 
     :param str|numpy.ndarray|Mask|Region mask:
         A `Region` or a mask that specifies which parts of the image to
         analyse. This accepts anything that can be converted to a Mask using
         `stbt.load_mask`. See :doc:`masks`.
@@ -60,14 +59,19 @@
     :param Iterator[stbt.Frame] frames: An iterable of video-frames to analyse.
         Defaults to ``stbt.frames()``.
 
     Changed in v33: ``mask`` accepts anything that can be converted to a Mask
     using `load_mask`. The ``region`` parameter is deprecated; pass your
     `Region` to ``mask`` instead. You can't specify ``mask`` and ``region``
     at the same time.
+
+    Changed in v34: The difference-detection algorithm takes color into
+    account. The ``noise_threshold`` parameter changed range (from 0.0-1.0 to
+    0-255), sense (from "bigger is stricter" to "smaller is stricter"), and
+    default value (from 0.84 to 25).
     """
     if frames is None:
         import stbt_core
         frames = stbt_core.frames()
 
     frames = limit_time(frames, timeout_secs)  # pylint: disable=redefined-variable-type
 
@@ -77,39 +81,75 @@
         warnings.warn(
             "stbt.detect_motion: The 'region' parameter is deprecated; "
             "pass your Region to 'mask' instead",
             DeprecationWarning, stacklevel=2)
         mask = region
 
     if noise_threshold is None:
-        noise_threshold = get_config('motion', 'noise_threshold', type_=float)
+        noise_threshold = get_config('motion', 'noise_threshold', type_=int)
 
     debug(f"Searching for motion, using mask={mask}")
 
     try:
         frame = next(frames)
     except StopIteration:
         return
 
-    differ = detect_motion.differ(frame, mask, threshold=noise_threshold)
+    differ = detect_motion.differ.replace(threshold=noise_threshold)
+    dm = DetectMotion(differ, frame, mask)
     for frame in frames:
-        result = differ.diff(frame)
+        result = dm.diff(frame)
         draw_on(frame, result, label="detect_motion()")
         debug("%s found: %s" % (
             "Motion" if result.motion else "No motion", str(result)))
         yield result
 
 
-detect_motion.differ : FrameDiffer = GrayscaleDiff
+detect_motion.differ : Differ = BGRDiff()
+
+
+class DetectMotion():
+    """Concrete implementation of the `detect_motion` algorithm.
+
+    This class is an internal implementation detail, not part of the public
+    API. It isn't part of `detect_motion` because it offers a more convenient
+    API for `press_and_wait` to use.
+
+    Responsibilities of this class:
+
+    - Remember the work done on already-seen frames (e.g. GrayscaleDiff's
+      colorspace conversion).
+    - The logic for when we update the "reference" frame.
+    """
+    def __init__(self, differ: Differ, initial_frame: FrameT,
+                 mask: MaskTypes = Region.ALL):
+        self.differ: Differ = differ
+        self.mask_tuple = differ.preprocess_mask(
+            mask, _image_region(initial_frame))
+        self.prev_frame = differ.preprocess(initial_frame, self.mask_tuple)
+
+    def diff(self, frame: FrameT) -> MotionResult:
+        new_frame = self.differ.preprocess(frame, self.mask_tuple)
+        motion = self.differ.diff(self.prev_frame, new_frame, self.mask_tuple)
+
+        if motion:
+            # Only update the comparison frame if it's different to the previous
+            # one.  This makes `detect_motion` more sensitive to slow motion
+            # because the differences between frames 1 and 2 might be small and
+            # the differences between frames 2 and 3 might be small but we'd see
+            # the difference by looking between 1 and 3.
+            self.prev_frame = new_frame
+
+        return motion
 
 
 def wait_for_motion(
     timeout_secs: float = 10,
     consecutive_frames: int = None,
-    noise_threshold: Optional[float] = None,
+    noise_threshold: Optional[int] = None,
     mask: MaskTypes = Region.ALL,
     region: Region = Region.ALL,
     frames: Iterator[FrameT] = None,
 ) -> MotionResult:
     """Search for motion in the device-under-test's video stream.
 
     "Motion" is difference in pixel values between two frames.
@@ -128,29 +168,34 @@
         * a string in the form "x/y", where "x" is the number of frames with
           motion detected out of a sliding window of "y" frames.
 
         This defaults to "10/20". You can override the global default value by
         setting ``consecutive_frames`` in the ``[motion]`` section of
         :ref:`.stbt.conf`.
 
-    :param float noise_threshold: See `detect_motion`.
+    :param int noise_threshold: See `detect_motion`.
     :param str|numpy.ndarray|Mask|Region mask: See `detect_motion`.
     :param Region region: See `detect_motion`.
     :param Iterator[stbt.Frame] frames: See `detect_motion`.
 
     :returns: `MotionResult` when motion is detected. The MotionResult's
         ``time`` and ``frame`` attributes correspond to the first frame in
         which motion was detected.
     :raises: `MotionTimeout` if no motion is detected after ``timeout_secs``
         seconds.
 
     Changed in v33: ``mask`` accepts anything that can be converted to a Mask
     using `load_mask`. The ``region`` parameter is deprecated; pass your
     `Region` to ``mask`` instead. You can't specify ``mask`` and ``region``
     at the same time.
+
+    Changed in v34: The difference-detection algorithm takes color into
+    account. The ``noise_threshold`` parameter changed range (from 0.0-1.0 to
+    0-255), sense (from "bigger is stricter" to "smaller is stricter"), and
+    default value (from 0.84 to 25).
     """
     if frames is None:
         import stbt_core
         frames = stbt_core.frames()
 
     if consecutive_frames is None:
         consecutive_frames = get_config('motion', 'consecutive_frames')
```

### Comparing `stbt_core-33.1.1/_stbt/multipress.py` & `stbt_core-34.0.0/_stbt/multipress.py`

 * *Files identical despite different names*

### Comparing `stbt_core-33.1.1/_stbt/ocr.py` & `stbt_core-34.0.0/_stbt/ocr.py`

 * *Files identical despite different names*

### Comparing `stbt_core-33.1.1/_stbt/precondition.py` & `stbt_core-34.0.0/_stbt/precondition.py`

 * *Files identical despite different names*

### Comparing `stbt_core-33.1.1/_stbt/pylint_plugin.py` & `stbt_core-34.0.0/_stbt/pylint_plugin.py`

 * *Files identical despite different names*

### Comparing `stbt_core-33.1.1/_stbt/stbt.conf` & `stbt_core-34.0.0/_stbt/stbt.conf`

 * *Files 18% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 interpress_delay_secs = 0.3
 
 [press_until_match]
 interval_secs = 3
 max_presses = 10
 
 [motion]
-noise_threshold=0.84
+noise_threshold=25
 consecutive_frames=10/20
 
 [is_screen_black]
 threshold = 20
 
 [run]
 save_video =
```

### Comparing `stbt_core-33.1.1/_stbt/transition.py` & `stbt_core-34.0.0/_stbt/transition.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,30 +11,33 @@
 https://github.com/stb-tester/stb-tester/blob/master/LICENSE for details).
 """
 
 from __future__ import annotations
 
 import enum
 import warnings
-from typing import Optional
+from typing import Iterator, Optional
 
-from .diff import FrameDiffer, GrayscaleDiff
+from .diff import BGRDiff, Differ
 from .imgutils import FrameT
-from .logging import ddebug, debug, draw_on
+from .logging import ddebug, debug, draw_on, warn
 from .mask import MaskTypes
+from .motion import DetectMotion
 from .types import KeyT, Region, SizeT
 
 
 def press_and_wait(
     key: KeyT,
     mask: MaskTypes = Region.ALL,
     region: Region = Region.ALL,
     timeout_secs: float = 10,
     stable_secs: float = 1,
-    min_size: SizeT = None,
+    min_size: SizeT | None = None,
+    retries: int = 0,
+    frames: Iterator[FrameT] | None = None,
     _dut=None,
 ) -> _TransitionResult:
 
     """Press a key, then wait for the screen to change, then wait for it to stop
     changing.
 
     This can be used to wait for a menu selection to finish moving before
@@ -62,14 +65,21 @@
     :type timeout_secs: int or float
 
     :param min_size: A tuple of ``(width, height)``, in pixels, for differences
         to be considered as "motion". Use this to ignore small differences,
         such as the blinking text cursor in a search box.
     :type min_size: Tuple[int, int]
 
+    :param int retries: Press the key again (up to this number of times) if
+        the first press didn't have any effect (that is, if the press failed
+        with `TransitionStatus.START_TIMEOUT`). Defaults to 0 (no retries).
+
+    :param Iterator[stbt.Frame] frames: An iterable of video-frames to analyse.
+        Defaults to ``stbt.frames()``.
+
     :returns:
         An object that will evaluate to true if the transition completed, false
         otherwise. It has the following attributes:
 
         * **key** (*str*) – The name of the key that was pressed.
         * **frame** (`stbt.Frame`) – If successful, the first video frame when
           the transition completed; if timed out, the last frame seen.
@@ -105,47 +115,68 @@
     Added in v33: The ``started``, ``complete`` and ``stable`` attributes of
     the returned value.
 
     Changed in v33: ``mask`` accepts anything that can be converted to a Mask
     using `load_mask`. The ``region`` parameter is deprecated; pass your
     `Region` to ``mask`` instead. You can't specify ``mask`` and ``region``
     at the same time.
+
+    Added in v34: The ``retries`` and ``frames`` parameters.
+
+    Changed in v34: The difference-detection algorithm takes color into
+    account.
     """
     if _dut is None:
         import stbt_core
         _dut = stbt_core
+    if frames is None:
+        frames = _dut.frames()
 
     if region is not Region.ALL:
         if mask is not Region.ALL:
             raise ValueError("Cannot specify mask and region at the same time")
         warnings.warn(
             "stbt.press_and_wait: The 'region' parameter is deprecated; "
             "pass your Region to 'mask' instead",
             DeprecationWarning, stacklevel=2)
         mask = region
 
-    t = _Transition(mask, timeout_secs, stable_secs, min_size, _dut)
+    result = _press_and_wait(key, mask, timeout_secs, stable_secs,
+                             min_size, frames, _dut)
+    for i in range(retries):
+        if result.status != TransitionStatus.START_TIMEOUT:
+            return result
+        warn("Keypress %s had no effect; retrying %i/%i", key, i + 1, retries)
+        result = _press_and_wait(key, mask, timeout_secs, stable_secs,
+                                 min_size, frames, _dut)
+    return result
+
+
+def _press_and_wait(key, mask, timeout_secs, stable_secs, min_size,
+                    frames, _dut) -> _TransitionResult:
+
+    t = _Transition(mask, timeout_secs, stable_secs, min_size, frames)
     press_result = _dut.press(key)
     debug("transition: %.3f: Pressed %s" % (press_result.end_time, key))
     result = t.wait(press_result)
     debug("press_and_wait(%r) -> %s" % (key, result))
     return result
 
 
-press_and_wait.differ: FrameDiffer = GrayscaleDiff
+press_and_wait.differ: Differ = BGRDiff()
 
 
 def wait_for_transition_to_end(
-    initial_frame: FrameT = None,
+    initial_frame: FrameT | None = None,
     mask: MaskTypes = Region.ALL,
     region: Region = Region.ALL,
     timeout_secs: float = 10,
     stable_secs: float = 1,
-    min_size: SizeT = None,
-    _dut=None,
+    min_size: SizeT | None = None,
+    frames: Iterator[FrameT] | None = None,
 ) -> _TransitionResult:
 
     """Wait for the screen to stop changing.
 
     In most cases you should use `press_and_wait` to measure a complete
     transition, but if you need to measure several points during a single
     transition you can use `wait_for_transition_to_end` as the last
@@ -160,58 +191,61 @@
     :param stbt.Frame initial_frame: The frame of video when the transition
         started. If `None`, we'll pull a new frame from the device under test.
 
     :param str|numpy.ndarray|Mask|Region mask: See `press_and_wait`.
     :param Region region: See `press_and_wait`.
     :param int|float timeout_secs: See `press_and_wait`.
     :param int|float stable_secs: See `press_and_wait`.
+    :param Iterator[stbt.Frame] frames: See `press_and_wait`.
 
     :returns: See `press_and_wait`.
     """
-    if _dut is None:
+    if frames is None:
         import stbt_core
-        _dut = stbt_core
+        frames = stbt_core.frames()
 
     if region is not Region.ALL:
         if mask is not Region.ALL:
             raise ValueError("Cannot specify mask and region at the same time")
         warnings.warn(
             "stbt.wait_for_transition_to_end: The 'region' parameter is "
             "deprecated; pass your Region to 'mask' instead",
             DeprecationWarning, stacklevel=2)
         mask = region
 
-    t = _Transition(mask, timeout_secs, stable_secs, min_size, _dut)
+    t = _Transition(mask, timeout_secs, stable_secs, min_size, frames)
     result = t.wait_for_transition_to_end(initial_frame)
     debug("wait_for_transition_to_end() -> %s" % (result,))
     return result
 
 
 class _Transition():
-    def __init__(self, mask, timeout_secs, stable_secs, min_size, dut):
+    def __init__(self, mask: MaskTypes, timeout_secs: float,
+                 stable_secs: float, min_size: SizeT | None,
+                 frames: Iterator[FrameT]):
         self.mask = mask
         self.timeout_secs = timeout_secs
         self.stable_secs = stable_secs
         self.min_size = min_size
-        self.dut = dut
+        self.frames = frames
 
-        self.frames = self.dut.frames()
         self.expiry_time = None
 
     def wait(self, press_result):
         self.expiry_time = press_result.end_time + self.timeout_secs
 
-        differ = press_and_wait.differ(initial_frame=press_result.frame_before,
-                                       mask=self.mask, min_size=self.min_size)
+        differ = press_and_wait.differ.replace(min_size=self.min_size)
+        dm = DetectMotion(differ, press_result.frame_before, self.mask)
+
         # Wait for animation to start
         for f in self.frames:
             if f.time < press_result.end_time:
                 # Discard frame to work around latency in video-capture pipeline
                 continue
-            motion_result = differ.diff(f)
+            motion_result = dm.diff(f)
             draw_on(f, motion_result, label="transition")
             if motion_result:
                 _debug("Animation started", f)
                 animation_start_time = f.time
                 break
             _debug("No change", f)
             if f.time >= self.expiry_time:
@@ -230,19 +264,19 @@
     def wait_for_transition_to_end(self, initial_frame):
         if initial_frame is None:
             initial_frame = next(self.frames)
         if self.expiry_time is None:
             self.expiry_time = initial_frame.time + self.timeout_secs
 
         first_stable_frame = initial_frame
-        differ = press_and_wait.differ(initial_frame=initial_frame,
-                                       mask=self.mask, min_size=self.min_size)
+        differ = press_and_wait.differ.replace(min_size=self.min_size)
+        dm = DetectMotion(differ, initial_frame, self.mask)
         while True:
             f = next(self.frames)
-            motion_result = differ.diff(f)
+            motion_result = dm.diff(f)
             draw_on(f, motion_result, label="transition")
             if motion_result:
                 _debug("Animation in progress", f)
                 first_stable_frame = f
             else:
                 _debug("No change since previous frame", f)
             if f.time - first_stable_frame.time >= self.stable_secs:
```

### Comparing `stbt_core-33.1.1/_stbt/types.py` & `stbt_core-34.0.0/_stbt/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,14 +242,16 @@
         :returns: The intersection of the passed regions, or ``None`` if the
             regions don't intersect.
 
         Any parameter can be ``None`` (an empty Region) so intersect is
         commutative and associative.
     """
 
+    ALL: "Region"
+
     def __new__(
         cls,
         x: float,
         y: float,
         width: Optional[float] = None,
         height: Optional[float] = None,
         right: Optional[float] = None,
@@ -346,17 +348,27 @@
         elif all(hasattr(other, a) for a in ("x", "y")):  # a Position
             return (self.x <= other.x < self.right and
                     self.y <= other.y < self.bottom)
         else:
             raise TypeError("Region.contains expects a Region, Position, or "
                             "None. Got %r" % (other,))
 
-    def translate(
-        self, x: Optional[float] = None, y: Optional[float] = None
-    ) -> Region:
+    @typing.overload
+    def translate(self, x: Region) -> Region:
+        ...
+
+    @typing.overload
+    def translate(self, x: float | None, y: float | None) -> Region:
+        ...
+
+    @typing.overload
+    def translate(self, x: tuple[int, int]) -> Region:
+        ...
+
+    def translate(self, x=None, y=None):
         """
         :returns: A new region with the position of the region adjusted by the
             given amounts.  The width and height are unaffected.
 
         ``translate`` accepts separate x and y arguments, or a single `Region`.
 
         For example, move the region 1px right and 2px down:
```

### Comparing `stbt_core-33.1.1/_stbt/utils.py` & `stbt_core-34.0.0/_stbt/utils.py`

 * *Files identical despite different names*

### Comparing `stbt_core-33.1.1/_stbt/wait.py` & `stbt_core-34.0.0/_stbt/wait.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,34 +101,37 @@
     """
     import time
 
     if predicate is None:
         predicate = lambda x: x
     stable_value = None
     stable_predicate_value = None
-    expiry_time = time.time() + timeout_secs
+    start_time = time.time()
+    expiry_time = start_time + timeout_secs
 
     while True:
         t = time.time()
         value = callable_()
         predicate_value = predicate(value)
 
         if stable_secs:
             if predicate_value != stable_predicate_value:
                 stable_since = t
                 stable_value = value
                 stable_predicate_value = predicate_value
             if predicate_value and t - stable_since >= stable_secs:
-                debug("wait_until succeeded: %s"
-                      % _callable_description(callable_))
+                debug("wait_until succeeded in %.3fs: %s"
+                      % (time.time() - start_time,
+                         _callable_description(callable_)))
                 return stable_value
         else:
             if predicate_value:
-                debug("wait_until succeeded: %s"
-                      % _callable_description(callable_))
+                debug("wait_until succeeded in %.3fs: %s"
+                      % (time.time() - start_time,
+                         _callable_description(callable_)))
                 return value
 
         if t >= expiry_time:
             debug("wait_until timed out after %s seconds: %s"
                   % (timeout_secs, _callable_description(callable_)))
             if not value:
                 return value  # it's falsey
```

### Comparing `stbt_core-33.1.1/setup.py` & `stbt_core-34.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 long_description = """\
 # Stb-tester open-source APIs (stbt_core)
 
 **Automated User Interface Testing for Set-Top Boxes & Smart TVs**
 
-* Copyright © 2013-2022 Stb-tester.com Ltd,
+* Copyright © 2013-2023 Stb-tester.com Ltd,
   2012-2014 YouView TV Ltd. and other contributors.
 * License: LGPL v2.1 or (at your option) any later version (see [LICENSE]).
 
 This package contains the `stbt_core` open-source Python APIs that you can use
 in test-scripts written for running on the [Stb-tester Platform]. The primary
 purpose of this package is to make the `stbt_core` library easy to install
 locally for IDE linting & autocompletion.
@@ -28,15 +28,15 @@
 
 [LICENSE]: https://github.com/stb-tester/stb-tester/blob/master/LICENSE
 [Stb-tester Platform]: https://stb-tester.com
 """
 
 setuptools.setup(
     name="stbt_core",
-    version="33.1.1",
+    version="34.0.0",
     author="Stb-tester.com Ltd.",
     author_email="support@stb-tester.com",
     description="Automated GUI testing for Set-Top Boxes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://stb-tester.com",
     packages=["stbt_core", "_stbt"],
```

### Comparing `stbt_core-33.1.1/stbt_core/__init__.py` & `stbt_core-34.0.0/stbt_core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from _stbt.black import (
     is_screen_black)
 from _stbt.config import (
     ConfigurationError,
     get_config)
 from _stbt.diff import (
     BGRDiff,
-    FrameDiffer,
+    Differ,
     GrayscaleDiff,
     MotionResult)
 from _stbt.frameobject import (
     for_object_repository,
     FrameObject)
 from _stbt.grid import (
     Grid)
@@ -94,20 +94,20 @@
     "BGRDiff",
     "Color",
     "ConfigurationError",
     "ConfirmMethod",
     "crop",
     "debug",
     "detect_motion",
+    "Differ",
     "Direction",
     "draw_text",
     "find_file",
     "for_object_repository",
     "Frame",
-    "FrameDiffer",
     "FrameObject",
     "frames",
     "get_config",
     "get_frame",
     "GrayscaleDiff",
     "Grid",
     "Image",
```

### Comparing `stbt_core-33.1.1/stbt_core.egg-info/PKG-INFO` & `stbt_core-34.0.0/stbt_core.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stbt-core
-Version: 33.1.1
+Version: 34.0.0
 Summary: Automated GUI testing for Set-Top Boxes
 Home-page: https://stb-tester.com
 Author: Stb-tester.com Ltd.
 Author-email: support@stb-tester.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,15 @@
 Provides-Extra: ocr
 License-File: LICENSE
 
 # Stb-tester open-source APIs (stbt_core)
 
 **Automated User Interface Testing for Set-Top Boxes & Smart TVs**
 
-* Copyright © 2013-2022 Stb-tester.com Ltd,
+* Copyright © 2013-2023 Stb-tester.com Ltd,
   2012-2014 YouView TV Ltd. and other contributors.
 * License: LGPL v2.1 or (at your option) any later version (see [LICENSE]).
 
 This package contains the `stbt_core` open-source Python APIs that you can use
 in test-scripts written for running on the [Stb-tester Platform]. The primary
 purpose of this package is to make the `stbt_core` library easy to install
 locally for IDE linting & autocompletion.
```

### Comparing `stbt_core-33.1.1/stbt_core.egg-info/SOURCES.txt` & `stbt_core-34.0.0/stbt_core.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 _stbt/cv2_compat.py
 _stbt/diff.py
 _stbt/frameobject.py
 _stbt/grid.py
 _stbt/imgproc_cache.py
 _stbt/imgutils.py
 _stbt/keyboard.py
+_stbt/libstbt.py
 _stbt/logging.py
 _stbt/mask.py
 _stbt/match.py
 _stbt/motion.py
 _stbt/multipress.py
 _stbt/ocr.py
 _stbt/precondition.py
 _stbt/pylint_plugin.py
+_stbt/sqdiff.py
 _stbt/stbt.conf
 _stbt/transition.py
 _stbt/types.py
 _stbt/utils.py
 _stbt/wait.py
 stbt_core/__init__.py
 stbt_core/pylint_plugin.py
```

